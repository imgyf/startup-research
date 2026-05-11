# Revenue Model & Unit Economics

**Phase:** 7 — Financial (Fast Track: revenue model + unit economics only)
**Project:** ai-website-sg-restaurants
**Date:** 2026-05-11
**Confidence:** Medium (unit economics rest on validation outcomes; ranges given for major assumptions)

---

## Pricing Strategy

| Tier | Price (SGD) | Includes | Target | Margin |
|------|-------------|----------|--------|--------|
| **Lite (one-time)** | 750 | 3-page site, GBP setup, menu page, mobile-first, 1-year hosting | Single-outlet, no PSG | ~80% gross |
| **Standard (one-time)** | 1,500 | 5-page site, GBP + photos, reservations embed, structured data, 1-year hosting, 14-day support | Mainstream single-outlet | ~80% gross |
| **PSG-listed** | 3,000 list (≈900 net) | Same as Standard + grant paperwork | PSG-eligible (post-approval) | ~75% gross net of compliance overhead |
| **Maintenance** | 79/mo | Unlimited menu/photo updates, monthly review responses, GBP refresh | Attach to any tier | ~70% margin per account |
| **Add-ons** | 200-800 | Photography pack, copywriting, ordering checkout setup | Upsell | 60-80% margin |

**Reasoning:**
- **SGD 750 lite tier:** below freelancer floor; for price-sensitive prospects who object to SGD 1,500. Captures otherwise-lost deals.
- **SGD 1,500 standard:** sits in unowned ground between Wix DIY and SG-agency floor (SGD 2,500+); the headline price.
- **SGD 3,000 PSG tier:** matches local-agency PSG-listed pricing; activates only after vendor approval; SGD 900 effective to customer with 70% subsidy.
- **SGD 79/mo maintenance:** low-friction attach. Below psychological SGD 100/mo threshold; 1-year LTV adds SGD 948.

## 12-Month Revenue Projections (Three Scenarios)

Assumptions used:
- Closes/month: derived from walk-in + email throughput per `01-discovery/raw/distribution.md`
- Maintenance attach rate: 15% (conservative) / 30% (base) / 50% (optimistic)
- ACV blend: weighted toward Standard tier with Lite/PSG mix

| Month | Conservative closes/mo | Base closes/mo | Optimistic closes/mo |
|-------|-----------------------:|---------------:|---------------------:|
| M1 | 3 | 6 | 10 |
| M2 | 5 | 10 | 15 |
| M3 | 7 | 14 | 20 |
| M4-6 | 8/mo | 16/mo | 25/mo |
| M7-9 | 8/mo | 18/mo | 30/mo (PSG approved) |
| M10-12 | 8/mo | 20/mo | 35/mo |

### Year 1 totals (SGD)

| Scenario | Total closes | Avg ACV | Year-1 site revenue | Year-1 maintenance revenue (annualized end-of-year) | Total Y1 revenue |
|----------|-------------:|--------:|--------------------:|----------------------------------------------------:|-----------------:|
| **Conservative** | ~85 | 1,000 | 85,000 | ~12,000 | **~97,000** |
| **Base** | ~180 | 1,200 | 216,000 | ~50,000 | **~266,000** |
| **Optimistic** | ~280 | 1,400 | 392,000 | ~135,000 | **~527,000** |

**[Opinion] The base case (SGD 266k Y1 revenue) is what success looks like for a 2-person team operating from a SGD 5k starting budget.** It funds two founder salaries at SGD 6-8k/month and modest reinvestment. It is not venture-scale, but it is a real bootstrapped business.

## Unit Economics — Per Deal

| Line | Lite (750) | Std (1,500) | PSG (3,000 list / 900 net) |
|------|-----------:|------------:|----------------------------:|
| Revenue (to us) | 750 | 1,500 | 3,000 |
| AI tooling per site [Assumption: SGD 30-80 at agency volume] | 50 | 60 | 80 |
| Hosting + domain (Year 1, paid upfront) | 30 | 30 | 30 |
| Founder time at SGD 50/hr × 6-12 hr per site | 300 | 400 | 600 (incl. PSG paperwork) |
| Compliance / accounting allocation | 30 | 50 | 100 |
| **Total COGS** | **~410** | **~540** | **~810** |
| **Gross profit per deal** | **340 (45%)** | **960 (64%)** | **2,190 (73%)** |

**[Opinion]** Gross margin is healthy at Standard and PSG tiers; thin at Lite. **Use Lite as a closer-of-last-resort**, not a default offer.

## Unit Economics — Customer Acquisition

