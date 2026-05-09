# Idea Scorecard — Final Validation

**Phase:** 8 — Validation
**Project:** pokemon-champions-team-workspace
**Date:** 2026-05-10
**Confidence:** Medium-High (each dimension grounded in Phase 3-7 evidence)

---

## Method

Each dimension is scored 1-10 with explicit rationale grounded in research findings. The overall score determines verdict per the Radical Honesty Protocol:
- **8-10:** Strong signal to proceed
- **6-7:** Conditional proceed with named conditions
- **4-5:** Significant concerns, validate before commitment
- **1-3:** Recommend against proceeding in current form

---

## Scorecard

| Dimension | Score | Rationale |
|---|---|---|
| **Problem severity** | **7** | Tool fragmentation + matchup uncertainty are real, recurring pains for Persona C — corroborated by 5+ Reddit threads and Champions' shipped limitations. But the pain is real-but-painful, not screaming-emergency. Persona C survives without us; they just lose hours per cycle. |
| **Market size** | **5** | TAM proxy (26.79M Scarlet/Violet units) is large but Persona C SOM is 200-1,200 paying Y1. This is a real bootstrap-business size, NOT a venture-scale opportunity. Ceiling appears to be $300-500K ARR Year 2-3. **Honest read:** small but real. |
| **Competitive advantage** | **5** | Three defensible unowned positions identified (versioned history, post-loss reflection, longitudinal memory) — but defensibility depends on flywheels that aren't yet spun up. No funded competitor exists, but 15+ tools shipped in 30 days post-launch. The window is technically open but narrowing. Founder must move fast. |
| **Feasibility** | **8** | Open-source ingredients (@pkmn/sim, @smogon/calc, @pkmn/client) + LLM grounding pattern (PokéLLMon paper validates) make MVP feasible in 12-15 weeks at the founder's commitment level. The killed feature (auto-replay analysis) is explicitly addressed via manual journaling. **Strong score.** |
| **Business model clarity** | **7** | Three-tier freemium with clear pricing rationale anchored in Mobalytics ($7.99) + Wolfey Patreon ($5-10) + Metafy ($25-30/hr) benchmarks. Conversion + retention assumptions inferred from adjacencies, not yet validated. Tier structure is opinionated but coherent. |
| **Founder-market fit** | **5** | Founder is hobbyist player + technical, not tournament-tier. This is the credibility gap Persona C will sense. Mitigation via advisor recruitment is a Week 1-2 task, not a launch task. Without an advisor, drops to 3. With a strong advisor, climbs to 7. **Score reflects current state, not post-mitigation state.** |
| **Timing** | **7** | Game launched 30 days ago; Worlds prep peak is 4 months away; competitive land grab is partway through but not consolidated; no funded incumbent. Tight but real window. Off-season trough creates a real Q2 retention challenge. |
| **Strategic risk** | **6** | TPC native-feature risk is moderate-likelihood, high-impact. Pikalytics could ship workspace anytime. Creator partnership unvalidated. Mitigations are credible but unproven. The risk register is manageable but not negligible. |
| **OVERALL** | **6.25** | **Conditional proceed.** |

---

## Verdict — Conditional Go (Score 6.25 / 10)

**This is a real opportunity, but not a slam-dunk.**

The math works at Base scenario or above, the market is genuinely underserved, and the competitive set is unfunded. The product can ship at the founder's commitment level with the constraints identified.

**However**, this is conditional on **all four** of the following being true within the first 4-6 weeks:

### Condition 1 — Customer-discovery validates the pain framing
*Specific:* From E1 interviews, ≥10/15 confirm tool fragmentation OR matchup uncertainty as a top-2 pain unprompted.
*If invalidated:* The product is solving the wrong problem; pivot or stop.

### Condition 2 — A credible competitive-player advisor signs on
*Specific:* At least one named competitive player with credibility on r/stunfisk and Smogon forums agrees to advise (formal or informal) by end of Week 4.
*If invalidated:* Founder credibility gap is unaddressed; persona C will reject the product. Either co-founder up or pivot away from coaching framing.

### Condition 3 — At least one creator partnership conversation is real
*Specific:* By Week 8, at least one of WolfeyVGC / CybertronVGC / Brady Smith is in active partnership conversation with a non-binding term sheet.
*If invalidated:* GTM rebuild required; ramp slows substantially; Conservative scenario becomes the most likely outcome.

