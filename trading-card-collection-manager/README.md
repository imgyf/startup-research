# Trading Card Collection Manager — Startup Design

**Project:** trading-card-collection-manager
**Mode:** Fast Track (compressed validation)
**Date:** 2026-05-10
**Verdict:** **CONDITIONAL** — Validate before building (Score: 5.4/10)

---

## One-Paragraph Overview

A mobile app for serious Pokemon collectors that turns the phone camera into a card scanner, returns identity + condition tag + real-time eBay sold-comp valuation, and tracks a 200–2,000 card collection's worth as the market moves. Freemium ($0 / 50 cards → $5.99/mo or $59.99/yr Pro) with a future marketplace fee layer (deferred until trust + community established). The market is real and lifestyle-business sized ($10–40M US SAM). The founder's $100–500K annual ceiling is reachable in Year 3 with sustained content + community + execution. **However**, the founder–market fit is the lowest-scoring dimension (3/10 — light collector, side-project pace, no community presence today), and the data-access cliff (TCGplayer + eBay APIs closed to new partners as of 2024–2025) converted what was a free table-stakes feature into a structural cost line. The wedge — Pokemon-only depth + eBay sold-comp pricing + custom alerts + modern UX — is real but copyable. **Recommendation: run the 30-day validation plan before writing any production code.**

---

## Key Findings From Research

### Market & Opportunity
- Pokemon TCG ecosystem ≈ **$2–4B/year globally** [Estimate]
- US SAM (paying-eligible serious hobbyists with paid-tool willingness) ≈ **$10–40M ARR**
- Active US Pokemon collectors ≈ 2.4–2.9M; serious 200–2,000 card hobbyists ≈ 500K; paying-eligible ≈ 200K
- Founder's $100–500K/year ceiling is structurally reachable but is a **Year 3+ outcome**, not Year 1
- Most realistic Y1: $10–50K ARR (Conservative–Base)
- **Pokemon TCG Pocket** at 100M+ users since Oct 2024 is a once-per-decade top-of-funnel surface — underexploited by current incumbents

### Competitive Landscape
- **Crowded but not consolidated.** Direct competitors: Collectr (~4M users, bootstrapped, $4.99/mo), CollX ($10M Series A March 2025), Card Ladder (acquired by Collectors/PSA Dec 2021), Pokellector (legacy/dated), Shiny + PokeScope (Pokemon-native doppelgangers shipping the same pitch), TCGplayer App + eBay App (free, platform-owned)
- **Card Ladder is now PSA-owned** — structurally subsidized via grading revenue; can run a Pokemon tracker at negative margin
- **No Pokemon-pure-play app raise found** in last 24 months — possible whitespace
- Card recognition is **fully commoditized** (90–99.5% accuracy across all incumbents); not a moat
- **Identifiable wedge:** Pokemon-only depth (English + Japanese + sealed) + eBay sold-comp pricing + custom per-card alerts + modern UX. *"The ManaBox of Pokemon."*