| Channel | Cost per attempt | Conversion (% sent→paid) | CAC (SGD) | Viability |
|---------|-----------------:|-------------------------:|----------:|-----------|
| Walk-in (founder time) | SGD 5 (transport) + 30 min | 5% [Estimate] | ~100 | ✅ |
| Cold email + pre-built site | SGD 2 (compute) + tools amortized | 1% [Estimate, post-pilot] | ~200 | ✅ if compute hits target |
| Instagram DM | SGD 1 (research time amortized) | 1-2% [Estimate] | ~50-100 | ✅ |
| Partner referral (Oddle/Chope) | 15-20% rev share | n/a | ~150-300 | ✅ — pursue post-month-3 |
| Google Ads on "restaurant website Singapore" | SGD 3-8 CPC | 1-2% landing→demo, 25% demo→close | ~600-1,500 | ❌ at this ACV |

**CAC payback:** All viable channels payback within the first deal at Standard ACV. Worst case (cold email at SGD 200 CAC, 750 Lite ACV): payback after the first sale, profitable from second.

**LTV (1-year):**
- One-time only: SGD 1,200 ACV blended → SGD 1,200 LTV
- With 30% maintenance attach × SGD 79/mo × 12mo: **+SGD 285** blended LTV
- With 50% attach: +SGD 474 blended LTV
- **Blended Y1 LTV (base case): ~SGD 1,485** → **LTV/CAC = 7-15x.** Healthy.

## Sensitivity Analysis

What changes if key assumptions are off by ±30%?

| Variable | Base | -30% | +30% | Impact on Y1 revenue (base case) |
|----------|------|-----:|-----:|---------------------------------:|
| Walk-in close rate (5%) | | 3.5% | 6.5% | SGD 186k / 346k |
| Email reply rate (10%) | | 7% | 13% | SGD 240k / 295k |
| Maintenance attach (30%) | | 21% | 39% | SGD 250k / 285k |
| ACV blend (SGD 1,200) | | 840 | 1,560 | SGD 186k / 346k |
| Per-site compute (SGD 60) | | 42 | 78 | Gross profit ±5% |

**Worst-case stress test (all variables at -30%): Y1 revenue ≈ SGD 130k.** Still cash-positive but no founder pay-yourself room without ~6 months runway. Reinforces case for the SGD 5k starting budget being **tight but survivable** with revenue funding ongoing spend.

**Best-case stress test (all variables at +30%): Y1 revenue ≈ SGD 430k.** Funds 1 hire by month 6.

## Break-Even Analysis

Fixed monthly costs (months 1-6):
- Tools (email, AI, hosting platform): SGD 600/mo
- Walk-in transport + tablet: SGD 250/mo
- Founder draw (subsistence, both partners): SGD 8,000/mo
- Compliance/insurance: SGD 100/mo
- **Total: SGD 8,950/mo**

Break-even closes/month at SGD 1,200 ACV × 75% gross margin = SGD 900 gross profit per deal:
- **Break-even = 10 closes/month**

This matches the base-case projection from month 3 onward. **Month 1-2 will run a loss; the SGD 5k buffer must absorb it.**

## Cash Runway Math

Starting cash: SGD 5,000
- Month 1 (3-6 closes × SGD 1,000 net cash = SGD 3-6k revenue; SGD 3k spend): **+SGD 0 to +SGD 3k net**
- Month 2 (5-10 closes × SGD 1k = SGD 5-10k revenue; SGD 4k spend): **+SGD 1k to +SGD 6k**
- Month 3 onward: revenue covers spend with margin

**[Opinion] Runway holds if month 1 hits at least 4 closes.** Lower than 4 = founders must take on contract work or accept zero personal income for month 2.

---

## Flags

**Red Flags:**
- **Founder draw of SGD 4k/mo each is below SG cost-of-living for many people.** If founders need SGD 6k+/mo personally, this business doesn't pay them properly until month 4-5 even in the base case. **This is a real lifestyle constraint** the founders must accept.

**Yellow Flags:**
- **Per-site compute cost is the load-bearing assumption.** Above SGD 100/site at scale, gross margin breaks and pricing must rise.
- **Maintenance attach at 30% is unproven.** If it lands at 10%, LTV/CAC drops to ~6x — still fine but less buffer.
- **No revenue model includes failure-to-deliver risk.** F&B operators with high mortality (~10% close/year) may demand refunds if they shutter before launch. Recommend a small refund reserve (5%) baked into pricing.

## Sources
- `01-discovery/market-analysis.md` (PSG, competitor pricing)
- `01-discovery/raw/distribution.md` (channel CAC estimates)
- `01-discovery/raw/competitors.md` (AI tooling cost benchmarks)
- Industry benchmarks: 70-80% gross margin for done-for-you AI productized services (Tier 2/3)
