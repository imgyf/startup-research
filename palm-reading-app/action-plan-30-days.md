# 30-Day Validation Action Plan

**Project:** palm-reading-app
**Date:** 2026-05-09
**Total budget:** ~$300 · Total time: ~25 hours

---

## North Star

By Day 30, you will have a clean go/no-go decision on each of three options:
- A. Build the literal idea (research already says **NO**, but Experiment 1 closes the loop)
- B. Pivot to palm-themed self-discovery / habit journal
- C. Pivot to B2B palm-reading API for spirituality creators

You are **not** writing app code in the next 30 days. You are *validating demand*.

---

## Week 1 — Substitution Test + Setup (Days 1–7)

### Goal
Kill or confirm the entire consumer-app thesis based on whether free ChatGPT prompts have already eaten the market.

### Tasks
- [ ] **Day 1 (4 hours) — Experiment 1: Substitution audit**
  - Pull top 10 TikTok videos under `#palmreading`, `#palmistry`, `#palmreadingapp` from the past 30 days
  - For each: read top 100 comments. Tally: (a) "I use ChatGPT for free", (b) "what app is that?", (c) "I paid $X for this"
  - Sample 200 1-star and 2-star reviews of top 5 palm reader apps (Palmist, Bliss, Astrology & Palmistry Coach, Palm Reader, Astroline) from past 6 months. Tally: % mentioning free LLM alternative
  - **Decision rule:** if >50% of negative reviews cite free ChatGPT, **kill all consumer variations** (A and B) and skip to Week 2 of B2B (Experiment 3) only
- [ ] **Day 2 (1 hour) — Founder profile reality check**
  - Honestly answer: do you have, or can you acquire in 30 days, a TikTok creator audience >10K? If no, Variation A is double-dead.
- [ ] **Day 3 (3 hours) — Variation B prep**
  - If Experiment 1 passes: build a 1-page Carrd / Framer landing page for Variation B
  - Hero: "Your palm tells a story. Discover it — daily reflections, weekly insights."
  - One mockup of the daily-prompt UI
  - Email capture (Mailchimp / Buttondown free tier)
  - Setup: Plausible Analytics (free, GDPR-safe) + simple TikTok pixel
- [ ] **Day 4–5 (3 hours) — Variation C prep**
  - Build Etsy seller list: search "tarot reading," "palm reading," "psychic reading"; pull 50 active stores with ≥20 sales
  - Build creator list: 20 spirituality TikTok creators with 50K+ followers selling readings/memberships
  - Draft outreach DM (under 50 words). Offer: 10-minute call in exchange for free pilot access.
- [ ] **Day 6–7 — Send outreach**
  - 50 Etsy DMs (use seller-message form)
  - 20 TikTok / Instagram DMs
  - Target: schedule 10 calls for Week 2

### End of Week 1 — Decision Gate
- If Experiment 1 fails (>50% free-substitute mentions): **stop both consumer variations**. Continue with C only.
- If Experiment 1 passes: proceed with B and C in parallel.

---

## Week 2 — Run Experiments (Days 8–14)

### Goal
Get demand signals on Variation B (smoke test) and Variation C (interviews).

### Tasks
- [ ] **Day 8 (2 hours) — Launch Variation B ad test**
  - $200 split: $80 TikTok / $80 Pinterest / $40 Instagram
  - 3 creative variants:
    - V1: founder-talking-head ("I built this because…")
    - V2: palm photo with overlay animation
    - V3: app-mockup screen with text overlay
  - Run 5 days. Daily monitor.
  - Target: 80 emails at ≤$3 each, ≥0.8% CTR on TikTok creative