### Strategy & Positioning
- **Beachhead:** Pokemon hobbyist with 200–2,000 cards, currently using Pokellector OR a spreadsheet OR Collectr's free tier
- **Pricing:** $5.99/mo or $59.99/yr (raised from founder's original $4.99/$39.99 to absorb pricing-data API costs)
- **Channels (organic-only required, CAC <$30):** Reddit utility-posting (r/pkmntcgcollections + r/pkmntcgtrades), Pokemon TCG Pocket trade-fairness wedge utility (free top-of-funnel test), micro-creator gifting (5K–50K-follower TikTok/YouTube)
- **Avoided:** Multi-TCG breadth, marketplace v1, AI-graded condition (oversells the tech), paid acquisition

### Financial Model
- Y1 (Conservative–Stretch): $4K–$56K net
- Y2 (Base): ~$24K net, $32K ARR run-rate
- Y3 (Base): ~$56K net, $90K ARR run-rate
- LTV ~$80, max CAC $25–28 → confirms organic-only strategy
- Gross margin 75–85% at scale
- Single biggest fragility: **pricing-data API cost** ($50–500/mo). Must be resolved before MVP.

---

## Top 3 Risks and Mitigation

### Risk 1 — Data-Access Cliff
TCGplayer + eBay APIs closed to new partners; pricing aggregation now has structural cost or legal risk.

**Mitigation:** Resolve in Week 1 of validation. Audit JustTCG, Scrydex, TCG API for cost + ToS + coverage. If cheapest viable tier exceeds $300/mo, **pivot the headline feature** away from real-time pricing aggregation toward catalog completeness + condition tracking (which doesn't need third-party live pricing).

### Risk 2 — Founder–Market Fit Deficit
Founder is light-collector; community trust must be earned from zero. Side-project pace makes this slower.

**Mitigation:** Pre-commit to **6 months of daily community participation** (15 min/day in r/pkmntcgcollections + r/pkmntcgtrades) before launch. This converts founder–market fit from 3/10 to 6/10. The week-1 daily-Reddit habit in the action plan starts this immediately. If the founder cannot commit to this, the project is structurally weaker than the score suggests.

### Risk 3 — Strategic Incumbent (PSA/Collectors)
Card Ladder is now PSA-owned. They can launch a competing tracker as a loss-leader for grading revenue.

**Mitigation:** Position deliberately as **grader-neutral** ("Built independently of any grading service"). PSA cannot match this without admitting their conflict-of-interest. Community trust over institutional brand. Watch for Card Ladder roadmap signals; if Pokemon-vertical product launches, prepare to shift differentiation entirely to Japanese-set + sealed depth.

---

## Confidence Dashboard Summary

**Highest confidence (act on this):**
- Mobile freemium economics force organic-only acquisition (LTV ~$80, max CAC <$30)
- Card recognition is commoditized — not a moat
- VC has validated the category (CollX $10M Series A)
- TCGplayer/eBay API access is restricted for new entrants

**Lowest confidence (treat as hypothesis):**
- Specific size of US Pokemon paying-eligible segment (200K is an estimate)
- Pain hierarchy and primary-persona detail (Wave 3 customer-voice deep-dive was skipped per Fast Track)
- "Collectr PRO does not advertise per-card price alerts" (single-source — must verify in-app)
- Pokemon TCG Pocket → physical-card bridge rate

See `01-discovery/confidence-dashboard.md` for the full claim-level table.

---

## Anti-Patterns Detected

A scan of the founder's pitch + research findings flagged these common founder anti-patterns:

| Anti-Pattern | Where it appeared | Honest restatement |
|--------------|-------------------|--------------------|
| **Solution looking for a problem (mild)** | Original pitch led with "camera scanner + portfolio + valuation" — feature framing — before establishing whose pain this solves | The serious 200–2,000 card hobbyist's spreadsheet-vs-eBay-tabs workflow is real pain, but customer interviews must validate intensity |
| **Boiling the ocean (mild)** | Original pitch said "Pokemon, MTG, AND sports cards" — three different communities, three different cultures | Resolved by Pokemon-only beachhead choice in intake; do not re-expand without explicit scope conversation |
| **Premature scaling** | Original pitch included "5–10% marketplace fee on trades facilitated through the app once trust is established" as a v1+ revenue layer | Correctly deferred to v2 in research; marketplace mechanics are an ops bet not a software bet, and KYC/AML/dispute obligations make this a separate company |
| **Ignoring unit economics (none)** | Founder did stipulate freemium economics from start | Properly framed; no anti-pattern flagged |
| **Vanity metrics (potential)** | The "real-time portfolio worth tracked as market moves" framing is feature-flavored, but real success metric is paid retention | North Star metric in Lean Canvas is "monthly active paid subscribers" — not downloads or signups |

---

## Document Index

```
trading-card-collection-manager/
├── README.md                                  ← you are here
├── action-plan-30-days.md                     ← what to do next, week-by-week
├── PROGRESS.md                                ← phase completion tracker
├── 00-intake/
│   ├── brief.md                               ← consolidated intake from founder pitch + Q&A
│   └── brainstorm.md                          ← 3 strategic variations (Tracker / Investor / Trade Hub)
├── 01-discovery/
│   ├── market-analysis.md                     ← TAM/SAM/SOM, unit economics, headwinds, timing
│   ├── competitor-landscape.md                ← 9 competitors profiled, comparison matrix, vulnerability map
│   ├── target-audience.md                     ← persona + pain hierarchy + language map (lite, mostly hypothesis)
│   ├── industry-trends.md                     ← tech/investment/behavioral shifts, regulatory trajectory
│   ├── confidence-dashboard.md                ← claim-level confidence and verification recommendations
│   ├── verification-report.md                 ← 0 critical issues, 4 warnings, all addressed
│   ├── research-gate.md                       ← Conditional Green Light decision
│   └── raw/                                   ← raw research files from 5 subagents
│       ├── market-size.md
│       ├── trends.md
│       ├── direct-competitors.md
│       ├── indirect-competitors.md
│       └── competitor-gtm.md
├── 02-strategy/
│   └── lean-canvas.md                         ← 9-cell business model
├── 05-financial/
│   └── revenue-model.md                       ← pricing + 3-scenario projections + sensitivity
└── 06-validation/
    ├── scorecard.md                           ← 5.4/10, conditional verdict
    ├── experiment-design.md                   ← 4 experiments to run in next 30 days
    └── kill-criteria.md                       ← 12 specific stop-or-pivot triggers
```

---

## Skipped Phases (Fast Track)

These phases were intentionally skipped per Fast Track mode:

- **Phase 5 — Brand:** Mission/vision/values, tone of voice, brand personality. Premature before validation; revisit only if 3+ validation experiments PASS.
- **Phase 6 — Product:** MVP definition, feature prioritization, user journey. Same logic — premature before validation.
- **Wave 3 — Customer Voice deep-dive:** Replaced by the 10-interview customer-discovery experiment in the 30-day action plan. The interview output replaces the inferred persona in `target-audience.md`.
- **Wave 4 — Distribution & Geographic:** Distribution covered partially in Wave 2 GTM analysis. Geographic decided in market-analysis.md (US beachhead).

If validation passes and the project graduates to MVP build, these phases should be re-engaged with the validated customer voice as input.

---

## Final Verdict — Plain English

The Pokemon TCG collection-manager idea is **not a slam dunk and it is not a clear no**. The market is real and the founder's $100–500K ceiling is reachable. The wedge ("Pokemon-only depth + eBay sold-comps + custom alerts + modern UX") is real, but copyable. The competition is dense, the data layer is no longer free, and the founder is a light-collector building as a side project — none of which are fatal but all of which compound into a 5.4/10 score.

**The next 30 days should be customer interviews and channel tests, not code.**

If after 30 days you have:
- 7+/10 interviewees describing acute current pain at $5–10/mo intent ✓
- A pricing-data plan that fits in the cost model ✓
- 100+ waitlist signups from a Pocket-wedge utility ✓
- A confirmed competitor feature gap ✓

…then you've earned the right to build, with materially higher conviction than you started with. If two or more come back negative, the validation phase has saved you 250+ hours and 4–6 months. Either outcome is a win.

**Score: 5.4/10. Verdict: CONDITIONAL. Action: Validate, don't build.**
