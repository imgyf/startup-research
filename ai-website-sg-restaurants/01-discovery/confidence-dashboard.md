# Confidence Dashboard

**Phase:** 3 — Research (data quality summary)
**Project:** ai-website-sg-restaurants
**Date:** 2026-05-11

---

## How to Read This

For every major claim the strategy and validation phases depend on, this dashboard records: the claim, source tier, number of independent corroborating sources, confidence rating, data age, and what to verify directly before betting on it.

**Source tiers:**
- **Tier 1** — Official/analyst (SingStat, IMDA, SFA, EnterpriseSG, government, named research firms)
- **Tier 2** — Tech press, established trade press, well-known industry blogs
- **Tier 3** — Vendor marketing pages, individual blogs, single-source social

**Confidence levels:**
- **High** — Tier 1 source OR 3+ Tier 2/3 sources converge OR primary data
- **Medium** — Tier 2 source + reasonable triangulation OR Tier 1 with caveats
- **Low** — Single Tier 3 source, stale data, or inferred estimate

---

## Key Claims by Confidence

### High Confidence

| Claim | Tier | Sources | Age | Verify if betting >SGD 5k |
|-------|------|---------|-----|---------------------------|
| PSG support rising to 70% from 1 April 2026, SGD 30k cap per UEN | T1 | 4+ | Current | Confirm via GoBusiness portal |
| Refreshed Food Services IDP includes AI use cases | T1 | 1 (IMDA primary) | 2025 | Read full IDP PDF |
| 95.1% SME digital adoption (2024) | T1 | 1 (IMDA primary) | 2024 | Solid as-is |
| 307 F&B closures/month in 2025 (vs 254 in 2024) | T2 | 2-3 | 2025 | Solid as-is |
| 25.1% F&B sales online (Oct 2025) | T1 | SingStat MRS | Current | Solid as-is |
| 78% of diners search online before visiting | T2 | 2-3 | 2025 | Solid as-is |
| FoodPanda/Grab commissions 15-35% | T2 | 3+ | 2025 | Solid as-is |
| Cold email legal under PDPA for B2B with opt-out + ID | T1/T2 | 4+ | 2025-26 | Solid as-is |
| Wix/Squarespace/Durable AI builder pricing USD 10-25/mo | T1 | Vendor primary | Current | Solid as-is |
| Local SG agency Basic tier SGD 1,500-5,000 | T2/T3 | 5+ convergent | 2025-26 | Pull live pricing pages |

### Medium Confidence

| Claim | Tier | Sources | Age | Verify if betting >SGD 5k |
|-------|------|---------|-----|---------------------------|
| ~27,000-30,000 addressable SG restaurants/cafes/bars | T1+Estimate | 1 SFA + inferred | 2023 (stale) | Pull SingStat SSIC 56 table |
| 82% of SG F&B never recorded profit | T3 | 1 (citing tax data) | 2025 | Triangulate via IRAS or accountant network |
| Local SG agency post-PSG effective pricing SGD 900-2,500 | T2/T3 | 3+ vendor pages | Current | Get a real quote from Verz/OOm |
| Walk-in close rate 3-6/week/founder at this ACV | T2 | Triangulated US/EU | 2025 | **Field-test in week 1** |
| Cold email reply rate 8-12% with pre-built site link | T2 | DataLane/FirstSales US data | 2025 | **Pilot 200 prospects month 1** |
| AI tooling cost USD 100-300/month for 2-person agency | Estimate | Vendor pricing | Current | Engineering spike before scaling |
| Verz/OOm/MediaPlus pricing tiers | T2/T3 | Vendor blogs | 2025-26 | Get a real quote |
| F&B owners 35-55, owner-operator, latent website pain | T2 + Estimate | Triangulated | Current | **5-10 owner interviews** |
| RAS membership ~SGD 235/yr for ordinary, vendor tier unclear | T1 | RAS site | Current | Call RAS directly |

### Low Confidence (Data Gaps)

| Claim / Question | Why Low | How to Fix |
|------------------|---------|------------|
| **% of SG independent F&B without a self-owned website** | No clean stat; working estimate 40-60% | **Manual 50-outlet Google audit (1 day)** |
| Persona split: 50-60% "owner does everything" | Analog data from France | 5-10 owner interviews in week 1 |
| Pre-built sample site compute cost (SGD/site) | Vendor pricing exists but real-world cost depends on prompt/scrape/QC pipeline | **Engineering spike: build 10 sample sites, measure** |
| Whether AI-generated sites are PSG-eligible | No published guidance | Call EnterpriseSG / submit PSG vendor application |
| Spec-site cold-outreach lift in SG specifically | Lift documented in US studies, no SG-specific data | **200-prospect pilot in month 1** |
| FoodMatch / FoodieSquare / GoFood status | Did not surface in 2026 search | Direct domain checks |

---

## What This Means for Decisions

**Decisions safe to make on current data:**
- General market is large enough and digitizing fast enough to be worth pursuing.
- PSG is the strategic fulcrum — apply for vendor approval ASAP.
- AI commoditization is real — move quickly, don't bet long-term on the AI-native label.
- One-time pricing fits the high-mortality customer base.
- Walk-ins beat cold email at this ACV.
- B2B cold email is legally safe in SG.

**Decisions that REQUIRE primary validation first:**
- Actual SG-specific cold outreach reply rates with pre-built site hook (don't scale email beyond a 200-prospect pilot until measured)
- True per-prospect compute cost (don't commit to volume claims until measured)
- Real % of SG F&B without owned websites (don't quote market size to investors until counted)
- Whether to build subscription tier (depends on first 10 customers' willingness to commit recurring spend)

**Decisions to defer pending more data:**
- Geographic expansion beyond SG (Year 2+)
- Hawker / coffeeshop segment (separate SKU, Year 2)
- Vertical adjacencies (clinics, salons) — only if restaurant economics fail

---

## Data Refresh Cadence

| Data | Refresh | When |
|------|---------|------|
| PSG vendor approval status | Re-check before each sales meeting | Quarterly |
| Outlet closure rates | Re-check at investor updates | Quarterly |
| AI tooling pricing | Re-check before tooling renewal | Monthly during scale-up |
| Competitor pricing | Re-check before any major pivot | Quarterly |
| Customer reply rate / close rate | **Continuous** — track every send/close | Daily/Weekly |

## Sources
- See `raw/market.md`, `raw/competitors.md`, `raw/customers.md`, `raw/distribution.md`
