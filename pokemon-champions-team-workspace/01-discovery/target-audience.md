# Target Audience

**Phase:** 3 — Discovery
**Project:** pokemon-champions-team-workspace
**Date:** 2026-05-09
**Confidence:** Medium-High (verbatim Reddit pains corroborated; persona segmentation is data-informed inference)

---

## Persona Hierarchy — Decision Summary

We segment the market into seven personas (full detail in `01-discovery/raw/wave3-personas.md`). Of these, three matter for launch:

| Code | Persona | TAM share | WTP | Launch role |
|---|---|---|---|---|
| **C** | **VGC Tournament Aspirant** | ~5% | High ($15-25/mo demonstrated) | **PRIMARY** |
| **B** | **Smogon Veteran Crossing Over** | ~10% | Medium ($8-12/mo) | **SECONDARY (credibility)** |
| **E** | Casual Favorite-Builder | ~50% | Near-zero | **DO NOT chase paid** (free-tier inbound only) |

The other personas (Bricked Champions Casual A, Returning Lapsed Player D, Coach Buyer F, Streamer G) are *served as a side-effect* of building well for C and B but are not paid-acquisition targets.

---

## Primary Persona — C: VGC Tournament Aspirant

### Snapshot

- **Name:** Tournament-Aspiring Trainer (TAT)
- **Age:** 19-32
- **Geography:** US/Canada/UK first; Western Europe + AUS/NZ secondary; Latam tertiary
- **Devices:** Switch 2 + Phone (looks at prep on phone), often Laptop for deep planning
- **Time pattern:** Heavy 5-10 days before each Regional/International event; light during quiet months

### Currently Spends On

- Pokémon HOME Premium ($16/yr) — already a paying customer of Pokémon-adjacent SaaS
- 2-3 creator Patreons: WolfeyVGC ($5-10/mo), CybertronVGC, Brady Smith / VGC Corner ($X/mo, 206 paid Patrons in his tier per Graphtreon — Tier 2)
- Occasional Metafy 1-1 coaching sessions ($25-30/hr)
- Tournament travel (flights + entries) for 2-4 events/year

**Total Pokémon-adjacent monthly spend: $30-100/mo** — a $15/mo workspace tool fits comfortably under existing budget.

### Job-To-Be-Done (verbatim framing)

> *"When I have a Regional in 10 days, I want a workspace that holds my candidate teams, the meta data I'm tracking, my matchup notes against each archetype I expect to see, and my counter-team experiments — so I don't lose a week of prep to scattered Discord notes and forgotten Showdown teams."*

### Pain Hierarchy (corroborated from Reddit, Smogon, Twitter)

1. **Tool fragmentation under tournament pressure** — "I have teams in Showdown, notes in Discord, pastes in a Google Doc, replays I can't actually save." Mentioned across 5+ Reddit threads.
2. **Champions' broken save model** — 3 free team slots; $4.99/mo Membership for 18; EV/IV lock on import; no version history. Direct, recent pain.
3. **Matchup uncertainty** — "I keep losing to rain and I can't tell what specifically I'm doing wrong." Verbatim sourced. The strongest single wedge.
4. **Meta velocity** — "By the time the Smogon analysis updates, the meta has already shifted." Real complaint about lag between top-cut tournament results and content publication.
5. **Counter-team spiral** — preparing for an opponent's likely team without losing match-up fitness vs. the rest of the field.

### Channel Map

- **Reddit:** r/stunfisk (257K members, primary discussion), r/PokemonChampions (launch-window land grab), r/VGC (smaller, more competitive)
- **Discord:** Pokémon Champions VGC server (~5K+ members), Smogon Discord (54K), individual creator Discords
- **Twitter/X:** comp Pokémon hashtag culture, #VGC2026
- **YouTube:** Wolfey, Cybertron, Brady Smith, EmbCommanderVGC, Aaron Zheng
- **Streaming:** Twitch around tournament weekends; not a primary discovery channel
- **Tournament events:** Limitless / Play! Pokémon Regionals, Internationals — physical word-of-mouth at Regionals matters

### Triggers — When They Reach for a Tool

1. **Tournament announced** (Regional or Worlds Qualifier) — opens 2-week prep window. *Highest-intent moment.*
2. **Lose 3+ in a row on Champions ranked** (or Showdown ladder) — frustration spike, seeks help.
3. **Meta shift after a major tournament** — pro player wins with novel team; whole community reorients.
4. **New creator content drops** — Wolfey video describing a meta archetype.

### Conversion Triggers (Free → Paid)

- Hitting team-slot limit (we set free at 3-5 saved teams; pro at 50+)
- Wanting AI coaching beyond a daily quota
- Wanting version history beyond last 3 versions
- Tournament-prep mode: meta projection, counter-team builder, opponent scouting

### Churn Triggers

- TPC ships native team management in a Champions update
- Tournament season ends and they coast through the off-season
- A creator-endorsed competitor launches with feature parity

### What We Build for Them (Top 5 Features)

1. **Team workspace with version history** + diff view + tags ("for Indianapolis," "vs. rain decks")
2. **AI matchup coach** that explains *why* a matchup is bad in plain English, grounded on @pkmn/sim + @smogon/calc
3. **Manual match journaling** — structured reflection prompts after a game; AI then synthesizes patterns over the last N games
4. **Tournament-prep mode** — calendar-aware: pulls recent regional usage data into your prep, helps build counter-cores
5. **Team sharing & paste import/export** — Showdown packed format, Poképaste link generation, optional team sharing with a coach/training partner

---

## Secondary Persona — B: Smogon Veteran Crossing Over

### Snapshot

