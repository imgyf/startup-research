# Kill Criteria — When to Stop or Pivot

**Phase:** 8 — Validation
**Project:** trading-card-collection-manager
**Date:** 2026-05-10

---

## Why Explicit Kill Criteria Matter

Founders are predisposed to sunk-cost bias. Once 100+ hours and $1,000+ are committed, the natural pull is "let me just build a little more and see." That instinct destroys more startups than under-funding does.

Each kill criterion below is **specific, measurable, and tied to a validation experiment or operating threshold.** If a criterion triggers, the founder should pause, treat it as a real signal, and choose between: pivot scope, pivot persona, or stop. Hidden in the third option is the scariest one — and it's also occasionally the right one.

A criterion triggering does not mean immediate shutdown — it means a forced re-evaluation that protects future months from being wasted on a known-broken assumption.

---

## Pre-Build Kill Criteria (during the 30-day validation phase)

### KC1 — Customer Pain Failure (E1)
**Trigger:** ≤3 out of 10 customer interviews describe an acute, current, monetizable pain.

**Action:**
- **STOP.** This is the most fundamental signal. If the target user does not experience the pain you assumed, no product will fix that.
- Document what they DO experience as pain — there may be a different product hiding in the data.
- If a different pain emerges from interviews (e.g., "I want a better trade-fairness calculator" or "I want to find my local card shop's stock"), pivot toward THAT problem and re-run abbreviated discovery.

### KC2 — No Pricing Intent (E1)
**Trigger:** ≤3 out of 10 interviews say they'd pay $5+/mo for a working solution, OR ≥6 out of 10 say "I'd only use it if it were free."

**Action:**
- **PIVOT to ad-supported model**, but recognize that the unit economics worsen dramatically (consumer apps ad ARPDAU at $0.01–$0.10 means $10–50K MAU is needed to match a 100-paying-user subscription). Almost certainly forces Stop instead.
- Or **PIVOT persona** — the secondary "Investor-Curious" user has higher WTP. Re-target Y1 to this slice, accept smaller TAM, raise price to $9.99/mo or $99/yr.

### KC3 — Pricing-Data Cliff (E2)
**Trigger:** No provider offers production-grade Pokemon-pricing data with terms allowing redistribution in a paid mobile app at <$300/mo at 500 DAU.

**Action:**
- **PIVOT headline feature** away from real-time pricing aggregation. Replacement framings:
  - "Catalog completeness + condition tracking" (no live pricing)
  - "Static-snapshot weekly valuation" (refresh once per week from cheaper provider, dramatically lower API cost)
  - "Manual-input price tracking + analytics" (user enters prices, app does math)
- Each pivot lowers the value-delivery vs. the original pitch. Whether it's still worth building is a question the founder must reanswer.

### KC4 — Wedge Collapse (E4)
**Trigger:** Collectr PRO is confirmed to offer per-card custom price alerts equivalent to the planned feature.

