# Intake Brief — Palm Reading Mobile App

**Phase:** 1 — Intake
**Project:** palm-reading-app
**Date:** 2026-05-09
**Confidence:** Medium (founder profile assumed in Auto/Fast Track mode — flagged below)
**Mode:** Fast Track

---

## The Idea (as submitted)

> "I want to build a consumer mobile app where it can do palm reading by generating palm analysis images using GPT Images 2.0, is it worth building?"

### Distilled

A consumer mobile app where the user takes a photo of their palm; the app uses an LLM-driven vision pipeline plus an image-generation model (referred to by the user as "GPT Images 2.0" — best-available proxy today is OpenAI `gpt-image-1` or Google Imagen 3 / Gemini Flash Image) to generate **annotated palm-analysis imagery** plus a written reading covering life line / heart line / fate line / personality / future predictions. Likely consumer entertainment/spirituality vertical, monetized via subscription or one-time readings.

**[Assumption]** "GPT Images 2.0" is shorthand — at the time of writing OpenAI's published image-generation model is `gpt-image-1` (released March 2025). A successor isn't publicly announced. The thesis works with any current frontier image model (gpt-image-1, Imagen 3, Stable Diffusion 3.5, Flux). The competitive moat does NOT come from model access — every palm-reading competitor will have it within ~30 days of any release.

---

## Founder Profile [ASSUMPTION — Auto Mode]

> ⚠️ **Flag**: The user did not provide background information. The intake below is **inherited from the prior session's profile** and assumed for continuity. Replace with real answers if any of these are wrong.

| Field | Assumed Value |
|---|---|
| Background | Solo, technically capable, can ship a mobile app independently |
| Co-founders | Solo |
| Time | Side-project / part-time |
| Budget | Bootstrapped (~$500–$5,000 launch; no VC) |
| Domain expertise in palmistry/spirituality | None assumed |
| Domain expertise in viral consumer mobile / TikTok ads | None assumed |
| Geography | Global English-language launch (US-first plausible; APAC plausible) |
| Existing assets | None (no prototype, no audience, no waitlist) |

**Founder-market fit (preliminary, [Opinion]):** Weak. This category is dominated by **performance-marketing studios** (Voodoo, Lightricks, Sensor Tower top-charts) whose unfair advantage is creative-testing infrastructure, ad-spend pools, and ASO ops — none of which a bootstrapped solo technical founder typically has. A technical edge does not translate into a moat here.

---

## The Problem & The "Customer"

**Problem statement [Opinion]:** This is **not a "pain" product** — it's an entertainment / curiosity / social-share product. Users do not have a problem they are trying to solve; they have idle 90-second curiosity ("what does my palm say about me?"). The buying motion is impulse, not consideration.

**Implication:** Standard "interview 10 customers about their pain" validation does not apply cleanly. The validation question is **demand intensity & willingness-to-pay-fast**, not pain severity.

**Target user [Estimate]:**
- Demographics: 18–34, ~70% female, smartphone-native, TikTok/Instagram active
- Psychographics: spirituality-curious, "manifestation" / astrology / tarot adjacent, low skeptic threshold
- Acquisition: TikTok organic + paid, Reels, Pinterest, Snap; **App Store / Play Store search** for "palm reader" / "palm reading"

---

## Business Model (intent)

**[Assumption]** Likely a **subscription** model based on category norms:
- Hard paywall after first reading (industry-standard for this vertical)
- Weekly trial: $4.99–$6.99/wk OR weekly sub $4.99/wk
- Annual: $39–$59/yr
- ARPU benchmark for viral spiritual apps: $15–$40 LTV (very short retention)

**Alternative model:** One-time reading credit ($1.99–$4.99 per analysis). Generally underperforms subs in this vertical per public Sensor Tower data.

---

## Default Assumptions (to challenge in research)

1. **[Assumption]** Palm-reading-as-entertainment is a viable consumer mobile niche.
2. **[Assumption]** Image-generation differentiation (annotated palm graphic) creates meaningful conversion lift over text-only readings.
3. **[Assumption]** TikTok organic content can drive enough installs to make CAC viable for a bootstrapped launch.
4. **[Assumption]** Existing palm-reading apps are weak enough that a quality entrant can win share.
5. **[Assumption]** Cost of generating one annotated palm image (~$0.04–$0.20 inference) does not break the unit economics at trial conversion rates of 2–5%.

---

## Hard Questions (founder must answer before serious investment)

1. **Why you?** What's the unfair advantage vs. a Voodoo / AppLovin-style studio that can outspend you 100× in TikTok creative testing?
2. **What if Co-Star, Sanctuary, or Nebula ships a palm-reading feature next month?** Their CACs are already amortized across an existing audience; yours is from zero.
3. **What's the strongest argument against?** [Opinion] App Store policies on "fortune-telling / spiritual" apps + Apple's increasing scrutiny on subscription dark-patterns + Google Play's restrictions on "deceptive content" — at least 3 palm-reading apps have been pulled per public dev forum reports.
4. **Have you talked to users?** Assumed: no.
5. **What would make you walk away?** Suggested kill criteria below in Phase 8.

---

## Yellow / Red Flags (Phase 1)

**Red Flags:**
- **Category is "performance marketing arbitrage," not "product."** Winners in viral spiritual mobile (Co-Star alumni, Voodoo studios) win on ad creative + LTV-payback math, not product quality. Solo bootstrapped founders rarely win these categories without studio infrastructure.
- **Differentiation thesis ("annotated palm image via gpt-image-1") is replicable in <30 days by any competitor with API access.** This is not a moat.
- **App Store / Play Store policy risk:** "Fortune-telling" content + subscription apps are an increasingly enforced category for rejections, refunds, and pulls.

**Yellow Flags:**
- Founder-market fit weak (no spirituality audience, no TikTok creator presence assumed).
- Audience is highly trend-cyclical — palm reading was a moment in 2022 ("face reading" / "Umax" wave 2024); trend longevity past 6 months is not guaranteed.
- Low LTV vertical: typical "novelty spirituality" apps see 80%+ churn in month 1.
- Subscription dark-pattern lawsuits (Apple class actions, FTC focus on auto-renew) make the dominant monetization path increasingly fragile.

---

## Sources
- [Tier 2] Sensor Tower public charts on spirituality apps (general knowledge)
- [Tier 3] Public app developer forums on Apple/Play store policy enforcement
- [Knowledge-based pre-research] All claims to be verified in Phase 3
