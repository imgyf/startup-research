# Market Analysis — Pokemon TCG Collector App Tools

**Phase:** 3 — Discovery (synthesis)
**Project:** trading-card-collection-manager
**Date:** 2026-05-10
**Confidence:** Medium (multiple Tier 2 sources cross-referenced; Tier 1 sources scarce; primary collector-population data is estimated)

---

## Executive Summary

The Pokemon TCG ecosystem is a **$2–4B/year global business** [Estimate, derived from $8.4–13.3B global TCG × 12% Pokemon share]. The US Pokemon-collector segment relevant to a paid mobile-tool — serious hobbyists with 200–2,000 cards and $1K–$50K collections — numbers **~200K paying-eligible users** [Estimate], implying a **US SAM of $10–40M ARR**. This is a **lifestyle-business sized opportunity**, well-aligned with the founder's stated $100–500K/year ceiling and side-project pace, but well below VC-scale thresholds.

The market is in a paradox: Pokemon TCG **engagement is at all-time highs** (Pokemon TCG Pocket has 100M+ downloads since Oct 2024 [Data, public news, 2025]; Pokemon was the #1 US toy property in 2025 at $2.5B [Data, Toy Insider/NPD-style trade press]) but the **secondary singles market is in a 20–30% correction through Q1 2026** [Data, market trade press 2025–2026]. TPCi printed 10.2B cards in FY24-25, **down 14.3% YoY** from 11.9B [Data, TPCi annual reports]. Net effect: more users, lower per-card valuations.

Timing is **Neutral leaning Positive**: technology is commoditized in the founder's favor (Ximilar API, multiple 90-99.5% accurate card-recognition stacks), demand validated by VC ($10M Series A for CollX, March 2025 [Data, TechCrunch]; PSA's parent acquired Card Ladder), and a 100M-user mobile-Pokemon app creates organic top-of-funnel.

---

## TAM (Total Addressable Market)

| Layer | Estimate | Source / Note |
|-------|----------|---------------|
| Global TCG market | $8.4B (GMInsights) – $13.3B (Mordor), 2025 | Tier 3 aggregators; definitions diverge ~60%. **No Tier 1 source available.** |
| Pokemon TCG share of global | ~12% [Estimate] | Trade-press triangulation |
| **Pokemon TCG primary cards (global, 2025)** | **~$1.0–1.8B** | Derived |
| + Secondary singles (eBay+TCGplayer GMV) | ~$1B+ [Estimate] | No public GMV figure published |
| + Grading services (PSA/CGC/BGS) | ~$200–400M [Estimate] | PSA Q4 reports indicate Pokemon ≈ 40-50% of submissions |
| + Accessories (sleeves, binders, storage) | ~$200–400M [Estimate] | Trade press |
| **Pokemon TCG ecosystem TAM** | **~$2–4B/year** | Order-of-magnitude estimate |

**Confidence: Medium.** Definitional fuzziness in global TCG figures; Pokemon share is a triangulated estimate. The order of magnitude is robust; the third significant figure is not.

## SAM (Serviceable Addressable Market — US Paid Tooling)

| Inputs | Value | Source |
|--------|-------|--------|
| US TCG retail (2025) | $2.2B | [Data, GameStop / industry trade] |
| US Pokemon share of TCG retail | ~50–60% [Estimate] | Triangulated; Pokemon dominates US |
| Estimated US Pokemon retail (2025) | $1.1–1.3B | Derived |
| Avg active-collector annual spend | ~$450/yr | [Estimate] from Helion via Tier-3 aggregator — **flagged for verification** |
| **Active US Pokemon collectors** | **~2.4–2.9M** | Derived |
| Founder's ICP ("200–2,000 cards, $1K–$50K") | ~20% of base = **~500K** | [Estimate, Wave 1 A1] |
| Paying-eligible (will pay $40+/yr for tools) | ~40% = **~200K** | [Assumption — must validate] |

**SAM bands:**
- **Tight US SAM** = 200K × $50/yr = **$10M ARR**
- **Loose US SAM** = 400K × $100/yr (incl. some expansion to high-end + adjacent TCG) = **$40M ARR**

**Founder's stated ceiling ($100–500K/year) sits at 1–5% of tight SAM** — achievable in principle, but requires real share displacement against incumbents (Collectr 4M users globally, Shiny 1M+).

## SOM (Realistic Year-1 Capture)

For a **side-project, organic-only entrant**:

| Scenario | Downloads (Y1) | Conversion | ARPU | Y1 ARR |
|----------|----------------|-----------|------|--------|
| Conservative | 5,000 | 2.0% | $40/yr | **$4K** |
| Base | 15,000 | 2.5% | $50/yr | **$19K** |
| Stretch (viral moment) | 50,000 | 3.0% | $50/yr | **$75K** |