### Condition 4 — Wizard-of-oz coach validates the differentiation
*Specific:* From E7 prototype, ≥5 unique users submit ≥3 questions in 2 weeks AND ≥4/10+ subjectively report the grounded approach as "noticeably different / better" than ChatGPT or VGCCoach.
*If invalidated:* The AI coach is not the differentiator we thought it was. Pivot to pure workspace; reduce ambition to Conservative-tier business.

---

## Why This Score and Not Higher / Lower

**Why not higher (7-8):**
- Founder credibility gap is a real penalty until addressed (-1.0)
- Market size ceiling caps long-term upside vs. venture-scale opportunities (-0.5)
- Tournament Prep tier WTP is the most-sensitive single number and is unvalidated (-0.5)
- Off-season retention through Q2 Y1 is genuinely uncertain (-0.5)

**Why not lower (4-5):**
- The core wedge (workspace + grounded AI coach) addresses real, named pains in a real, paying audience
- Adjacent benchmarks (Mobalytics, Chess.com, WolfeyVGC's Patreon) validate the pattern
- Technical feasibility is high; build cost is bounded
- IP risk is low; entry is unobstructed
- No funded competitor exists today

The score reflects "real opportunity for a side-project bootstrap, real risks that need active management" — not "obviously winning idea" or "obviously losing idea."

---

## Recommended Next Steps

1. **Run E1, E2, E3, E7 concurrently in Weeks 1-6.** These cumulatively address the 4 conditions above.
2. **Decide at Week 6 whether to commit to the full MVP build.** All 4 conditions met → commit. 2-3 met → narrow scope, address weak area, then commit. 0-1 met → pivot or stop.
3. **Set Month 6 (Nov 2026) review meeting with self.** This is the KC5 milestone. Discipline at this checkpoint is the single most important commitment.

---

## Comparison Against Original Idea

The original framing — *"persistent team workspace serving casuals + competitives in one paid product, AI matchup analysis from replays, $5-8/mo pricing"* — would have scored ~3-4 (likely no-go) given Phase 3 findings:

- Casuals + competitives = bifurcated product, broken pricing
- Auto-replay analysis = technically infeasible
- $5-8 pricing = below WTP signal, math doesn't work

The three pivots (tournament-prep persona primary, manual journaling, $12-25/mo) move the score from 3-4 to 6.25. **The pivots are the difference between viable and not.**

---

## Honest Founder-Facing Summary

> You have a real opportunity here — a real audience with real WTP, an active gap in the market, and a feasible MVP. But this is a side-project-to-bootstrap-business size opportunity, not a unicorn. Year 2-3 ARR ceiling is probably $300-500K. Year 1 ARR depends heavily on whether creator partnerships materialize and whether your AI coach actually grounds (i.e., doesn't bluff).
>
> The single most important first step is recruiting a competitive-player advisor — without that, Persona C will sniff out the credibility gap and your conversion math collapses. Spend Week 1-2 on that, not on code.
>
> If you do the four pre-build experiments and 3-4 of them validate, build it. If they don't, pivot or stop early.
>
> Be honest with yourself at the Month 6 milestone. The kill criteria exist for a reason.

---

## Flags

**Red Flags:**
- None at the scorecard level.

**Yellow Flags:**
- A 6.25 score is the lower edge of "conditional proceed." The four conditions above are not optional — they are the basis for the score.
- The founder's emotional investment will increase month over month. The kill-criteria document is a forcing function for honesty at later milestones.
- Year 2-3 ARR ceiling caps the long-run upside. Founder should pursue this expecting a bootstrap-business outcome, not a venture-scale outcome.

## Sources

- All Phase 3 research (`01-discovery/`)
- `02-strategy/lean-canvas.md`, `02-strategy/positioning.md`, `02-strategy/business-model.md`, `02-strategy/go-to-market.md`
- `04-product/mvp-definition.md`, `04-product/feature-prioritization.md`
- `05-financial/revenue-model.md`, `05-financial/projections.md`
- `06-validation/validation-playbook.md`, `06-validation/risk-analysis.md`, `06-validation/kill-criteria.md`