- [ ] **Day 8–14 (8 hours) — Run Variation C interviews**
  - Conduct 10 × 15-minute calls with creators / Etsy sellers
  - **Required questions** (don't skip):
    1. How do you currently provide readings to customers? (workflow)
    2. How long does it take per reading?
    3. Have you ever wished you could automate part of this? Which part?
    4. If I gave you a $19/mo widget that did automated palm readings using your branding, would you use it?
    5. Would you pay $49/mo? $99/mo? At what price would you say no?
    6. What % of your revenue comes from readings vs other products?
    7. Would you commit to a 30-day paid pilot if I built it?
  - Record verbatim quotes. **Do not pitch — discover.**
- [ ] **Day 14 — Synthesize**
  - Tally B signups + cost-per-email
  - Tally C willingness-to-pay + LOI commitments
  - Write a one-paragraph verdict per variation

### End of Week 2 — Decision Gate
| Variation | Pass | Mid | Fail |
|---|---|---|---|
| B | ≥80 signups @ ≤$3 each | 40–79 signups | <40 signups → drop B |
| C | ≥4/10 willing to pay $19+/mo + ≥2 paid-pilot LOIs | 2–3 willing | <3 willing → drop C |

---

## Week 3 — Deepen the Surviving Variation (Days 15–21)

### Goal
Strengthen the strongest signal into a concrete, fundable next step.

**If both B and C survived:** focus 70% of effort on whichever scored highest, 30% on the other.

**If only one survived:** all-in on that one.

**If neither survived:** skip to Week 4 (close-out).

### If Variation B is alive
- [ ] **Day 15–17 (4 hours) — Survey email list**
  - Send a 5-question survey to all signups: which palm-derived "focus" sounds most useful (5 options)? would you pay $9.99/mo? what would make you stop using such an app?
  - Target: ≥30% response rate
- [ ] **Day 18–21 (4 hours) — Wizard-of-Oz pilot**
  - Pick top 10 most engaged respondents
  - Manually send each a personalized "weekly palm-derived reflection" via email — *you* write it, no app
  - Measure: do they reply? do they engage? do they ask for the second one?
  - **Pass:** ≥6/10 reply with engagement signal AND ≥3/10 ask "when can I pay for this?"

### If Variation C is alive
- [ ] **Day 15–17 (6 hours) — Build clickable mockup**
  - No code. Figma or even Notion-page mockup of the embed widget
  - Show 3 customers from the interview list: "would you pay $19/mo for this if it worked?"
- [ ] **Day 18–21 (6 hours) — Hand-build 1 manual integration**
  - Pick 1 friendly Etsy seller from interviews
  - Manually generate palm readings for their next 5 customer orders (using ChatGPT yourself, formatted in their brand)
  - Charge them $49 flat for the week
  - Measure: did the seller pay? did their customers like it? does the seller want week 2?

---

## Week 4 — Decide & Document (Days 22–30)

### Goal
Make a clear go / no-go / pivot decision and write it down.

### Tasks
- [ ] **Day 22–25 — Compile evidence**
  - One-page verdict per variation citing specific numbers (signups, conversion rates, LOIs, paid pilots, engagement rates)
  - Identify the *single most important assumption that's still untested*
- [ ] **Day 26–28 — Decision meeting (with yourself)**
  - Write down the decision and *why* — 1 page max
  - Three possible outcomes:
    - **GO:** one variation has clear demand signal + viable economics. Define the next 60-day build sprint.
    - **PIVOT:** the original variations failed but the interviews/data revealed a third opportunity. Re-run /startup:startup-design on the new framing.
    - **STOP:** no signal. Document what you learned and apply it to the next idea.
- [ ] **Day 29–30 — Write learning doc**
  - Save to `palm-reading-app/learnings.md` regardless of outcome
  - Include: what you tested, what worked, what didn't, and what surprised you
  - This is the most valuable output of the 30 days *even if you stop* — it sharpens your next attempt

---

## Budget Summary

| Item | Cost |
|---|---|
| Variation B ad test (TikTok + Pinterest + IG) | $200 |
| Wizard-of-Oz pilot tools (Mailchimp / Buttondown free, Carrd $19) | $19 |
| Variation C manual pilot (your time, $0 out-of-pocket) | $0 |
| Optional: TikTok creator pilot ad ($50) | $50 |
| Buffer | $50 |
| **Total** | **~$320** |

---

## Hard Rules

1. **No app development this month.** If you find yourself writing Swift / Kotlin code before Day 30, you've already lost.
2. **Document everything.** Every interview, every signup count, every comment-section tally. Future-you needs the artifacts.
3. **Trust the kill criteria.** If Experiment 1 fails, the right move is to stop, not to look harder for permission to keep going.
4. **Talk to humans.** This entire plan is gated by 10 conversations with real potential users/customers. Don't replace them with more research.

---

## When You're Done

Come back with the learning doc and run `/startup:startup-design` again on whichever variation survived (or on the new direction the data revealed). The next pass will be much sharper because you'll have real evidence to feed it.
