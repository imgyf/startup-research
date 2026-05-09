# MVP Definition

**Phase:** 6 — Product
**Project:** pokemon-champions-team-workspace
**Date:** 2026-05-09
**Confidence:** Medium-High (scope grounded in Wave 4 feasibility study; effort estimates are inferred)

---

## MVP Hypothesis

> **Tournament-aspiring VGC players will pay $12/mo for a workspace that holds their teams with full version history, lets them journal matchups in plain language, and provides a grounded AI coach that explains *why* matchups are hard — if it ships before Worlds 2026 prep peak (target: late June 2026 public launch).**

The MVP exists to test this hypothesis. It is **not** the eventual product. It is the smallest possible footprint that lets us measure:
- Free → paid conversion at $12/mo
- Persona C activation (do they save 2+ teams in 7 days)
- AI coach trust (do users return to it; what's the hallucination complaint rate)
- Tournament-cycle retention (do they come back for the next tournament)

---

## MVP Must-Haves (Core Features for v1.0)

These are the minimum features required to validate the hypothesis. **Cut anything not on this list.**

### M1 — Account, Team Workspace Foundation
- Email + Google sign-in
- Save unlimited teams (Pro), 5 teams (Free)
- Each team has: name, format/regulation tag, member-Pokémon (species, item, ability, moves, EVs, IVs, nature, Tera type), notes textarea
- Showdown packed-format **import** (paste-in)
- Showdown packed-format **export** (copy-out)
- Poképaste-style public team page (with our branding)

### M2 — Version History (Pro)
- Auto-save on edit; explicit "save version" with optional label
- Version list shows date, optional label, and summary diff
- Diff view: visual side-by-side of two versions of a team
- Restore to previous version (creates a new version, doesn't destroy history)

### M3 — Matchup Tags
- Manual tag taxonomy: rain, sun, sand, snow, trick room, stall, hazards, setup, priority — and free-text user tags
- Each team can be tagged "good vs. X" / "bad vs. X" / "untested"
- Per-tag note (one-line user reflection)
- Filterable by tag

### M4 — AI Matchup Coach (the differentiator)
- Chat-style interface, scoped to a single team
- **Grounding stack:**
  - LLM (Sonnet 4.6 with smart routing to Haiku for cheaper queries)
  - Tool calls to @pkmn/sim (run sim battles for matchup probability)
  - Tool calls to @smogon/calc (specific damage rolls)
  - Retrieval over Smogon usage stats (most recent month + last 3 months)
  - Retrieval over Smogon strategy Pokédex
- **Citation discipline:** every claim must cite a tool-call output OR refuse to answer ("I don't have a source for that")
- Quotas: 10 turns/day Free, 100 turns/day Pro, 500 turns/day Tournament Prep
- Per-turn cost cap (LLM kill-switch on runaway prompts)

### M5 — Manual Match Journal
- After-battle prompt: structured questions (opponent's archetype, my best play, my worst play, what surprised me, what I'd change)
- Free-text reflection field
- AI synthesizes patterns over last N journal entries on request ("show me what's been hurting me lately")
- Journal entries link to the team that played

### M6 — Tournament Prep Mode (basic — Tournament Prep tier)
- Set an active tournament target (date + name)
- Days-to-event countdown on dashboard
- "Prep checklist" surfaces: candidate teams, archetype matchup notes, recent journal entries
- Scoped down: NO meta projection, NO counter-team builder, NO opponent scouting in MVP — those are post-MVP features

### M7 — Billing + Free / Pro / Tournament Prep tiers
- Stripe integration
- $12/mo, $25/mo monthly + annual
- Free → Pro → Tournament Prep upgrade flows
- Cancel anytime
- Email receipts

### M8 — Founder Direct Support
- In-app email link to founder for Year-1 support
- Public Discord for community Q&A (founder is active)

---

## MVP Nice-to-Haves (v1.1, NOT v1.0)

These are tempting but cut from MVP to ship by late June 2026:

- Mobile-native iOS app (web-responsive only at MVP)
- Coach-mode (read/comment sharing) — defer to v1.2
- Counter-team builder — defer
- Meta projection from Regional data — defer
- Opponent scouting — defer
- Spanish localization — defer to v1.3
- Team / club workspaces — defer
- Streamer overlay / OBS integration — defer
- Public team explore / discover feed — defer
- Custom archetype tag definitions (admin) — defer

---

## Explicitly Out of Scope (Do NOT Build)

These are anti-scope items where founder discipline matters most:

- ❌ Battle simulator UI (Showdown's job)
- ❌ Type calculator standalone (Pikalytics has it; we don't compete)
- ❌ Public RMT forum (Smogon's job)
- ❌ Casual fun-team-builder mode (Pulls toward Persona E; never paid acquisition)
- ❌ TCG / Pokémon GO / mainline ranked stats (out of category)
- ❌ Auto-replay analysis (technically infeasible — Champions has no replay URLs)
- ❌ "Build my team for me" generator (vibes; not on-mission)
- ❌ Fortune-telling features ("predict your match outcome!")
- ❌ Tournament organizer tools (out of scope for VGC player workspace)

If a feature request feels exciting but lands here, it's a no.

---

## Success Criteria for MVP

We declare MVP successful **and decide whether to invest a Phase 2 of effort** based on:

| Metric | Target by week 8 of public launch | What it tells us |
|---|---|---|
| Free signups | 1,000+ | Are we reaching Persona C/B audience? |
| Free → Pro conversion (30-day) | ≥2% | Is the hypothesis valid at $12/mo? |
| AI coach usage | ≥20 turns/Pro user/week | Is the coach the actual hook? |
| 4-week paid retention | ≥70% | Is the workspace value sticky? |
| Hallucination complaints | <5% of users | Is groundedness holding? |
| At least one creator partnership active | yes | Is the GTM working? |

**If all 6 met:** validated; invest in v1.1 (mobile, coach-mode, counter-team builder).

**If 4-5 met:** conditionally valid; identify which metric failed and run a focused experiment.

**If ≤3 met:** the hypothesis isn't holding at scale. Consider pivot to a more focused product (e.g., AI coach as standalone tool; or full free utility play with creator content marketplace as monetization).

---

## Build Time Estimate

[From `01-discovery/raw/wave4-technical.md` and Phase 6 scoping above]

| Module | Hours (solo founder, mid-experience) |
|---|---|
| M1 — Account + Workspace | 60-80 |
| M2 — Version history | 30-50 |
| M3 — Matchup tags | 20-30 |
| M4 — AI Matchup Coach (grounded) | 100-140 |
| M5 — Match journal + pattern synthesis | 50-70 |
| M6 — Tournament prep mode (basic) | 30-50 |
| M7 — Billing | 25-40 |
| Design, polish, launch | 40-60 |
| **Total** | **355-520 hours** |

At 15-25 hrs/week, that's a **15-26 week build window**. Compressed to ~12 weeks with creator-locked beta launching at week 6, public launch at week 10-12. **Tight but achievable for the late-June target.**

---

## Critical Build Risks

| Risk | Mitigation |
|---|---|
| AI coach grounding takes longer than estimated | Use VGCCoach's stateless/uncited approach as a forced-floor; ship with limited scope but rigorous grounding before expanding |
| LLM costs balloon | Per-user quotas at MVP; smart routing (Haiku for cheap queries); per-turn cost cap |
| Showdown packed-format edge cases | Use `@pkmn/sets` parser library; test against 50+ real-world team imports before launch |
| Solo-founder velocity assumption breaks | Hire 1 contractor for visual design (~$1,000) at week 4-6 if pacing slips |
| Founder credibility gap | Advisor recruitment in Week 1-2 (already a non-negotiable in Phase 4) |

---

## What v1.1 Looks Like (after MVP validation)

If success criteria are met:

- Coach-mode collaborative sharing
- Counter-team builder (sim-based matchup tradeoff preview)
- Native iOS app
- Meta projection from Regional usage
- Opponent scouting (publicly known top-cut teams)
- Spanish localization
- Public team explore feed (with attribution and creator content)

These are the differentiators that pull retention through the off-season trough and set up the Q1 2027 spike.

---

## Flags

**Red Flags:**
- None.

**Yellow Flags:**
- The 12-week target is tight. If founder velocity falls below 20 hrs/wk, slipping to early August is possible — still survives Worlds-prep window but loses 4-6 weeks of demand spike.
- AI coach module is 30%+ of total build effort. If grounding architecture proves harder than expected, MVP scope must reduce on workspace polish, not on grounding rigor.
- "Manual journaling" replaces auto-replay analysis cleanly *if users actually do it*. We need to validate journaling adoption in closed beta — if users don't journal, the AI synthesis feature loses its substrate.

## Sources

- `01-discovery/raw/wave4-technical.md` — feasibility, build estimates, open-source ingredients
- `02-strategy/lean-canvas.md` — pricing tiers and metrics
- `02-strategy/positioning.md` — must-have category positioning
- `02-strategy/value-proposition.md` — value claims that the MVP must deliver
