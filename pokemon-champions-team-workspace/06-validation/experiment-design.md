# Experiment Design — Top 3

**Phase:** 8 — Validation
**Project:** pokemon-champions-team-workspace
**Date:** 2026-05-10
**Confidence:** Medium-High (designs follow standard customer-discovery and lean-validation practice)

---

## Why These Three

From the playbook, the top 3 highest-leverage experiments are:

1. **E1 — 15 customer-discovery interviews** (validates A4, A5, A2, A3 — the foundation of every other assumption)
2. **E3 — Creator partnership outreach** (validates A8 — the highest-leverage GTM channel)
3. **E7 — Wizard-of-oz AI coach prototype** (validates A7 — whether the differentiator is real)

These three together address the riskiest assumptions and can run in parallel within the first 4-6 weeks.

---

## Experiment 1 — Customer Discovery Interviews

### Hypothesis

> Persona C (VGC Tournament Aspirants) experience tool fragmentation as a top-2 prep pain, AND will pay $12/mo for a workspace that consolidates teams + matchup notes + grounded AI coach.

### Method

**Recruitment:**
- Target 50 outreach DMs / emails to recruit 15 interviews
- Source pool:
  - r/stunfisk active posters who have mentioned Regionals, Worlds, or VGC tournaments in past 90 days (filter by post search)
  - Pokémon Champions VGC Discord active members
  - X / Twitter accounts using #VGC or #PokemonChampions hashtags with engagement
- Outreach DM template:

> "Hey — I'm building a prep workspace for VGC tournament players (think Notion + grounded AI coach for Pokémon teams). Before I build the wrong thing, I'd love a 20-minute call to learn how you actually prep. No pitch — I just want to understand your workflow. Open to chat in the next 2 weeks?"

**Interview structure (20 min):**

1. (3 min) Warm-up: tell me about your last tournament prep cycle
2. (5 min) Walk me through your current tool stack — concrete example: walk me through how you built and refined your team for [last Regional]
3. (4 min) What's the most frustrating moment in your prep cycle?
4. (3 min) If I waved a wand, what would change?
5. (3 min) Pricing probe: "I'm thinking of charging $X/mo for [described feature set]. Would you pay that? Why or why not?" — test $12 with half, $25 with the other half
6. (2 min) Wrap: would you be willing to try a beta? Can I follow up?

**Important:** Don't pitch. Don't lead. Use silence. Repeat their words back. If they describe a pain you didn't anticipate, follow that thread.

### Metrics

- **Pain validation:** ≥10/15 mention tool fragmentation OR matchup uncertainty in their top 2 pains, unprompted
- **Persona match:** ≥10/15 fit Persona C profile (tournament-prep focus, paying for at least one creator Patreon or Pokémon HOME)
- **WTP signal:** ≥5/15 say "yes, I'd pay $12/mo" without significant pushback; ≥3/15 say "yes" at $25 for Tournament Prep
- **Beta interest:** ≥10/15 say yes to beta invite

### Success Criteria

- ≥2 of 3 metrics hit thresholds → A4, A5 validated; proceed with confidence
- 1 of 3 hits → narrow validation; refine targeting and re-run
- 0 of 3 hits → fundamental persona/pain mismatch; pivot before building

### Cost

- 50 outreach DMs: ~3 hrs founder time
- 15 × 20-min interviews: ~5 hrs
- Synthesis writeup: ~3 hrs
- **Total: ~11-15 hrs over 2-3 weeks**

### Deliverable

- Raw call notes (consent-gated; anonymized in synthesis)
- 1-page synthesis: pain hierarchy ranked by frequency, verbatim language map (top 10 quotes), WTP signal distribution, beta interest list
- Updated `06-validation/assumptions-tracker.md`

### Risk of bad data

