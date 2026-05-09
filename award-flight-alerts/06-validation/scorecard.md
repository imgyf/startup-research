# Idea Scorecard

**Phase:** 8 — Validation (Fast Track: scorecard + top 3 experiments + kill criteria)
**Project:** award-flight-alerts
**Date:** 2026-05-09
**Confidence:** High (verdict is well-supported by Phase 3 research)

---

## Scorecard

| Dimension | Score (1–10) | Rationale |
|---|---|---|
| **Problem severity** | 7 | Real, validated, painful — manual award searching across programs is genuinely tedious. Multiple sources confirm the pain. [Data] |
| **Market size** | 4 | TAM is real but the *paying* market for an award-search subscription is ~150K–250K worldwide today, and the category ARR ceiling is roughly $30M–80M. Seats.aero alone holds an estimated ~25% of category ARR. [Estimate, see `market-analysis.md`] |
| **Competitive advantage** | 1 | The literal proposed UVP ("mobile app with push notifications") is **already shipped** by Seats.aero (v 2026.1.2) and Roame.travel. No founder unfair advantage stated. No defensible angle identified. [Red Flag] |
| **Feasibility** | 5 | Technically buildable (mobile + scraping is well-trodden) but data acquisition is hard and getting harder — Air Canada lawsuit, Star Alliance offensive, ExpertFlyer's loss of access to 26 airlines. [Yellow Flag] |
| **Business model clarity** | 5 | Pricing model is obvious (mimic Seats.aero/PointsYeah) but pricing band is locked — no room for premium pricing. Concierge upsell is viable but operational. |
| **Founder-market fit** | 3 | No domain edge stated. The successful entrants had specific edges: Seats.aero (scraping engineer), point.me (fintech BD/Citi-Amex). The default-assumed founder profile matches neither. [Yellow Flag — could go up if founder discloses an unfair advantage] |
| **Timing** | 2 | Worst possible timing. Category is mid-late maturity; major card-issuer distribution slots are claimed (Amex/Bilt); active US litigation; airline anti-scraping crackdown ongoing. [Red Flag] |
| **OVERALL** | **3.9 / 10** | **NO-GO for the literal idea. Pivot or stop.** |

## Verdict

**Score 3.9/10 → "Significant concerns" / borderline NO-GO.**

This is a **NO-GO for the literal idea** as described ("mobile app for frequent flyers to receive alerts for availability of flight bookings with airline miles"), for three converging structural reasons:

1. **The UVP is already in market.** Seats.aero ($8M ARR, 500K MAU) and Roame.travel (1M+ users) both ship native iOS apps with push-notification award alerts. The mobile-first thesis cannot be honestly used at launch in 2026.
2. **No unfair advantage.** The two breakout success stories in the category (Seats.aero, point.me) each had a specific structural edge — scraping engineering or fintech BD relationships. The founder profile inferred from the intake has neither.
3. **Acquisition math doesn't close.** Paid CAC ($300–1,500 per paying user) exceeds LTV ($237) at category-standard pricing. The viable path is organic/content, which takes 12–24 months and requires founder skills not stated.

**However**, this is **not** a NO-GO on the broader space. There are three genuinely open angles surfaced by the research:

| Pivot | Why it's open | Why it might fit a builder-founder |
|---|---|---|
| **AI strategic-insight overlay** ("explain *why* this redemption is good, which transfer partner to use") | Universal complaint across all incumbent reviews; LLMs make this newly tractable; no incumbent has shipped it well | Builder-friendly; no partnerships needed; differentiates on intelligence not data |
| **Travel-advisor B2B SaaS** ("Seats.aero for travel agents" with white-label, multi-client management, commission tracking) | ~30K US travel agents book client awards routinely; no purpose-built B2B tool; recurring per-seat ARR | BD lighter than card-issuer route; defensible because consumer tools won't pivot |
| **Non-US / Asia-Pacific power-user focus** | US-centric tools under-cover Singapore KrisFlyer, Cathay Asia Miles, Lufthansa M&M; large EU + APAC enthusiast communities exist | Less head-to-head with Seats.aero/point.me; geographically defensible |

**Recommendation:**
- **Do not build the literal "mobile app for award alerts."** It is structurally late.
- **Run validation experiments below if you want to test a pivot.** Otherwise, stop and look for a different problem.
- If the founder *does* have an unfair advantage (audience, partnership, scraping infra) that wasn't stated in intake, **re-run this analysis with that disclosure** — the verdict could move materially.

---

## Top 3 Validation Experiments

### Experiment 1 — Customer-Voice "Pivot Validation" Interviews (Week 1–2, ~$50)

**Hypothesis:** Among existing Seats.aero / point.me / Roame users, there is a meaningful segment who would pay for an AI-strategic-insight overlay or a non-US-focused tool.

**Method:**
- Post in r/awardtravel and r/churning (mod-permitted threads only): "Award-search-tool research — paid for your time, 20-min Zoom."
- Compensate $20 Amazon gift card per call (target: 12 interviews).
- Script:
  1. "What award-search tools do you use today?"
  2. "What's the *most* annoying thing about them?"
  3. "When you find a result, do you ever feel uncertain whether it's actually a good redemption?"
  4. "Walk me through the last redemption you booked. Where did you get stuck?"
  5. "If a tool *explained why a redemption was good* and *which transfer partner to use*, would you pay for it? How much?"
  6. "Do you redeem mostly for US-based or international/foreign carriers?"

