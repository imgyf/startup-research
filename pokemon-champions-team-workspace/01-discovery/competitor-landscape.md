# Competitor Landscape

**Phase:** 3 — Discovery
**Project:** pokemon-champions-team-workspace
**Date:** 2026-05-09
**Confidence:** High (direct observation of competitor sites; usage signals are inferred but corroborated)

---

## Competitive Set Overview

The market splits into three layers:

1. **Established Pokémon tooling incumbents** — Showdown, Smogon, Pikalytics, Poképaste. Massive audiences, free, slow to ship workspace features, focused on data/simulation.
2. **Champions-specific entrants (post April 2026 launch)** — 15+ tools shipped within 30 days. Mostly solo-founder side projects. Some sharp, most thin.
3. **Indirect substitutes** — ChatGPT/Claude as informal coaches, Discord servers + spreadsheets as workflow stacks, paid 1-1 human coaching (Metafy).

---

## Comparison Matrix

| Tool | URL | Pricing | Target | Workspace? | AI? | Mobile? | Differentiator | Threat Level |
|---|---|---|---|---|---|---|---|---|
| **Pokémon Showdown** | pokemonshowdown.com | Free | Comp + casual | Stateless cookie-storage; recently added server-side teams | No | Web only (no native iOS) | The simulator + the de facto teambuilder. Unkillable as core infra. | Indirect (we sit beside, not against) |
| **Smogon** | smogon.com | Free | Comp | RMT forums (manual) | No | Web | Strategy Pokédex, 20+ years of indexed analysis, SEO moat | Indirect (content authority) |
| **Pikalytics** | pikalytics.com | Free + ads | VGC | Has team builder, Champions ruleset support shipped <30 days post-launch | No | Web responsive | Usage stats authority; fastest competitor to ship Champions support | **High** |
| **Poképaste** | pokepast.es | Free | All | Read-only paste hosting; the link primitive everyone uses | No | Web | Universal share link format | Indirect (primitive to embrace) |
| **VGCCoach** | vgccoach.pro | Free, no signup | Champions VGC | No (stateless team scoring) | **Yes** — claims 112,480-battle training data | Web | First-mover on "AI coach for Champions"; ranks #1 for that query | **High** |
| **ChampDex** | champdex.com + iOS app | Free | Casual + comp | Light team save | Limited | **iOS-native** (only one) | Owns mobile niche by default | Medium-high |
| **Champions Lab** | championslab.xyz | Free, open source | Comp | Limited | Monte Carlo sim (2M battles) | Web | Technical credibility from open-source dev | Medium |
| **PokéBase (Champions)** | pokebase.app/pokemon-champions | Free | All | Saves teams; community-submitted | No | Web | Existing brand authority extended to Champions | Medium |
| **Porygon Labs** | porygonlabs.com | Free | VGC niche | Damage calc king | No | Web | Niche depth in damage calc | Low-medium |
| **ChampTeamAI** | champteamai.com | Free | Champions | Team scoring | Yes (basic) | Web | Generic naming, thin features | Low |
| **Champions Builder** | championsbuilder.com | Free | Casual | Team builder | No | Web | Thin — no founder presence | Low |
| **BattleWise AI** | battlewiseai.com | Free | Champions | Limited | Yes (basic) | Web | Weekend project signature | Low |
| **ChampionsHub.gg** | championshub.gg | Free | Champions | Tools directory | No | Web | Aggregator | Low |
| **ChampionsMeta / StrataDex / Reportworm** | various | Free | Various | Specialty (meta, tier list, replay stats) | No (Reportworm: stats) | Web | Niche utilities | Low |
| **ChatGPT/Claude (informal use)** | n/a | $20/mo (already paying) | All | n/a | Yes (general) | n/a | The actual "AI coach" most people try first | Medium (substitute) |
| **Metafy human coaching** | metafy.gg | $25-30/hr | Tournament-prep | Human; not a tool | n/a | n/a | Human-in-the-loop, the gold standard | Indirect (premium ceiling) |

[Tier 2 sourcing on traffic and feature claims; competitor URLs verified live as of 2026-05-09.]

---

## Established Incumbents (Pre-Champions)

