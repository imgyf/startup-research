# Validation Playbook

**Phase:** 8 — Validation
**Project:** ai-website-sg-restaurants
**Date:** 2026-05-11
**Confidence:** High (experiment design is concrete; outcomes are unknown by construction)

---

## Principles

The goal of validation is **not** to confirm the founder's beliefs. It is to find the cheapest, fastest experiment that could **prove the business won't work**. If those experiments don't kill it, then it might be worth full investment.

Experiments are ordered cheapest-first. Run them in sequence (not parallel) for the first 14 days — each informs the next.

---

## Experiment 1: Engineering Spike — "Can we ship 10 spec sites in 1 day for <SGD 20?"

**Cost:** 1 day of one founder's time, <SGD 20 in AI compute
**Tests:** Per-site cost economics + production-ready quality at speed

**Procedure:**
1. Pick 10 real SG restaurant Google Business Profiles (random sample from Joo Chiat + Tanjong Pagar)
2. For each: scrape menu (if available), photos, hours, location
3. Use Lovable / Bolt / v0 to generate a 4-page mobile-first site personalized to that restaurant
4. Measure: total time (target <45 min/site), total compute cost (target <SGD 2/site), output quality (does it look professional?)
5. Get a non-founder (friend, partner) to rate each site 1-10 on visual appeal

**Success criteria:**
- ≤45 min wall-clock per site (founder + AI together)
- ≤SGD 2 compute cost per site at small batch
- Non-founder rating ≥7/10 average

**Kill signal:** If sites cost >SGD 8/site or take >2 hours/site at small batch, the cold-email economics break — pivot to walk-in-only motion at higher ACV, or reconsider tooling.

**Timeline:** Days 1-2.

---

## Experiment 2: Walk-In Pilot — "Will 20 random SG restaurant owners want to see their site?"

**Cost:** 1 week of one founder's time, ~SGD 80 in transport + tablet rental if needed
**Tests:** Walk-in viability, reception of spec-site pitch, real conversion rate

**Procedure:**
1. Generate spec sites for 20 restaurants in advance (output of Experiment 1)
2. Walk into each between 2-4 PM (the lull)
3. Open with: "Hi, I'm [name] — I build websites for SG restaurants. I made a sample of what yours could look like — can I show you for 60 seconds on this tablet?"
4. If they look: explain what we'd do (5 pages, Google ranking, reservations, SGD 1,500 / SGD 750 lite), offer to leave a link to the live preview
5. Capture in spreadsheet: did they look? did they engage? did they ask price? did they ask for a callback? did they commit?

**Success criteria:**
- ≥60% of owners present and willing to look at tablet
- ≥30% of those who look engage in 2+ minute conversation
- ≥2 paying customers (10% close rate of total walked-in)
- Even 1 paying customer = directional proof of concept

**Kill signal:** If <40% of owners are even willing to look at tablet, the wedge mechanic is broken in SG and the entire model needs rethinking.

**Timeline:** Days 3-9.

---

## Experiment 3: Customer Interviews — "Why did those who said NO say no?"

**Cost:** 5 hours of founder time
**Tests:** Objection landscape, pricing sensitivity, missing features

**Procedure:**
1. Take the 14-18 walk-ins from Experiment 2 who DID NOT close
2. Ask: "I understand you're not buying — can I ask why? I'll buy you a coffee."
3. 5-10 of them will agree to chat for 10 minutes
4. Probe: pricing, trust, timing, missing features, what would have made them say yes
5. Tag each objection: TRUST / PRICE / TIMING / FEATURE / OTHER

**Success criteria:**
- ≥5 interviews completed
- Objections cluster in <3 categories (means the problem is tractable)
- At least 30% say price is acceptable but timing/trust is the blocker (means model works, ramp is needed)

**Kill signal:** If >70% say "I don't see why I need this" — the pain is too latent and the spec-site pitch isn't doing enough work to demonstrate loss. Either redesign the pitch or pivot.

**Timeline:** Days 8-14 (overlap with Experiment 2 tail).

---

## Experiment 4: Cold Email Pilot — "Does the wedge work without face-to-face?"

