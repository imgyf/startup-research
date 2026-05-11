# Validation Experiment Design — Top 3 (Plus 1)

**Phase:** 8 — Validation (Fast Track)
**Project:** trading-card-collection-manager
**Date:** 2026-05-10
**Confidence:** High (experiments are concrete, low-cost, and produce binary signals)

---

## Experiment Selection Logic

The 30-day validation phase has four critical unknowns to resolve. Three are highest-leverage and need formal experiments; the fourth is a hands-on feature audit that is procedurally simple and is included for completeness.

| # | What's tested | Why it's critical |
|---|---------------|-------------------|
| 1 | Customer pain reality | If pain is "annoying" not "burning," conversion will collapse to <1% |
| 2 | Pricing-data feasibility | If data costs >$300/mo, model breaks |
| 3 | Organic-channel pull (Pocket wedge) | If no organic signal, paid acquisition is unviable, business is unviable |
| 4 | Competitor feature audit (Collectr PRO) | If wedge feature already exists in incumbent, differentiation evaporates |

---

## Experiment 1 — Customer Discovery Interviews (10 sessions)

### Hypothesis
*"Serious Pokemon collectors with 200–2,000 cards experience acute, recurring pain managing their collection's value, current tools (spreadsheet + eBay tabs) break at this scale, and they would pay $4.99–$9.99/mo for a Pokemon-native app that solves it."*

### Method
1. **Recruit:** Post in r/pkmntcgcollections and r/pkmntcgtrades. Title: *"Solo dev building a Pokemon collection app — 30-min Zoom for $20 Amazon gift card to hear what your current workflow is missing."* Comply with subreddit rules (likely require mod approval — DM mods first).
2. **Targeting:** Filter respondents for "200+ cards" and "currently uses spreadsheet OR Pokellector OR Collectr OR nothing." Reject sub-50 card and graded-only collectors.
3. **Schedule:** 10 interviews over 2 weeks. Zoom or Discord voice. 30 min each.
4. **Script** (in order, do not lead):
   - "Walk me through the last time you wanted to know a specific card's value. What did you actually do?" (observation, not solution)
   - "What's the most annoying part of managing your collection right now?" (pain identification)
   - "What tools do you currently use? Why those specifically?" (alternatives audit)
   - "Tell me about the last time you considered switching tools. What stopped you?" (switching cost)
   - "How would your life be different if you could [reflect their stated pain back] in seconds?" (value test)
   - "If a tool did exactly that, what's the most you'd pay per month?" (pricing — open-ended)
   - "What would have to be true for that to be worth $9.99/mo?" (pricing pressure test)
   - "Where would you have heard about a tool like this?" (channel discovery)
   - **End with:** "If I built this, would you want me to email you when there's a beta?" (intent capture; collect email)

### Metrics & Success Criteria
- **Primary:** ≥7 out of 10 interviewees describe a recurring, self-acknowledged collection-tracking pain that is current (in the last 30 days), not historical
- **Primary:** ≥6 out of 10 say they'd pay something for a working solution
- **Primary:** ≥4 out of 10 say "$5–10/mo" or higher when asked unprompted what they'd pay
- **Secondary:** ≥7 out of 10 leave their email for the beta waitlist
- **Secondary:** Capture verbatim language for use in marketing copy
- **Secondary:** Identify 1+ feature gap the founder did NOT predict (signals depth of customer understanding)

### Time & Cost
- **Time:** 20 hours founder time over 2 weeks (10 interviews × 1.5 hrs incl. notes + recruit messaging)
- **Cost:** $200 ($20 × 10 gift cards)

### Result interpretation
- **PASS:** ≥3 of 4 primary metrics hit. Pain is real and monetizable.
- **MIXED:** 2 of 4. Pain is real but pricing or channel signal is weak — adjust accordingly.
- **FAIL:** ≤1 of 4. Pain is "annoying," not "burning." **Stop or pivot.**

---

## Experiment 2 — Pricing-Data Feasibility Audit (Trade-Off)

### Hypothesis
*"There exists a paid Pokemon-pricing-data provider whose cost (≤$200/mo at <500 daily active users), ToS (allows display in a paid mobile app), and data quality (eBay sold-comps for ≥80% of US-printed Pokemon cards) make the planned business model financially viable."*