### Pokémon Showdown
[Tier 2] **>1M MAU, >30K peak concurrent, 18M visits/month at 21-min sessions.** Built and maintained by Smogon volunteers. Recently shipped server-side team save (post-2022) but UX still feels 2008-era. Cannot ship native iOS due to Apple policy on simulators. **Implication:** Showdown is the gravitational center of competitive Pokémon — a third-party workspace must integrate, not compete. Import/export to Showdown's packed-team format is table stakes.

### Smogon University
[Tier 2] Forum-based. RMT (rate-my-team) subforum is where serious players ask for human feedback. Slow turnaround (24-72 hours), depends on volunteer reviewers. Strategy Pokédex updates lag 2-4 weeks behind format shifts. **Implication:** Smogon is the content brand we must respect; it's a co-op, not a competitor — but it's also where we recruit advisors.

### Pikalytics
[Tier 2] The data-authority site. Shipped a complete Champions Pokédex, ruleset-aware damage calc, team builder, and gamified calc-quiz **within 30 days of Champions launch**. Owner is single operator (per public references); revenue model is ads + light affiliate. **Implication:** Pikalytics is the most directly comparable competitor for "Champions tool that adds workspace value." If they add team-versioning, our workspace differentiator narrows. They have not historically shipped social/coaching features.

### Poképaste
Pure paste hosting. Open source, free. **Strategy: integrate, don't replace.** Every team in our workspace should one-click export to a Poképaste link.

---

## Champions-Specific Entrants (Threat Triage)

### High-Threat Tier

**VGCCoach (vgccoach.pro)** — leading the AI-coach SEO race
- Free, no signup, sub-3-second team scoring
- Claims **112,480-battle training dataset**
- Owns position #1 for "Pokemon Champions AI coach"
- **Strength:** First-mover on the AI coaching SEO angle, no friction signup, fast UX
- **Weakness:** Stateless (no workspace, no memory), no version history, no longitudinal coaching, free with no monetization signal — likely a solo-founder project that can't sustain
- **What we do:** Compete on workspace + memory, not on "first AI coach." VGCCoach is point-in-time scoring; we're the persistent companion.

**ChampDex (Ahmed Elsayed)** — owns iOS-native niche
- Web + native iOS app (App Store), shipped within 30 days of Champions
- **Strength:** Mobile-first, real engineering investment
- **Weakness:** Light on workspace and AI features
- **What we do:** Mobile-responsive web for MVP; consider native app post-product-market-fit. Don't chase ChampDex's wedge — they own it.

### Medium-Threat Tier

**Champions Lab (Andrew21P)** — open-source 2M-battle Monte Carlo sim
- Open source on GitHub
- Technical credibility, "the engineer's tool"
- **Threat:** If they ship a workspace UI on top of their sim, they become formidable
- **What we do:** Could potentially partner — their sim is open source

**PokéBase Champions** — leveraging existing brand
- Existing PokéBase audience extended to Champions
- Community-submitted teams, light save features
- **Threat:** Brand authority + ramp velocity
- **What we do:** Differentiate on workflow and AI coaching layer — PokéBase remains a strategic-content destination, not a workspace

**Porygon Labs** — niche damage calc king
- Specialty product
- **Threat:** Low for our workspace positioning; integrate-not-compete

### Low-Threat (Weekend-Project Tier)

ChampTeamAI, Champions Builder, Champions Team Builder, BattleWise AI, PikaChampions, PokeChampions.co, ChampionsHub.gg, ChampionsMeta, StrataDex, Reportworm — most have generic naming, thin features, no visible founder presence, and no signs of sustained development. **Impact:** they fill SERPs and clutter the discovery surface. Our positioning needs to slice cleanly through.

---

## Indirect Competitors / Substitutes

**ChatGPT/Claude as informal coaches:**
[Opinion + Tier 3 signal] Surprisingly low community footprint. Mining Reddit/Twitter shows few posts about "I asked ChatGPT for my Pokémon team" — most are dunks on hallucinated movesets. Off-the-shelf LLMs hallucinate at high rates on specific competitive Pokémon mechanics (EVs, abilities, item interactions) without grounding. **Implication:** A vertical AI grounded on @pkmn/sim + @smogon/calc + Smogon stats has a real edge over the generic horizontal coaches. The window to build the "Pokémon-correct" AI coach is open.

