# Validation Playbook

**Phase:** 8 — Validation
**Project:** pokemon-champions-team-workspace
**Date:** 2026-05-10
**Confidence:** Medium-High (each experiment maps directly to a Phase 3 unknown; sequencing is opinion)

---

## Sequencing Principle

> **Cheapest, fastest, riskiest-assumption-first.**

The single biggest unknowns from research are: (a) does WolfeyVGC or another top creator agree to partner; (b) does Persona C respond to our specific positioning; (c) does the AI coach's grounded approach actually feel different from VGCCoach in practice; (d) is $25/mo Tournament Prep WTP real.

Run validation in this order, not in product-build order.

---

## Experiment Sequence

### Week 1 — Customer Discovery + Advisor + Creator Outreach

**E1: 15 customer-discovery interviews (Persona C/B)**

- *Tests:* Are the pains we identified the real pains? Is "between tournaments" framing resonant? Would they pay $12-25/mo?
- *Method:* DM 50 active posters on r/stunfisk (filter for tournament/Regional mentions in their post history). Offer a 20-minute call. Ask open-ended: "Tell me about how you prep for a Regional. Walk me through last week."
- *Measure:* Verbatim language, current tool stack, number who confirm WTP at $12 / $25 specifically (test both prices)
- *Validation threshold:* ≥10/15 confirm tool fragmentation + matchup uncertainty pains; ≥5/15 say "I would pay" at $12/mo
- *Cost:* Founder time, ~10-15 hrs
- *Deliverable:* Raw call notes + 1-page synthesis

**E2: Recruit a competitive-player advisor**

- *Tests:* Is there a credible competitive player willing to advise / be visible on the team?
- *Method:* Identify 5-10 candidates from Smogon ladder leaders, Regional top-cuts, mid-tier creators. Cold outreach — equity / revshare offer. Have a 15-minute pitch ready.
- *Measure:* Did anyone say yes within 2 weeks?
- *Validation threshold:* 1 advisor signed within Week 2
- *Cost:* Founder time + potential equity dilution
- *Deliverable:* Signed advisor agreement OR pivoted plan B (team-of-3 informal advisors)

**E3: Top-3 creator partnership outreach**

- *Tests:* Is WolfeyVGC / CybertronVGC / Brady Smith open to a Patreon-tier-locked partnership?
- *Method:* Direct message via Patreon DMs, X DMs, business contact emails on their websites. Pitch concise: free Pro for top tier patrons + revshare on conversions. Optional advisor seat for the lead partner.
- *Measure:* Replies, meeting bookings, terms discussed.
- *Validation threshold:* At least 1 of the 3 expresses real interest within 4 weeks (not commitment, but conversation in motion)
- *Cost:* Founder time + future revshare commitments
- *Deliverable:* Creator partnership log; signed term sheet (at least non-binding) by Week 8

---

### Weeks 2-3 — Landing Page + Pricing Test

**E4: Landing page with email capture**

- *Tests:* Does the positioning copy resonate enough to capture email signups from cold traffic?
- *Method:* Single-page site: hero, value prop, three feature highlights (workspace, grounded coach, tournament prep), pricing tiers, founder + advisor names, email capture. No product yet.
- *Measure:* Visitors → email captures. From Reddit organic + X content + creator soft-mentions.
- *Validation threshold:* ≥10% conversion of visitors to email; ≥500 emails captured in 30 days
- *Cost:* ~5-10 hrs founder time + $50/mo hosting + analytics
- *Deliverable:* Live landing page; email list growth dashboard

**E5: Pricing test ($12 vs $15 vs $25)**

- *Tests:* What pricing maximizes signal? Specifically, is $25/mo Tournament Prep too high?
- *Method:* On the landing page pricing section, A/B test three configurations:
  - Variant A: Pro $9, TP $19
  - Variant B: Pro $12, TP $25 (current plan)
  - Variant C: Pro $15, TP $30
- *Measure:* Email capture rate per variant, plus a "which tier are you most interested in?" follow-up question
- *Validation threshold:* Variant B converts within 70-100% of Variant A's rate (small enough drop-off to justify the higher pricing)
- *Cost:* 2-3 hrs founder time
- *Deliverable:* Pricing data table + recommendation

**E6: Reddit testing post — positioning**

- *Tests:* Does the positioning land in Persona C/B's home community?
- *Method:* Founder writes a thoughtful r/stunfisk post titled something like "I'm building a workspace for VGC tournament prep — would love to validate the problem before I build it." Lead with the pain, not the solution. Ask for feedback.
- *Measure:* Upvotes (>50 = working; >200 = strong signal), comment quality, hostile vs. constructive reactions, email captures driven from post
- *Validation threshold:* >50 upvotes; >25 substantive comments; <20% hostile reception
- *Cost:* 3-5 hrs founder time including engagement
- *Deliverable:* Post archived + verbatim feedback collated

---

### Weeks 4-6 — Closed Beta + Wizard-of-Oz AI Coach

**E7: Wizard-of-Oz AI coach prototype**

