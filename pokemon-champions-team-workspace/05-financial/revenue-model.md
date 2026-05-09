# Revenue Model

**Phase:** 7 — Financial
**Project:** pokemon-champions-team-workspace
**Date:** 2026-05-10
**Confidence:** Medium (pricing benchmarks strong; conversion + retention need validation)

---

## Pricing Strategy & Rationale

| Tier | Monthly | Annual | Implied Annual Discount |
|---|---|---|---|
| Free | $0 | $0 | — |
| **Pro** | **$12** | **$99** | ~31% off (1.7 months free) |
| **Tournament Prep** | **$25** | **$199** | ~34% off (2 months free) |

**Why these specific numbers:**
- **$12/mo Pro:** Sits 50% above Mobalytics' $7.99/mo because our market is smaller and more concentrated; sits within Wolfey Patreon $5-10/mo ceiling that the community has already validated.
- **$25/mo Tournament Prep:** Anchored against Metafy human coaching ($25-30/hr). Framing: "1 hour of human coaching per month" — but always-on. Persona C is already paying $30/hr occasionally; $25/mo is a lateral budget reallocation, not a new spend.
- **Annual discounts of 31-34%:** Aggressive enough to incentivize annual commits during tournament-season prep windows; common SaaS practice.
- **Free tier real and useful:** 5 saved teams + basic AI Q&A is a working tool, not a 7-day teaser. This costs us LLM money but is essential for Persona E inbound + Persona C trial-before-buy behavior.

**Why NOT lower pricing:**
- $5-8/mo (the original intake hypothesis) underprices by half the WTP signal. Year 1 ARR collapses below subsistence.
- Charging less doesn't increase conversion meaningfully — Persona C makes the buy-or-not decision based on perceived value, not on $12 vs $8.

**Why NOT higher pricing:**
- $35+/mo for Tournament Prep would push past the "lateral reallocation from existing tool/coaching budget" framing into "new significant expense" territory; conversion would drop sharply.

---

## Year 1 Revenue Projections — Three Scenarios

All scenarios assume MVP launches end of June 2026 (Week 12 of build). Year 1 = July 2026 to June 2027.

### Conservative Scenario

**Assumptions:**
- 5,000 Free signups over the year
- 1.5% Free → Pro conversion = 75 paying Pro users
- 0.5% Free → Tournament Prep direct conversion = 25 TP users
- 50/50 monthly/annual split on paid
- 20% monthly churn after 4 weeks
- Average paid LTV: 4 months

**Math:**
- Pro: 75 users × ~3 months avg paid × $12 = $2,700 + annual contracts ~$1,500 = **~$4,200**
- TP: 25 users × ~3 months avg paid × $25 = $1,875 + annual contracts ~$1,250 = **~$3,125**

But end-of-year MRR is more telling:
- End-Y1 active Pro: ~50 (high churn)
- End-Y1 active TP: ~15
- End-Y1 MRR: 50 × $12 + 15 × $25 = $975/mo
- **End-Y1 ARR run rate: ~$11,700**

**Total Y1 collected revenue: ~$15-25K**

This scenario does NOT cover the founder's opportunity cost. Side-project signal at best.

### Base Scenario

**Assumptions:**
- 12,000 Free signups (creator partnership + Reddit organic compounds)
- 2.5% Free → Pro = 300 Pro users
- 0.8% Free → TP = 100 TP users (some upgrade from Pro mid-year)
- 60/40 monthly/annual split on paid
- 15% monthly churn after 4 weeks
- Average paid LTV: 6 months

**Math:**
- Pro: 300 users × 6 months avg paid × $12 (blended monthly+annual) = ~$21,600
- TP: 100 users × 6 months avg paid × $25 = ~$15,000
- Plus annual contracts (~40% of paid users, paid upfront): ~$25,000-30,000

End-Y1 active:
- Pro active: ~180
- TP active: ~70
- End-Y1 MRR: 180 × $12 + 70 × $25 = $3,910/mo
- **End-Y1 ARR run rate: ~$47,000**

**Total Y1 collected revenue: ~$50-70K**

This is meaningful side-project revenue covering founder opportunity cost partially and giving a clear path to a hire-someone-as-contractor budget.

### Optimistic Scenario

**Assumptions:**
- 25,000 Free signups (WolfeyVGC + CybertronVGC + Brady Smith all partner; Reddit launch goes well; SEO compounds)
- 3.5% Free → Pro = 875 Pro users (some upgrade to TP)
- 1.5% Free → TP = 250 TP users (post-upgrades; Tournament Prep tier resonates with serious players)
- 50/50 monthly/annual on paid
- 10% monthly churn (creator-partnership-driven retention)
- Average paid LTV: 8 months

**Math:**
- Pro: 875 users × 8 months × $12 = ~$84,000 — but realistic adjusted for cohort timing: ~$60,000
- TP: 250 users × 8 months × $25 = ~$50,000 — adjusted: ~$40,000
- Annual upfront: ~$45,000

End-Y1 active:
- Pro active: ~600
- TP active: ~190
- End-Y1 MRR: 600 × $12 + 190 × $25 = $11,950/mo
- **End-Y1 ARR run rate: ~$143,000**

