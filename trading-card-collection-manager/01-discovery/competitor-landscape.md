# Competitor Landscape — Pokemon TCG Collection Apps

**Phase:** 3 — Discovery (synthesis)
**Project:** trading-card-collection-manager
**Date:** 2026-05-10
**Confidence:** Medium-High (10+ competitors profiled with public data; deep feature audit deferred to founder hands-on testing)

---

## Competitive Overview

The Pokemon-collection-tools market is **crowded but not consolidated**. There is a clear leader (Collectr, ~4M users [Estimate]), a well-funded #2 (CollX, $10M Series A, March 2025 [Data, TechCrunch]), several Pokemon-specific incumbents in various states of disrepair (Pokellector, Shiny, PokeScope), one strategic incumbent owned by the grading category leader (Card Ladder under Collectors/PSA), and the platform-owners themselves (TCGplayer App, eBay App).

**Threat density:** High. **Concentration:** Medium-low. **Whitespace:** Yes — at the intersection of Pokemon-only depth + eBay sold-comp pricing + custom alerts + modern UX.

---

## Competitor Profiles (Summary)

> Full profiles in `raw/direct-competitors.md`. Data labeled where verifiable; estimates where not.

### 1. Collectr — `consumer.gg` — **Threat: HIGH**
- **Founded** ~2020. Bootstrapped. Multi-TCG (Pokemon, MTG, Sports, Lorcana, others).
- **Users:** ~4M [Estimate, public claims + a16z scout activity]
- **Pricing:** Free + Collectr PRO at $4.99/mo or $39.99/yr [Data, app store]
- **Ratings:** 4.80/5 Android, 32K reviews [Data, Google Play, 2025]
- **Strengths:** Brand and review velocity; multi-TCG positioning attracts crossover collectors; clean modern UX
- **Weaknesses:** Multi-TCG breadth means Pokemon-specific depth (sets, sealed product, Japanese cards) is shallower than Pokemon-native incumbents; Collectr PRO does not appear to advertise per-card price alerts on its public pricing page [Estimate, must verify in-app]
- **Why it's a HIGH threat:** Network effects in marketplaces, pricing match at $4.99/mo or $39.99/yr (matches founder's plan exactly), and 4M users means most "best collection app" search results name Collectr first.

### 2. CollX — `collx.app` — **Threat: HIGH**
- **Founded** ~2019. Series A $10M (March 2025) [Data, TechCrunch].
- **Multi-TCG focus, US-based.**
- **Pricing:** Free + Pro tier (verify exact price)
- **Strengths:** Capital, marketing budget, marketplace ambitions
- **Weaknesses:** Multi-TCG dilution; some review complaints about scan accuracy
- **Why HIGH threat:** Capital advantage and visible PR push.

