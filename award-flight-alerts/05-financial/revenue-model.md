# Revenue Model (Fast Track)

**Phase:** 7 — Financial (Fast Track: revenue model only, no full projections)
**Project:** award-flight-alerts
**Date:** 2026-05-09
**Confidence:** Medium (anchored to public competitor data; ranges given)

---

## Pricing Strategy

The category has converged on a tight price band. Anchor pricing at competitor parity; do not assume premium-pricing room.

| Tier | Price | Rationale |
|---|---|---|
| Free | $0 | Required — Seats.aero, Roame, PointsYeah, AwardFares all have free tiers; cannot launch without one |
| Pro | $9.99/mo or $99/yr | Direct match to Seats.aero ($9.99/$99.99) and PointsYeah ($11.99/$99.99) |
| Concierge add-on (optional) | $149/booking | Margin product; competitors charge $200+ |

**[Estimate]** Blended ARPU for paid users: **$80–110/year** (mix of monthly churners + annual subscribers).

## Conversion Benchmarks (from public competitor data)

| Tool | MAU | ARR | Implied paid users | Implied free→paid |
|---|---|---|---|---|
| Seats.aero | 500K | $8M | ~80K (at $100 ARPU) | ~16% [Estimate] |
| point.me | ~unknown | $2.9M (2024) | (mix of paid + Amex-funded free) | low (free Amex tier dominates) |

**[Estimate]** Realistic free→paid conversion for a *new* entrant (no brand): **2–5%**, lower than incumbents.

## Year-1 Revenue Sensitivity (literal version)

Assumptions: solo founder + 1 contractor; bootstrapped; paid social + content marketing; **no card-issuer partnership**; no incumbent feature parity gap.

| Scenario | MAU EOY 1 | Free→Paid | Paid users | ARPU | Year-1 ARR |
|---|---|---|---|---|---|
| **Pessimistic** | 5,000 | 1.5% | 75 | $90 | **$6.8K** |
| **Base** | 15,000 | 2.5% | 375 | $95 | **$36K** |
| **Optimistic** | 40,000 | 4% | 1,600 | $100 | **$160K** |
| **Stretch (requires audience or partnership)** | 100,000 | 5% | 5,000 | $100 | **$500K** |

**Sensitivity check (±30% on the base case):**

| Variable | -30% | Base | +30% |
|---|---|---|---|
| MAU growth | $25K | $36K | $47K |
| Conversion | $25K | $36K | $47K |
| ARPU | $25K | $36K | $47K |

The base case is **$36K Year-1 ARR**, which is **below sustainable solo-founder income** in any US metro. Even the Optimistic case ($160K ARR) supports a 1-person business but does not pay 2 people.

## CAC Sanity Check

Industry benchmark for paid mobile-app subscription (consumer travel utility):
- iOS install CAC (paid social, US): **$5–25**
- Install → free signup: ~30%
- Install → paid: ~1.5% (per [Estimate] above)
- **Effective paid CAC: $300–1,500 per paying user**

Against $90 ARPU and ~24-month payback assumption, **paid acquisition does not work** unless conversion is 2–3× the assumed rate, or LTV is materially higher (concierge upsell).

**[Red Flag]** CAC math does not close on paid channels. The business **must** rely on organic / content / partnership channels to be viable. The founder has neither in the intake brief.

## Unit Economics — Honest Read

| Metric | Value [Estimate] | Benchmark |
|---|---|---|
| Gross margin | ~85% (SaaS-typical, after infra/scraping) | Healthy |
| LTV (at $95 ARPU, 30mo retention) | $237 | OK for a niche product |
| Target CAC | <$80 (≤30% of LTV) | Difficult — see above |
| Payback period target | <12 months | Difficult on paid |

**Verdict:** Unit economics are *theoretically* fine on organic acquisition. They **do not work** on paid acquisition. The viability of the business is therefore the viability of the founder's organic channel — which is unspecified.

## Revenue Comparison vs. Competitors

| Tool | Years to current ARR | Founder background | Take-away |
|---|---|---|---|
| Seats.aero | ~3 yrs to $8M ARR | Founder is a software engineer who built scraping infra during COVID | Bootstrapped path is possible but founder had a clear technical edge in scraping |
| point.me | ~5 yrs to $2.9M revenue | Founders had financial-industry / fintech BD relationships → Citi, Amex partnerships | The "raise + BD" path requires fintech network |
| ExpertFlyer | 17+ yrs | Built during a far less competitive era | Not a replicable path in 2026 |

A new entrant with the literal idea, no existing audience, and no partnership matches *none* of these paths.

---

## Flags

**Red Flags:**
- Paid CAC does not work at category-standard pricing.
- Year-1 base-case ARR ($36K) does not sustain even one full-time founder.
- All known successful entrants had a structural edge (scraping infra, fintech BD, or pre-2010 first-mover timing) that the current founder has not stated.

**Yellow Flags:**
- Theoretical unit economics are fine — the bottleneck is acquisition, not monetization.
- Concierge add-on could materially shift LTV but is operationally heavy and a different business.

## Sources
- See `01-discovery/competitor-landscape.md` for revenue/funding figures.
- ARR Club, PitchBook, Latka, PR Newswire for competitor revenue.
- Author financial modeling [Estimate].
