# Intake Brief — Pokémon Champions Team Workspace

**Phase:** 1 — Intake
**Project:** pokemon-champions-team-workspace
**Date:** 2026-05-09
**Confidence:** Medium (founder profile clear; market specifics need research)

---

## The Idea

A **persistent team workspace** for the upcoming game *Pokémon Champions* (TPC's standalone competitive battling game, announced Feb 2025 Pokémon Presents). Players save teams, analyze matchups vs. archetypes (rain, stall, hazards, setup, priority endgames), version-track teams across the season, and receive AI-assisted improvement suggestions after losses.

Two segments served from one product surface:

- **Casual players** — guided team building around a favorite Pokémon, with progressive depth (move/item/EV explanations on demand).
- **Competitive players** — deep matchup prep, archetype recognition, counter-team construction, EV/move/item optimization.

The core thesis is that **team building is currently a one-off act** (build → battle → forget) and the opportunity is to convert it into an **ongoing season-long workflow** players return to weekly.

## Problem Framing

**Problem statement:** Existing Pokémon competitive tools (Showdown teambuilder, Pikalytics, damage calcs, paste lists) provide raw data and one-shot calculations but **don't explain *why* a team works**, **don't model the opponent's likely plan**, and **don't help a player improve over time**. The casual-to-competitive funnel is broken — players hit a wall going from "I built a team I like" to "I understand why I keep losing to rain."

**Why now [Assumption]:** *Pokémon Champions* is a TPC first-party launch designed specifically for ranked play, which is expected to (a) bring a fresh wave of casual-to-competitive crossover players who lack mentors, and (b) consolidate competitive activity onto one platform after years of fragmentation across Sword/Shield, Scarlet/Violet, and Showdown.

## The Founder

- **Profile:** Hobbyist Pokémon player (not top-tier competitive) with technical/build skills.
- **Domain edge:** Moderate. Knows the game, plays casually, can ship software. Lacks the "name brand" of Smogon contributors or top-cut players. **[Yellow Flag]** — community trust is currency in this niche; founder will need credible advisors or a named-player partnership.
- **Commitment:** Serious side project, 15-25 hrs/week, ~$500-$2k/month budget, 3-6 month runway before reassessment.

## Target Customer (Initial Hypothesis)

- **Primary persona [Hypothesis]:** "Casual-competitive Pokémon player," age 18-34, plays ranked but struggles to climb past mid-ladder. Watches competitive content (Wolfey, CybertronVGC, Aaron Zheng), uses Showdown occasionally, owns 1+ mainline games, will buy *Champions* at launch.
- **Secondary [Hypothesis]:** Serious VGC/competitive ladder player who currently uses a stack of disconnected tools (Poképaste, Pikalytics, damage calc, Discord notes).
- **Geography:** Global English-speaking first; JP/KR/EU expansion later.

## Existing Alternatives (Initial Map)

- **Pokémon Showdown teambuilder** — free, browser-based, the de facto standard. Strength: huge audience, simulator integrated. Weakness: stateless, no analysis layer, ugly UI.
- **Pikalytics** — usage stats and team archetypes. Strength: data depth. Weakness: read-only, no team workspace.
- **Smogon Strategy Pokédex** — definitive analysis, written by humans. Weakness: format-specific, slow to update, not interactive.
- **Poképaste** — share-only paste hosting. No analysis.
- **Damage calculators** — point-in-time math, not workflow.
- **Discord servers / spreadsheets** — what serious players actually use for tracking. Workflow-shaped but unstructured.

## Business Model (Hypothesis)

Freemium SaaS:
- **Free tier:** save 3 teams, basic matchup tags, community paste import.
- **Pro tier ($5-$8/mo or $40-$60/yr):** unlimited teams, AI matchup analysis, version history, EV/move optimizer, post-loss improvement suggestions.
- **Future:** coach-mode, team sharing/clubs, format-specific premium content.

Revenue ambition (Y1 conservative): 500 paying users at $5/mo = ~$30K ARR. Y2 ambition: 3,000 paying = ~$180K ARR.

## IP/Legal Posture

- Founder elects **standard fan-tool risk** posture — Smogon/Pikalytics-style positioning.
- No sprites, no ROM-derived assets, no logo lookalikes.
- Use generic icons, public Pokédex data (already widely scraped from PokéAPI), and original UI.
- Avoid implying official endorsement.

## Constraints & Preferences

- Mobile-first not required, but mobile-responsive web is needed (players reference teams on phone before matches).
- Tech stack flexible; founder is technical.
- Brand should feel **earnest and competent** — trustworthy to serious players, welcoming to casuals.

## Hard Questions — Founder Self-Assessment

These were not posed live; below are the assumptions under which we're proceeding. Each becomes a validation target.

| Question | Working Assumption | Tag |
|---------|--------------------|-----|
| Why are *you* the right person? | Technical execution + lived player perspective. Not the strongest moat — needs supplemental community credibility (advisor, partnership). | [Assumption] |
| What if a well-funded competitor launches this tomorrow? | Most plausible incumbent attacks: Smogon (community-led, slow to ship product); TPC itself (ships in-game features in Champions). Both reduce upside but unlikely to ship a *workflow* tool quickly. | [Opinion] |
| Strongest argument against this idea? | TPC builds team-management features into *Champions* itself, eliminating the need for a third-party tool. Probability moderate. | [Assumption — needs research] |
| What did real customers say? | None interviewed yet. **Customer discovery is the highest-leverage Week 1 task.** | [Gap] |
| What would make the founder walk away? | Implicit — if Y1 paying users <100 after 6 months of effort, or if TPC ships native team workspace, or if IP risk materializes. To formalize in Phase 8 kill criteria. | [To define] |

## Critical Unknowns to Resolve in Research

1. **Game launch timing & feature scope** — When does *Pokémon Champions* launch? What team-building features ship in-game? (Determines TAM timing and incumbency risk.)
2. **Active competitive Pokémon player count** — How big is the addressable competitive ladder population? (Pikalytics monthly visits, Showdown registered users, VGC tournament participation.)
3. **Willingness-to-pay benchmarks** — Has anyone successfully monetized a Pokémon companion tool? Do players pay for Smogon Premium, Discord boosts, content creators' Patreons?
4. **TPC enforcement posture** — Recent C&D activity vs. companion tools (vs. ROM hacks, which are clearly enforced).
5. **Top 3-5 direct competitors** — Functional comparison and any visible product roadmap signals.

---

## Flags

**Red Flags:**
- None confirmed yet — pending research.

**Yellow Flags:**
- **Founder credibility gap** — moderate-not-strong domain edge in a community where top-tier player association is a major trust signal. Mitigation: recruit a known competitive player as advisor or co-founder before launch.
- **Single-game dependency** — building on top of one specific TPC release means the business is exposed to TPC's product decisions and game lifecycle.
- **Customer discovery zero** — no actual conversations with target users yet. This is the largest knowable risk for any pre-product startup.
- **Free-tool culture** — competitive Pokémon community has strong norms around free, community-built tools. Monetization may face cultural friction even if product value is real.

## Sources
- User intake (this conversation), 2026-05-09.
- Public knowledge (training data) of Pokémon competitive tooling landscape — to be verified in Phase 3 research.
