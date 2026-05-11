# Revenue Model — Pokemon Collection Manager

**Phase:** 7 — Financial (Fast Track: Revenue Model only)
**Project:** trading-card-collection-manager
**Date:** 2026-05-10
**Confidence:** Medium (benchmarks Tier 2; Y1 download rate is the largest assumption)

---

## Pricing Strategy

| Tier | Price | What's included |
|------|-------|-----------------|
| **Free** | $0 | Up to 50 cards in collection. Manual entry, basic catalog browse. CSV import + export always free. |
| **Pro Monthly** | **$5.99/mo** | Unlimited cards, camera scan, real-time eBay sold-comp valuation, 10 custom price alerts, basic analytics, ad-free. |
| **Pro Annual** | **$59.99/yr** (~17% discount vs monthly) | Pro Monthly + unlimited price alerts + early access to Japanese-set additions. |

**v2 (post-PMF, optional):**
- **Pro Plus** ($9.99/mo or $99/yr): Sealed-product tracking, set-completion ROI, time-series analytics, tax/insurance export. Targets the secondary "Investor-Curious" persona.
- **Marketplace Fee** (5–8% of trade GMV): Only after community trust is established. Adds KYC/AML/payment-processing/dispute obligations — a separate ops bet.

### Pricing Rationale

1. **Floor of $5.99 is set by data-cost arithmetic, not aspiration.** Pricing-data APIs cost $50–200/mo; at 100 paid users, that's $0.50–$2/user/mo, plus app-store fee 15% ≈ $0.90/$5.99. Lower price points (founder's original $4.99) have less margin headroom than the math comfortably allows.
2. **$59.99/yr undercuts Card Ladder ($199/yr with PSA bundle, $99–149/yr standalone) and matches Collectr's $39.99/yr only on monthly equivalency** — annual price is $20 higher than Collectr's because the value prop (Pokemon depth + eBay sold + alerts) is more specific.
3. **The $4.99/mo monthly anchor common to mobile is preserved psychologically by being just $1 above** — collectors will not perceive this as a different category from "the standard $5/mo TCG app."
4. **The 50-card free tier matches Collectr exactly.** This is intentional; we are NOT competing on free-tier generosity. Free tier is a trial mechanism, not a sustainable use case.

(Cross-references `01-discovery/competitor-landscape.md` Comparison Matrix; `01-discovery/market-analysis.md` Unit Economics Benchmarks.)

---

## Y1 Revenue Projections — 3 Scenarios

**Critical assumptions, applicable to all scenarios:**
- Y1 = 12 months from public launch (assume launch month 4 of project, post 4-month build)
- Mix: 50% choose Annual ($59.99 upfront), 50% choose Monthly ($5.99/mo with mid-year average tenure of 6 months)
- Effective Y1 revenue per paid user: 0.5 × $59.99 + 0.5 × ($5.99 × 6) = ~$48
- App store fee 15% (small business pricing) → net ARPU Y1 ≈ **$41/paid user**
- Pricing-data API cost $100/mo (mid-point of estimated range)
- All values [Estimate] unless otherwise noted

### Conservative Scenario

| Input | Value | Source / Logic |
|-------|-------|----------------|
| Total Y1 downloads | 5,000 | Slow Reddit traction, no viral moment |
| Y1 free→paid conversion | 1.5% | Below median — accounts for crowded market |
| Y1 paying users (cumulative) | **75** | |
| Y1 net revenue per paid user | $41 | After app-store fee |
| Y1 gross revenue (net of app store) | **~$3,075** | |
| Y1 data-API cost | $1,200 | $100/mo × 12 |
| Y1 dev/hosting | $500 | Apple/Google fees + minimal hosting |
| **Y1 net** | **~$1,375** | (Plus uncompensated founder time) |

### Base Scenario

| Input | Value | Source / Logic |
|-------|-------|----------------|
| Total Y1 downloads | 15,000 | Modest organic + 1–2 micro-creator hits |
| Y1 free→paid conversion | 2.0% | Slightly below median; reasonable for crowded niche |
| Y1 paying users (cumulative) | **300** | |
| Y1 net revenue per paid user | $41 | |
| Y1 gross revenue | **~$12,300** | |
| Y1 data-API cost | $1,800 | $150/mo avg × 12 (scales slightly with usage) |
| Y1 dev/hosting | $700 | |
| **Y1 net** | **~$9,800** | |

