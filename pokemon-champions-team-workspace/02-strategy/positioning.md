# Positioning

**Phase:** 4 — Strategy
**Project:** pokemon-champions-team-workspace
**Date:** 2026-05-09
**Confidence:** Medium-High (April Dunford framework applied; market category is opinion until tested)

---

## April Dunford Positioning Framework

### 1. Competitive Alternatives

What happens *if we don't exist* — the realistic stack a tournament-prep VGC player uses today:

- **Pokémon Showdown teambuilder** (free, lossy save, no version history)
- **Pikalytics** (free, data-only, no workspace)
- **Champions Membership** ($4.99/mo for 18 team slots, no other workspace features)
- **Smogon Strategy Pokédex + RMT** (free, slow, manual)
- **Discord servers + Google Sheets** for personal notes
- **Poképaste** for share links
- **Occasional Metafy 1-1 coaching** ($25-30/hr)
- **ChatGPT/Claude** for ad-hoc questions (often hallucinates)
- **Among Champions-specific entrants:** VGCCoach (point-in-time scoring, stateless), ChampDex (mobile, light), Champions Lab (sim-focused), PokéBase (community teams)

The tournament-prep player today maintains **5-8 tools** + their own discipline. None of these tools share state. The player is the integration layer.

### 2. Unique Attributes

What we have that the competitive alternatives don't:

| Attribute | We have | Alternatives |
|---|---|---|
| **Persistent versioned team workspace** | Yes (unlimited on Pro, with diffs and tags) | Showdown saves stateless; Pikalytics no save; Champions $4.99/mo for 18 slots; PokéBase saves but no diffs |
| **AI matchup coach grounded on @pkmn/sim + @smogon/calc + cited sources** | Yes (every claim cited; refuses to bluff) | VGCCoach has AI but stateless and uncited; ChatGPT hallucinates; no incumbent has rigorous grounded coaching |
| **Manual match journaling with pattern synthesis** | Yes (structured prompts; AI synthesizes patterns over N games) | Reportworm has stats only; no one has reflection workflow |
| **Calendar-aware tournament-prep mode** | Yes (Tournament Prep tier) | No tool integrates the VGC tournament calendar |
| **Cross-format Showdown ↔ Champions sync** | Yes (packed-format I/O at MVP, Replica Code import as Champions data permits) | No tool bridges both natively |
| **Coach-mode collaborative sharing** | Yes (read/comment access for training partner) | Discord + Poképaste links; not collaborative |
| **Workspace optimized as a "first-class object," not a side feature** | Yes | Every other tool treats team-save as a tab in a larger product |

### 3. Value (What Those Attributes Enable for Customers)

Translating attributes to outcomes:

- **Stop losing prep work between tournaments.** Version history + tags + journals mean the season's learning compounds rather than evaporating.
- **Understand *why* a matchup is hard, not just that it is.** Cited AI coaching turns "I keep losing to rain" into "rain pressures your slow grass-types in turns 3-5; here are 3 pivots."
- **Replace the 5-8 tool ad-hoc stack with one workspace.** Save 2-4 hours per tournament cycle in context-switching alone.
- **Carry your prep across formats.** Move from Showdown ladder testing to Champions ranked without re-typing teams.
- **Share with a coach or training partner without giving up your team to a public link.**
- **Trust the AI.** Sources cited. Sim runs visible. No bluffs.

These are *operational* benefits — the kind that compound week-over-week, not exciting demo moments. That fits the JTBD: tournament-prep is a recurring grind, not a flash-of-insight problem.

### 4. Target Market — Who Cares the Most

We will NOT try to be everything to everyone. The cleanest version of the target market:

> **English-speaking VGC tournament aspirants (Persona C) — players who are climbing toward a Regional, International, or Worlds spot in 2026-2027, who already pay for at least one creator Patreon or Pokémon HOME Premium, and who currently maintain a fragmented prep stack across 5+ tools.**

Secondary: **Smogon Veterans Crossing Over to Champions (Persona B)** — for credibility and word-of-mouth on r/stunfisk and Smogon forums.

Explicitly NOT our paid target: Casual Favorite-Builders. Their pain is real, but their WTP is near-zero and their feature requests pull product toward subjective vibes.

### 5. Market Category

**The hardest cell — the one that determines whether we get found.**

#### Category candidates considered

1. **"Pokémon AI coach"** — VGCCoach owns this. Direct head-on attack is unwinnable on SEO.
2. **"Pokémon team builder"** — Showdown is the gravitational center. Unwinnable.
3. **"Pokémon competitive workspace"** — descriptive but unsearched (zero existing demand for the term).
4. **"VGC prep workspace"** — narrow but accurate to our target persona; could create demand.
5. **"Pokémon tournament prep app"** — closer to the JTBD; more searchable; less crowded.
6. **"VGC notebook"** — short, memorable, on-brand; creates fresh category.