**Y2 reaches the $100K target only with sustained content/community presence + a category-recognized wedge.** Hitting $500K/year (the founder's optimistic ceiling) requires the project to graduate from "side project" to "primary effort" by month 12–18.

**Comparable companies:**
- **Collectr** — 4M users, ~$1M-low-8-figure ARR [Estimate, bootstrapped, no public financials], multi-TCG, ~5–7 years old
- **CollX** — Series A $10M (March 2025) [Data, TechCrunch], multi-TCG, 6+ years
- **Shiny** — 1M+ users [Estimate, app store data], Pokemon-focused, smaller team
- **PokeScope** — ~50K users [Estimate], Pokemon-focused, indie

The fact that **Collectr reached 4M users bootstrapped** is the most decision-relevant data point: a side-project trajectory CAN produce a real business in this category, but the time-to-scale is years, not months.

---

## Unit Economics Benchmarks (Mobile Freemium Apps)

| Metric | Median | Top Quartile | Source |
|--------|--------|--------------|--------|
| Free → Paid conversion | 2.18% | 5–8% | RevenueCat State of Subscriptions 2025 [Data, Tier 2] |
| Mobile subscription ARPU | $5.65/mo | $8–12/mo | RevenueCat 2025 [Data, Tier 2] |
| Monthly churn (consumer subs) | 5–10% | 3–5% | RevenueCat / industry [Data, Tier 2] |
| Annual plan 1-year retention | ~36% | ~50% | RevenueCat [Data, Tier 2] |
| Implied LTV (median) | ~$100 | ~$200 | Derived |
| **Maximum sustainable CAC** | **<$30** | **<$70** | LTV ÷ 3 |

**Implication:** At <$30 CAC, paid acquisition channels (Google Ads, Meta Ads, Apple Search Ads — typically $3–8 CPI in mobile but blended $15–40 to a paid sub) are **structurally infeasible** for a side-project bootstrap. **The business must be organic or it's not a business.**

---

## Market Headwinds & Risks

### Red Flags (could kill the business)

1. **Data-access cliff.** TCGplayer's developer API closed to new partners in late 2024 (post-eBay acquisition). eBay Finding API was decommissioned February 2025; current eBay Browse API ToS forbid storing pricing data for "market research" purposes [Data, eBay developer docs 2025; cross-referenced in B2 raw research]. This means the founder's core "real-time TCGplayer + eBay aggregation" feature has **no free data source**. Options: paid third-party aggregators (JustTCG, Scrydex, TCG API, PokeWallet) at recurring cost ~$50–500/mo, or scraping (fragile + ToS-violating). **This is the single highest-impact discovery from research and must be addressed before MVP scoping.**
2. **PSA/Collectors as structural competitor.** Collectors (PSA's parent) acquired Card Ladder (analytics + portfolio tracking, December 2021), owns Beckett, and bundles Card Ladder Pro free with the $199/yr PSA Premium grading tier [Data, PSA pricing pages 2025]. Every raw-card user the founder serves is a future grading lead for PSA — Collectors can subsidize a free competing app indefinitely.

### Yellow Flags

3. **Scanning is commoditized.** Multiple shipping apps (Collectr, CollX, Shiny, Ludex, CardSight, CardGrader, Ximilar B2B API) advertise 90–99.5% recognition accuracy [Data, vendor claims]. Card recognition is not a moat — features and data are.
4. **The TCG correction.** Modern Pokemon singles are down 5–15% (some chase cards down 30%+) through Q1 2026 [Data, market trade press]. ARPU may compress as collectors spend less. Vintage WOTC and PSA 9/10 graded are holding value.
5. **TPCi print volume cooling.** -14.3% YoY printing in FY24-25 [Data, TPCi]. Suggests the supply side anticipates softer demand — neutral to mildly negative for a tracking-tool ARPU floor.
6. **IP and platform risk.** Pokemon imagery and trademark risk from TPCi if the app uses card art prominently in marketing or features. Most incumbents avoid this by linking out to TCGplayer for purchase rather than displaying full card art at scale.

---

## Geographic Beachhead

**United States** is the correct beachhead choice:

- Largest single Pokemon market by retail $ ($1.1–1.3B [Estimate])
- eBay/TCGplayer pricing references are US-USD denominated
- US App Store + Reddit/TikTok creator economy aligns with growth strategy
- Currency volatility in EU/Asia adds complexity to "real-time portfolio value"

Expansion path post-PMF: **Canada → UK → Australia** (English-language, eBay-active markets) before Japan (Pokemon's birthplace but completely different secondary marketplace structure — Mercari + Yahoo Auctions Japan rather than eBay/TCGplayer).

---

## Timing Assessment — Net Verdict

**Neutral, leaning Positive.** Ship now, but with the data-access plan resolved before MVP.

| Tailwind | Headwind |
|----------|----------|
| Pokemon TCG Pocket at 100M+ users (organic top-of-funnel for Pokemon-adjacent apps) | Modern singles in 20–30% correction through Q1 2026 |
| Asset-class framing now mainstream (Fortune 2025; Gen Z portfolio behavior) | Card-recognition tech commoditized — no moat from scanning alone |
| Card-recognition tech is cheap and reliable | TCGplayer/eBay APIs closed/restricted — no free pricing data |
| VC validated the category (CollX $10M Series A) | PSA/Collectors structurally subsidizing competing tracker |
| Card Ladder M&A signals incumbent consolidation, but also reveals strategic gap (no Pokemon-only vertical) | Collectr's 4M-user lead in multi-TCG is hard to attack |
| Light-collector founder can ship a niche product with execution edge | Founder lacks community-trust capital; must build it from zero |

---

## Strategic Implications (used by Phase 4)

1. **Beachhead must be Pokemon-only depth, not multi-TCG.** Going wide loses to Collectr by definition.
2. **The founder's headline pricing-aggregation feature is at risk.** Either commit to paying for data (e.g., JustTCG ~$50–200/mo) and price the subscription to cover it, or pivot the headline feature away from real-time pricing toward something less data-dependent (catalog completeness, condition assessment, collection analytics).
3. **CAC must be near-zero.** Strategy must be 100% organic. (Wave 4 distribution research was deferred per Fast Track; Wave 2 GTM analysis is a partial substitute and recommends Reddit + r/PTCGP + micro-creator gifting — see `competitor-landscape.md`.)
4. **Year-1 ARR target should be honestly framed at $10–50K** with a stretch case at $75K+. Founder's $100K+/year ceiling is a Year-2+ outcome.
5. **Differentiation candidates ranked by feasibility:**
   - **(A) Pokemon-native depth** — Pokellector-grade catalog (English + Japanese + sealed + non-PSA grades) with modern UX.
   - **(B) eBay sold-comp pricing** as primary signal — most competitors lean on TCGplayer asks; eBay sold-comps are less commercially restricted in some interpretations and more credible to power users (subject to ToS verification).
   - **(C) Custom price alerts** — Collectr PRO does not advertise price alerts as of research [Estimate, Wave 2 B1]. **Test this in-app to confirm before building.**

---

## Data Gaps (Founder Verification Needed)

| # | Gap | Suggested verification | Priority |
|---|-----|----------------------|----------|
| 1 | Actual cost & ToS of paid Pokemon-pricing APIs (JustTCG, Scrydex, TCG API) | Sign up, request quote, read ToS | **Critical** |
| 2 | Whether eBay Browse API ToS allows displaying sold-comp data for non-resale use | Read current eBay developer agreement; consult IP lawyer if needed | **Critical** |
| 3 | Confirmed paid-feature set of Collectr PRO (does it have price alerts?) | Subscribe for one month, document features | **High** |
| 4 | True paid conversion of Pokemon-niche apps (Shiny, PokeScope, Pokellector) | App Annie / Sensor Tower if accessible; ask app communities | High |
| 5 | Active US Pokemon serious-collector count (200K is an estimate) | Survey 100 Reddit/Discord collectors; collect "serious vs casual" split | High |
| 6 | TPCi/Pokemon Company position on third-party apps using card art | Research cease-and-desist history; consult IP counsel | Medium |
| 7 | Pokemon TCG Pocket third-party access (any data hooks at all?) | Read recent dev community discussions | Medium |

---

## Strategic Connections

- **→ `competitor-landscape.md`** — The data-access cliff explains why no entrant has dethroned eBay's free price-check workflow: the price-check IS the moat, and it requires data the platforms now restrict. The wedge must come from above (collection analytics) or beside (community/social) the price layer.
- **→ `industry-trends.md`** — Pokemon TCG Pocket's 100M+ users are the most underexploited distribution surface; Collectr/CollX's multi-TCG positioning makes them slow to ride that wave.
- **→ Phase 4 Lean Canvas** — The "Unfair Advantage" cell will be uncomfortable to fill given founder's light-collector status. The honest answer is "execution speed + niche depth + community participation" — not domain authority.

---

## Flags

**Red Flags:**
- Pricing-data access has no free path. Headline feature has structural cost or legal risk.
- PSA/Collectors operates a competing tracker as a loss-leader for grading revenue — sustainable competitor cannot be matched on price.

**Yellow Flags:**
- Modern Pokemon singles correction will compress ARPU at margin during Y1.
- Founder's $100–500K ceiling target requires graduating the project from side-project to primary focus by Y2.
- All collector-population numbers are derived estimates; a 30% error in any direction would still be honest.

## Sources

- [Wave 1 raw — market-size.md (Tier 2/3 sources, RevenueCat 2025, GameStop, GMInsights, Mordor, TCGplayer trade press)]
- [Wave 1 raw — trends.md (TechCrunch, Fortune 2025, public news on Pokemon TCG Pocket)]
- [Wave 2 raw — direct-competitors.md (vendor pricing pages, app stores, Crunchbase)]
- [Wave 2 raw — indirect-competitors.md (eBay developer docs, TCGplayer API status, Cardmarket reference)]
- [Wave 2 raw — competitor-gtm.md (Reddit subreddit observations, TikTok creator content, Product Hunt)]
- All raw files in `01-discovery/raw/`