- Self-selection bias: people who agree to interview are more engaged than typical Persona C
- Mitigation: include some lurker outreach (DMs to people who comment but don't post often)
- Pricing-question bias: people overstate willingness in interviews vs. checkout
- Mitigation: pair interview WTP with E5 landing-page pricing test

---

## Experiment 3 — Creator Partnership Outreach

### Hypothesis

> At least one of WolfeyVGC, CybertronVGC, or Brady Smith / VGC Corner is open to a Patreon-tier-locked partnership with revshare in exchange for free Pro / Tournament Prep access for their top-tier patrons.

### Method

**Outreach sequencing:**

1. **Brady Smith / VGC Corner (Tier 1 priority — most reachable, most aligned)**
   - Reach via: Patreon DM + email
   - Pitch: "Champion's Notebook is a workspace + grounded AI coach for VGC tournament players. I'd like to offer your top-tier ($X) patrons free Pro for life as a perk. Revshare 20% on conversions you drive. Co-branded landing page. Thoughts?"

2. **CybertronVGC / Aaron Zheng (Tier 1)**
   - Reach via: business email on his website + X DM
   - Pitch: similar; emphasize Stanford-business-savvy framing — "Mobalytics × esports streamers playbook applied to VGC"

3. **WolfeyVGC / Wolfe Glick (Tier 1, highest payoff, hardest to reach)**
   - Reach via: business contact on his Patreon page + Patreon DM + X DM (in that order, 5-day intervals)
   - Pitch: short, specific. "I'm building [X]. Your audience is exactly our target. Open to a 15-min call about a partnership where your top-tier patrons get free Pro indefinite, plus revshare?"

4. **Backup pool (if all 3 decline within 3 weeks):**
   - EmbCommanderVGC, Trainer Tower contributors, smaller VGC creators (5-10 names from `wave2-gtm.md`)
   - Different pitch: "smaller-scale partnership, free Pro for your community Discord, light revshare"

**Engagement tools:**

- A 1-pager PDF describing the product + the partnership offer (carefully designed)
- A short Loom or screen recording of the workspace prototype (after Week 4 when prototype exists)
- A clear "next step" CTA: "20-minute call this week or next?"

### Metrics

- **Reply rate:** Tier 1 reply within 14 days = positive signal; no reply within 21 days = decline signal
- **Meeting bookings:** target 1+ scheduled call within 4 weeks
- **Term-sheet outcome:** target 1 non-binding partnership term sheet within 8 weeks

### Success Criteria

- 1 Tier 1 partnership term-sheet by Week 8 → A8 validated; GTM proceeds as planned
- 0 Tier 1 + 1 backup-pool partnership by Week 8 → partial validation; GTM ramp slower
- 0 partnerships by Week 8 → A8 invalidated; rebuild GTM around founder content + SEO + Reddit organic

### Cost

- Pitch materials prep: ~5-8 hrs
- Outreach + follow-up: ~2-3 hrs/week × 4 weeks = ~10 hrs
- Meetings: ~1-3 hrs across the period
- **Total: ~15-25 hrs founder time**

### Deliverable

- Outreach log (date, channel, reply, status per creator)
- Term sheet drafts as ready
- Updated `06-validation/assumptions-tracker.md` for A8

### Risk of bad data

- Creator ghost-replies are common; a delayed yes is still a yes — don't kill outreach prematurely
- Mitigation: 5-day follow-up cadence; max 3 follow-ups per channel before moving on
- WolfeyVGC may be locked into another partnership; not failure of category, just timing
- Mitigation: assume Wolfey is a stretch; plan around Cybertron + Brady as realistic top tier

---

## Experiment 7 — Wizard-of-Oz AI Coach Prototype

### Hypothesis

> Pokémon competitive players will return to use a grounded, citation-discipline AI coach 3+ times in 2 weeks AND will subjectively report it as "meaningfully different" from ChatGPT or VGCCoach.

### Method

**Setup (1 week build):**
- Simple web form: paste a Showdown team + ask a question + email contact
- Submission → emails the founder + logs to a spreadsheet
- Founder responds within 10 minutes during posted hours (3-hour windows × 4 days/week, posted publicly to manage expectations)
- Each response uses Showdown's damage calc + sim runs + Smogon stats lookup, formatted with explicit citations:

> *"Against typical Reg G rain leads (Pelipper / Kingdra), your Iron Hands is OHKO'd by max-spread Hydration Kingdra Hydro Pump 87.5% of the time [@smogon/calc 506-595 dmg roll]. Pelipper usage in May Smogon stats: 24.3% [smogon.com/stats]. Suggested counter: a Tera Steel pivot or faster Electric — see options in [generated team variant]."*

- Promote prototype on r/stunfisk, X, and to E1 interviewees

**Run for 2 weeks:**
- Track unique users, repeat-question rate, qualitative feedback
- Founder maintains response quality discipline (no shortcuts; every claim cited)

### Metrics

- **Engagement:** ≥10 unique users submit ≥1 question; ≥5 submit ≥3 questions
- **Differentiation perception:** Survey users at end ("How does this compare to ChatGPT for the same question?"); ≥4/10+ say "noticeably different / better"
- **Citation value:** ≥6/10+ say citations make them trust the answer more
- **WTP probe:** Ask "would you pay $X/mo for this responsiveness automated?" — capture pricing reactions

### Success Criteria

- All 3 metrics hit → A7 validated; the grounded approach is the right wedge; build the real coach
- 1-2 hit → mixed signal; refine prompt design / citation UX before building real coach
- 0 hit → A7 invalidated; reconsider the AI coach's role in the product. Maybe pivot to pure workspace + reference-content layer

### Cost

- Build the simple form: ~5-8 hrs
- 2 weeks × 12 hrs/wk founder response time: ~24 hrs (significant — but cheaper than building the wrong product)
- Survey + synthesis: ~5 hrs
- **Total: ~35-40 hrs over 3 weeks**

### Deliverable

- Prototype URL (public)
- Spreadsheet of all interactions (anonymized)
- Survey results
- Synthesis memo: differentiation evidence; UX learnings; whether to invest in the full grounded stack or pivot

### Risk of bad data

- 10-minute response time isn't representative of real product (fast LLM = 5-10 sec); users may overweight the slow speed and underweight the quality
- Mitigation: explicitly note "this is a prototype; in the real product, responses will be 5-10 seconds"
- Founder fatigue producing lower-quality responses by week 2
- Mitigation: cap at 12 hrs/week; have a draft template library ready

---

## Stop / Continue Decision Tree

After all 3 experiments complete (~Week 6):

```
E1 + E3 + E7 results:
  ALL pass thresholds → continue to MVP build with high confidence
  2/3 pass → continue to MVP, address weak area in product or GTM
  1/3 pass → significant pivot needed before MVP build
  0/3 pass → reconsider proceeding; either dramatically pivot or stop
```

This is the **Week 6 gate** — before significant build investment commits.

---

## Flags

**Red Flags:**
- None.

**Yellow Flags:**
- E7 (wizard-of-oz) is exhausting for the founder. Plan rest days; don't burn out before MVP build.
- E3 (creator outreach) carries the longest unknown timeline (creators may take 4-6 weeks to respond). Don't gate MVP build on this completing — gate only the public launch on it.
- E1 interview respondents may not fully represent Persona C — bias toward more engaged users. Triangulate with E4 landing-page data.

## Sources

- `06-validation/validation-playbook.md` — full experiment list
- `06-validation/assumptions-tracker.md` — assumption-to-experiment mapping
- `01-discovery/raw/wave2-gtm.md` — creator outreach details
- `02-strategy/value-proposition.md` — pitch language for outreach
