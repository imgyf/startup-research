# Idea Scorecard — Palm Reading App

**Phase:** 8 — Validation
**Project:** palm-reading-app
**Date:** 2026-05-09
**Confidence:** High
**Mode:** Fast Track

---

## Scorecard — Variation A (literal idea as submitted)

| Dimension | Score (1-10) | Rationale |
|---|---|---|
| **Problem severity** | 3 | Curiosity, not pain. Impulse purchase. Not enough urgency to support recurring sub revenue at scale. |
| **Market size** | 5 | Astrology umbrella is healthy ($4–5B and growing 20%), but mobile-app palm-reading sub-niche is ~$30–80M and largely captured. |
| **Competitive advantage** | 1 | No moat. "AI palm image" replicable in 1–2 weeks. 10+ direct competitors plus free ChatGPT substitute. |
| **Feasibility** | 8 | Buildable in 4–8 weeks by a competent solo dev. The thing works. |
| **Business model clarity** | 4 | Standard weekly-trial sub — *but* unit economics do not close at bootstrap-scale CAC. |
| **Founder-market fit (assumed)** | 2 | Solo technical founder vs. creative-test studios + serial-app TikTok creators. Wrong profile for this game. |
| **Timing** | 2 | Window was 2023 – early 2024. Free ChatGPT-prompt substitute closed it by Q4 2024. |
| **Overall** | **3.6** | **NO-GO** |

---

## Verdict — Variation A

🔴 **NO-GO. Do not build the literal idea.**

The category is mature, saturated, has hostile App Store policy, has a free $0 substitute that 22M+ TikTok posts teach users to use directly, and has unit economics that don't close at any realistic acquisition cost for a bootstrap-scale solo founder.

This is not a "needs more validation" verdict. The research provides clear, converging evidence that the idea-as-submitted is structurally weak.

> The honest summary: **You are 24 months too late, in the wrong cost structure, with the wrong founder profile, against incumbents who already ship your differentiator.** Building this would burn 3–6 months and produce ~$1K–$30K total revenue at best.

---

## What To Do Instead — Two Validate-First Pivots

### Variation B — Palm-themed self-discovery / habit journal

| Dimension | Score (1-10) | Rationale |
|---|---|---|
| Problem severity | 5 | Self-discovery + reflection is a more recurring need than novelty palm reading |
| Market size | 7 | Wellness/journaling app market is $4–6B; less crowded sub-niche |
| Competitive advantage | 5 | Habit-loop + spiritual framing isn't owned by any incumbent; modest moat |
| Feasibility | 6 | Requires content engine + notification design — more work than A |
| Business model clarity | 6 | Yearly $59 pricing model is more defensible; 50% annual retention plausible |
| Founder fit | 4 | Still requires audience-building, but channels are friendlier (Pinterest, wellness influencers) |
| Timing | 6 | "AI for self-improvement" has open headroom; not as saturated as fortune-telling |
| **Overall** | **5.6** | **CONDITIONAL — validate first** |

### Variation C — B2B palm-reading / spirituality content API

| Dimension | Score (1-10) | Rationale |
|---|---|---|
| Problem severity | 6 | Spirituality creators / Etsy sellers / Shopify spiritual brands have a real "how do I add automation" problem |
| Market size | 4 | TAM tens of thousands of creators; ceiling ~$300K–$2M ARR |
| Competitive advantage | 7 | No incumbent in B2B palm-API space; embedding switching costs are real |
| Feasibility | 7 | Solo technical founder can ship this; sales motion is the challenge |
| Business model clarity | 7 | Clear $/usage or $/seat pricing; clean B2B economics |
| Founder fit | 6 | Fits a technical bootstrapper better than mass-consumer mobile |
| Timing | 7 | Creator economy still expanding; spirituality creator vertical lightly tooled |
| **Overall** | **6.3** | **CONDITIONAL — validate first** |

---

## Top 3 Validation Experiments (next 30 days)

### Experiment 1 — ChatGPT Substitution Test (validates whether *anyone* still pays for AI palm reading apps)
**Hypothesis:** If users prefer free ChatGPT prompts on TikTok over paid apps, no version of the idea — A, B, or C — has wind at its back.
**Method:**
1. Pull top 10 TikTok videos tagged #palmreading or #palmistry from past 30 days
2. Read top 100 comments on each — look for: do users mention apps, or only ChatGPT/Gemini? Mention price sensitivity? Mention they paid for a reading?
3. Sample 200 App Store / Play Store reviews on top 5 palm reader apps from past 6 months — what % of negative reviews mention "I can do this free in ChatGPT"?
**Success threshold:**
- Pass: <30% of negative reviews mention free LLM substitute AND >40% of TikTok comments express interest in apps over chatgpt-prompts
- Fail: >50% mention free substitute → kill all variations
**Cost:** $0, 4 hours
**Output:** Brief written verdict.

### Experiment 2 — Variation B Landing-Page Smoke Test (validates demand for "palm-themed self-discovery journal")
**Hypothesis:** A "discover yourself through your palm — daily reflections, weekly insights" wellness positioning attracts ≥80 emails at ≤$3 CAC.
**Method:**
1. Build single-page Carrd / Framer site (1 hour). Hero: "Your palm tells a story. Discover it daily." 1 visualization mockup. Email capture for "early access."
2. Run $200 in TikTok / Pinterest ads with 3 creative variants (founder-talking-head, palm-image, app-mockup)
3. Run for 5 days, measure email captures + cost per email
**Success threshold:**
- Pass: ≥80 signups at ≤$3 each (+ qualitative survey signal)
- Mid: 40–79 signups → iterate, retest
- Fail: <40 signups → drop Variation B
**Cost:** ~$250 (ads + tools), 6 hours setup
**Output:** Email list + verdict.

### Experiment 3 — Variation C Customer Discovery (validates B2B creator demand)
**Hypothesis:** ≥4 of 10 spirituality creators / Etsy reading shops will tell you they'd pay $19–$49/mo for a white-label palm-reading widget.
**Method:**
1. Identify 50 active sellers on Etsy in "tarot reading," "palm reading," "psychic reading" categories with ≥20 sales
2. Identify 20 spirituality TikTok creators with 50K+ followers selling readings or memberships
3. DM / email a short pitch: "I'm researching whether AI palm reading would be useful for sellers like you — could I ask 10 minutes of questions in exchange for early access?"
4. Conduct 10 calls. Specific questions: how do you serve readings today? Would you pay for an API/embed? What price?
**Success threshold:**
- Pass: ≥4/10 explicitly say they'd pay $19+/mo AND ≥2 will commit to a paid pilot
- Fail: <3/10 with payment willingness → drop Variation C
**Cost:** $0, ~10 hours over 2 weeks
**Output:** Interview log + signed-LOI count.

---

## Kill Criteria (run after Day 30)

Stop and document learnings if any of these are true:
1. Experiment 1 finds >50% negative-review mentions of free ChatGPT substitute → all consumer variations dead
2. Experiment 2 yields <40 signups at $3 CAC → Variation B dead
3. Experiment 3 yields <3/10 willingness-to-pay creators → Variation C dead
4. None of the three experiments produced a green signal by Day 30 → close the project, write learnings doc

---

## Flags

**Red Flags:**
- Variation A scorecard 3.6/10 — clearly below 5.0 stop-or-pivot threshold.
- The single largest threat (free ChatGPT substitute) is structural and won't go away.

**Yellow Flags:**
- Variation B scorecard 5.6/10 and Variation C 6.3/10 are both *conditional* — validation, not commitment.

## Sources
- All Phase 3 findings; see `01-discovery/`
