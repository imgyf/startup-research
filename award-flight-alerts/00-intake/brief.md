# Intake Brief

**Phase:** 1 — Intake
**Project:** award-flight-alerts
**Date:** 2026-05-09
**Confidence:** Medium (assumptions inferred — not founder-confirmed)

---

> **Note on this brief:** The founder asked a single validation question ("is it worth building?") and explicitly opted out of a clarifying interview. The fields below are therefore **default assumptions** the rest of the analysis will work from. Where a default could materially flip the verdict, it is flagged inline. The founder should correct any wrong assumption — the analysis can then be re-run on the affected phase.

## The Idea (verbatim)

> "A mobile app for frequent flyers to receive alerts for availability of flight bookings with airline miles."

## Idea Decomposition

- **Job to be done [Assumption]:** Help points-and-miles holders find and book scarce award seats (especially premium-cabin partner awards) before they are taken.
- **Trigger [Assumption]:** User has ~50K–500K+ miles in one or more programs and a route/date they want to redeem on.
- **Channel [Assumption]:** Native iOS/Android app with push notifications. Web companion likely needed for actual booking research.
- **Data source [Assumption]:** Scraped or API-fed availability from airline award engines and partner search engines. **[Yellow Flag]** Data acquisition is the operational core — most airlines actively block scraping of award inventory; Cathay, JAL, ANA, United, Air Canada, AC partner displays are the typical targets and many of these have hostile anti-bot protections.

## The Founder

- **Background [Assumption]:** Not stated. Default assumption: a builder who is also a points enthusiast, but without prior travel-industry, airline-data, or fintech distribution experience.
- **Solo / co-founders [Assumption]:** Solo or 2-person.
- **Time commitment [Assumption]:** Side project or pre-funding full-time.
- **Budget [Assumption]:** Bootstrapped, sub-$50K. Cannot afford airline-grade GDS contracts or licensed inventory feeds at launch.
- **Unfair advantage [Assumption]:** None disclosed. **[Yellow Flag]** In this market, the unfair advantage is usually one of: (a) a proprietary scraping infrastructure that survives airline countermeasures, (b) an existing audience (newsletter, podcast, YouTube channel), or (c) a relationship with a card-issuer / OTA who can pay for distribution. None of these are assumed present.

## The Market

- **Ideal customer:** US-based credit-card-points enthusiasts, 25–55, who hold 200K+ flexible points (Chase UR, Amex MR, Capital One, Citi TY, Bilt) and aspire to redeem for international business/first class.
- **Geography:** US first. Global aspirational.
- **Existing alternatives [Data — common knowledge in space]:**
  - Doing it manually on each airline website
  - Seats.aero (web, premium subscription)
  - point.me (web, redemption search)
  - ExpertFlyer (web, long-running availability alerts)
  - Roame.travel, Pointhound, AwardLogic (newer search/alert tools)
  - Reddit r/awardtravel, FlyerTalk forum monitoring
  - Free tools (e.g., ANA's own search, United's calendar view)
- **Competitive intensity [Opinion]:** High. The "search + alert" niche has at least 5–8 funded or revenue-generating players already.

## The Business

- **Revenue model [Assumption]:** Freemium subscription. Free tier with limited searches/alerts, paid tier $5–20/month for unlimited alerts, advanced filters, partner programs.
- **Pricing benchmarks [Data, see competitor research]:** Seats.aero ~$10/mo (Pro) and ~$30/mo (Premium); point.me ~$129/year; ExpertFlyer ~$10/mo Premium.
- **Unit economics [Estimate]:** ARPU likely $80–150/year. CAC needs to be under $40–60 to be viable. **[Red Flag candidate]** Acquisition is the hardest problem in this category — content/SEO is dominated by The Points Guy, Thrifty Traveler, View From The Wing, OMAAT, etc.
- **Success [Assumption]:** Founder probably wants $10K–50K MRR within 12 months, exit-path optional.

## Constraints & Preferences

- **Mobile-first** — explicit user constraint. **[Opinion]** This is actually a real differentiation lever: incumbents are largely web-first. Mobile + push is genuinely better for "alert me when X opens" UX.
- **No regulatory exposure assumed.** Some scraping risk (CFAA / TOS violations) but no consumer-protection / financial-licensing layer.

## Hard Questions (founder has not answered — flagged for self-test)

1. **Why are you the right person?** No unfair advantage stated. If the founder is "a builder who likes travel," that is the median entrant in this space.
2. **What if Seats.aero or point.me launches a great mobile app tomorrow?** They could, easily. Mobile is a feature, not a moat.
3. **Strongest argument against:** Customer acquisition is brutal in this space; the existing players have head-starts on data scraping infrastructure and audience.
4. **What customers actually said:** Unknown. No interviews assumed completed.
5. **Walk-away condition:** Unknown.

---

## Flags

**Red Flags:**
- None confirmed yet — pending Phase 3 research.

**Yellow Flags:**
- Founder has no stated unfair advantage in a mature, content-driven category.
- Data acquisition (scraping airline award inventory) is the hard, expensive, ongoing operational problem; assumed to be unsolved at intake.
- Mobile-first is a real but easily copied differentiator.
- Acquisition channel is unclear — incumbents own SEO and the influencer layer.

## Sources
- Founder's verbatim idea statement (Tier 1 — direct from founder).
- Author general knowledge of points-and-miles ecosystem (Tier 3 — to be validated in Phase 3).
