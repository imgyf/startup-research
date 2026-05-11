# Target Audience — Pokemon Serious Hobbyist (Lite Profile)

**Phase:** 3 — Discovery (synthesis, **Fast Track lite version**)
**Project:** trading-card-collection-manager
**Date:** 2026-05-10
**Confidence:** Low-Medium (Wave 3 customer-voice deep-dive was skipped per Fast Track. This document synthesizes available signals from Wave 1–2 research; **founder must do customer interviews in Week 1**.)

---

## ⚠️ Honesty Note

Fast Track mode skipped the dedicated customer-voice + demand-signals research wave. This document is built from indirect evidence: competitor reviews, subreddit observations, market-segmentation logic, and founder-stated assumptions. **Treat every persona detail below as a hypothesis to validate, not a finding.** The 30-day action plan in `action-plan-30-days.md` schedules the customer interviews that should produce the real version of this document.

---

## Primary Persona — "The Returning Hobbyist"

**Vivid sketch (hypothesis, not data):**
- 28–42 years old, US, primarily male (the segment skews male per consumer research; female collectors are a real and growing minority)
- Disposable income $50K+, hobby budget $1K–$5K/year
- Returned to or doubled down on Pokemon collecting during 2020–2022 boom; still active in 2026
- Owns 200–2,000 cards, current value $1K–$50K
- **Currently uses some combination of:**
  - A spreadsheet (~30–40% likelihood)
  - eBay sold-listings as their canonical price-check (~70–85% likelihood)
  - Pokellector or Collectr free tier (~50% likelihood; ~10% paid)
  - Memory + binders + nothing systematic (~20% likelihood)
- **Engages on:** r/pkmntcgcollections (collection showcases), r/pkmntcgtrades (active trading), r/PokemonTCG (general), Pokemon TikTok (passive consumer), occasional Discord servers

**Triggers that make them seek tools:**
- Collection just crossed 500 cards and the spreadsheet is breaking
- Sold a card on eBay and discovered it was worth more than they thought (or less)
- Insurance question after move/theft
- Family asks "what's all this worth?"
- Saw a TikTok of someone's "$30K Pokemon collection tracker" and got curious

**What they value (hypothesis, ranked):**
1. **Knowing what their collection is actually worth right now** (not 6 months ago)
2. **Not having to maintain it manually** (scan and forget)
3. **Trustworthy pricing** ("eBay sold" > "TCGplayer asks" > "some app's number")
4. **Pokemon-native catalog** (Japanese sets, all variants, full set checklists)
5. **Privacy** (do not want to publish their net worth to a community feed)
6. **No ads if they're paying**
7. **Their data not being held hostage** (CSV export, not lock-in)