### 3. Card Ladder — `cardladder.com` — **Threat: HIGH (strategic, not direct)**
- **Acquired by Collectors (PSA's parent), Dec 2021** [Data, public news]
- **Pricing:** $14.99/mo or ~$99–199/yr; bundled free with PSA Premium ($199/yr) [Data, Card Ladder + PSA pricing pages]
- **Sports-card heritage; Pokemon support added but secondary**
- **Why HIGH threat:** Cross-subsidized via grading revenue. Collectors can run a competing Pokemon tracker at negative margin to feed PSA grading volume.

### 4. Pokellector — `pokellector.com` — **Threat: LOW (vulnerable)**
- **Founded** 2012. Small team / sole operator [Estimate].
- **Pricing:** Free + ~$60/yr Pro [user-cited; not officially published]
- **Strengths:** Best Pokemon catalog completeness — English + Japanese sets, comprehensive checklists
- **Weaknesses:** Aged codebase, "laggy", "ads annoying" common complaints; lost mind-share to Collectr
- **Why LOW threat (and key vulnerability target):** Catalog is the asset; UX is the failure. A modern app that ports Pokellector's catalog completeness into a Collectr-tier UX displaces it.

### 5. Shiny / PokeScope — **Threat: HIGH (doppelganger risk)**
- **Pokemon-native, scan + portfolio + custom price alerts + eBay sold-comps**
- **Smaller teams, ratings mixed; camera bugs in user reviews**
- **Why HIGH threat:** **These are the founder's pitch already shipped.** The differentiation challenge is "why are you better than Shiny?" — and execution-speed alone is a thin answer.

### 6. TCGplayer App (eBay-owned) — **Threat: MEDIUM-HIGH**
- **Free, ubiquitous, official pricing data**
- **Limited collection-management UX** — designed for buying, not tracking
- **Why MEDIUM-HIGH:** "Free" is a permanent gravity well. Most Pokemon collectors have it installed by default. The founder's app must answer "why do I need a separate app?"

### 7. eBay App — **Threat: MEDIUM**
- **Free, has Watchlist (lite portfolio), sold-listings filter is the canonical price-check workflow**
- **Why MEDIUM:** Already used by ~70–85% of serious collectors as the price-check tool [Estimate, Wave 2 B2]. The founder's app must replace this workflow or be a layer on top of it.

### 8. Ludex — **Threat: LOW-MEDIUM (vulnerable)**
- **Multi-TCG scanner, sports-first DNA**
- **Pokemon library has gaps for "well-known cards"; scan accuracy complaints; $50/yr pricing**
- **Why LOW-MEDIUM:** Pokemon-depth focus outguns them.

### 9. ManaBox (MTG, not Pokemon — comp/reference)
- **Solo indie, MTG-only, $22.99/yr**
- **Why included:** Proof point that a focused single-TCG app from a solo developer can build a sustainable business. Validates the "ManaBox of Pokemon" wedge concept.

---

## Comparison Matrix

| App | Price (annual) | Free Tier | Pokemon-native? | Scan | Portfolio | Custom Alerts | Marketplace | App Rating | Funding | **Threat** |
|-----|---------------|-----------|-----------------|------|-----------|--------------|-------------|------------|---------|------------|
| **Collectr** | $39.99 | Yes | No (multi-TCG) | Yes | Yes | Unclear* | Yes | 4.80/5 (32K) | Bootstrapped | **HIGH** |
| **CollX** | ~$36–60 | Yes | No (multi-TCG) | Yes | Yes | Yes | Yes | 4.5/5 [Estimate] | $10M Series A | **HIGH** |
| **Card Ladder** | $99–199 (free w/ PSA) | Demo | No (sports-first) | Limited | Yes (analytics) | Yes | No | n/a | PSA-owned | **HIGH (strategic)** |
| **Shiny / PokeScope** | $0–30 | Yes | **Yes** | Yes | Yes | Yes | No | Mixed | Bootstrap/indie | **HIGH (doppelganger)** |
| **Pokellector** | ~$60 | Yes | **Yes** | Limited | Yes | No | Limited | 3.5/5 [Estimate] | Indie | **LOW (vulnerable)** |
| **Ludex** | $50 | Yes | No (multi-TCG) | Yes | Yes | Yes | No | 3–4/5 [Estimate] | Bootstrap/seed | **LOW-MED (vulnerable)** |
| **TCGplayer App** | $0 | Full | Indirect | No | Limited | No | **Yes (own)** | 4/5 | eBay-owned | **MED-HIGH** |
| **eBay App** | $0 | Full | No | No | Watchlist | Yes (saved searches) | **Yes (own)** | 4.5/5 | eBay public | **MED** |
| **ManaBox (ref)** | $22.99 | Yes | n/a (MTG) | Yes | Yes | Yes | Limited | 4.6/5 | Indie | n/a (validates wedge) |

*Collectr PRO price-alert support requires in-app verification — Wave 2 B1 noted this as a high-leverage gap.

---

## Positioning Map

```
                       FOCUSED  (Single TCG)
                              |
                              |
              [Pokellector]   |   [Shiny]
              (legacy, deep)  |   [PokeScope]
                              |   (founder's lane)
                              |   [ManaBox = MTG]
                              |
LOW QUALITY UX  ──────────────┼────────────── HIGH QUALITY UX
                              |
                              |   [Collectr]
                              |   [CollX]
                              |   [Card Ladder]
              [Ludex]         |   [TCGplayer App]
                              |
                              |
                       BROAD  (Multi-TCG / cross-category)
```

**Whitespace:** Top-right quadrant — **Pokemon-native + modern, polished UX**. Pokellector occupies the "Pokemon-native + dated UX" cell. Shiny/PokeScope are closest competitors and are the real fight. Collectr occupies the "multi-TCG + great UX" cell.

---

## Vulnerability Analysis (Most → Least Displaceable)

1. **Pokellector** — 13-year-old codebase, UX debt, lost mind-share. Has the asset (catalog) but can't defend it. **Easiest displacement target.**
2. **Ludex** — Sports-first DNA, Pokemon library gaps, scan accuracy complaints at $50/yr. Pokemon-depth focus wins.
3. **Shiny / PokeScope** — Already in the lane but execution issues (camera bugs, smaller teams). Hard to displace if execution gap is small; possible if founder ships markedly better.
4. **CollX** — Capital-strong but multi-TCG positioning dilutes Pokemon advocacy. Hard to displace from sharing dollars; possible to compete for "Pokemon-only" mindshare.
5. **Collectr** — Network effects + brand + 4M users. **Cannot be beaten head-on; must be flanked.**
6. **Card Ladder / Collectors** — Strategic incumbent with grading-revenue subsidy. **Cannot be matched on price; must compete on Pokemon-native UX.**
7. **TCGplayer App / eBay App** — Free + platform gravity. **Cannot be displaced; must coexist as a layer on top.**

---

## Indirect Competitors & Status Quo

(Synthesized from `raw/indirect-competitors.md`)

| Substitute | Prevalence (% of 200K paying-eligible US base) | Why it sticks | Where it breaks |
|-----------|-------------------------------------------------|---------------|------------------|
| **Spreadsheets** (Excel/Google Sheets) | ~30–40% | Custom schemas, zero lock-in, free | Past 500–1,000 cards, manual maintenance becomes brittle |
| **eBay sold-listings** as price reference | ~70–85% (often layered with other tools) | Free, canonical, US-USD, trusted | No portfolio aggregation, manual lookup per card |
| **TCGplayer manual lookup** | ~50–60% | Free, official-feeling pricing | "Asks" not "comps"; manual per-card |
| **Nothing / binders + memory** | ~40–55% | Lowest friction; works for casual collectors | Breaks at theft/sale/insurance/move events |
| **PSA Set Registry / pop reports** | ~20–25% (graded-card collectors only) | Authoritative for grading data | Doesn't track raw cards or value |
| **Discord + Reddit community pricing** | ~20% | Social signal, recent comps from real trades | Inconsistent, requires participation |

**Switching costs (what would actually move a serious collector?):**
- **Bulk-import** (CSV from existing spreadsheet) — non-negotiable
- **Mobile scan** (clearly faster than typing 200 names)
- **Credible US pricing source** (eBay sold > TCGplayer asks > Cardmarket EUR)
- **Clean CSV export** (collectors fear lock-in; portability is trust)

If any of these four is missing, **the spreadsheet stays**. This is the floor of any MVP.

---

## Platform Risk Assessment

| Platform | Likely to absorb our functionality? | Timeline | Why | Mitigation |
|---------|--------------------------------------|----------|-----|------------|
| **PSA / Collectors** | **High** | 12–18 months for raw-card | Owns Card Ladder; raw users = grading leads | Own the "non-grading-aligned" persona; community trust as moat |
| **TCGplayer / eBay** | Medium | 12–36 months | Owns the data; could ship a portfolio feature | Compete on UX, alerts, neutrality |
| **Pokemon Company / TPCi** | Low–Medium | 24+ months, possibly never | Brand-protective, focused on physical-card sales + Pocket | IP-clean implementation; avoid card-art-heavy marketing |
| **Generic portfolio trackers (Kubera, etc.)** | Low | n/a | Collectibles is a hobbyist long-tail | Domain depth |
| **Pokemon TCG Pocket** | n/a (different product) | — | Pocket is digital-only; physical is a separate workflow | Treat as adjacent + as a top-of-funnel (see GTM) |

**Single biggest existential platform threat: PSA / Collectors.** They are simultaneously the most-resourced player and the most-motivated to absorb the raw-card tracking layer. Their structural advantage is grading-revenue subsidy. The mitigation is psychological (collectors who don't grade everything are a real persona that PSA's brand can't fully serve) and community-based (PSA has no community asset; Reddit/Discord trust is a different muscle).

---

## Competitor GTM Summary

(Synthesized from `raw/competitor-gtm.md`)

| Competitor | Primary acquisition channel | Sales motion | Notable detail |
|-----------|------------------------------|--------------|----------------|
| Collectr | TikTok creator gifting (top tier saturated), Reddit organic, App Store ASO, Product Hunt | Self-serve | Has paid PR program (e.g., "BEST PR PACKAGE I'VE EVER RECEIVED" creator content) |
| CollX | TechCrunch PR + paid TikTok + ASO post-Series A | Self-serve | Capital-backed marketing |
| Pokellector | Aged SEO authority on `pokellector.com` | Self-serve | Organic-only, declining |
| TCGplayer App | Cross-promotion from eBay/TCGplayer marketplace | Self-serve | Distribution by default |

---

## Channel Opportunity Map (for the entrant)

| Channel | Saturation | Founder Opportunity | Estimated CAC | Notes |
|---------|-----------|--------------------|----------------|-------|
| **r/PTCGP + Pokemon TCG Pocket trade-tracker wedge** | Low | **High** | ~$0 | 100M+ Pocket users; Collectr/CollX treat Pocket as checkbox; existing Pocket trackers are web-based |
| **r/pkmntcgcollections + r/pkmntcgtrades** | Medium | **High** | ~$0 | Showcase culture; app screenshots are native content; comply with 90/10 rule |
| **Micro-creator gifting (5K–50K followers)** | Low | **High** | $0 (Pro codes) | Long tail beyond Collectr's saturated top tier |
| App Store ASO (Pokemon scanner keywords) | High | Low | $0 but slow | 10+ apps already on page 1; minor gains only |
| Google SEO ("pokemon card value") | Very high | Low | $0 but very slow | PriceCharting/TCGplayer/eBay dominate |
| Paid Meta/Google/ASA | n/a | **Avoid** | $15–40/sub | Above $30 LTV-derived ceiling |
| LCS (local card shop) partnerships | Low | Low | High effort | No competitor has succeeded; shop owners have no incentive |
| r/PokemonTCG (1.3M subs) | High | Low | $0 | Strict moderation, anti-self-promo |

**Top 3 organic channels for $0-budget entrant (per Wave 2 B3 recommendation):**
1. **Pokemon TCG Pocket trade-tracker as the entry wedge → r/PTCGP + TikTok demos.** Pocket's 100M+ users + the absence of a great mobile-native Pocket trade tool = real opening.
2. **Long-tail Reddit utility-posting on r/pkmntcgcollections + r/pkmntcgtrades.** Daily 10-min participation, screenshot showcases, follow 90/10 rule.
3. **Micro-creator gifting** (under 50K followers, free Pro codes + beta access).

---

## Strategic Recommendations

### Where to Compete
- **Pokemon-only depth** with English + Japanese + sealed + non-PSA condition coverage (Pokellector's catalog asset, modernized)
- **eBay sold-comp pricing as primary signal** (most competitors use TCGplayer asks; sold-comps are more credible to power users — subject to ToS verification)
- **Custom price alerts as a headline feature** (suspected Collectr gap — must verify in-app)
- **A Pokemon TCG Pocket sub-app or trade-calculator wedge** (genuine 100M-user top-of-funnel opening)

### Where NOT to Compete
- **Multi-TCG breadth** — loses to Collectr/CollX by definition
- **Free-tier feature parity with TCGplayer App** — they have the marketplace data; chasing this is unwinnable
- **Grading workflow integration** — Card Ladder/PSA dominate; entry would be subsidized away
- **Marketplace transactions in v1** — chicken-and-egg + KYC + fraud = ops bet, not software bet (defer to v2 only after PMF)

### Differentiation Angle (one paragraph)
*"The Pokemon-only collection app for serious hobbyists who care about real eBay sold-comp pricing, Japanese sets, and instant alerts when a card you own actually moves. Built by a Pokemon collector, not a sports-card platform — and not bundled with a grading service we want to upsell you to."*

The implicit promise:
- **Depth over breadth** (Pokemon only)
- **Real pricing** (eBay sold > TCGplayer asks)
- **Independence** (not PSA's lead-generation funnel)
- **Modern UX** (vs. Pokellector)

---

## Vulnerability Map — Recommended Strategic Sequence

1. **Phase 1 — Displace Pokellector users.** They have the most acute pain (laggy app + ads) and the lowest switching cost. Win the "Pokellector refugee" persona first.
2. **Phase 2 — Coexist with eBay/TCGplayer apps as the layer above them.** Don't compete for "where do I buy"; own "what do I own and what's it worth."
3. **Phase 3 — Compete for Pokemon-mindshare against Shiny/PokeScope on execution and depth.** This is a knife fight; must win on speed of new-set support, scan accuracy, and community presence.
4. **Phase 4 — Flank Collectr from the Pokemon-only side.** Never engage on multi-TCG terrain.
5. **Never engage Card Ladder/PSA on price.** Grade-agnostic positioning + Pokemon-native UX.

---

## Data Gaps

- Sensor Tower / App Annie data on competitor downloads, paid conversion, and revenue
- In-app feature audit for Collectr PRO, CollX Pro, Shiny, PokeScope (especially: do they have custom price alerts?)
- Subreddit moderator policy specifics for self-promotion (need direct sidebar reads)
- Disclosed sponsorship history for top-tier Pokemon YouTubers (PokeRev, Smpratte) to confirm rate cards
- Pocket-tracker takedown-notice history (legal risk on the wedge channel)

---

## Strategic Connections

- **→ `market-analysis.md`** — The data-access cliff (TCGplayer + eBay APIs closed) means even the official platforms can't easily build a great free aggregator app — which is paradoxically protective for an indie that pays for data.
- **→ Phase 4 Lean Canvas** — The "Channels" cell flows directly from this document's Channel Opportunity Map. The "Unfair Advantage" cell maps to community participation + Pokemon-native focus + execution speed.
- **→ Phase 8 Validation** — The hypothesis "Collectr PRO has no custom price alerts" is the highest-leverage feature-gap test; if true, the wedge is real; if false, the wedge collapses.

---

## Flags

**Red Flags:**
- Two of the three closest competitors (Shiny, PokeScope) ship the founder's exact pitch. Without a sharp wedge, the founder's app is a "fourth Pokemon scanner."
- Card Ladder/PSA can subsidize a competing tracker indefinitely.

**Yellow Flags:**
- Collectr's 4M-user lead is decisive in any head-on multi-TCG framing.
- Custom-price-alerts gap in Collectr PRO is unverified; if present, the wedge is weakened.
- Pokemon TCG Pocket cross-promotion has unclear legal/IP risk; takedown precedent exists for fan trackers.

## Sources

- `01-discovery/raw/direct-competitors.md` (8 competitor profiles, 18+ source links)
- `01-discovery/raw/indirect-competitors.md` (Reddit threads, eBay developer docs, TCGplayer API status)
- `01-discovery/raw/competitor-gtm.md` (TikTok creator content, Reddit threads, Product Hunt, app store data)
- TechCrunch (CollX Series A, March 2025)
- Public news on Card Ladder acquisition by Collectors (Dec 2021)
- Collectr Google Play listing, 2025
