# Wave 4: Technical Feasibility — Pokémon Champions AI Coach + Prep Workspace

**Research date:** 2026-05-09
**Agent:** D1
**Scope:** Technical risk gate. What's possible, what isn't, what we should kill.

---

## TL;DR Verdict

- **No public API. No replay infrastructure. No exportable structured match data.** The "post-loss replay analysis" feature as imagined (auto-ingest replay → turn-by-turn AI critique) is **infeasible** at MVP scope. We must redesign or kill it.
- **Replica Team codes ARE the team-data primitive** — but they're opaque codes redeemable in-game only; not parseable into Showdown packed format without manual user re-entry.
- **Open-source ingredients are exceptional.** `@pkmn/sim`, `@smogon/calc`, `@pkmn/client`, Showdown packed-team format, Smogon usage stat dumps (chaos JSON, public domain), Pikalytics (scrapeable), and an existing **MCP server wrapping `@smogon/calc`** dramatically de-risk the build.
- **AI grounding pattern is solved.** PokéLLMon (arxiv 2402.01118) shows GPT-4 hallucinates type matchups ~16% of the time without grounding. RAG over Smogon stats + tool-calling into the damage calc closes most of the gap. Precedent exists.
- **IP posture:** Showdown's MIT license covers code, not data. Names/types/moves are nominative fair use *if* non-commercial, no logos, no sprites, no money flow on Pokémon-named features. Champions-launch competitor `vgccoach.pro` and Pikalytics already do this in market.
- **6-month solo build (15-25 hrs/wk):** Achievable for team builder + meta browser + grounded AI Q&A. **Not achievable** for full automated replay analysis or native iOS app from day one.

---

## Section 1: Data Access & Replay (THE Critical Section)

### 1.1 Champions has NO public API