### Stretch Scenario (one viral moment + sustained content)

| Input | Value | Source / Logic |
|-------|-------|----------------|
| Total Y1 downloads | 50,000 | One Reddit post hits front page + creator amplification |
| Y1 free→paid conversion | 3.0% | Top quartile of mobile freemium |
| Y1 paying users (cumulative) | **1,500** | |
| Y1 net revenue per paid user | $41 | |
| Y1 gross revenue | **~$61,500** | |
| Y1 data-API cost | $3,600 | $300/mo avg × 12 (scaling) |
| Y1 dev/hosting | $1,500 | |
| **Y1 net** | **~$56,400** | |

### Y1 ARR Snapshot (run-rate at month 12)

| Scenario | Active paid subs at M12 | Monthly run rate | **ARR** |
|----------|--------------------------|------------------|---------|
| Conservative | ~50 (after churn) | ~$300 | **~$3,600** |
| Base | ~200 | ~$1,200 | **~$14,400** |
| Stretch | ~1,000 | ~$6,000 | **~$72,000** |

---

## Year 2 Projection (Base Scenario, with sustained content + 1 expansion)

| Input | Value |
|-------|-------|
| Total Y2 net new downloads | 30,000 |
| Y2-end paid subs (incl. retained Y1) | ~600 |
| Y2 net revenue per paid user (with Pro Plus uptake at 10%) | $48 |
| Y2 gross revenue | **~$28,800** |
| Y2 data-API cost | $3,600 |
| Y2 dev/hosting | $1,500 |
| **Y2 net** | **~$23,700** |
| **Y2 ARR run-rate at M24** | **~$32,000** |

### Y3 Projection (Base Scenario, project graduates beyond side-project)

| Input | Value |
|-------|-------|
| Y3-end paid subs | ~1,500 |
| Y3 net revenue per paid user | $50 |
| Y3 gross revenue | **~$75,000** |
| **Y3 ARR run-rate at M36** | **~$90,000** |

**The founder's $100K+/year ceiling is reachable in Y3 base case, $200–500K is reachable in Y3 stretch case — but ONLY if the project graduates beyond side-project capacity by Y2.** At pure side-project pace (15 hrs/week), Y3 likely tops out at $50–80K.

---

## Sensitivity Analysis (Base Scenario, ±30% on key variables)

| Variable | -30% | Base | +30% |
|----------|------|------|------|
| Y1 downloads (15K) | 10,500 → ARR ~$10K | $14K | 19,500 → ARR ~$19K |
| Conversion rate (2%) | 1.4% → ARR ~$10K | $14K | 2.6% → ARR ~$19K |
| ARPU (~$48 effective) | $34 → ARR ~$10K | $14K | $62 → ARR ~$19K |
| Monthly churn (7%) | 5% → ARR ~$17K | $14K | 9% → ARR ~$11K |
| Data-API cost ($150/mo) | $105/mo → +$540 net | n/a | $195/mo → -$540 net |

**Interpretation:** Base case is robust within ±30%. **The single biggest swing factor is Y1 downloads,** which is dominated by organic-channel performance (Reddit + creator gifting). If organic channels produce <500 downloads/mo, the conservative case becomes more accurate — and the founder should not invest 12 months in this plan.

**Worst plausible case:** 5,000 downloads × 1% conversion = 50 paying users × $41 = **~$2,050 gross Y1**. Founder time at $100/hr opportunity cost: $30K. Net: significantly negative when time is priced. **This is the realistic floor of "ship and pray for viral."**

**Best plausible case:** 75K downloads × 3.5% conversion (one Reddit front page + one PokeRev-tier creator mention) = 2,600 paying × $48 = **~$125K gross Y1**. Highly improbable without paid distribution, but not impossible.

---

## Unit Economics Summary

| Metric | Value | Source / Logic |
|--------|-------|----------------|
| Effective net ARPU (Y1 mix) | $41/paid user/yr | Net of 15% app-store fee |
| Annual churn (paid) | ~50–60% (median 36% retention) | RevenueCat 2025 [Data, Tier 2] |
| LTV (annual basis) | ~$80 | Median-comp consumer subscription |
| Variable cost per paid user (data API + hosting allocated) | ~$3–6/yr | Scales with usage |
| Gross margin (after app-store + variable cost) | ~75–80% | Healthy for consumer subs |
| Maximum sustainable CAC (LTV/CAC ≥ 3) | **$25–28** | Confirms organic-only |
| Payback period (organic) | ~immediate (no CAC spend) | Time investment is real but not cash |