**Cost:** SGD 300 (Instantly subscription + Apollo credits + ~SGD 200 compute for 100 spec sites)
**Tests:** Cold-outreach lift in SG specifically, asynchronous-channel viability

**Procedure:**
1. Build 100 spec sites in advance (capacity test from Experiment 1)
2. Split into two cohorts:
   - **Cohort A (50 emails):** generic pitch — "We build restaurant websites in Singapore from SGD 750"
   - **Cohort B (50 emails):** pre-built site personalized — "Built you a preview, see [link]"
3. Same subject-line variation, same send-time window, same sending domain reputation
4. Track: open rate, click rate, reply rate, calls booked, paying customers

**Success criteria:**
- Cohort B reply rate ≥2× Cohort A reply rate (replicates the DataLane lift)
- ≥1 paying customer from Cohort B
- End-to-end Cohort B sent-to-paid rate ≥1%

**Kill signal:** If Cohort B is no better than Cohort A, the wedge is theatrical, not real — return to walk-ins only.

**Timeline:** Days 15-30. Must run after Experiment 1 confirms compute economics.

---

## Experiment 5 (Optional / Long-Lead): PSG Vendor Application Probe

**Cost:** 4 hours of founder time, no cash
**Tests:** Realistic timeline + bar for becoming PSG-approved

**Procedure:**
1. Read GoBusiness PSG vendor application requirements end-to-end
2. Call EnterpriseSG help line (or use chat) and ask: "What's the typical approval timeline for a new web-design vendor? Is an AI-assisted delivery process acceptable?"
3. Find one PSG-approved vendor founder (LinkedIn search) — buy them lunch (SGD 30) and ask their honest experience

**Success criteria:**
- Clear answer on whether AI-assisted delivery is policy-acceptable
- Realistic timeline expectation (<12 months ideal, <18 months acceptable)

**Kill signal:** If approval looks like a 2+ year project or requires team size we don't have, scrap PSG strategy and double down on non-PSG segment.

**Timeline:** Days 4-30 (start as soon as Experiment 2 is running).

---

## Decision Framework After 30 Days

| Outcome | Action |
|---------|--------|
| Experiments 1-2 pass, ≥2 paying walk-in customers | **GO** — invest months 2-3 building case studies and applying for PSG |
| Experiment 1 passes, Experiment 2 closes <2 | **Pivot pitch** — refine the diagnostic; rerun Experiment 2 with a "show your Google loss" overlay before the spec site |
| Experiment 1 fails (compute >SGD 8/site) | **Pivot to walk-in-only at higher ACV** (drop email channel, raise pricing to SGD 2,000+) |
| Experiment 2 fails (<40% even look at tablet) | **STOP** — fundamental wedge problem; consider Variation C (different vertical) |
| All 4 pass | **Scale aggressively** in month 2-3 |
| Experiment 4 (email) fails after walk-ins succeed | **No email channel — walk-in-only business** (caps at ~SGD 10-15k MRR/founder) |

---

## What This Plan Costs

| Line | Cost (SGD) |
|------|-----------:|
| AI compute for 110 spec sites (Exp 1+2+4) | 220 |
| Cold email tools 1-month (Exp 4) | 300 |
| Transport + tablet + coffee for interviews (Exp 2+3) | 180 |
| Misc | 100 |
| **Total** | **~800** |

**Out of the SGD 5,000 budget, validation costs ~16%. The remaining SGD 4,200 funds month 2-3 operations.**

## What This Plan Earns (In the Base Case)

If Experiment 2 closes 2 customers + Experiment 4 closes 1 = **3 customers × SGD 1,000 average net = SGD 3,000 revenue in month 1**, with another 5-10 closes likely in month 2 from continuing momentum.

---

## Flags

**Red Flags:**
- None identified specific to this plan.

**Yellow Flags:**
- All experiments rely on founder discipline and consistency. Skipping the no-answer interviews (Experiment 3) because they're emotionally uncomfortable is the single most likely failure mode.

## Sources
- `01-discovery/raw/distribution.md` (channel benchmarks, walk-in throughput estimates)
- `01-discovery/raw/customers.md` (objection patterns, decision criteria)
- DataLane and FirstSales studies on spec-pitch lift (Tier 2)
