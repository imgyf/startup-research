# Pokémon Champions Team Workspace — Executive Summary

**Project:** pokemon-champions-team-workspace
**Working name:** Champion's Notebook
**Date:** 2026-05-10
**Verdict:** **CONDITIONAL GO** (Score 6.25 / 10) — proceed if 4 named conditions are met in Weeks 1-6

---

## One-Paragraph Overview

A persistent prep workspace and grounded AI coach for serious VGC tournament players competing in *Pokémon Champions* (TPC's standalone competitive battling game, launched April 8, 2026). The product consolidates a player's teams, version history, matchup notes, and post-game journaling into one workspace — and pairs it with an AI assistant grounded on the @pkmn/sim simulator and @smogon/calc damage calculator that explains *why* matchups are hard, with cited sources, no hallucinations. Free tier (5 teams, basic AI Q&A) acts as inbound funnel; Pro ($12/mo) is the daily-driver workspace; Tournament Prep ($25/mo) adds meta projection, counter-team builder, and coach-mode collaboration. Target launch is **late June 2026** — into the Worlds 2026 prep peak (Aug 28-30).

---

## Key Findings From Research

1. **The wedge is real and recent.** *Pokémon Champions* launched April 8, 2026 with deliberate gaps: only 3 free team slots, $4.99/mo for 18 slots, no replay URLs, no version history, no coaching layer. Reviews mediocre (Metacritic 65 / OpenCritic 58). Players are actively frustrated *right now*.

2. **WTP is concretely demonstrated.** WolfeyVGC has 10,893 paid Patrons (added 5,706 in 30 days post-launch). Brady Smith has 206+ in a single tier. Metafy charges $25-30/hr for Pokémon coaching. Mobalytics (LoL companion adjacency) was acquired by ESL FACEIT in March 2025.

3. **No funded competitor exists.** All 15+ Champions-specific tools shipped in the first 30 days are solo-founder or hobbyist projects. The land grab is partway through, not consolidated.

4. **Three defensible unowned positions:** (a) versioned team history with diffs ("Notion for VGC"), (b) post-loss reflection via manual journaling + AI synthesis (auto-replay analysis is infeasible — Champions has no replay URLs), (c) longitudinal coaching memory.

5. **Standard fan-tool IP risk.** TPC has not C&D'd Showdown / Smogon / Pikalytics in 15+ years. Standard posture is appropriate.

6. **Original idea required three pivots to be viable:**
   - Pivot 1: Target tournament-prep persona (Persona C), not casual market (Persona E)
   - Pivot 2: Manual match journaling, not auto-replay analysis
   - Pivot 3: Pricing $12/$25, not $5-8

---

## Strategic Positioning Summary

**Category created:** *VGC prep notebook — the workspace serious Pokémon Champions players use between tournaments.*

**Positioning statement:**
> For VGC tournament aspirants who lose hours to fragmented prep across 5+ tools and can't tell why their matchups slip, **Champion's Notebook** is a persistent prep workspace and grounded AI assistant that consolidates teams, version history, matchup notes, and reflection journals into one place — between tournaments, all the way to Worlds.
> Unlike Showdown's stateless teambuilder, Pikalytics' read-only stats, or generic AI coaches that hallucinate moves, we are built on the same simulator pros trust, cite every source, and never forget what you've learned.

**Brand archetype:** Sage (truth, citations, earned expertise) + Caregiver secondary (custodial of your prep work). Visual references: Lichess, Linear, Notion. Voice: earnest, capable, grounded, calm.

---

## Top 3 Risks and Mitigations

### Risk 1 — Founder credibility gap (Medium / High)
The founder is a hobbyist player + technical builder, not a tournament-tier player. Persona C will sense this.
**Mitigation:** Recruit a named competitive-player advisor in Week 1-2. Non-negotiable.

### Risk 2 — TPC ships native team management within 6-12 months (Medium / High)
Could erase ~30% of value prop overnight.
**Mitigation:** Build moats TPC won't replicate quickly — AI coaching grounded on @pkmn/sim, longitudinal memory, cross-format (Showdown ↔ Champions) sync.

### Risk 3 — All 3 top creator partnerships decline (Medium / High)
Creator partnerships are the highest-leverage acquisition channel. Without them, GTM ramp slows substantially toward Conservative scenario.
**Mitigation:** Pursue 3 in parallel (Wolfey, Cybertron, Brady Smith); have a smaller-creator backup pool of 5+ ranked candidates; have content + tournament sponsorship as Plan B GTM.

---

## Confidence Dashboard Summary

**Solid ground (high confidence):**
- Pokémon Champions launch state and gaps
- WTP exists in this community
- No funded competitor in the field
- IP risk is moderate-low
- Tournament calendar is concrete
- Open-source ingredients are real and current

**Thin ice (low confidence — must validate):**
- SOM estimate (200-1,200 paying users Y1)
- Persona C TAM share (~5%)
- Tournament Prep tier $25 WTP
- Creator partnership viability
- Manual journaling adoption rate
- Off-season retention rates

Full detail in `01-discovery/confidence-dashboard.md`.

---

## Generated Documents

### Phase 1 — Intake
- [`00-intake/brief.md`](00-intake/brief.md) — Idea, founder profile, target customer hypothesis, IP posture, unknowns
- [`00-intake/brainstorm.md`](00-intake/brainstorm.md) — 8 idea variations, convergence on hybrid approach

### Phase 3 — Discovery
- [`01-discovery/market-analysis.md`](01-discovery/market-analysis.md) — TAM/SAM/SOM, growth, monetization benchmarks, regulatory
- [`01-discovery/competitor-landscape.md`](01-discovery/competitor-landscape.md) — Comparison matrix, deep dives on incumbents and 15+ Champions-specific entrants
- [`01-discovery/target-audience.md`](01-discovery/target-audience.md) — Persona C/B/E definitions, JTBD, channels, triggers
- [`01-discovery/industry-trends.md`](01-discovery/industry-trends.md) — Trend analysis: esports companion category, LLM coaching, tournament cycles
- [`01-discovery/confidence-dashboard.md`](01-discovery/confidence-dashboard.md) — Full claims-to-source mapping
- [`01-discovery/verification-report.md`](01-discovery/verification-report.md) — PASS WITH WARNINGS
- [`01-discovery/research-gate.md`](01-discovery/research-gate.md) — YELLOW LIGHT (Conditional GO with three pivots)
- [`01-discovery/raw/*`](01-discovery/raw/) — Wave 1-4 raw research with source URLs

### Phase 4 — Strategy
- [`02-strategy/lean-canvas.md`](02-strategy/lean-canvas.md) — Full Lean Canvas with risk heat map
- [`02-strategy/value-proposition.md`](02-strategy/value-proposition.md) — Value Proposition Canvas, one-sentence prop, substitution equation
- [`02-strategy/business-model.md`](02-strategy/business-model.md) — Three-tier pricing, unit economics, scalability
- [`02-strategy/positioning.md`](02-strategy/positioning.md) — April Dunford framework, category creation
- [`02-strategy/go-to-market.md`](02-strategy/go-to-market.md) — Tournament-calendar GTM, channels ranked, creator partnership plan

### Phase 5 — Brand
- [`03-brand/mission-vision-values.md`](03-brand/mission-vision-values.md) — Mission, vision, 5 values with decision-test framing
- [`03-brand/tone-of-voice.md`](03-brand/tone-of-voice.md) — Voice principles, vocabulary guide, sample copy across touchpoints
- [`03-brand/brand-personality.md`](03-brand/brand-personality.md) — Sage archetype, visual direction, brand adjacencies

### Phase 6 — Product
- [`04-product/mvp-definition.md`](04-product/mvp-definition.md) — Must-haves, nice-to-haves, anti-scope, success criteria
- [`04-product/feature-prioritization.md`](04-product/feature-prioritization.md) — RICE + MoSCoW, 12-week build sequence
- [`04-product/user-journey.md`](04-product/user-journey.md) — End-to-end persona journey, aha moment, failure modes

### Phase 7 — Financial
- [`05-financial/revenue-model.md`](05-financial/revenue-model.md) — Three scenarios (Conservative $20K, Base $60K, Optimistic $150K Y1)
- [`05-financial/cost-structure.md`](05-financial/cost-structure.md) — Fixed + variable + one-time costs; LLM cost dynamics
- [`05-financial/projections.md`](05-financial/projections.md) — Quarterly cash flow + Y2-Y3 outlook + funding analysis

### Phase 8 — Validation
- [`06-validation/validation-playbook.md`](06-validation/validation-playbook.md) — 10 experiments sequenced cheapest-fastest-first
- [`06-validation/risk-analysis.md`](06-validation/risk-analysis.md) — Full risk matrix + top-5 mitigation plans
- [`06-validation/assumptions-tracker.md`](06-validation/assumptions-tracker.md) — 25 critical assumptions with status
- [`06-validation/experiment-design.md`](06-validation/experiment-design.md) — Top 3 experiments designed in detail
- [`06-validation/kill-criteria.md`](06-validation/kill-criteria.md) — 8 hard + 6 soft kill triggers
- [`06-validation/scorecard.md`](06-validation/scorecard.md) — Final 6.25/10 verdict with conditions

### Action Plan
- [`action-plan-30-days.md`](action-plan-30-days.md) — Week-by-week first-month plan

### Progress Tracking
- [`PROGRESS.md`](PROGRESS.md) — Phase completion status

---

## Anti-Patterns Detected

This idea showed early warning signs of common founder anti-patterns. Each was addressed:

| Anti-Pattern | Where it appeared | How addressed |
|---|---|---|
| **Boiling the ocean** | Original idea served casuals + competitives in one paid product | Pivot 1: Tournament-prep persona only; casuals as inbound funnel |
| **Solution looking for a problem** | "Auto-replay analysis" was the headline differentiator | Pivot 2: Manual journaling addresses same JTBD given data constraints |
| **Vanity metrics risk** | Initial framing leaned on "downloads" and "engagement" | Switched North Star to **Weekly Active Paid Users**, retention curves over 4-week post-tournament window |
| **Premature scaling** | Initial plan included native iOS at MVP | Mobile-responsive web only at MVP; native iOS as Year-1 follow-up |
| **Ignoring unit economics** | Initial $5-8/mo pricing didn't cover LLM costs at margin | Pivot 3: $12/$25 pricing aligns with WTP benchmarks |
| **Building in stealth too long** | Plan implied 6-month closed build before any user contact | Restructured around Week 1 customer discovery + closed beta in Weeks 4-6 |

---

## What Success Looks Like

**Year 1 (July 2026 - June 2027):**
- 12,000 free signups (Base scenario)
- 400 paying users acquired
- $60K revenue, $40K net cash, MRR ~$3,900 by year-end
- One creator partnership active
- Named competitive-player advisor on the team
- 4-week paid retention >70%
- AI coach hallucination rate <5%

**Year 2:**
- $150-300K ARR
- v1.1 (coach-mode, counter-team builder, meta projection) shipped
- v1.2 (mobile-native iOS, Spanish localization) shipping
- Creator content marketplace launches
- Founder considers contractor or co-founder for product velocity

**Year 3 (aspirational):**
- $400-600K ARR
- Bootstrap-business viability with optional path to small seed round if generalization plan is credible

---

## What Failure Looks Like

If the project lands at Conservative scenario (Y1 ARR <$25K) and kill criterion KC5 fires at Month 6, the founder should:

1. Run a sunset analysis honestly
2. Open conversations with key paying users about a 1-year-prepaid sunset model OR soft acquisition
3. Wind down gracefully, write a public retrospective
4. Reclaim 15-25 hrs/week for higher-leverage work

The kill-criteria doc exists to make this easier when the time comes. It's not pessimism — it's protecting the founder's time from sunk-cost continuation.

---

## Next Steps

See [`action-plan-30-days.md`](action-plan-30-days.md). The first month is **NOT a build month**. It's a customer-discovery + creator-outreach + advisor-recruitment month, with a wizard-of-oz coach prototype as the only "build" task.

Build commits at Week 6 only after the four scorecard conditions are validated.

---

## Final Honest Assessment

This is a **real opportunity for a side-project bootstrap business**, not a unicorn. Year 1 economic profit is realistically -$10K to +$70K depending on scenario. Year 2-3 caps at $300-500K ARR most likely. Pursue this if:

- You enjoy the problem space and would be playing competitive Pokémon anyway
- You're committed to running the four pre-build experiments before committing to a 12-week build
- You're willing to recruit a competitive-player advisor in Week 1-2
- You're disciplined about the kill criteria at Month 6
- You're OK with the bootstrap-business ceiling

Don't pursue this if:

- You expected a venture-scale outcome
- You can't or won't recruit an advisor
- You're not willing to delay building until Week 6 customer-discovery validates
- You can't sustain 15-25 hrs/week for 12+ weeks

---

*Generated through the startup-design skill (v1.0) — Full Mode, Deep research tier, all 8 phases completed 2026-05-09 to 2026-05-10.*