**Total Y1 collected revenue: ~$130-170K**

This is the "side-project becomes bootstrap business" scenario — enough revenue to invest in v1.1, hire a contractor, and seriously consider it as more than a side project.

---

## Sensitivity Analysis

What happens if individual assumptions move ±30%?

### Free signups ±30%

| Variation | Conservative | Base | Optimistic |
|---|---|---|---|
| -30% | $11K | $35K | $90K |
| Baseline | $15-25K | $50-70K | $130-170K |
| +30% | $20K | $90K | $220K |

Free signups is the single largest lever. Creator partnerships are the most efficient way to move it.

### Free → Paid conversion ±30%

| Variation | Conservative | Base | Optimistic |
|---|---|---|---|
| -30% (1.05% / 0.6% / 2.45%) | $10K | $35K | $90K |
| Baseline | $15-25K | $50-70K | $130-170K |
| +30% | $20K | $90K | $220K |

Conversion improves with: better onboarding, sharper coach UX, creator co-promotion.

### Tournament Prep tier WTP — what if $25 is wrong?

The riskiest single number in the model. Sensitivity:

| TP Pricing | Base scenario impact | Optimistic scenario impact |
|---|---|---|
| $15/mo (TP fails to differentiate from Pro at high level) | -$10K | -$30K |
| $20/mo | -$5K | -$15K |
| **$25/mo** (baseline) | $50-70K | $130-170K |
| $30/mo (small WTP boost) | +$3K | +$10K |
| $35/mo (likely conversion drops sharply) | -$5K | -$20K |

**Key insight:** Pricing is sticky on the downside. If $25 is too high, the right move is **not** to lower price but to **add more value to the tier** (counter-team builder, opponent scouting in v1.1) so the price feels right for what's offered. Phase 8 includes a direct pricing test.

### Churn ±30%

| Monthly churn | Base scenario LTV impact |
|---|---|
| 10% (well-retained) | LTV ~10 mo, +$25K |
| **15%** (baseline) | LTV ~6 mo |
| 20% (off-season collapse) | LTV ~4 mo, -$15K |
| 25%+ (broken model) | LTV ~3 mo, -$25K |

Churn after the off-season trough is the biggest single retention threat. v1.1 Tournament Prep features (Q4 2026) must ship to interrupt the trough.

---

## Year 2 Outlook

If Year 1 lands in Base or above, Year 2 looks like:

| Line | Base Y2 | Optimistic Y2 |
|---|---|---|
| Pro subscriptions (steady-state ~500-800 active) | $80-120K | $150-220K |
| Tournament Prep (~150-300 active) | $45-90K | $90-180K |
| Creator content marketplace (Year 2 launch) | $20-50K | $40-80K |
| Team/club seats (Year 2 launch) | $10-30K | $20-50K |
| API access (Year 2 launch) | $5-20K | $10-30K |
| **Total Y2 ARR** | **$160-310K** | **$310-560K** |

Y2 is when the business starts generating "could quit my job" cash flow at the upper end — but only if the product earns retention through the off-season trough and the v1.1 ship lands well.

---

## What "Worth It" Looks Like

The founder's stated time/budget commitment is **15-25 hrs/week, ~$500-2K/mo, 3-6 months runway before reassessment**.

At founder time-value of ~$50-100/hr (market rate for a hobbyist+technical builder), 6 months × 22 hrs/wk × $75/hr = **~$39,000 opportunity cost**.

| Scenario | Y1 collected | Net of opportunity cost |
|---|---|---|
| Conservative | $20K | -$19K (loss) |
| Base | $60K | +$21K (positive) |
| Optimistic | $150K | +$111K (clearly worthwhile) |

**Decision rule:** If the project is tracking Conservative at the 6-month checkpoint (Worlds 2026 over, Sept-Oct demand trough hitting), the founder should reassess seriously. Base or above = continue. Below conservative = pivot or shutter.

This becomes a Phase 8 kill criterion.

---

## Flags

**Red Flags:**
- None at projection level.

**Yellow Flags:**
- Conservative scenario doesn't cover opportunity cost. The deal is real only at Base or above.
- Tournament Prep tier WTP is the single most-sensitive number. Phase 8 must include a direct $15 vs $25 pricing test in Week 2-3.
- Annual contract revenue concentration (40% of paid users buying annual upfront) front-loads cash but means Y2 churn looks worse on the books — annual users may not renew at the same rate as monthly users return after one tournament cycle.
- LLM cost per Pro user could surprise upward if usage exceeds 50 turns/month. Per-user cost discipline is critical.
- The model assumes creator partnership materializes. If all 3 top creators decline, Free signups likely lands at -30% to -50% of baseline; we'd be in Conservative territory.

## Sources

- `01-discovery/market-analysis.md` — pricing benchmarks (Mobalytics, Wolfey, Metafy, HOME Premium)
- `01-discovery/raw/wave3-personas.md` — Persona C WTP signals
- `02-strategy/business-model.md` — tier definitions
- `02-strategy/go-to-market.md` — channel acquisition assumptions
- `04-product/mvp-definition.md` — launch timing assumptions