(Cross-references `01-discovery/market-analysis.md` Unit Economics Benchmarks. Numerical consistency verified.)

---

## Break-Even Analysis

**Cash break-even (ignoring founder time):** Achieved at ~Month 3–6 in Base case (data-API + Apple/Google fees ≈ $200–300/mo; ~5–10 paying users covers it).

**Comprehensive break-even (priced founder time at $100/hr):** Not reached in Y1 in any scenario. Reached in Y2 Stretch, Y3 Base, never in Conservative.

**Founder must internalize:** This is not a cash-rich business. It is a slow-compounding lifestyle business that pays back over 24–36 months IF the project clears the validation gates and IF the founder stays committed past month 12 fatigue.

---

## What Could Break the Model

### Pricing-data cost rises beyond plan
- $100/mo plan → $300/mo plan cuts ~$200 from Y1 net. Manageable.
- $100/mo → $500/mo cuts ~$1,200/mo and forces a price increase to $7.99/mo, which lowers conversion. **Material risk; verify in Action Plan Week 1.**

### Conversion below 1%
- Crowded market + light differentiation could push effective conversion to <1%.
- Y1 ARR would compress to <$5K in Conservative case. **Validation experiments (Phase 8) must produce a 5%+ paid-intent signal before MVP investment.**

### Churn at 12%/mo (vs assumed 7%)
- LTV drops from ~$80 to ~$50. CAC ceiling drops to ~$15. Not a model-killer at organic-only acquisition, but materially worse Y2/Y3 ARR run-rate.

### Apple/Google policy changes
- Currently 15% small-business fee; could rise. Each 5% increase = -3% on margin. Manageable but worth tracking.

### Competitor PRO subscription drops
- If Collectr cuts price to $2.99/mo or PSA launches free Pokemon-tracking, conversion compresses sharply.
- This is the single biggest external risk. Mitigation: differentiate on depth and community, not price.

---

## Founder's Stated Ceiling vs. Model Output

The founder stated **$100–500K/year as a realistic ceiling** for "becoming the standard tool for one specific TCG community."

**Model output:**
- Y1: $1.4K–$56K (Conservative–Stretch)
- Y2: $14K–$120K (Conservative–Stretch)
- Y3: $32K–$200K (Conservative–Stretch)

**Honest verdict:** $100K is achievable in **Y3 Base case** or **Y2 Stretch case**. $500K is achievable only in a **Y3 Stretch + sustained content + Pro Plus tier uptake** scenario, AND requires the project to leave side-project status by Y2.

The founder's stated ceiling is **not unreasonable**, but is **not Y1 territory**. Side-project pace + 12-month horizon = $10–50K most likely.

---

## Strategic Connections

- **→ `02-strategy/lean-canvas.md`** — Pricing ($5.99/$59.99) and unit economics ($80 LTV, $25–28 max CAC) inherited directly.
- **→ `01-discovery/market-analysis.md`** — All unit-economics benchmarks (RevenueCat 2025) cross-reference.
- **→ Phase 8 Validation** — The "1.5% conversion / 5,000 download" Conservative-case threshold is the implicit kill criterion.

---

## Flags

**Red Flags:**
- Founder's optimistic ceiling ($500K/year) is structurally a Y3+ outcome that requires graduating beyond side-project. If founder cannot commit beyond Y1, model collapses to lifestyle floor of $20–50K.
- Pricing-data cost is the single most fragile assumption in the model. **Resolve before MVP build.**

**Yellow Flags:**
- Y1 download projection (5K Conservative / 15K Base) is the largest single estimate; depends entirely on organic-channel performance which has not yet been demonstrated.
- Conversion rate assumes a niche-market premium over the generic 2.18% median; if niche dynamics actually depress conversion (smaller buying-intent signal), Conservative is more realistic.
- 50% Annual / 50% Monthly mix is industry-typical but unverified for this specific user base. Annual-heavy mixes improve cash; monthly-heavy mixes improve flexibility.

## Sources

- `01-discovery/market-analysis.md` (unit economics)
- `01-discovery/competitor-landscape.md` (pricing benchmarks)
- `references/industry-benchmarks.md` (B2C SaaS / Consumer Subscription rows)
- RevenueCat State of Subscriptions 2025 (Tier 2)
- Apple App Store Small Business Program; Google Play 15% tier