**What they will NOT pay for:**
- A scanner alone (commoditized, multiple free options)
- "Social" features (most are not in the showcase culture; that's a different sub-persona)
- Marketplace fees on top of subscription

## Secondary Persona — "The Investor-Curious Collector"

- Smaller slice of the base, ~10–15% of paying-eligible
- Sealed-product hoarder + PSA 9/10 graded card stacker
- Uses Card Ladder if grades-heavy; otherwise eBay sold + spreadsheets
- **Higher willingness-to-pay** ($100+/yr is easy)
- Wants: comp-sale alerts, set-completion ROI, condition-stratified valuation
- This is the segment that maps to the brainstorm's V2 "Investor's Edge" variation

## Anti-Persona — Who NOT to Target

- **Casual Pokemon TCG Pocket-only player** — digital-only, no physical collection, will never pay for portfolio tools
- **Competitive player (Standard format meta)** — uses ManaBox-equivalent for deck-building tools, not collection value tracking
- **High-end dealer/LCS owner** — needs B2B inventory + invoicing; different product
- **Casual binder collector with <50 cards** — under the free-tier threshold, will never convert
- **Sports-card crossover collector** — Card Ladder + PSA already serve them well

---

## Pain Hierarchy (Hypothesis — Verify in Customer Interviews)

| # | Pain | Frequency (estimated) | Intensity | Existing alternative |
|---|------|----------------------|-----------|---------------------|
| 1 | "I don't actually know what my collection is worth right now" | Very high | Medium-high (acute on triggers) | Spreadsheet + manual eBay lookup |
| 2 | "Manually entering 500 cards is a nightmare" | High (when entering large collections) | High at moment of entry | Don't enter; or scan-once apps |
| 3 | "TCGplayer asks aren't what I'd actually sell for" | Medium | Medium | Manual eBay sold-listings filter |
| 4 | "I want to know when a card I own gets a comp sale on eBay" | Low–Medium | High when relevant | eBay saved searches per card (impractical at scale) |
| 5 | "I want to track Japanese sets and sealed product, not just NA singles" | Niche but acute | High (deal-breaker for affected segment) | Pokellector (clunky); nothing else |
| 6 | "I want to insure / report-to-tax / show-family the total value" | Low frequency, high intensity | Critical at trigger event | Spreadsheets, screenshots |
| 7 | "I want to see how my collection has appreciated/depreciated over time" | Low–Medium | Medium | Card Ladder (sports-first), not really anywhere for Pokemon |

**The wedge feature mapping:**
- Pain 1 → real-time portfolio value (table stakes)
- Pain 2 → bulk camera scan + bulk CSV import (table stakes)
- Pain 3 → eBay sold-comp aggregation (DIFFERENTIATED — if data ToS allows)
- Pain 4 → custom price alerts (DIFFERENTIATED — if Collectr really doesn't have this)
- Pain 5 → Japanese sets + sealed product + variants (DIFFERENTIATED — Pokemon-only depth)
- Pain 6 → polished export (table stakes)
- Pain 7 → time-series analytics (DIFFERENTIATED but expensive to build)

---

## Jobs-to-Be-Done Framework

**Functional jobs:**
- "Help me know what my collection is worth right now."
- "Help me add 500 cards without losing my mind."
- "Help me decide whether to sell or hold."
- "Help me prove the value to family / insurance / tax."

**Social jobs:**
- "Help me look like a serious collector to my Reddit/Discord peers." (subset)
- "Help me trade fairly without getting ripped off." (subset who use r/pkmntcgtrades)

**Emotional jobs:**
- "Help me feel control over my collection."
- "Help me feel smart about my hobby spending."
- "Reduce the dread of opening the binder and realizing I don't actually know."

---

## Language Map (Hypothesis — verify by reading r/pkmntcgcollections daily for two weeks)

Words customers actually use:
- "My collection" (not "my portfolio", except for the investor sub-persona)
- "Comps" (sold prices on eBay; **use this word**)
- "Pulls" (cards from packs)
- "Sealed" (unopened product)
- "Slabs" or "graded" (PSA/CGC/BGS-encapsulated)
- "Binder" (storage)
- "WOTC" (Wizards of the Coast era — vintage 1999–2003)
- "Modern" (post-Sword & Shield era)
- "Vintage" (WOTC + early-2000s)
- "Chase" (rare card collectors specifically want)
- "Master set" (every card in a set, including reverse holos and variants)

Words the founder should AVOID using in copy:
- "Investor" (alienates the hobbyist majority; reserve for the secondary persona)
- "Asset class" (Wall Street speak)
- "Portfolio" (Wall Street speak; the secondary persona will tolerate it)
- "ROI" / "yield" (alienates)
- "AI-powered scanning" (commoditized, sounds like marketing)

---

## Buying Behavior

**Decision process (hypothesis):**
1. **Trigger** (collection-size pain, trigger event, social signal)
2. **Search** (App Store: "pokemon card scanner", "pokemon collection tracker"; or Reddit: "what app should I use")
3. **Sample** the top 2–3 free apps; usually settles on Collectr if they do nothing else
4. **Friction wall** at 50–100 free cards; either upgrade, switch, or abandon
5. **Pay** if the friction is high enough AND the paid tier feels worth it (this is the conversion moment)

**Decision criteria, ranked (hypothesis):**
1. App store rating (≥4.5 stars table stakes)
2. Reddit consensus ("what's everyone using?")
3. Free tier size (50 cards is now the de-facto floor; below this is hostile)
4. Pricing relative to alternative ($4.99/mo is the anchor; $39.99/yr is fair)
5. Specific feature need (Japanese sets, alerts, sealed)

**Cycle length:** Days to weeks for free signup; weeks to months for paid conversion (if at all).

**Common objections:**
- "I already have a spreadsheet" → must show clear ROI on switching
- "Collectr is fine" → must show Pokemon-specific advantage
- "I don't trust app pricing" → must show data sourcing transparently (eBay sold = credible)
- "I don't want my collection in the cloud" → privacy guarantees, optional anonymous mode, local-first option

---

## Where to Reach Them (Channel Density)

(Cross-references `competitor-landscape.md` Channel Opportunity Map.)

| Channel | Density of target persona | Cost | Notes |
|---------|----------------------------|------|-------|
| **r/pkmntcgcollections** | Very High | $0 | Showcase culture; native screenshot content welcome |
| **r/pkmntcgtrades** | Very High | $0 | Active traders, would benefit most from price alerts |
| **r/PTCGP** (TCG Pocket) | Adjacent (different product) | $0 | 100M+ Pocket users, some bridge to physical |
| r/PokemonTCG (1.3M subs) | High | $0 (but anti-self-promo) | Avoid direct promo |
| **TikTok Pokemon collecting** | High | $0 (organic) – low (gifting) | Micro-creators 5K–50K = best ROI |
| **YouTube Pokemon collecting** | Medium-High | Variable | PokeRev, Smpratte are top-tier; long tail more accessible |
| **Discord servers** (Elite Four, PokeBeach) | Medium | $0 (relationships) | Slow, high trust |
| **App Store search** | High but saturated | $0 | Generic ASO has 10+ competitors page 1 |
| **Pokemon TCG conventions** (PCS-style events) | Niche but high-intensity | Travel cost | Geographically constrained |

---

## Demand Validation — Available Signals

Strong signals from Wave 1–2 (not from a dedicated demand wave):

- **Collectr at 4M users + bootstrapped** → strong evidence the demand exists at scale
- **CollX $10M Series A (March 2025)** → VC validates the demand independently
- **Pokemon = #1 US toy property in 2025 ($2.5B)** → consumer attention is high
- **r/pkmntcgcollections active showcase culture** → engaged community
- **Pokemon TCG Pocket 100M+ downloads** → mobile-Pokemon engagement is at all-time high

**Signals against:**
- Modern singles in 20–30% correction → ARPU compression risk
- TPCi printing -14.3% YoY → supply side anticipates softer demand

**Net read on demand:** Real and at scale. The question is not "is there demand?" but "can a 4th-place entrant capture enough share?"

---

## Data Gaps (this document's biggest weaknesses)

| # | Gap | How to fill |
|---|-----|-------------|
| 1 | Real verbatim quotes from target collectors | Read 50+ r/pkmntcgcollections threads; conduct 10 interviews |
| 2 | Actual prevalence of spreadsheet vs. app users | Survey via Reddit post or Google Form posted in 2 subreddits |
| 3 | Actual willingness-to-pay distribution ($4.99 acceptable? $9.99? $19.99?) | Pricing van Westendorp on a survey |
| 4 | Pokemon TCG Pocket → physical-card crossover rate | Direct question in r/PTCGP and r/PokemonTCG |
| 5 | Exact friction points in current Collectr/Shiny/PokeScope users | App-store negative reviews + Reddit gripe threads |
| 6 | True mix of investor sub-persona vs. main hobbyist persona | Survey question on "do you treat this as collection or investment?" |

---

## Strategic Connections

- **→ `market-analysis.md`** — Persona size estimate (~200K paying-eligible US) is consistent with $10–40M SAM range.
- **→ `competitor-landscape.md`** — Pain hierarchy maps to vulnerability analysis: Pokellector users (Pain 5 + UX) are the easiest displacement target.
- **→ Phase 4 Lean Canvas** — "Customer Segments" cell uses the Returning Hobbyist as primary; "Problem" cell uses Pains 1, 3, 4, 5.
- **→ Phase 8 Validation** — The customer-interview script is the highest-priority experiment because this entire document is hypothesis.

---

## Flags

**Red Flags:**
- This entire persona document is hypothesis. Founder must run customer interviews in Week 1; building before validating these claims is the most likely failure mode.

**Yellow Flags:**
- Founder is light-collector → community language and triggers will feel slightly off without immersion. Two-week r/pkmntcgcollections daily-read habit is non-negotiable.
- The "investor-curious" secondary persona has higher WTP and lower churn but smaller TAM — ongoing tension between primary and secondary segment.

## Sources

- `01-discovery/raw/direct-competitors.md` (review-mining for collector pain)
- `01-discovery/raw/indirect-competitors.md` (status-quo prevalence estimates)
- `01-discovery/raw/competitor-gtm.md` (community channel observations)
- Public observations of r/pkmntcgcollections, r/PokemonTCG, r/pkmntcgtrades
