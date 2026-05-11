# Confidence Dashboard — Where We Stand on Solid Ground vs. Thin Ice

**Phase:** 3 — Discovery (synthesis, meta-layer)
**Project:** trading-card-collection-manager
**Date:** 2026-05-10
**Confidence (overall):** Medium

---

## Overview

This document is the meta-layer above the four discovery deliverables. It tells the founder where the strategic conclusions rest on solid evidence and where they rest on assumption. The mode is **Fast Track**, which means Wave 3 (customer voice) and Wave 4 (distribution) deep dives were not run, and Wave 2 ran without dedicated B3 follow-ups. Confidence is therefore lower than a Standard tier would deliver, but the structural conclusions are still robust enough for a go/no-go decision.

---

## Claim-Level Confidence Table

| # | Claim | Source Tier | # Corroborating Sources | Confidence | Data Age |
|---|-------|-------------|-------------------------|------------|----------|
| 1 | Global TCG market is $8–13B in 2025 | T2/T3 | 2 (GMInsights, Mordor) | Medium | 2025 |
| 2 | Pokemon ≈ 12% of global TCG → ~$2–4B Pokemon ecosystem | T3 (triangulated) | 1 + inference | Low-Medium | 2025 |
| 3 | US Pokemon active collectors ≈ 2.4–2.9M | T3 (estimate) | 1 (Helion via aggregator) | Low | 2024 |
| 4 | US paying-eligible serious hobbyists ≈ 200K | Estimate | Derived | Low | 2026 |
| 5 | US SAM = $10–40M ARR | Estimate | Derived | Medium | 2026 |
| 6 | Pokemon = #1 US toy property 2025 at $2.5B | T2 | 1 (Toy Insider/NPD trade press) | Medium-High | 2025 |
| 7 | TPCi printed 10.2B cards FY24-25, -14.3% YoY | T2 (TPCi annual reports) | 1 (primary) | High | 2025 |
| 8 | Pokemon TCG Pocket has 100M+ downloads (Feb 2025) | T2 | 2 (public news, app stores) | High | Feb 2025 |
| 9 | Modern singles correction 20–30% Q4 2024 – Q1 2026 | T2/T3 | 2 (market trade press) | Medium-High | Active |
| 10 | CollX raised $10M Series A March 2025 | T2 | 1 (TechCrunch) | High | Mar 2025 |
| 11 | Collectors (PSA's parent) acquired Card Ladder Dec 2021 | T2 | 1 (public news) | High | Dec 2021 |
| 12 | Collectr has ~4M users | Estimate | Vendor claim + a16z scout activity | Medium | 2024-2025 |
| 13 | Mobile freemium median paid conversion = 2.18% | T2 | 1 (RevenueCat 2025) | High | 2025 |
| 14 | Mobile sub ARPU median = $5.65/mo | T2 | 1 (RevenueCat 2025) | High | 2025 |
| 15 | Consumer subscription monthly churn 5–10% | T2 | RevenueCat + industry consensus | High | 2025 |
| 16 | Card recognition CV is commoditized (90–99.5% accuracy across multiple shipping apps) | T2 | 5+ vendors | High | 2025 |
| 17 | TCGplayer API closed to new partners post-eBay acquisition | T2 | 1 (eBay/TCGplayer dev portal status) | Medium-High | Late 2024 |
| 18 | eBay Finding API decommissioned Feb 2025 | T2 | 1 (eBay dev docs) | High | Feb 2025 |
| 19 | eBay Browse API ToS forbids storing pricing data for "market research" | T2 | 1 (eBay developer agreement) | Medium-High (interpretation may vary) | 2025 |
| 20 | Spreadsheet usage among serious collectors ≈ 30–40% | Estimate | Reddit/community observation | Low-Medium | 2025-2026 |
| 21 | eBay sold-listings used as price reference by 70–85% of serious collectors | Estimate | Reddit/community observation | Low-Medium | 2025-2026 |
| 22 | "Collectr PRO does not advertise per-card price alerts" | Estimate | Public pricing page (single source) | Low | 2026 |
| 23 | Pain hierarchy and primary persona for Returning Hobbyist | **Hypothesis** | Indirect inference | **Low** | Hypothetical |
| 24 | Pokemon TCG Pocket is realistic top-of-funnel for physical-card apps | Opinion + Estimate | Inference from population scale | Medium | 2025-2026 |
| 25 | Card Ladder/PSA will absorb raw-card tracking 12–18 months from now | Opinion / Forecast | Strategic inference | Medium-Low | Forward-looking |

---

## Highest Confidence Findings (act on these)

- **Mobile freemium economics are bad for paid acquisition.** Median LTV ≈ $100; max sustainable CAC <$30. Paid ads are off the table. This conclusion is rock-solid.
- **Card recognition is commoditized.** Cannot be a moat. Build accordingly.
- **VC has validated the category.** CollX Series A is a hard data point.
- **Card Ladder is owned by the grading category leader.** The competitive landscape includes a structurally subsidized incumbent.
- **TCGplayer/eBay API access is restricted for new entrants.** Founders building today must pay for pricing data or accept ToS/scraping risk.

## Lowest Confidence Findings (treat as hypothesis to test)

- **The size and composition of the US Pokemon paying-eligible hobbyist segment** — every collector-population number is a triangulation from limited data.
- **The pain hierarchy and persona detail** — Wave 3 customer-voice research was skipped. The persona is a hypothesis to validate via interviews.
- **The exact prevalence of spreadsheet-vs-app behavior** — community observation only.
- **The "Collectr lacks custom price alerts" feature gap** — single-source observation; must be verified hands-on.
- **The real bridge rate from Pokemon TCG Pocket → physical collecting.**
- **Pokemon-specific app paid-conversion rates** (Shiny, PokeScope, Pokellector) — no public data.

---

## Critical Unknowns (could change the strategy if resolved differently)

| # | Unknown | If true (negative case) | If true (positive case) |
|---|---------|------------------------|------------------------|
| A | Cost & ToS of paid Pokemon-pricing APIs | $200+/mo data cost forces pricing to $9.99/mo, which loses on the conversion floor | $50/mo data cost is absorbable at $4.99/mo with margin |
| B | Whether Collectr PRO has price alerts | Wedge collapses; founder must find a different feature gap | Wedge confirmed; build with confidence |
| C | Customer-interview validation of pain hierarchy | Pains 3+5 (eBay sold-comp + Japanese sets) are not as differentiating as assumed | Pains 3+4+5 are confirmed deal-breakers |
| D | Pocket → physical bridge rate | Wedge channel produces noise, not signal; falls back to Reddit alone | Wedge channel becomes #1 acquisition lever |
| E | Founder time commitment beyond 12 months | Side-project pace can't reach $100K ARR before fatigue | 18+ month commitment + content cadence reaches stretch case |

---

## Recommendations — What the Founder Should Verify First

**Before a single line of code is written**, validate these in priority order:

1. **(Critical)** Get pricing & ToS from JustTCG, Scrydex, and TCG API. 30-min phone call or email. Cost: $0. Time: 1 day.
2. **(Critical)** Read the current eBay Browse API developer agreement carefully. Consult an IP/contract lawyer if cost-justified for a 1-hour read. Cost: $200–500. Time: 2 days.
3. **(Critical)** Subscribe to Collectr PRO for one month, document every paid feature. Confirm or refute the price-alert gap. Cost: $4.99. Time: 1 week of in-app testing.
4. **(High)** Conduct 10 customer interviews via r/pkmntcgcollections + Discord. Cost: $0 (Pro codes as thank-you). Time: 2 weeks.
5. **(High)** Read 50 r/pkmntcgcollections threads to validate language map and pain hierarchy. Cost: $0. Time: 4 hours.
6. **(High)** Post a survey via Reddit (after community participation builds reputation) measuring spreadsheet/app prevalence and willingness-to-pay. Cost: $0. Time: 2 weeks.
7. **(Medium)** Test the Pokemon TCG Pocket bridge channel: build a tiny Pocket trade-fairness web tool, post in r/PTCGP, measure click-through to a "sign up for the physical-card app waitlist" page. Cost: ~10 hrs dev. Time: 2 weeks.

These verifications collectively cost <$1,000 and <30 hours of founder time but will resolve 5 of the 6 lowest-confidence findings before MVP investment.

---

## Source Quality Distribution

| Tier | Definition | Count of citations | Examples |
|------|-----------|----------------------|----------|
| Tier 1 | Industry analyst reports, government, SEC, academic | **0 directly cited** | (None for this niche) |
| Tier 2 | Reputable trade press, company filings, vendor primary sources | ~12–15 | TechCrunch, Fortune, RevenueCat, TPCi annual report, eBay/TCGplayer developer docs, Toy Insider |
| Tier 3 | Blogs, market aggregators, Reddit, community observation | ~10–15 | GMInsights aggregator, Helion via aggregator, market trade press, Reddit threads |

The absence of Tier 1 sources is a known weakness for niche consumer categories. **The conclusion structure does not depend on any single Tier 3 source for a critical decision.** Where Tier 3 is the only available source, the claim is labeled [Estimate] and confidence is rated Low or Medium, never High.

---

## Honest Bottom Line

The discovery research has produced enough evidence to make a defensible **CONDITIONAL go-no-go** decision. The market exists, the demand is real, the side-project ceiling is reachable, the competitors are mappable, and the wedge is identifiable.

**What's missing (and necessary before the founder commits time at scale):**
- Direct customer voice (5–10 interviews)
- Direct competitor in-app feature audit (Collectr PRO, Shiny, PokeScope)
- Resolved data-access plan (paid API or scrape, with cost & ToS read)
- Demonstrated organic-channel feasibility (one Reddit post that clears 100 upvotes; one TikTok demo at 10K+ views)

These four gates are scheduled in the 30-day action plan. **Founder should not start building MVP code until these gates are cleared.**