**Success criteria:**
- ≥ 7/12 interviewees describe the "which program / why this redemption" pain unprompted, AND
- ≥ 5/12 say they would pay $50+/yr for an AI-insight tool layered on top of an existing search tool.

**Cost:** ~$240 (gift cards) + 8–10 hours of founder time.

### Experiment 2 — Landing-Page Smoke Test (Week 2–3, ~$300)

**Hypothesis:** A landing page positioned around "award-search insight" (not "another search tool") converts at >2% on cold paid traffic.

**Method:**
- Build a single landing page (Carrd, Framer, or Webflow): headline = "Stop guessing if your award redemption is a good deal."
- Sub-headline = "We'll tell you which transfer partner to use, why this seat is a sweet spot, and when prices will change."
- Single CTA: email capture for "Early access — first 100 free for life."
- Run $300 of Reddit Ads targeting r/awardtravel, r/churning, r/travel + Facebook Ads targeting "Chase Sapphire Reserve" interest.
- Run for 7 days.

**Success criteria:**
- ≥ 2.5% click-to-email conversion, AND
- ≥ 100 signups for $300 spend (~$3 CAC), AND
- ≥ 25% open rate on the welcome email and ≥ 5 replies indicating willingness to pay.

**Cost:** $300 ad spend + 4 hours founder time.

### Experiment 3 — "Wizard of Oz" Manual Service Test (Week 3–4, ~$0)

**Hypothesis:** Real users will pay for the *insight* layer — even if delivered manually, not via app.

**Method:**
- Take 10 of the email-capture leads from Experiment 2.
- Offer them a manual service: "Tell me your points balances and your travel goals. I'll send you a custom 'best 3 redemptions for you right now' report within 48 hours, for $39."
- Build the report manually using existing tools (Seats.aero, point.me, etc.) and the founder's own analysis.
- Track: how many pay? how do they react? would they pay again?

**Success criteria:**
- ≥ 4/10 pay $39 unprompted, AND
- ≥ 2/10 say they would pay again next month, AND
- The work takes ≤ 1 hour per report (otherwise the unit economics don't scale even with automation).

**Cost:** $0 + ~10 hours founder time (10 reports × 1 hr).

**Why this experiment matters most:** It tests *willingness to pay for insight*, not for software. If users pay $39 for a manual report, the AI-insight pivot is worth pursuing. If they don't, the entire category opportunity for *this* founder is closed and the right answer is to stop.

---

## Kill Criteria

The founder should **stop or pivot away from this idea** if any of the following occur:

1. **Fewer than 5/12 interviewees in Experiment 1** describe the strategic-insight pain unprompted and say they'd pay $50+/yr for it.
2. **Landing-page conversion in Experiment 2 falls below 1.5%** on cold paid traffic, OR CAC exceeds $20/email.
3. **Fewer than 3/10 leads in Experiment 3 pay the $39** for a manual insight report.
4. **The founder cannot identify an unfair advantage** (audience, partnership, technical edge, domain ops experience) by end of Week 4.
5. **A material new development** in the Air Canada v. Seats.aero lawsuit indicates US courts will rule against scrapers (raises legal cost above tolerable level for a bootstrapped startup).
6. **Any major card issuer (Chase, Capital One) signs an exclusive distribution deal with an existing competitor** during the 30-day validation window — this materially shrinks the addressable distribution layer.
7. **At end of 30 days, no concrete signal of paying customer demand for a non-commodity wedge.** Don't extend the validation window — stop.

---

## Risk Snapshot (one-pager — full risk matrix not produced in Fast Track)

| Risk | Likelihood | Impact | Top mitigation |
|---|---|---|---|
| Incumbent ships an obvious feature that erases differentiation | High | Critical | Don't build a feature-only differentiator |
| Air Canada lawsuit precedent extends to all scrapers | Medium | High | Keep US incorporation flexibility; consider non-US base |
| Airline blocks data access mid-product-life | High (already happens) | High | Multi-source data; don't depend on any one airline |
| Card-issuer distribution slot taken by competitor | Already happening | Medium | Don't build a strategy that depends on this |
| Founder runs out of runway before audience builds | High at $0 marketing | Critical | Validate willingness-to-pay before product build |

---

## Anti-Patterns Detected

Cross-checking the founder's framing against common founder pitfalls:

- ✅ **Solution looking for a problem.** The framing leads with "mobile app" (technology choice) before establishing a problem that *isn't* already solved by Seats.aero/Roame's mobile apps.
- ✅ **Boiling the ocean.** "Frequent flyers" is too broad — every credit-card holder with miles is technically a frequent flyer; the actual paying segment is much narrower.
- ⚠️ **Ignoring unit economics.** Pricing/ACV/CAC math was not asked about; the literal idea fails this math.
- ✅ **Premature scaling thinking.** "Mobile app" implies cross-platform investment before any validation.

---

## Flags

**Red Flags:**
- Literal product wedge (mobile-first award alerts) is already shipped by category leaders.
- No founder unfair advantage stated.
- Paid CAC math does not close at category-standard pricing.
- Active legal jeopardy in scraping-based business model.

**Yellow Flags:**
- Three real adjacent opportunities exist (AI insight, travel-advisor B2B, non-US focus) — but none match the founder's stated framing.
- Anti-pattern detection: "solution looking for a problem" and "boiling the ocean" both present.

## Sources
- `01-discovery/market-analysis.md`, `01-discovery/competitor-landscape.md`, `01-discovery/research-gate.md`, `02-strategy/lean-canvas.md`, `05-financial/revenue-model.md`.
