# Idea Scorecard — Pokemon Collection Manager

**Phase:** 8 — Validation
**Project:** trading-card-collection-manager
**Date:** 2026-05-10
**Confidence:** Medium

---

## Scoring Guide
- **Score 8–10:** Strong signal to proceed
- **Score 6–7:** Conditional proceed (specific conditions must validate first)
- **Score 4–5:** Significant concerns (run validation experiments before committing)
- **Score 1–3:** Recommend against proceeding in current form

---

## Scorecard

| Dimension | Score (1–10) | Rationale |
|-----------|-------------|-----------|
| **Problem severity** | **6** | Real pain exists at the 200–2,000 card threshold (spreadsheet breaks, manual entry is brutal, eBay-comp lookup is tedious). But the problem is "annoying," not "burning" — most collectors live with it via spreadsheet + eBay tabs. The category itself is more "premium convenience" than "must-have" for the median collector. |
| **Market size** | **5** | US SAM of $10–40M ARR is real and lifestyle-business-sized. Enough room for the founder's $100–500K ceiling. **But not large enough to support multiple winners**, and incumbents already occupy multi-TCG positioning. Niche size is the right size for a side project, the wrong size for VC-scale. |
| **Competitive advantage** | **4** | Founder has NO innate unfair advantage today (light-collector + bootstrapped + side-project + no community presence). Wedge ("Pokemon-only depth + eBay sold-comps + custom alerts + modern UX") is real but copyable. Long-term advantages (community participation, execution speed on new sets, grading-neutrality) are buildable but unproven. |
| **Feasibility** | **6** | Mobile dev expertise + commoditized card-recognition tech + existing third-party pricing APIs make MVP technically feasible in 2–4 months. **The primary feasibility risk is data access** (TCGplayer/eBay APIs closed; paid third-party adds structural cost). Resolvable but adds expense. |
| **Business model clarity** | **7** | Freemium subscription is a known-good model for hobbyist tools, with clear benchmarks (RevenueCat 2025: 2.18% median conversion, $5.65/mo ARPU, 5–10% monthly churn). Pricing tested at $5.99/$59.99 against direct comps. Future marketplace fee is optional, properly deferred. **Model is coherent; ceiling is honestly framed.** |
| **Founder–market fit** | **3** | This is the lowest score and it's deliberate. Light-collector + side-project pace + no community trust + mobile dev expertise = an execution-first profile in a category where incumbents win on community participation and Pokemon-native depth. **The founder is not the obviously-right person for this project today.** Can be improved via 6-month deliberate community embedding. |
| **Timing** | **7** | Pokemon TCG Pocket (100M+ users) is a once-per-decade top-of-funnel surface that did not exist 18 months ago. Asset-class framing is mainstream. Card-recognition tech is cheap and reliable. VC validates the category. **The 12–18 month window before PSA/Collectors potentially absorbs raw-card tracking is real and closing.** Ship now, but with eyes open. |
| **Overall** | **5.4 / 10** | Conditional, leaning concerned |

---

## Verdict — **CONDITIONAL** (lean toward proceed-to-validation, not proceed-to-build)

The math says **5.4/10**, which by the scoring guide is "significant concerns; run validation experiments before committing."

Translated to plain English:

**This idea is not a slam dunk and the founder should not start building yet.** It is also not a clear no — there is a defensible wedge, the market is real, the timing is favorable, and the business-model math holds up. The reason the score isn't higher is **founder–market fit (3/10)** and **competitive advantage (4/10)** — both of which are buildable over months but cannot be conjured by good engineering alone.

### What would push the score to 7+ (clear proceed)
- Founder commits to **6+ months of deliberate Pokemon community participation** before launch (daily Reddit + Discord + 50+ collector interviews), not as marketing but as domain-fluency-building. **Competitive advantage 4 → 7. Founder–market fit 3 → 6.**
- Founder confirms **data-access plan** with paid pricing API at <$200/mo. **Feasibility 6 → 8.**
- Founder runs the **4 validation experiments** in the 30-day plan and gets positive signal on at least 3 of 4 (especially the customer-interview experiment producing strong "I would pay for this" signal).

### What would push the score to 4 or below (recommend against)
- Customer interviews show satisfaction with current spreadsheet + eBay workflow. **Problem severity 6 → 3.**
- Pricing-data costs exceed $300/mo with no workaround. **Feasibility 6 → 3.**
- Collectr PRO already offers per-card price alerts (wedge collapses). **Competitive advantage 4 → 2.**
- Founder cannot commit beyond 6 months, period. **All scores compress; project not viable.**

### What does NOT change the score
- Whether the original "$4.99/mo" pricing or the corrected "$5.99/mo" is right — small variance, equally testable.
- Whether the project starts on Pokemon, MTG, or sports cards — the structural picture is similar; Pokemon was a defensible beachhead choice.
- App-store rating speed in Y1 — affects ARR magnitude, not direction.

---

## Honest Recommendation

**To the founder, in plain language:**

This idea is buildable, but it is not the obvious slam-dunk it might feel like. The Pokemon TCG market is real and your $100–500K/yr ceiling is reachable, but you are not yet the right person to build this app — you can become the right person through 6 months of deliberate community immersion before you write a line of production code.

The idea passes Phase 3 research **conditionally**: ship-worthy wedge identified, market sized, business model coherent, but founder–market fit is the lowest-scoring dimension by a wide margin. **Do the four validation experiments in the 30-day action plan. If three of four come back positive, you have permission to build. If not, this is not the right hill — and there's no shame in walking away with a clearer head than you started with.**

The most likely failure mode if you build now without validating: 4 months of dev time, 1,000 free downloads, 10 paying users, and a slow realization at month 9 that Collectr already has price alerts and your wedge was a story you told yourself.

The most likely success mode if you validate first: 30 days of customer immersion, an MVP scoped to what collectors actually said hurts (which may not be what you assumed), and a 12–18 month build-to-$50K-ARR trajectory that compounds into a real lifestyle business by Y3.

**Score: 5.4. Verdict: VALIDATE before you BUILD.**

---

## Cross-References

- Validation experiments: `06-validation/experiment-design.md`
- Kill criteria: `06-validation/kill-criteria.md`
- Strategic foundation: `02-strategy/lean-canvas.md`
- Financial model: `05-financial/revenue-model.md`
- Research basis: `01-discovery/research-gate.md`

## Flags

**Red Flags:**
- Founder–market fit at 3/10 is the load-bearing weakness. If the founder cannot commit to 6 months of community embedding, the project is structurally weaker than the score suggests.

**Yellow Flags:**
- Competitive advantage at 4/10 reflects a buildable-but-unbuilt advantage; relies on follow-through over months.
- The combined "Conditional Green Light" of Phase 3 research and the 5.4 scorecard score are aligned — both say "validate first, build later."
