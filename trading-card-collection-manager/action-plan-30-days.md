# 30-Day Action Plan

**Project:** trading-card-collection-manager
**Date:** 2026-05-10
**Mode:** Pre-build validation phase (NOT MVP development)

---

## Premise

Phase 8's scorecard returned **5.4/10** — Conditional. The founder must run four validation experiments before committing to MVP development. This plan schedules those experiments week-by-week so they can be executed at side-project pace (~15 hrs/week).

If, at the end of 30 days, **3 of 4 experiments PASS**, the founder has earned permission to start building. If **2 or fewer PASS**, this plan ends with a written "stop or pivot" decision.

---

## Week 1 — Founder Immersion + Pricing-Data Audit

**Theme:** Become a participant, not just an observer. Resolve the data-cliff question.

| Day | Task | Time | Output |
|-----|------|------|--------|
| Mon | Subscribe to Collectr PRO ($4.99). Begin the 1-month feature audit (Experiment 4). Set up screenshot folder, daily 15-min log. | 1.5 hr | Audit log started |
| Mon | Email/contact JustTCG, Scrydex, TCG API requesting: (1) production pricing tiers, (2) ToS clauses on display in paid mobile apps, (3) eBay sold-comp coverage. Use a single-page comparison spreadsheet to capture responses. | 2 hr | 3 vendor emails sent |
| Tue | Deep-read eBay Browse API current developer agreement. Highlight any clause governing display of pricing data in third-party apps. Flag ambiguity. | 2 hr | Annotated ToS doc |
| Tue–Wed | Begin daily participation in r/pkmntcgcollections (~15 min/day going forward, every day, for the rest of the month and beyond). Comment supportively on collection showcases; do NOT promote anything yet. | 0.5 hr/day × 7 | Reddit account with 5+ helpful comments |
| Thu | Read 30 r/pkmntcgcollections threads from the past 6 months. Capture: language used (verbatim phrases), pain mentions, app references. Build a "Language Map v1" doc. | 3 hr | Language Map v1 |
| Fri | Compile vendor responses into the comparison spreadsheet. Score each: cost, ToS, coverage, quality. Decide: data-cliff PASS / MIXED / FAIL. Document the decision. | 2 hr | Decision recorded |
| Sat | (Optional) If ToS interpretation is ambiguous, schedule a 1-hour contract-lawyer consultation for Week 2. Cost ~$200. | 0.5 hr | Lawyer scheduled |
| Sun | Recap notes; prep customer-interview recruit messaging for Week 2. | 1 hr | Interview script v1 |

**Week 1 deliverable:** GO/PIVOT/STOP signal on Experiment 2 (data feasibility). Daily Reddit participation habit established.

---

## Week 2 — Customer Discovery (First 5 Interviews) + Pocket Wedge Build

**Theme:** Talk to humans. Build the channel test.

| Day | Task | Time | Output |
|-----|------|------|--------|
| Mon | Post a recruit thread in r/pkmntcgcollections (DM mods first to clarify rules). Title: *"Solo dev building a Pokemon collection app — 30-min Zoom for $20 gift card to learn what your current workflow is missing."* Cross-post to r/pkmntcgtrades. | 2 hr | Recruit posts live |
| Tue–Sat | Schedule + conduct 5 customer interviews (Experiment 1). Each = 30 min Zoom + 30 min notes. Use the script from `06-validation/experiment-design.md`. Send $20 gift card after. | 7.5 hr | 5 interview transcripts + notes |
| Tue–Wed | Begin building the Pocket-wedge utility (Experiment 3). Pick one of: trade-fairness calculator OR collection-completion tracker. Choose the simpler one — single-page web app, no backend if possible. | 6 hr | Utility v1 functional |
| Thu | Continue interviewer scheduling for Week 3 batch (5 more). | 1 hr | 5 more interviews scheduled |
| Fri | Write up consolidated interview notes from this week's 5: pain hierarchy, language patterns, pricing reactions, feature surprises. | 2 hr | Interview notes round 1 |
| Sun | Continue daily Reddit (15 min). Note any Pokellector / Collectr / app-related complaints in r/pkmntcgcollections feed. | 0.25 hr × 2 | Competitive intelligence log |

**Week 2 deliverable:** 5 interviews complete + Pocket utility 80% built. Initial customer-pain signal directional.

---

## Week 3 — Customer Discovery Round 2 + Pocket Utility Launch

**Theme:** Complete interviews. Test the channel.

| Day | Task | Time | Output |
|-----|------|------|--------|
| Mon | Final polish on Pocket utility. Add waitlist email-capture footer ("Building the same kind of tool for your physical collection"). Deploy to Vercel/Cloudflare Pages. | 3 hr | Live URL |
| Mon | Post the Pocket utility on r/PTCGP. Title focused on the utility itself, not promotion. Engage actively in comments for 4 hours after posting. | 3 hr | Reddit post + responses |
| Tue | Record 2 short TikTok videos demonstrating the Pocket utility. Hook: *"I built this for Pocket. Building the same for physical Pokemon next."* Post both. | 2 hr | 2 TikToks live |
| Tue–Sat | Conduct 5 more customer interviews (rounds 6–10). | 7.5 hr | 10 interviews complete |
| Wed | Continue daily Reddit (15 min). | 0.25 hr × 7 | (week-long habit) |
| Fri | Begin in-app testing of Collectr PRO competitor features for the Experiment 4 audit. Document with screenshots. | 1 hr | Audit progress |
| Sat | Synthesize all 10 interviews. Update the Language Map and Pain Hierarchy documents. Re-write the "primary persona" in `target-audience.md` with verbatim quotes replacing hypotheses. | 4 hr | Pain hierarchy v2 (data-backed) |
| Sun | Read all utility analytics + waitlist signups. Document Pocket-channel signal. | 1 hr | Channel-test data |