**Discord servers + spreadsheets:**
What real tournament prep currently looks like — a Pokémon Champions VGC Discord server, a Google Sheet for matchup notes, Poképaste links for team versions, Showdown for testing. **This is the workflow we replace.** It's a dozen tools held together with duct tape. Our workspace is the Notion-shaped consolidation.

**Metafy human coaching:**
[Tier 2] $25-30/hr. Premium ceiling. Tiny addressable market but proves the high-end of WTP. **Implication:** A workspace tool at $15/mo is a 10x cheaper alternative for the person who can't justify a coaching session every week.

---

## Positioning Map

```
                     HIGH WORKSPACE / STATEFUL
                              ▲
                              │
                              │
     (UNOWNED)                │
   "Notion for VGC"           │
   ◄ Our positioning ►        │
                              │
HIGH AI ◄──────────────────────┼──────────────────────► LOW AI / DATA-ONLY
                              │
   VGCCoach (AI but stateless)│   Pikalytics
   ChampTeamAI                │   Showdown
                              │   Smogon
   ChatGPT (generic, low      │   Poképaste
   accuracy)                  │
                              │
                              ▼
                     LOW WORKSPACE / STATELESS
```

The unowned quadrant is **High Workspace + High AI**. Every existing tool sits in one of the other three quadrants. This is where we build.

---

## Three Defensible Unowned Positions (from Wave 2)

1. **Versioned team history with diffs** — every existing tool is stateless or single-snapshot; PokéBase saves teams but doesn't diff them. *"Notion for your VGC team."*
2. **Post-loss reflection, not auto-analysis** — automated replay analysis is technically infeasible (Champions has no replay URLs; see `01-discovery/raw/wave4-technical.md`). But structured manual journaling + grounded AI reflection *is* feasible and unowned. *"The match log that asks the right questions."*
3. **Longitudinal coaching memory** — every product forgets you the moment you close the tab. An AI that has read your last 50 games and your team versions has unique compounding value. **This is the strongest moat available**, and only feasible with a stateful workspace as the substrate.

---

## Platform & GTM Risk

**Platform risk:** Moderate-low. Showdown is open source (MIT) and stable. Pokémon HOME's API is closed but irrelevant to our scope. PokéAPI is open. Smogon stats files are explicit public domain. **The technical substrate is durable.**

**Channel risk:** SEO is dominated by incumbents (Showdown, Smogon, Pikalytics) and by VGCCoach for the "AI coach" narrow query. **Implication:** SEO is a slow long-term play, not a launch channel. Creator partnerships and Reddit organic are the launch channels.

**TPC ships native features risk:** Moderate. TPC's product velocity is historically slow. But Champions' obvious gaps (no replay URL, no team versioning) are exactly what TPC could close in a content patch. **We should assume TPC eventually ships the equivalent of a 5-team save and a basic replay viewer** within 6-12 months. Our wedge has to remain valuable past that point — i.e., AI coaching + longitudinal memory + workflow. Don't build around features TPC will inevitably copy.

---

## Flags

**Red Flags:**
- None. The competitive set is crowded but not consolidated; no funded incumbent exists.

**Yellow Flags:**
- **Speed-to-ship pressure** — competitors are real and shipping. A 6-month build that misses the Worlds-prep demand peak (June-Aug) lands into a much weaker market.
- **VGCCoach owns the "AI coach" SEO narrative** — we cannot win that direct keyword race. We must reposition to "Pokémon team workspace" or "Pokémon prep companion" or similar — a fresh category we own.
- **Pikalytics could ship workspace features** — they've already proven 30-day-ship velocity for Champions. If they add team versioning, our wedge narrows substantially.

## Sources

- `01-discovery/raw/wave2-champions-competitors.md` — full deep dive with URLs (Tier 1 direct observation)
- `01-discovery/raw/wave1-competitors.md` — established incumbent analysis
- `01-discovery/raw/wave2-gtm.md` — channel and creator analysis
- VGCCoach, ChampDex, Champions Lab, PokéBase URLs verified live 2026-05-09
- WolfeyVGC Patreon via Graphtreon (Tier 2)
- Metafy.gg pricing (Tier 1, direct)
