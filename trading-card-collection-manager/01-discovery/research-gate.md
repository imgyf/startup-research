# Research Gate — Go / Pivot / Stop Decision

**Phase:** 3.5 — Research Gate
**Project:** trading-card-collection-manager
**Date:** 2026-05-10

---

## What the Research Found

After Wave 1 (market sizing + trends) and Wave 2 (direct competitors + indirect/platform risk + GTM), the picture is clearer than the founder's pitch suggested:

### Things that argue FOR proceeding
- **Real demand at scale.** Collectr at 4M users (bootstrapped) and CollX at $10M Series A confirm a paid market exists.
- **Founder ceiling is reachable.** US SAM of $10–40M ARR comfortably contains the founder's stated $100–500K/year target. This is a lifestyle-business sized opportunity that fits side-project pace if executed for 18+ months.
- **Tech is in the founder's favor.** Card recognition is commoditized at near-zero cost. A capable mobile dev can ship a competitive scanner in weeks, not months.
- **Identifiable wedge exists.** "Pokemon-only depth + eBay sold-comp pricing + custom price alerts + modern UX" — no current competitor combines all four. Two independent research agents converged on this same wedge.
- **Pokemon TCG Pocket (100M+ users)** is a genuine, underexploited top-of-funnel.
- **Asset-class framing is mainstream.** Customer culture is primed for portfolio-tracking tools.

### Things that argue AGAINST proceeding
- **Data-access cliff is the most material finding.** TCGplayer + eBay APIs closed/restricted for new partners. The founder's headline real-time-pricing feature has structural cost ($50–500/mo paid aggregators) or legal risk (scraping). This was not in the original pitch.
- **PSA/Collectors is a structurally subsidized competitor.** Card Ladder under PSA can run a competing tracker at negative margin to feed grading volume. The threat clock is 12–18 months for raw-card.
- **Two doppelgangers already ship the founder's pitch.** Shiny and PokeScope are Pokemon-native scan + portfolio + custom alerts + eBay sold-comp apps. Differentiation must come from execution speed, depth, or community — not feature-level novelty.
- **Founder is light-collector.** Community trust must be earned from zero. Side-project pace makes this slower.
- **CAC <$30 ceiling means paid acquisition is essentially infeasible.** Strategy must be 100% organic.
- **Modern singles in 20–30% correction through Q1 2026.** Pressure on collector spending at margin.

---

## Recommendation: **CONDITIONAL GREEN LIGHT** — Proceed to validation, NOT to MVP build.

The data does not support an immediate MVP build. It DOES support a **structured validation phase** that resolves the four critical unknowns before any code is written:

1. **Data-access plan** — Confirm cost & ToS of paid pricing APIs (JustTCG, Scrydex, TCG API). If the cheapest viable plan exceeds $100/mo, re-price the subscription before continuing.
2. **Competitor feature audit** — Subscribe to Collectr PRO for one month. Document features. Confirm or refute the custom-price-alerts gap.
3. **Customer interviews** — Talk to 10 r/pkmntcgcollections users. Validate the pain hierarchy and persona hypothesis.
4. **Organic channel feasibility test** — Build a Pokemon TCG Pocket trade-fairness web tool (no backend, ~10 hours). Post in r/PTCGP. Measure click-through to a waitlist page for the physical-card app.

If all four checks pass within ~30 days, proceed to MVP. If any one fails, re-design the strategy at that point — don't sunk-cost-build through a known-broken assumption.

---

## What Would Change the Recommendation

| If we learn… | Recommendation flips to |
|--------------|------------------------|
| Pricing-data cost > $300/mo with no feasible workaround | **PIVOT** — drop pricing-aggregation as headline feature; pivot to catalog-completeness + condition-tracking app |
| Collectr PRO already has custom price alerts | **PIVOT** — find a different feature wedge or change the persona target |
| Customer interviews show no acute pain (satisfied with eBay + spreadsheet workflow) | **STOP** — demand assumption was wrong |
| Pocket → physical bridge is <0.5% (test produces no signal) | **PROCEED with smaller GTM expectations** — Reddit + creator gifting only |
| Founder cannot commit beyond 6 months | **STOP** or convert to a "release as paid app and stop developing" lifestyle product |

---

## Founder Decision Required

**Question for the founder:** *"Will you spend ~30 days and ~$1,000 running these four validation experiments before writing any production code?"*

- **Yes** → Proceed to Phase 4 (lean strategy) and Phase 8 (validation playbook). The action plan in `action-plan-30-days.md` will lay out the four experiments week-by-week.
- **No, I want to start building** → **STOP and reconsider.** Building before validating the data-access plan, competitor gap, and customer pains is a high-probability path to wasted months.
- **No, I want to walk away** → Acceptable; the research has saved months of misdirected effort. Sometimes the right answer is "this is not the right hill."

For this exercise, we proceed under the assumption of **Yes**.