#### Selected positioning

> ***A VGC prep notebook — the workspace serious Pokémon Champions players use between tournaments.***

**Why this category:**
- It carves a fresh space. We're not "another Pokémon tool" — we're a **notebook** (workspace metaphor) for a **specific lifecycle** (between tournaments). No incumbent owns this framing.
- It carries the workflow promise (notebook = persistent, organized) and the audience marker (VGC = serious, format-aware).
- It SEO-supports content marketing — "VGC prep notebook," "VGC tournament prep," "Pokémon Champions prep" are all winnable long-tail terms.
- "Notebook" is calm, capable language — not "AI coach hype." Suits the tone needed for Persona B trust.

**What this means for product decisions:**
- The home tab is a journal/notebook view, not a teambuilder
- Onboarding starts with "name your tournament" or "name your goal," not "build a team"
- Marketing copy leans on "between tournaments," "the notebook," "prep continuity"
- We avoid the "AI coach" headline (let VGCCoach own that); we use "your AI assistant" as a feature, not a category

---

## Positioning Statement

**For** VGC tournament aspirants
**Who** lose hours to fragmented prep across 5+ tools and can't tell why their matchups slip
**Champion's Notebook** is a persistent prep workspace and grounded AI assistant
**That** consolidates teams, version history, matchup notes, and post-game reflections into one place — between tournaments, all the way to Worlds.
**Unlike** Showdown's stateless teambuilder, Pikalytics' read-only stats, or generic AI coaches that hallucinate moves
**We** are built on the same simulator pros trust, cite every source, and never forget what you've learned.

---

## Competitive Frame in One Slide

```
                  ┌──────────────────────────────────┐
                  │         AI / Coaching            │
                  │                                  │
   VGCCoach ●     │   ●  Champion's Notebook       │
   ChampTeamAI ●  │      (HIGH WORKSPACE +          │
                  │       HIGH AI + WORKFLOW)       │
                  │                                  │
   ───────────────┼──────────────────────────────────┼──────────
                  │                                  │
   Showdown ●     │   PokéBase ●                    │
   Smogon ●       │   ChampDex (iOS) ●              │
   Pikalytics ●   │                                  │
                  │         Workspace / Stateful     │
                  └──────────────────────────────────┘
                  Stateless / Single-snapshot

       Generic AI            ←→             Pokémon-grounded AI
```

---

## "Anti-positioning" — What We Will Be Mistaken For (and how we correct)

| Mistaken as | Why it happens | How we correct |
|---|---|---|
| "Just another Pokémon AI coach" | The land grab is loud | Lead with "notebook," not "AI coach" |
| "A Showdown alternative" | Workspace overlap | Always frame as "imports from Showdown" |
| "Pikalytics with a UI" | Surface comparison | Emphasize workflow + journaling |
| "ChatGPT for Pokémon" | LLM coaching everywhere | Show citations, sim runs, calc rolls — visibly grounded |
| "A casual onboarding tool" | If we lean too hard on free tier | Tournament Prep tier copy is dead serious |

---

## Brand Adjacency Check (input to Phase 5)

The positioning implies a brand that feels:
- **Earnest, not flashy** — VGC tournament aspirants are skeptical of marketing energy
- **Capable, not magical** — workflow over wow-moments
- **Grounded, not hype** — the AI claim must feel like "Stockfish for Pokémon," not "AI changes everything"
- **Communal, not corporate** — built with players, for players
- **Quiet confidence, not aggressive** — leave the loud branding to lesser tools

Phase 5 brand work should reflect these adjacencies.

---

## Flags

**Red Flags:**
- None.

**Yellow Flags:**
- "Notebook" is a fresh category — fresh categories take time to land. Early SEO traffic will be thin until the brand earns its term.
- VGC is a smaller community-of-aware than "Pokémon" generally. "VGC prep notebook" is precise but limits inbound from broader Pokémon-curious search traffic. Trade we accept for sharper positioning.
- The positioning leans heavily on "grounded AI." If we ship LLM features that bluff, the entire positioning collapses. Phase 6 product engineering must enforce groundedness as a hard constraint.

## Sources

- April Dunford, *Obviously Awesome* — positioning framework
- `01-discovery/competitor-landscape.md` — alternative-set + positioning map
- `01-discovery/target-audience.md` — Persona C profile
- `02-strategy/value-proposition.md` — substitution equation, value claims
- `01-discovery/raw/wave2-gtm.md` — SEO category analysis
