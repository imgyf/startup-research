# Lean Canvas

**Phase:** 4 — Strategy (Fast Track: Lean Canvas only)
**Project:** award-flight-alerts
**Date:** 2026-05-09
**Confidence:** Medium (canvas is internally consistent; viability is graded down by competitive findings)

---

> This canvas is filled out for the **literal** founder idea: "mobile app for frequent flyers to receive award-availability alerts." It is graded honestly — most boxes have a `[?]` or `[Weak]` annotation because the research showed the wedge is occupied. A version of the canvas for one of the recommended pivots (B2B travel-advisor, AI-insight overlay, non-US focus) would look different and is not done in this Fast Track pass.

## 1. Problem (top 3)

1. Award seats are scarce and disappear quickly when they open up. Manual searching across multiple FF programs is tedious and time-consuming. **[Real, validated]**
2. Premium-cabin partner awards (the highest-value redemptions) are especially intermittent. **[Real, validated]**
3. Users don't always know *which* program to transfer to and *when*. **[Real — but not solved by alerts; solved by overlay/concierge]**

**Existing alternatives:** Manually searching airline sites; Seats.aero, Roame, PointsYeah, point.me, ExpertFlyer (all already provide alerts); r/awardtravel sweet-spot threads.

## 2. Customer Segments

- **Primary [Assumption]:** US-based credit-card-points enthusiasts, 30–55, 200K+ flexible points balance, redeeming for international premium cabin.
- **Early adopter [Assumption]:** r/awardtravel power users, FlyerTalk regulars, listeners of Award Travel 101 podcast, newsletter readers (Frequent Miler, Points Party).

**[?]** This is the *exact* same segment Seats.aero, Roame, and PointsYeah already serve.

## 3. Unique Value Proposition

> *Stated thesis:* "The first mobile-first award alert app — never miss a seat, even when you're not at your desk."

**[Weak]** This UVP is **factually false in 2026**. Seats.aero and Roame both ship native iOS apps with push notifications. The literal UVP cannot be honestly used in a launch.

**Possible salvageable UVPs:**
- "Award alerts that *explain* the redemption" (AI overlay) — different product, still viable
- "Award alerts for Asia-Pacific carriers" (geographic niche) — different product, still viable
- "Award alerts built for travel advisors" (B2B) — different product, still viable

## 4. Solution

A native iOS + Android app that lets users:
1. Save target routes / dates / cabin / programs
2. Receive push notifications when matching availability is found
3. Tap through to the airline booking page

**[?]** Functionally identical to Seats.aero (currently $8M ARR) and Roame (1M users). Building this in 2026 is **rebuilding a product that already exists at the leader-of-category level**.

## 5. Channels

| Channel | Effectiveness for new entrant | Notes |
|---|---|---|
| SEO ("award flight search tool") | Low | Dominated by TPG, NerdWallet, OMAAT, Frequent Miler — all reviewing competitors, not us |
| Reddit r/awardtravel | Low (mod-restricted) | Self-promotion is restricted; competitor mentions established |
| FlyerTalk | Low | Highly skeptical audience, requires reputation |
| TPG / OMAAT / Frequent Miler partnerships | Medium | Pay-to-play, expensive; competitors already have placements |
| Card-issuer partnership (Amex/Bilt/Chase/CapOne) | Closed for Amex+Bilt; possible for Chase/CapOne but 9–18mo BD | Real but not a 2026-launch channel |
| App Store ASO | Low | Seats.aero ranks for category terms |
| Paid social (TikTok/IG Reels travel-hacking content) | Medium | Real but very crowded; CAC unknown |
| Founder-led content (YouTube, newsletter) | Medium-High | Best org-cost channel, but takes 12–24 months |

**[Yellow Flag]** No clear, capital-efficient channel. The most realistic answer ("build a personal brand for 12–24 months, then launch") is *also* the answer for any founder in this space.

## 6. Revenue Streams

- Freemium subscription: $9.99/mo or $99/yr — **price-anchored to Seats.aero and PointsYeah**, no premium room
- Concierge add-on: $99–250/booking — viable but operational
- Affiliate: card-application affiliate via existing influencer network — **payouts are $50–500/CPA** but only if the app drives application volume, which requires audience first

## 7. Cost Structure

**Year-one realistic burn (solo / two-person team):**

| Item | Annual cost [Estimate] |
|---|---|
| Founder compensation (2 founders, sweat equity) | $0 cash, $200K opportunity cost |
| Mobile dev contractors (initial) | $30K–80K |
| Cloud infra + scraping rigs | $10K–25K |
| Anti-bot bypass tooling (residential proxies, captcha solvers) | $15K–40K |
| Legal retainer (DMCA / CFAA exposure) | $10K–25K |
| Marketing (paid social experiments) | $10K–50K |
| **Total cash burn (Year 1)** | **$75K–220K** |
| **Total inc. opportunity cost** | **$275K–420K** |

## 8. Key Metrics

- Daily/Weekly active alert checks
- Free → Paid conversion (industry benchmark from Seats.aero implied 5–10%)
- Alert → click-through rate (signal of data quality)
- Time-to-book after alert (signal of actionability)
- Churn (industry benchmark for points-tools: ~3–5% monthly)

## 9. Unfair Advantage

**[None stated by founder.]** The intake brief flagged this; the research confirms it is the single most important question. Without one of:
- Pre-existing audience (newsletter, YouTube, podcast)
- Card-issuer relationship
- Proprietary scraping infrastructure or data license
- Hands-on award-booking concierge expertise

…the founder has **no structural advantage** over Seats.aero (bootstrapped to $8M ARR), point.me ($38.5M raised), Roame (1M users), or PointsYeah (NerdWallet's #1 in 2026).

---

## Strategic Verdict on the Literal Idea

| Box | Strength | Comment |
|---|---|---|
| Problem | Real | Validated — but already solved |
| Customer | Clear | Same as 6 incumbents |
| UVP | **Broken** | "Mobile-first" thesis is factually wrong in 2026 |
| Solution | Clear but commodity | Identical to Seats.aero / Roame |
| Channels | **Weak** | No capital-efficient route to acquisition |
| Revenue | Capped | Pricing band locked at $99–129/yr |
| Cost | Lean but real | Anti-bot + legal exposure are non-trivial |
| Metrics | Standard | Fine |
| Unfair advantage | **Missing** | Fatal in this competitive context |

## Flags

**Red Flags:**
- UVP is factually invalidated by current market (Seats.aero + Roame both have iOS push apps).
- "Unfair Advantage" box is empty — the most diagnostic signal in a Lean Canvas for a crowded market.
- No identifiable capital-efficient acquisition channel.

**Yellow Flags:**
- Pricing capped by category convergence.
- Anti-bot + legal costs likely under-estimated by typical solo-founder mental model.

## Sources
- See `01-discovery/competitor-landscape.md` and `01-discovery/market-analysis.md` for all underlying data.
