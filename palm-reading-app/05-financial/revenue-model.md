# Revenue Model — Palm Reading App

**Phase:** 7 — Financial (Revenue Model only — Fast Track)
**Project:** palm-reading-app
**Date:** 2026-05-09
**Confidence:** Medium (assumptions clearly stated)
**Mode:** Fast Track

---

## Pricing Strategy (Variation A as submitted)

Industry-standard for viral consumer-AI / spirituality apps:

| Tier | Price | Why |
|---|---|---|
| Free trial | 1 reading free | Industry default; needed for App Store policy ("first reading free, paywall after") |
| Weekly | $4.99/wk (auto-renew after 3-day trial) | RevenueCat 2025 benchmark; Cal AI / Umax / Palmist all use weekly |
| Monthly | $14.99/mo | Up-sell tier; minority of subscribers |
| Annual | $39–$59/yr | Best-retention tier; lowest take rate |
| One-time premium read | $1.99–$4.99 | Optional add-on; marginal contribution |

## Conversion & Retention Assumptions

Anchored to RevenueCat 2025 benchmarks + spirituality-vertical reality check:

| Metric | Industry benchmark | This app — base case [Estimate] |
|---|---|---|
| Install → free-trial start | 25–40% | **30%** |
| Free-trial → paid conversion | 4.8% (mobile avg) | **3.5%** (sub-avg due to weak differentiation) |
| **Net install → paid** | ~1.4% | **~1.05%** |
| Weekly sub 12-mo retention | <10% | **5%** |
| Avg paying-user lifespan | 6–10 weeks | **7 weeks** [Estimate] |
| LTV per paying user | $50–$100 | **~$35** at $4.99 × 7 weeks (gross before take rate) |
| Net LTV after 30% App Store + 10% refund | ~$22 | **~$22** |

## Acquisition Cost Reality Check

Three CAC scenarios:

| Scenario | TikTok install cost | Trial-to-paid conv | **CAC per paying user** | Net LTV | Verdict |
|---|---|---|---|---|---|
| Optimistic (Cal-AI-grade creative, viral hit) | $1.50 | 4.8% | **$143/0.048 = $30** | $22 | **Underwater** |
| Base (typical bootstrap) | $5.00 | 3.5% | **$143** | $22 | **Severely underwater** |
| Pessimistic (saturated keywords) | $12.00 | 2.5% | **$480** | $22 | **Catastrophic** |

(Math: $X TikTok install cost / 30% trial-start rate / Y trial-to-paid % = CAC.)

**[Data]** RevenueCat 2025: 9% monthly churn; weekly plans churn 3× faster than monthly; 50–60% yearly retention only at year-plans.

**[Opinion]** Even the optimistic case loses $8 per paying user pre-overhead. The base case loses $121 per paying user. **There is no realistic scenario in which paid acquisition pays back for a bootstrap-scale founder in this category.**

## Organic-Only Scenario

Assume the founder ditches paid entirely, builds organic TikTok content, and converts followers.

| Lever | Realistic 12-month range |
|---|---|
| Organic TikTok followers (assumed: founder is not a creator) | 0–5,000 |
| Conversion to install | 5–15% |
| Total organic installs | 0–750 |
| Trial starts (30%) | 0–225 |
| Paying users (3.5%) | 0–8 |
| Year-1 ARR | **$0–$280** |

**[Opinion]** Organic is essentially zero unless the founder (or a co-founder) is already a TikTok creator with a relevant audience, which is not assumed.

## Three-Year Projections — Variation A

Scenario | Year 1 ARR | Year 2 ARR | Year 3 ARR | Comments
---|---|---|---|---
**Conservative (organic-only)** | $300 | $1,500 | $3,000 | Side-project pocket money
**Base (some paid + organic)** | $5,000 | $25,000 | $40,000 | Below founder subsistence; net negative on time invested
**Optimistic (viral creative hit, $5K paid spend pays back)** | $30,000 | $150,000 | $300,000 | Possible only with founder TikTok creator advantage — assumed absent

Industry comparable: Cal AI took 12 months and $770K/mo ad spend to reach $1.4M MRR. Palmist's claimed "1.2M users" took 5+ years.

## Sensitivity Analysis (Base Case ± 30%)

| Lever | -30% | Base | +30% |
|---|---|---|---|
| Trial-to-paid conversion (3.5%) | 2.45% | 3.5% | 4.55% |
| Year-1 ARR | $3,500 | $5,000 | $6,500 |
| Weekly sub price ($4.99) | $3.49 | $4.99 | $6.49 |
| LTV | $15 | $22 | $29 |
| TikTok install cost ($5) | $3.50 | $5 | $6.50 |
| CAC per paying user | $100 | $143 | $186 |

**Sensitivity reading:** None of the realistic ranges produce LTV > CAC. The model is broken **across the entire ±30% sensitivity envelope**, not just at the base case.

---

## Variation B (Pivot) Quick Revenue Sketch

Different model, different math:

| Item | Variation B value |
|---|---|
| Pricing | $9.99/mo or $59/yr |
| Trial conversion | 5–7% (wellness-positioned apps trend higher than pure novelty) |
| 12-mo retention (yearly tier) | 50% |
| LTV (yearly tier) | $59 × 0.5 retention + churn = ~$80 |
| Channel | Pinterest + influencer + wellness ASO (lower CAC) |
| Realistic CAC per paying user | $40–$80 |
| **LTV / CAC** | **1.0–2.0×** (marginal but viable) |

Still tight, but not *broken*. Worth validating.

---

## Revenue Model Verdict

**[Verdict]** The Variation A revenue model is **structurally broken**. Unit economics do not close under realistic assumptions, and the founder profile excludes the only known viable path (creative-test-budget arbitrage).

The founder should not invest development time in Variation A. The model can plausibly close for Variation B if validation shows demand, but that requires user research, not coding.

## Flags

**Red Flags:**
- LTV < CAC under all realistic scenarios for Variation A.
- Inference cost ($0.10–$0.30 per free reading) consumes 30–80% of revenue at low conversion rates.

**Yellow Flags:**
- Pricing ceiling for the spiritual-app category appears stuck at $4.99–$7.99/wk. Premium pricing experiments rarely succeed in this vertical.
- Subscription auto-renew dark-pattern enforcement (FTC 2025+) further erodes the model.

## Sources
- [Tier 1] [RevenueCat State of Subscription Apps 2025](https://www.revenuecat.com/state-of-subscription-apps-2025/)
- [Tier 1] [CNBC Cal AI revenue + ad spend Sep 2025](https://www.cnbc.com/2025/09/06/cal-ai-how-a-teenage-ceo-built-a-fast-growing-calorie-tracking-app.html)
- [`competitor-landscape.md`](../01-discovery/competitor-landscape.md)