**Week 3 deliverable:** Customer interviews complete. Pocket-wedge channel data in. Competitor audit ~70% complete.

---

## Week 4 — Decision Week

**Theme:** Synthesize evidence. Make the build-or-walk call.

| Day | Task | Time | Output |
|-----|------|------|--------|
| Mon | Finalize Experiment 4 (Collectr PRO audit). Document feature parity gap. PASS / MIXED / FAIL on wedge hypothesis. | 3 hr | Audit complete |
| Tue | Cross-reference all 4 experiments. Score each formally against the criteria in `06-validation/experiment-design.md`. | 2 hr | Score sheet |
| Wed | Update the Lean Canvas based on what was learned. Adjust price if interviews demanded it. Re-run the financial model with corrected assumptions. | 4 hr | Canvas v2 + Financial v2 |
| Thu | Make the formal decision and document it. Three possible outcomes: |
| | **GO** — 3 of 4 PASS. Commit to MVP build (next 30-day plan = MVP scoping). |
| | **PIVOT** — 2 of 4 PASS, but the failures suggest a different framing. Document the new framing and re-run a focused 2-week mini-validation. |
| | **STOP** — ≤1 of 4 PASS, or any single experiment is a definitive STOP signal (e.g., wedge collapsed, no customer pain). Write the post-mortem. | 4 hr | Decision document |
| Fri | Pre-commit (in writing, even to yourself) to honoring kill criteria KC1, KC3, KC4 from `kill-criteria.md`. Send a copy to a trusted accountability partner. | 1 hr | Pre-commitment letter |
| Sat | If GO: Begin MVP scoping (RICE-prioritize features from Lean Canvas Solution cell, draft a 60-day MVP build plan). | 4 hr | MVP scope doc OR pivot/stop announcement |
| Sun | Continue daily Reddit (15 min). Now beginning to be perceived as a regular community member. | 0.25 hr | Habit continued |

**Week 4 deliverable:** Build decision made. If GO, MVP plan exists. If PIVOT, new framing with 2-week mini-validation. If STOP, public sunset post and lessons-learned doc.

---

## Total Time, Cost, and Outcome

- **Founder time:** ~70 hours over 30 days (~2.3 hrs/day average; ~16 hrs/week — comfortable side-project pace)
- **Cash cost:** $200 (interview gift cards) + $30 (Collectr PRO + competitor subs) + $0–500 (optional lawyer) + $0 (Pocket utility hosting) = **$230–730 total**
- **What you'll know on Day 30 that you don't know today:**
  - Whether the customer pain is real and monetizable
  - Whether you can afford to build this with paid pricing data
  - Whether your wedge feature actually exists as a competitor gap
  - Whether your assumed organic GTM channels actually work
  - Whether YOU can be present as a community member, not just a builder

If after 30 days you cannot make a confident GO call with 3+ experiment passes, **the cost of stopping is $700 + 70 hours**. The cost of building first and discovering this in month 5 is **$0 spent + 250 hours of wasted dev + a half-finished app**.

---

## Day-by-Day Anti-Patterns to Avoid

- **Don't start coding the MVP** during these 30 days. The temptation is real. If you start building, you'll prioritize coding over interviews and the validation collapses.
- **Don't post the Pocket utility on r/PokemonTCG (1.3M subs).** It will be removed for self-promo and may damage your account. Stick to r/PTCGP and r/pkmntcgcollections.
- **Don't lead the customer interviews to your assumed pains.** Open-ended questions only.
- **Don't subscribe to a 1-year contract** with a pricing-data provider until at least Week 4. Use trials and monthly tiers.
- **Don't skip the ToS read on eBay Browse API** because "everyone scrapes anyway." A C&D from eBay's legal team kills startups; an honest read takes 2 hours.
- **Don't try to brand the project yet.** Naming, logo, color palette — all wasted effort until validation passes.

---

## Beyond Day 30 (If GO)

If validation passes, the next 30 days are MVP scoping + initial build:

- Days 31–45: RICE-prioritize features. Pick the smallest viable subset. Build a paid waitlist landing page (collect $5 deposits as conviction-test if comfortable with the "pay before product" model).
- Days 46–90: Build MVP (3 problems → 3 solutions from the Lean Canvas, no more).
- Days 91+: Beta with the 100 people on the waitlist. Iterate on real usage data.
- Months 5+: Public launch. Begin the slow-compound grind described in the financial projections.

---

## Beyond Day 30 (If STOP)

A graceful stop is a real outcome with real value:

- Write the post-mortem publicly (LinkedIn, blog, Reddit). The Pokemon community will respect honesty more than a half-finished app.
- The 70 hours of customer interviews + market research is portable to OTHER startup ideas. The skill of validation-first thinking compounds.
- The 30-day window has explicitly NOT consumed your savings, your relationships, or a year of life.

This is the expensive insurance policy that protects against the much-more-expensive default outcome of "just build it and see."