- *Tests:* Does the *grounded coach* experience feel meaningfully different from VGCCoach / ChatGPT? Will users return?
- *Method:* Before building the full grounded stack, create a thin web app that lets users submit a team + question. Founder manually answers using Showdown's damage calc + sim, with explicit citations. Aim to respond within 10 minutes.
- *Measure:* Number of unique users who submit ≥3 questions; qualitative responses to "how does this compare to ChatGPT for the same question?"
- *Validation threshold:* 5+ unique users submit 3+ questions each in 2 weeks; 4+ explicitly note the citation/grounding feels valuable
- *Cost:* ~10-20 hrs founder time + 1 simple form-and-database app
- *Deliverable:* Validation memo on whether the grounded approach is differentiating

**E8: Closed beta with 30-50 invitees**

- *Tests:* Does the actual MVP (when shipping) deliver on activation, conversion intent, and value?
- *Method:* Invite-only beta. Recruit from E1 interviewees, E4 email list, E6 Reddit responders, E7 prototype users. Build invite codes; observe usage.
- *Measure:*
  - Activation: % saving 2+ teams in 7 days
  - Engagement: % using AI coach ≥5 times in 14 days
  - Stated WTP: % saying "yes I'd pay $12/mo" in survey
  - Bug/issue density per user (target: <3 issues/user, indicating quality MVP)
- *Validation threshold:* ≥60% activation; ≥50% coach engagement; ≥30% stated WTP at $12
- *Cost:* Founder time + LLM API costs
- *Deliverable:* Beta retrospective + go/no-go for public launch

---

### Weeks 7-12 — Public Launch + Real Conversion Data

**E9: Public launch + 30-day cohort metrics**

- *Tests:* Does Free → Pro conversion hit Base scenario (2.5%)? Does AI coach engagement hold up at scale? Does retention through tournament cycle hold?
- *Method:* Public launch via Reddit + creator partnership + founder content. Track first 30-day cohort tightly.
- *Measure:*
  - Free signups
  - Free → Pro 30-day conversion rate
  - Free → TP direct conversion rate
  - 4-week retention (paid)
  - Coach engagement (turns/user/week)
- *Validation threshold:* All of: 1,000+ signups in 30 days; 2%+ conversion; 70%+ 4-week retention; <5% hallucination complaint rate
- *Cost:* Already-built MVP + ongoing founder time
- *Deliverable:* Cohort dashboard + Month-1 retro

**E10: Tournament-cycle retention (E9 follow-on)**

- *Tests:* Do users come back after their first tournament prep cycle?
- *Method:* Track weekly active paid through Worlds prep window (Aug 2026)
- *Measure:* % of Pro users who used the coach in the week after Worlds; % who created a new team version post-tournament
- *Validation threshold:* ≥60% return engagement post-tournament
- *Deliverable:* Tournament-cycle retention curve

---

## Quick-Reference Validation Roadmap

| Week | Experiment | Cost | Decision impact |
|---|---|---|---|
| 1 | E1 interviews + E2 advisor + E3 creator outreach | Founder time | Kill or continue |
| 2-3 | E4 landing + E5 pricing + E6 Reddit | $50 + time | Refine positioning |
| 4-6 | E7 wizard-of-oz coach + E8 closed beta | Time + LLM | Validate AI value prop |
| 7-12 | E9 public launch + E10 tournament cycle | Already invested | Scale or pivot |

---

## What Each Experiment Validates / Invalidates

| Experiment | Validates | Invalidates if... |
|---|---|---|
| E1 interviews | Pain framing + persona match | <8/15 confirm pains → wrong persona or wrong pain |
| E2 advisor | Founder credibility addressable | No advisor in 4 weeks → MVP launch likely premature |
| E3 creator | GTM channel viable | All 3 decline → must rebuild GTM around content/SEO alone |
| E4 landing | Positioning resonates | <5% email conversion → positioning wrong |
| E5 pricing | $12/$25 WTP | Variant B converts <50% of Variant A → reduce price |
| E6 Reddit | Community accepts framing | >40% hostile → wrong tone or wrong pitch |
| E7 wizard-of-oz | AI coach differentiating | Users don't return → pivot from "coach" to pure workspace |
| E8 beta | MVP is shippable | Activation <30% → product not ready |
| E9 public | Hypothesis valid at scale | Conversion <1% → fundamental product or market mismatch |
| E10 retention | Tournament cycle compounds | Retention <40% → seasonal-only product, smaller business |

---

## Flags

**Red Flags:**
- None.

**Yellow Flags:**
- E7 (wizard-of-oz coach) requires founder to manually answer questions for 2 weeks. This is exhausting but cheaper than building the wrong product.
- E1 (interviews) is the highest-leverage activity in Week 1. Founders skip this and regret it.
- E5 (pricing test) could be misleading from a small sample. Treat directional, not definitive.

## Sources

- `01-discovery/research-gate.md` — three-pivot decision and risks
- `02-strategy/go-to-market.md` — channel rankings
- `04-product/mvp-definition.md` — features being validated
- `05-financial/revenue-model.md` — conversion thresholds