**Action:**
- **PIVOT differentiation angle.** The remaining defensible positioning options:
  - **Japanese-set depth alone** (Collectr's Japanese-set support is documented to be shallow)
  - **Sealed-product investor tooling** (target the secondary persona, raise price)
  - **Privacy-default + local-first** stance (some Collectr competitor reviews mention privacy concerns)
- If none of these feel substantive, **STOP**. The category is too saturated for an undifferentiated entrant.

### KC5 — No Channel Pull (E3)
**Trigger:** Pocket-wedge utility produces <300 unique sessions, <30 waitlist signups, AND organic Reddit posts produce <20 upvotes total over 2 weeks.

**Action:**
- **PIVOT GTM expectations downward.** Drop the Stretch Y1 scenario from the model. Expect the Conservative scenario ($1–4K Y1 ARR). If founder cannot accept that ceiling, **STOP**.
- Or **PIVOT to creator-only GTM** — gift Pro codes to 30+ micro-creators, accept slower compounding.

### KC6 — Founder Time Reality Check
**Trigger:** Halfway through the 30-day validation, founder has logged <30 hours of actual experiment work.

**Action:**
- Be honest about life and capacity. If even 70 hours over 30 days is unsustainable, the 600+ hours required for MVP build + Y1 community building is unsustainable.
- **Defer the project** to a later life-window where time exists, OR **scale ambition down** to a v1.0-and-stop "paid app, no further development" lifestyle product.

---

## Post-Launch Kill Criteria (Y1 of operation)

### KC7 — Free-User Engagement Failure
**Trigger:** Day-30 free-user retention is <5% (median benchmark 8–15%) for 3 consecutive monthly cohorts.

**Action:**
- **STOP marketing.** Don't pour fuel on a leaky bucket.
- **Onboarding rebuild required.** Engage 5 churned users in interviews. If pain is real but onboarding is broken, fix it. If pain disappeared after 30 days, the value prop is shallow — significant pivot or stop.

### KC8 — Conversion Floor Breach
**Trigger:** Free→paid conversion is <0.7% across 3 consecutive monthly cohorts at sufficient volume (≥500 free users/cohort) once organic-channel work is established.

**Action:**
- **Pricing test** — try $3.99/mo for one month to see if the issue is price, not value
- **Feature test** — implement the most-requested missing feature from the customer interviews and remeasure
- **STOP if both fail.** Sub-1% conversion in this category is a value-proposition failure, not a marketing failure.

### KC9 — Churn Spiral
**Trigger:** Monthly paid churn exceeds 12% for 3 consecutive months.

**Action:**
- **Direct outreach to 10 churned subscribers.** "What broke for you?"
- If data quality is the issue → resolve API quality, possibly upgrade provider tier (raises cost, may force price increase)
- If "I don't actually use it" is the issue → engagement loop is missing; build daily-active surface (daily-summary email, push of "your top mover today")
- **STOP if both fail.** A $5.99/mo product with 12%+ monthly churn has LTV of <$50 — model breaks.

### KC10 — Competitor Move
**Trigger:** Collectr or PSA/Collectors launches a Pokemon-only or grader-neutral price-alert feature within 6 months of our launch, with marketing reach we cannot match.

**Action:**
- This is structurally likely; plan for it.
- **Differentiation must shift to depth and community.** Press the Japanese-set advantage, Pocket-bridge, and indie-trust positioning. Drop "scan + alert" parity battles.
- **STOP if depth advantage compresses to <2 weeks of execution lead** — that's not a moat.

### KC11 — Founder Burnout
**Trigger:** Founder reports (privately or publicly) that the project has become a chore for 6+ consecutive weeks.

**Action:**
- **Pause public development.** Maintain the app for paying users; halt feature work.
- Take 60 days off entirely.
- After break, decide: re-engage refreshed, or formally sunset the app with a refund and goodwill announcement.
- **Don't burn the community goodwill** by under-shipping while present. Better to graceful-close than slow-decay.

### KC12 — Data Provider Failure
**Trigger:** Pricing-data provider goes down for >7 days, or doubles their pricing without notice, or Pokemon Company sends a cease-and-desist on data use.

**Action:**
- This is a single-point-of-failure risk that must have a contingency from Day 1.
- **Always maintain a backup data ingestion path** (manual user input, weekly batch re-scrape from a different provider, or stale-but-functional cached data with a "data is N days old" disclaimer).
- **STOP if no backup viable** — this is exactly the existential dependency that should be eliminated by design.

---

## Composite Stop Signal

**If 2+ post-launch kill criteria trigger simultaneously**, the right answer is almost always to **STOP, ship a refund + sunset announcement, and post-mortem in public.** The signal is rarely just one thing — it's compounding fragility.

A graceful sunset (paying users get a year of free service or a refund, app remains available, codebase open-sourced) is significantly better for the founder's long-term reputation than a slow-bleed maintenance mode. The Pokemon collector community is small enough that founder reputation matters across decades.

---

## Strategic Connections

- **→ `06-validation/experiment-design.md`** — KC1–KC5 map to E1–E4 pass/fail thresholds
- **→ `06-validation/scorecard.md`** — KC failures push the overall score below 4 and convert "Conditional" to "Recommend Against"
- **→ `01-discovery/research-gate.md`** — These criteria implement the "what would change the recommendation" matrix from the Research Gate

## Flags

**Red Flags:**
- Founders ignore kill criteria approximately 80% of the time. If the founder cannot pre-commit (in writing, before validation begins) to honoring KC1, KC3, and KC4, the value of writing them down evaporates.

**Yellow Flags:**
- KC9 (churn spiral) is the most common Y2 failure mode for consumer subscriptions; building a daily-active surface (daily mover email, push notifications on owned cards) from launch is the cheapest insurance.
- KC10 (competitor move) is structurally likely within 6–18 months; plan for it rather than hoping it doesn't happen.