### Method
1. **List providers (already identified in research):** JustTCG, Scrydex, TCG API, PokeWallet, Ximilar (image-recognition only, not price), and any others surfaced via Google.
2. **For each (~3 hrs/provider):**
   - Sign up for free tier or trial
   - Email or chat sales for: (a) production pricing tiers, (b) ToS for redistributing prices in a paid mobile app, (c) coverage of eBay sold-comp data vs. TCGplayer asks vs. Cardmarket EUR, (d) update frequency, (e) historical-data depth.
   - Fetch sample data for 50 cards across 5 set generations and verify quality vs. eBay sold listings (manual spot-check)
3. **Read eBay Browse API ToS section on third-party display.** Document interpretation; if ambiguous, consult a contract lawyer for 1 hour ($150–300).
4. **Construct a 3-tier cost matrix:** Best-case (cheapest viable provider), expected-case (mid-tier), worst-case (most-credible-data provider).

### Metrics & Success Criteria
- **PASS:** At least one provider hits ≤$200/mo at 500 DAU pricing tier, allows redistribution in a paid app, covers ≥80% of relevant Pokemon cards including some eBay sold-comp signal.
- **MIXED:** Pricing in $200–400/mo range with workable terms — forces price increase to $7.99/mo or feature-scope reduction (e.g., daily refresh, not real-time).
- **FAIL:** No provider meets ToS + cost requirements. **Pivot the headline feature** away from real-time pricing aggregation toward catalog-completeness + condition-tracking (which doesn't need third-party live pricing).

### Time & Cost
- **Time:** ~15 hours founder time over 1 week
- **Cost:** $0–500 (lawyer consult if needed; potentially $50 for a 1-month paid trial of a top candidate to see real production data)

### Result interpretation
This is the most actionable single experiment. The result directly determines whether the planned pricing ($5.99/mo) holds, must rise, or whether the entire feature framing must shift.

---

## Experiment 3 — Pocket-Wedge Channel Test

### Hypothesis
*"Pokemon TCG Pocket players are a viable top-of-funnel for a physical-card collection app — at least 1% of Pocket users on r/PTCGP are also active physical collectors, and a free utility tool can convert that crossover audience to a waitlist for the physical app at ≥10% click-through."*

### Method
1. **Build a tiny, scope-controlled web utility** (no app required):
   - "Pokemon TCG Pocket Trade Fairness Calculator" — paste in two card lists from Pocket, get a fairness score based on rarity/recency.
   - Or: "Pocket Collection Completion Tracker" — paste your Pocket booster code, see what % of the current set you have.
   - Single-page web app, no auth, no backend (or minimal). Build estimate: 8–12 hours of dev time.
2. **Add a banner footer:** *"Building the same kind of tool for your physical Pokemon collection — get notified at launch."* → email capture form.
3. **Post in r/PTCGP** (active Pocket subreddit, ~500K+ members, less moderated than r/PokemonTCG): one post titled clearly as "I built a free utility for Pocket trades — feedback welcome." Comply with self-promo rules; if any.
4. **Post 2 TikTok videos** demonstrating the tool with a "I'm building a physical-card version" hook.

### Metrics & Success Criteria
- **Primary:** ≥1,000 unique sessions on the utility within 2 weeks
- **Primary:** ≥10% click-through rate from utility users to the waitlist signup
- **Primary:** ≥100 emails captured for the physical-card-app waitlist
- **Secondary:** Reddit upvotes ≥50 on the launch post (signals not-rejected by community)
- **Secondary:** TikTok views ≥5,000 across both videos
- **Secondary:** Track waitlist email survey question: "Are you a physical Pokemon collector with 100+ cards?" — measure crossover rate

### Time & Cost
- **Time:** ~25 hours total (12 hrs dev + 6 hrs content + 7 hrs community participation around launch)
- **Cost:** $0 (free hosting on Vercel/Cloudflare Pages)

### Result interpretation
- **PASS:** All 3 primary metrics. The Pocket wedge is real, GTM viability confirmed.
- **MIXED:** 2 of 3. Channel works for awareness but not signup intent — pivot to Reddit-direct content + creator gifting only.
- **FAIL:** ≤1 of 3. The Pocket bridge is a story without substance — fall back to organic Reddit + creator gifting only, lower Y1 download projections by ~50% to Conservative scenario.

---

## Experiment 4 — Competitor Feature Audit (Collectr PRO)

### Hypothesis
*"Collectr PRO does not offer per-card eBay-sold-comp custom price alerts, leaving an explicit feature gap in the dominant competitor's offering."*

### Method
1. Subscribe to Collectr PRO ($4.99/mo, single month).
2. Use the app daily for 1 month, with a 50-card test collection that includes:
   - 10 Pokemon English modern cards
   - 10 Pokemon English vintage (WOTC)
   - 10 Pokemon Japanese (test if supported)
   - 10 graded PSA cards
   - 10 sealed product items (test if supported)
3. **Document every feature with screenshots.** Specifically test for:
   - Per-card price alerts? Threshold-based or just notifications on rarity?
   - Pricing source — TCGplayer asks, eBay sold-comps, or both?
   - Japanese-set support depth?
   - Sealed-product tracking?
   - Bulk import?
   - CSV export?
4. **Repeat for CollX Free + CollX Pro (1 month).**
5. **Repeat for Shiny + PokeScope** (free testing, paid if needed).

### Metrics & Success Criteria
- **PASS:** Confirms Collectr lacks custom per-card eBay-sold price alerts → wedge is real.
- **MIXED:** Confirms Collectr has some alerts but they're rarity-based or low quality → wedge weakened but not gone.
- **FAIL:** Confirms Collectr PRO has full custom per-card eBay-sold alerts → wedge feature collapses; founder must find a different differentiation angle (e.g., Japanese-set depth alone, condition-tracking, or community).

### Time & Cost
- **Time:** ~12 hours of attentive use across 1 month (averages 25 min/day)
- **Cost:** ~$30 (Collectr PRO + CollX Pro + maybe Shiny/PokeScope premium)

### Result interpretation
This is the cheapest of the four experiments and produces the highest-leverage information about whether the planned wedge survives.

---

## Experiment Sequence (Recommended)

Run in parallel where possible to fit in 30 days:

| Week | Activity |
|------|----------|
| Week 1 | E2 (Pricing-data audit) — research/contact providers in parallel with E4 (Collectr PRO subscription) |
| Week 1–2 | E1 (Customer interview recruit + first 5 interviews); E4 (continue documenting Collectr) |
| Week 2 | E3 dev (Pocket utility build) — 2-3 evenings |
| Week 3 | E1 (last 5 interviews); E3 (post utility, drive traffic) |
| Week 4 | Synthesize all results → make build-or-walk decision |

**Total time: ~70 hours over 30 days. Total cost: <$1,000.** This is the cheapest possible derisking of a 4–6 month MVP build commitment.

---

## What This Protects Against

| Failure mode this experiment set prevents |
|--------------------------------------------|
| Building 4 months of MVP only to discover collectors are satisfied with their spreadsheet (E1) |
| Pricing the subscription at $5.99 only to discover data costs are $400/mo at scale (E2) |
| Investing in a Pocket-wedge GTM that produces zero conversion (E3) |
| Marketing "custom price alerts" as a wedge that already exists in Collectr (E4) |

Any one of these failure modes would represent a 4–6 month, 250-hour wasted effort. The experiments collectively cost <70 hours and <$1,000 to prevent them.

---

## Strategic Connections

- **→ `06-validation/scorecard.md`** — Score moves from 5.4 toward 7+ if 3 of 4 experiments PASS, toward 3- if 3 of 4 FAIL.
- **→ `06-validation/kill-criteria.md`** — Each experiment has formal pass/fail thresholds that map to kill-or-pivot decisions.
- **→ `01-discovery/research-gate.md`** — These four experiments are the four gates the Research Gate identified.
- **→ `action-plan-30-days.md`** — Week-by-week schedule maps to this experiment sequence.

## Flags

**Red Flags:**
- If the founder skips E1 (customer interviews) and goes straight to MVP, this is the highest-probability path to a months-of-wasted-time outcome. The interview is non-negotiable.

**Yellow Flags:**
- E3 (Pocket wedge test) requires public posting which exposes the project idea pre-MVP. Keep the project name + branding ambiguous; the goal is signal, not stealth.
- E2 (data API audit) interpretation of eBay ToS is genuinely ambiguous; lawyer consultation recommended even at $300 cost.
