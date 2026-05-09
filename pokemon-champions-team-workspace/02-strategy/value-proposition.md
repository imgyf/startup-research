# Value Proposition

**Phase:** 4 — Strategy
**Project:** pokemon-champions-team-workspace
**Date:** 2026-05-09
**Confidence:** Medium-High (canvas grounded in Phase 3 customer voice; one-sentence prop is opinion until tested)

---

## Value Proposition Canvas

### Customer Profile — VGC Tournament Aspirant (Persona C)

**Jobs (functional, social, emotional)**

- **Functional:** Build, iterate, and remember teams across a tournament season; understand and prepare for archetype matchups; track personal improvement.
- **Social:** Train with partners; share teams with a coach; visibly progress in a community where rating and tournament results carry status.
- **Emotional:** Feel prepared and confident going into a Regional. Avoid the "I tilted into rating loss because I forgot what I learned last season" spiral.

**Pains (in order of intensity, from `target-audience.md`)**

1. Tool fragmentation under tournament pressure — losing hours to context-switching across 5+ tools
2. Champions' broken save model — only 3 free team slots, no version history, EV/IV lock on import
3. Matchup uncertainty — "I keep losing to rain and don't know why"
4. Meta velocity — by the time Smogon analyses update, the meta has moved
5. Counter-team spiral — preparing for one matchup compromises another
6. Lost learning between tournaments — last season's hard-won knowledge fades

**Gains (what they'd love)**

1. One workspace where everything lives — teams, notes, journals, matchup tags
2. AI that explains matchups in plain English with cited sources, never hallucinates moves
3. Calendar awareness — knows the Regional is in 10 days, prioritizes accordingly
4. Visible improvement signals — "you're 60% vs. rain now, was 35% three weeks ago"
5. Coach-mode collaboration — share with a training partner without giving up your team
6. Cross-format continuity — Showdown packed-format compatible, Poképaste-link friendly

---

### Value Map — How We Address Each

**Pain Relievers**

| Pain | Relief |
|---|---|
| Tool fragmentation | Workspace as "single source of truth" — Showdown import, Poképaste export, internal notes/journals/matchup tags all live here |
| Champions broken save | Unlimited team saves on Pro, full version history with diffs, format-aware tags (we hold what Champions doesn't) |
| Matchup uncertainty | AI matchup coach grounded on @pkmn/sim runs and @smogon/calc damage rolls, plus cited Smogon usage data — explains *why* a matchup is bad and what to change |
| Meta velocity | Real-time Smogon stats integration; weekly meta-shift digests for Pro users; archetype tag library updated by community |
| Counter-team spiral | Counter-team builder runs 1000s of @pkmn/sim battles to preview matchup tradeoffs before committing |
| Lost learning between tournaments | Persistent journal — your reflection notes survive seasons, AI synthesizes patterns from your match history |

**Gain Creators**

| Gain | How we create it |
|---|---|
| Single workspace | Notion-shaped UX optimized for VGC team objects |
| Plain-English AI coach | Grounded LLM with simulator-tool calls + source citations; refuses to bluff |
| Calendar awareness | Tournament Prep tier knows your event date; prioritizes prep accordingly |
| Visible improvement | Personal stats over time — win rate vs. archetypes, confidence trends |
| Coach-mode | Shareable team links with role-based read/comment access |
| Cross-format continuity | First-class Showdown packed-format I/O; Poképaste link generation; future Champions Replica Code import (when feasible) |

---

## The One-Sentence Value Prop

Three drafts (in tightening focus):

1. *"A persistent prep workspace and grounded AI coach for serious Pokémon Champions players who want to climb without losing what they learn."*

2. *"Build, version, and prep your VGC teams in one place — with an AI coach that knows your last 50 games and never makes up moves."*

3. **(Recommended)** ***"The prep workspace VGC players actually use between tournaments — your teams, your notes, your AI coach, all the way to Worlds."***

The third is shortest, names the persona ("VGC players"), names the calendar pattern ("between tournaments... to Worlds"), and includes the core delivery ("teams, notes, AI coach"). Test variants in Phase 8.

## High-Concept Pitch (Two-Word Format)

**"Notion for VGC."**

Used selectively in conversations where the audience already knows VGC. The fuller value prop above is for landing-page and creator-partnership pitches.

---

## Proof Points & Credibility Signals

What we'll lead with on a landing page (when each becomes truthfully claimable):

| Signal | When truthful | Where shown |
|---|---|---|
| Built on @pkmn/sim — the same simulator that powers Pokémon Showdown | Day 1 | Hero subhead, FAQ |
| Verified-correct damage calculations (powered by @smogon/calc) | Day 1 | Coach feature page |
| AI cites every source — Smogon usage stats, simulator runs, damage rolls | Day 1 | Coach feature page |
| Advised by [Competitive Player Name] | After advisor recruited (Week 1-2) | Footer + creator section |
| Trusted by 100+ tournament players preparing for [Regional] | After 100 paid users | Hero |
| Used in prep for X teams that top-cut 2026 Regionals | After Regionals end | Hero, social proof |
| Featured in [WolfeyVGC video / Patreon] | After creator deal | Hero, partnership page |

**Critical: never claim signals before they're truthful.** Persona B (Smogon Veteran) is the most allergic to manufactured authority and will publicly call out fluff.

---

## Substitution Equation (Reframing for Sales)

We compete against the *combined* alternative stack:

> **Champions Membership ($4.99/mo, 18 slots, no other features) + Showdown teambuilder (free, but lossy save) + Pikalytics (free, no workspace) + Discord notes + Google Sheets + occasional Metafy session ($25-30/hr) = ~$60-150/mo of fragmented tools and time-cost.**

> **Champion's Notebook Pro ($12/mo) replaces ~80% of that workflow with a single workspace. Tournament Prep ($25/mo) replaces ~95% of it including the coaching layer.**

This framing matters in landing-page copy and creator-partnership pitches. We are not "yet another Pokémon tool" — we are the **consolidator** of an existing ad-hoc stack.

---

## What We're Not

Saying no clearly:

- ❌ **Not a Pokémon Showdown replacement.** We import to/from Showdown. Showdown remains the simulator.
- ❌ **Not a Smogon competitor.** Smogon is the analysis authority. We use their data.
- ❌ **Not a casual team builder.** "Make my Charizard work" is not our job (free tier serves it inbound only).
- ❌ **Not an AI hype tool.** Every AI claim is grounded on sim/calc/stats. Sources cited. No bluffing.
- ❌ **Not an in-game replacement.** Champions stays the game; we sit beside it.

---

## Flags

**Red Flags:**
- None.

**Yellow Flags:**
- The "Notion for VGC" pitch is memorable but assumes audience knows Notion. Doesn't translate well to non-tech-savvy creators or international audiences.
- The substitution equation depends on the user *currently* using a fragmented stack. Persona C does, by definition. But we should validate this in customer interviews (Phase 8 Week 1).
- "AI coach with cited sources, never bluffs" is a strong claim. We must enforce it technically — every AI response in MVP needs to either cite a tool-call result (sim run, damage roll, stat lookup) or say "I don't have a source for this."

## Sources

- `01-discovery/target-audience.md` — JTBD, pain hierarchy, gain framing
- `01-discovery/competitor-landscape.md` — substitution equation
- `02-strategy/lean-canvas.md` — pricing tiers
- `01-discovery/raw/wave4-technical.md` — technical feasibility of "grounded AI"