There is no official Pokémon Champions API. A GitHub issue on PokéAPI (#1484) requesting Champions support has no resolution — confirming the community has not yet found or built one. Pikalytics, ChampDex, Champions Lab, and Porygon Labs all derive their Champions data from **(a) in-game Battle Data menu screenshots** and **(b) tournament submissions** — not from any feed.

The in-game **Battle Data menu** shows aggregate top Pokémon, top moves, top items, top teammates per Pokémon, similar to Pikalytics-lite. Players see this client-side; there's no documented endpoint behind it.

### 1.2 Replays in Champions are deliberately crippled

This is the most consequential finding for our scope:

- **You can save ONE replay at a time, for ONE HOUR.** The "better" replay system requires a paid in-game membership (similar criticism: "Replays in this game are pathetic" — official Pokémon Forums).
- **No replay URLs.** Unlike Pokémon Showdown (`replay.pokemonshowdown.com/<id>`), Champions has no shareable replay link.
- **No turn-by-turn structured export.** What players *can* do: export the **Battle Log** — text dump to clipboard. This is a flat text log similar to TCG Live's, parseable but not officially documented for Champions yet (community parsers exist for Showdown logs; community would need to build a Champions-flavor parser).
- **Community sentiment:** GameFAQs and Pokémon Forums threads explicitly ask "will the game ever get a real replay feature" — answer is "maybe, devs say they're working on bugs." No timeline.

**Implication:** "Auto-ingest replay → turn-by-turn AI critique" requires either (a) a battle-log copy/paste flow where users manually paste their text log, or (b) OCR/CV on screenshot or video upload. Both impose meaningful user friction. Showdown-style "paste replay URL, get analysis" is **impossible** for Champions matches.

### 1.3 Replica Teams: opaque codes, not portable data

- Replica Teams are alphanumeric codes redeemable only inside Champions. They encode a full team (6 mons + items + abilities + natures + moves + EVs). Players generate via Training → Replica Teams → Share.
- They are **NOT decodable** outside the game (no published encoding scheme; The Pokémon Company controls the namespace).
- Players manually retype team contents into Showdown packed format if they want to use third-party tools. Tools like Champions Builder and Pikalytics Team Builder support **Showdown export string** as their portable format — meaning users build *in* the tool and export *to* Showdown packed; they don't auto-import from a Replica Team code.
- **No bidirectional sync** between Showdown and Champions. Even if you build a perfect team in Showdown packed format, you must re-create it in-game from your existing Pokémon box (also requires you actually own the mons + items in your inventory).

### 1.4 Pokémon HOME ↔ Champions

- Pokémon HOME 4.0.0 added official support for Champions transfers (HOME → Champions for owned Pokémon).
- HOME has **no third-party API**. There is a community-documented mobile app API gist (zaksabeast on GitHub) but it's an internal/unofficial reverse-engineering effort and using it commercially would be a fast path to a takedown.
- HOME is for moving owned Pokémon between Nintendo titles — **not a team-data export channel**.

### 1.5 Reverse-engineering status

- PRET (Pokémon Reverse Engineering Team) has fully decompiled Gen 1-3 era games. Champions (April 2026 launch) has no public decomp project.
- ReMasters (Pokémon Masters reverse engineering) is the closest precedent for a modern Pokémon mobile-app decomp; it's small-scale, individual-driven, lawful-gray.
- **Implication:** Counting on reverse-engineered access to Champions internals is high-risk and unethical for a public product. Treat as off-limits.

### 1.6 What Showdown/Smogon DOES expose (the contrast)

For comparison — the Showdown ecosystem is the gold standard, and Champions has none of it:

| Capability | Showdown | Champions |
|---|---|---|
| Public replay URLs | Yes (replay.pokemonshowdown.com) | No |
| Replay JSON / log download | Yes | No |
| Public usage stats dumps | Yes (smogon.com/stats, monthly, chaos JSON) | No |
| Team import/export string | Yes (packed format, well-documented in `sim/TEAMS.md`) | Replica Code (opaque) |
| Open-source simulator | Yes (`@pkmn/sim`, MIT) | No |
| Open-source damage calc | Yes (`@smogon/calc`, MIT) | Wraps Showdown calc anyway |
| Programmatic battle access | Yes (poke-env, @pkmn/client) | No |

---

## Section 2: Open-Source Ingredients (What We Can Build On)

These reduce build risk by **70%+** for the parts of our product that don't depend on Champions internals.

### 2.1 Battle simulator: `@pkmn/sim`

- npm: `@pkmn/sim` (current 0.10.7, published ~monthly), MIT license.
- Modular extraction of Pokémon Showdown's `sim/` directory by the `@pkmn` org (Kirk Scheibelhut, Showdown maintainer).
- TypeScript-first. Stable API. Gens 1-9. Excludes random-team generation (in `@pkmn/randoms`).
- Use case: programmatic battle simulation, validating teams, running "what if" scenarios.

### 2.2 Damage calculator: `@smogon/calc`

- npm: `@smogon/calc` (current 0.11.0). MIT.
- The same engine powering `calc.pokemonshowdown.com`.
- Already wrapped as an **MCP server** by community (Skywork.ai writeup) — meaning AI agents can call it via standardized JSON I/O. **This is the single biggest unlock for our AI coach.**
- Pikalytics maintains a public fork (`pikalytics/pikalytics-calc`).

### 2.3 Battle state tracking: `@pkmn/client`

- Replicates Showdown's official client battle class in a small, headless environment.
- Processes log files to track battle state turn-by-turn — **the exact thing we'd need if we get any structured Champions log dump.**

### 2.4 Replay parsing (Showdown only, but reusable)

Existing community tools to study or fork:
- `bretgourdie/pokemon-replay-analyzer` (PHP, KO/death/winner analysis)
- `MDFowler/Showdown-Parser` (records team from log)
- `NoahvdV/Pokemon-Showdown-Replay-Parser` (singles + VGC)
- `Pocolip/vs-recorder` (VGC-specific replay analyzer with usage stats, lead patterns, matchup spreads — closest to our "post-match analysis" vision)
- Hugging Face dataset `jakegrigsby/metamon-parsed-replays` (parsed RL trajectories)

If a Champions battle-log text format stabilizes and is similar enough to Showdown's protocol message format (`|switch|`, `|move|`, `|damage|`, etc.), these parsers are **directly portable**. If Champions' log is its own beast, we'd need a new parser — solo-buildable in 1-2 weeks for a single format.

### 2.5 Smogon usage stats (public domain)

- `smogon.com/stats/` — monthly aggregate JSON in `chaos/` subfolder (moveset, metagame, lead, monotype variants).
- License: aggregated stats are explicitly **public domain**; only set/analysis text is Smogon-copyrighted.
- File naming: `{tier}-{baseline}.txt` (e.g., `gen9vgc2026regm-1630.0.txt`).
- Wrappers: `pkmn/smogon` (TypeScript), `GriffinLedingham/smogon-usage-parser` (Pikalytics' own ingestion stack).
- Updated monthly. **This is our meta-grounding data layer.**

### 2.6 Pikalytics (scrapeable, but check ToS)

- Pikalytics scrapes Smogon usage and presents it; their app ToS does not appear to grant API access to third parties.
- Better path: ingest Smogon's chaos JSON directly (public domain) and skip Pikalytics entirely. Same data, no relationship risk.

### 2.7 Showdown packed team format

- Documented in `pokemon-showdown/sim/TEAMS.md`.
- Two formats: **packed** (compact, console-ready) and **JSON** (PokemonSet[]).
- Universal in the VGC tools ecosystem (Champions Builder, Pikalytics Team Builder, vgccoach.pro all import/export it).
- **Adopt Showdown packed format as our internal team-data canonical form.** Users paste Showdown text → we own the data layer → they re-create in Champions manually if/when they want to play it. Same friction every other tool has.

---

## Section 3: AI Feasibility (Grounding Strategy)

### 3.1 Out-of-the-box LLM accuracy is poor

PokéLLMon (arxiv 2402.01118v2) benchmarks on competitive Pokémon:
- **GPT-4: 84% accuracy on type advantage prediction** (i.e., 16% hallucination on a basic mechanic).
- LLaMA-2 and GPT-3.5 are dramatically worse — "severe hallucination."
- GPT-4 vs heuristic bot: 26% win rate (vs 60% for human players).
- Common failure modes: incorrect type matchups, persisting on ineffective moves, sending mons into disadvantage.

Recent work (arxiv 2512.17308 — "LLMs as Pokémon Battle Agents") notes Claude 4.5+ and GPT-5 Mini show measurable improvements in move-generation tasks but still benefit massively from grounding.

### 3.2 The grounding playbook is well-known

PokéLLMon itself proposes:
- **Knowledge-augmented generation (RAG)** over the Showdown data layer.
- **In-context reinforcement** (feeding turn outcomes back).

Practical implementation for our product:
1. **Tool calls** to `@smogon/calc` (via MCP or direct) for any damage / KO probability question. **Never let the LLM compute damage from memory.**
2. **RAG retrieval** over Smogon usage stats (chaos JSON) for "what does Garchomp usually run in Reg M-A?" type questions.
3. **Grounded type chart** as a static tool/prompt (small enough to inline).
4. **Team validation** via `@pkmn/sim` (legality check before any analysis).

This is the "Stockfish-grounds-chess-analysis" pattern, and it's genuinely available off-the-shelf via the existing MCP server wrapping `@smogon/calc`.

### 3.3 LLM cost (May 2026 pricing)

For a chat-style coach session (assume 5K input tokens of context + RAG, 1K output per user turn, 10 turns/session):

- **Claude Haiku 4.5** ($1/$5 per M): ~$0.075/session
- **Gemini 2.5 Flash** ($0.15/$0.60): ~$0.014/session
- **Claude Sonnet 4.6** ($3/$15): ~$0.225/session
- **Claude Opus 4.6** ($5/$25 — overkill): ~$0.375/session

For a free MVP with 100 active users averaging 5 sessions/week using Sonnet 4.6 with prompt caching:
- ~2,000 sessions/month × $0.20 (cached avg) = **~$400/month** worst case.
- Routing 70% of queries to Haiku 4.5 cuts that to **~$120-150/month**.

Vector store (for RAG over usage stats): Pinecone serverless, Supabase pgvector, or just JSON in memory (data is small — Reg M-A chaos JSON is <50 MB). **In-memory or Supabase pgvector at zero/low cost is fine for MVP.**

### 3.4 Existing AI coach competitor

`vgccoach.pro` is **already shipping** a free AI VGC coach for Champions Reg M, "trained on 112,000 real VGC battles." This means:
- Our AI-coach feature is not a moat — it's table stakes.
- They already have the data ingestion problem we'd have to solve. They likely scrape Showdown VGC ladder replays (since Champions has none).
- Differentiation must come from workflow (matchup prep, opponent recon, journaling) not from "we have AI."

---

## Section 4: Build Cost Estimate (15-25 hrs/wk solo, 6 months)

Total available: ~390-650 hours over 6 months. Realistic productive coding: ~60% of that = **235-390 hours**.

| Module | Hours | Risk | Notes |
|---|---|---|---|
| Auth + user model + Supabase setup | 20 | low | standard SaaS plumbing |
| Team builder (Showdown packed I/O) | 40 | low | clone Champions Builder UI patterns; @pkmn/data for autocomplete |
| Damage calc UI (wraps @smogon/calc) | 30 | low | many open-source examples to fork |
| Meta browser (ingests Smogon chaos JSON monthly) | 25 | low | cron job + simple UI |
| AI coach chat (RAG + tool-calling to calc) | 60 | medium | grounding/prompt engineering iteration |
| Match journal (manual entry forms) | 30 | low | basic CRUD; no replay parsing |
| Battle log paste-and-parse (text log → structured) | 50 | high | depends on Champions log format stability |
| Mobile-responsive web | 20 | low | Tailwind / shadcn responsive |
| Polish, deploy (Vercel), bug-fixing | 40 | medium | always more than estimated |
| **Total** | **~315** | | fits in 235-390 envelope |

**Cuts to make if we slip:** drop battle-log parsing, ship as manual journaling only. That recovers ~50 hours and removes the highest-risk technical work.

**Hosting:**
- Vercel hobby/pro: $0-20/mo
- Supabase free/pro: $0-25/mo
- LLM API (above): ~$120-400/mo at 100 active users
- Domain: $12/yr
- **Total burn: ~$150-450/mo at MVP scale.** Survivable on personal funds.

---

## Section 5: IP Technical Posture

### 5.1 Showdown / @pkmn/sim / @smogon/calc — MIT, but…

- The **code** is MIT — usable in commercial products legally.
- The **data they encode** (Pokémon names, moves, abilities, type chart) is Nintendo/TPC IP.
- Showdown itself "remains online because it operates as a fan-made, non-commercial project that avoids direct sale or distribution of Nintendo's game software" (Wikipedia + community legal analysis).
- **Practical rule:** building on these libraries is the same risk profile as any unofficial Pokémon companion app. The risk doesn't come from the libraries' license; it comes from the underlying data.

### 5.2 PokéAPI — same posture

- PokéAPI's own LICENSE.md notes: "Pokémon and Pokémon character names are trademarks of Nintendo."
- Free for non-commercial use. Commercial use is technically against TPC's stance.
- Pikalytics, ChampDex, vgccoach.pro all monetize lightly (ads, sponsorships, premium tiers) and remain unbothered as of May 2026.

### 5.3 Smogon stats files — public domain (the cleanest input)

- Aggregated usage data: explicit public domain.
- Set/analysis text: Smogon copyright.
- **Use the chaos JSON freely. Do not lift Smogon's analysis prose.**

### 5.4 Names / types / moves text — nominative fair use

The Pokémon Company's stance: "license is limited strictly to non-commercial uses."

Reality on the ground (May 2026):
- Pikalytics, ChampDex, Champions Lab, Champions Builder, Porygon Labs, vgccoach.pro all use Pokémon names, type names, move names freely.
- None have been C&D'd as of this research. Pattern: TPC enforces against (a) ROM hacks/games, (b) fan-game **launches with funding** (Kickstarter triggers them per former TPC chief legal officer, per Game8 interview), (c) anything using sprites/art/audio/logos.

### 5.5 Hard rules for our build

- **DO** use names, types, moves, abilities as text labels.
- **DO** use Smogon chaos JSON (public domain).
- **DO** use `@pkmn/sim`, `@smogon/calc`, `@pkmn/data` (MIT).
- **DO NOT** use sprites or official art. Use abstract icons, type-color squares, or commission original mon-portraits in our own art style.
- **DO NOT** use the word "Pokémon" or stylized PokéBall in our brand mark.
- **DO NOT** use audio cues or trademarked phrases.
- **DO NOT** Kickstarter-fund a Pokémon-named feature.
- **DO** include an "unofficial / not affiliated with Nintendo, Game Freak, or The Pokémon Company" disclaimer (Pikalytics' wording is a usable template).
- Monetization should be on the workflow/coach value, not on Pokémon-the-IP.

### 5.6 C&D pattern in 2024-25

Recent enforcement (Wikipedia "Pokémon fan games"):
- Relic Castle (fan-game forum) — March 2024 — taken down.
- Palworld Pokémon mod — Jan 2024.
- Multiple ROM hacks ongoing.
- **Companion apps (no game content, no sprites) appear safe.** ChampDex, Pikalytics, Champions Lab, vgccoach.pro all in market untouched.

---

## Section 6: Mobile Path

### 6.1 ChampDex shipped iOS-native within 30 days

ChampDex's existence on the App Store (id: 6761497339) proves Apple approves unofficial Pokémon companion apps as long as they:
- Don't use sprites/audio/trademarks in branding.
- Position as "unofficial companion" with disclaimers.
- Don't claim affiliation.

Pikalytics: Battle Strategy (id: 1511370166) has been on App Store since 2020. Same pattern.

### 6.2 Realistic mobile strategy for solo founder

**Phase 1 (MVP, months 1-6):** Mobile-responsive web app with PWA install. Tailwind + shadcn. **No native app.**
- Faster to build, cheaper to maintain.
- Works on iOS, Android, desktop with one codebase.
- Pikalytics' own web product is the proof point — it's the data tool of record for VGC players, and it's just a website.

**Phase 2 (post-PMF, months 7+):** React Native or Capacitor wrapper if mobile usage data justifies it. ChampDex chose native; Pikalytics chose hybrid (web + companion app). Either is viable; web-first is lower risk.

**Avoid:** SwiftUI native + Android Kotlin native parallel tracks. Solo founder cannot maintain two native apps.

---

## Decision Matrix: Feature Feasibility (6-month hobbyist build)

| Feature | Verdict | Rationale |
|---|---|---|
| Team builder w/ Showdown import-export | **FEASIBLE** | Multiple OSS examples, well-known format |
| Damage calculator | **FEASIBLE** | `@smogon/calc` directly; existing MCP server |
| Live meta browser (usage stats) | **FEASIBLE** | Smogon chaos JSON public domain |
| AI Q&A coach (grounded RAG + calc tool-call) | **FEASIBLE** | PokéLLMon pattern; MCP precedent; ~$150-400/mo |
| Manual match journal (user logs lessons) | **FEASIBLE** | Basic CRUD |
| Matchup prep notes per Pokémon | **FEASIBLE** | Workflow on top of meta data |
| Mobile-responsive web (PWA) | **FEASIBLE** | Standard modern stack |
| Battle-log paste → structured analysis | **RISKY** | Depends on Champions log format; parser is solo-buildable but format may shift |
| Opponent ladder recon (their last 10 teams) | **RISKY** | Requires Champions ladder data we cannot access |
| Champions Replica Code → team data import | **RISKY** | Codes are opaque; requires either users to retype or unofficial decoding (legal/ethical issues) |
| Native iOS app at launch | **RISKY** | Solo founder bandwidth; ChampDex did it but they're focused on a single feature |
| **Auto replay analysis (URL → turn-by-turn AI critique)** | **INFEASIBLE** | **No replay URLs exist in Champions. Period.** |
| Live battle assistant (real-time during play) | **INFEASIBLE** | No game-state hooks; would need OCR on running game; against ToS |
| Showdown ↔ Champions team sync | **INFEASIBLE** | No bidirectional channel exists |
| Pokémon HOME team scraping | **INFEASIBLE** | No public API; using unofficial reverse-engineered API = takedown risk |
| Reverse-engineering Champions data files | **INFEASIBLE** | Off-limits ethically and legally |
| Native Android app at launch | **INFEASIBLE** | Bandwidth |

---

## Recommended MVP Cuts (Kill List)

1. **KILL: "Post-loss replay analysis" as auto-ingest.** Replace with **manual match journal + structured prompts** ("what was your lead? what did opponent reveal turn 1? what did you learn?"). User does the data entry; AI helps with structured reflection. This sidesteps the no-replay-URL problem entirely while preserving the "post-loss learning" job-to-be-done.
2. **KILL: Native mobile at launch.** PWA only. Revisit at month 6 with usage data.
3. **DEFER: Battle-log paste parsing.** Ship without it; add only if community settles on a stable Champions log format.
4. **DEFER: Opponent ladder recon.** No data source exists. Could partner with vgccoach.pro or Pikalytics later if ladder data becomes accessible.

---

## Sources

- [PokéAPI](https://pokeapi.co/) | [PokéAPI license](https://github.com/PokeAPI/pokeapi/blob/master/LICENSE.md) | [PokéAPI Champions issue #1484](https://github.com/PokeAPI/pokeapi/issues/1484)
- [Pokémon Champions Battle Data Menu - GamesGG](https://games.gg/news/pokemon-champions-battle-data-menu-hidden/)
- [Champions Replica Teams - Serebii](https://www.serebii.net/pokemonchampions/replicateams.shtml)
- [Champions Replica Teams Guide - GameRant](https://gamerant.com/pokemon-champions-replica-teams-explained-team-codes/)
- [Champions replay limitations - Pokémon Forums](https://community.pokemon.com/en-us/discussion/19703/replays-in-this-game-are-pathetic)
- [Champions replay feature discussion - GameFAQs](https://gamefaqs.gamespot.com/boards/517117-pokemon-champions/81134751)
- [Pokémon HOME Mobile API gist - zaksabeast](https://gist.github.com/zaksabeast/e031a6512cb89de42aea70a8ca674619)
- [@pkmn/sim on npm](https://www.npmjs.com/package/@pkmn/sim) | [pkmn/ps GitHub](https://github.com/pkmn/ps)
- [@smogon/calc on npm](https://www.npmjs.com/package/@smogon/calc) | [smogon/damage-calc GitHub](https://github.com/smogon/damage-calc)
- [Pokémon Showdown sim/TEAMS.md (packed format)](https://github.com/smogon/pokemon-showdown/blob/master/sim/TEAMS.md)
- [Smogon usage stats index](https://www.smogon.com/stats/) | [Smogon Usage Stats Discussion mk.3](https://www.smogon.com/forums/threads/official-smogon-university-usage-statistics-discussion-thread-mk-3.3591776/)
- [pkmn/smogon wrapper](https://github.com/pkmn/smogon) | [smogon-usage-parser](https://github.com/GriffinLedingham/smogon-usage-parser)
- [VGC Damage Calculator MCP Server (Skywork)](https://skywork.ai/skypage/en/ai-pokemon-battles-damage-calculator/1981907305164279808)
- [PokéLLMon paper (arxiv 2402.01118)](https://arxiv.org/html/2402.01118v2)
- [LLMs as Pokémon Battle Agents (arxiv 2512.17308)](https://arxiv.org/pdf/2512.17308)
- [Pokémon Showdown Replay Parser - Pocolip vs-recorder](https://github.com/Pocolip/vs-recorder)
- [poke-env documentation](https://poke-env.readthedocs.io/en/stable/examples/quickstart.html)
- [Metamon parsed replays dataset (Hugging Face)](https://huggingface.co/datasets/jakegrigsby/metamon-parsed-replays)
- [Pokémon Showdown Wikipedia (legality)](https://en.wikipedia.org/wiki/Pok%C3%A9mon_Showdown)
- [Pokémon Showdown LICENSE (MIT)](https://github.com/smogon/pokemon-showdown/blob/master/LICENSE)
- [Pokémon fan games Wikipedia (C&D pattern)](https://en.wikipedia.org/wiki/Pok%C3%A9mon_fan_games)
- [Former Pokémon lawyer on fan project enforcement - Dexerto](https://www.dexerto.com/pokemon/former-pokemon-lawyer-reveals-no-one-likes-suing-fan-projects-2592964/)
- [Pokémon HOME 4.0.0 / Champions connectivity - Game8](https://game8.co/games/Pokemon-Champions/archives/501825)
- [ChampDex on App Store](https://apps.apple.com/us/app/champdex/id6761497339)
- [Pikalytics: Battle Strategy on App Store](https://apps.apple.com/us/app/pikalytics-battle-strategy/id1511370166)
- [VGC Coach (vgccoach.pro)](https://vgccoach.pro/)
- [Champions Builder](https://www.championsbuilder.com/)
- [Porygon Labs](https://www.porygonlabs.com/)
- [Pikalytics Champions](https://www.pikalytics.com/champions)
- [LLM API Pricing 2026 - TLDL](https://www.tldl.io/resources/llm-api-pricing-2026)
- [LLM API Cost Comparison - InventiveHQ](https://inventivehq.com/blog/llm-api-cost-comparison)