- **Name:** Smogon Veteran (SV)
- **Profile:** Long-time Showdown ladder competitor (often 5+ years on Smogon), now also playing Champions on Switch
- **Identity:** Skeptical of "AI hype" tools. Values rigor, simulation accuracy, references to Smogon analyses.
- **WTP:** $8-12/mo. Will pay if convinced of substance, will publicly call out fluff.

### JTBD

> *"When I'm running parallel Showdown and Champions ladders, I want one workspace where my teams live in both formats and the matchup analysis is *actually correct* — not LLM hallucinations."*

### Why They Matter Strategically

Their endorsement carries disproportionate weight on r/stunfisk (257K) and Smogon forums. A handful of SV testimonials ("I'm a 1700+ Smogon ladder player and this workspace actually saves me hours") is worth more than 50 casual reviews. **Use them as beta testers and case studies before paid launch.**

### Differentiators They'll Care About

- @pkmn/sim integration accuracy (no hallucinations on EV spreads, abilities)
- Smogon set imports (one-click import of "OU sample teams" or "VGC Reg G samples")
- Showdown packed-format compatibility (round-trip without data loss)
- Visible source citations on AI claims ("This counter is from Smogon Reg G usage stats, June 2026")

### Risk

If we ship LLM coaching that hallucinates competitive Pokémon facts, this segment is the loudest critic — their negative reviews will spread fast. **Build with rigor or don't go after them.**

---

## Anti-Persona — E: Casual Favorite-Builder (DO NOT chase as paid)

### Why They're Tempting

Largest TAM by far (~50% of Pokémon Champions buyers). High emotional engagement. Vocal on Reddit/Twitter ("how do I make Charizard work?"). Marketing copy could lean on them easily.

### Why We Don't Chase Them

- **Near-zero WTP.** They expect tools to be free. Pikalytics, Showdown, Smogon all are.
- **Pull product toward vibes, not rigor** — feature requests like "make my Vaporeon work" are subjective and irreducible. Building for them dilutes everything Persona C and B value.
- **Low retention** — they want one team for fun, not a season-long workflow. Once they have "their team," they don't return.
- **No sharp triggers** — no calendar urgency, no defined success metric.

### How We Still Serve Them

- **Free tier as inbound funnel** — they search "best Charizard build Pokemon Champions," land on a free public-team page, see our product. Some convert later when they get more serious.
- **SEO long-tail** — landing pages per favorite Pokémon are cheap to produce and serve this audience without distorting product.
- **Never run paid acquisition against them.** Never build features for them that aren't byproducts.

---

## Verbatim Language Map (for marketing copy)

Real user phrases mined from Reddit and Twitter (Tier 3 sources but corroborated across multiple threads):

- *"I think they match you up with bots after a couple of losses, I just can't prove it"* — the "I don't understand why I'm losing" phenomenon
- *"My team disappeared after closing Showdown again"* — Showdown's perennial save bug
- *"Competitive is going to suck for a while"* — Joe Merrick (Serebii) on Champions launch state
- *"I have like five different places I keep team notes"* — tool fragmentation
- *"I know I'm bad against rain but I don't know how to fix it"* — the matchup-analysis wedge
- *"By the time Smogon updates the analysis the meta has already moved on"* — content lag complaint
- *"I'd actually pay for this if it remembered my battles"* — overheard WTP signal in r/stunfisk replies (paraphrased composite)

These should anchor headline copy and onboarding microcopy.

---

## Buying Behavior

- **Decision criteria** (in order): creator endorsement → trusted-player review → Reddit thread testimonial → SEO discovery
- **Trial behavior:** Will try free tier 1-2 times before committing. Onboarding has to deliver value in <5 minutes.
- **Purchase moment:** Almost always after a specific frustrating event (hit team-slot limit, lost a streak, has a tournament next week).
- **Annual vs. monthly:** Tournament-prep persona buys annual when their tournament season is announced. Otherwise monthly.
- **Word-of-mouth:** Strongest within Discord communities and during tournament Discord chatter. Direct sharing of paste links could be a viral mechanic.

---

## Geographic Strategy

- **Phase 1 (months 1-6):** English-only. US/Canada/UK/AUS as primary geos.
- **Phase 2 (months 7-12):** Spanish (large Latam VGC scene; Victory Road bilingual partnership).
- **Phase 3 (year 2):** Japanese (Pokémon Champions launches in Japan with strong native scene; requires localization investment + cultural credibility).
- **Korean** is high-density competitive but small absolute market; deprioritize until y2.

---

## Flags

**Red Flags:**
- None.

**Yellow Flags:**
- **Persona C is small in absolute terms.** Estimated SOM is 200-1,200 paying users in Year 1. The business model must work at this scale; don't plan around 10K customers in Year 1.
- **Founder-persona credibility mismatch.** Founder is "hobbyist player" — not a tournament-tier player. Persona C will sniff this out fast. **Mitigation: recruit a competitive-player advisor before launch and credit them visibly on the product.**
- **Champions native upgrades** — TPC adds team versioning to Champions in a content patch and we lose ~30% of the workflow value. Mitigation: lean on AI coaching + cross-format sync + creator-content layers as moats that TPC won't ship.

## Sources

- `01-discovery/raw/wave3-personas.md` — Persona deep-dive (Tier 2/3 from Reddit/Discord/Twitter mining)
- `01-discovery/raw/wave1-customer.md` — Verbatim pain quotes
- WolfeyVGC, Brady Smith Patreon Tiers via Graphtreon (Tier 2)
- Reddit: r/stunfisk, r/PokemonChampions, r/VGC threads (Tier 3)
- Joe Merrick / Serebii public commentary on Champions launch (Tier 2)
