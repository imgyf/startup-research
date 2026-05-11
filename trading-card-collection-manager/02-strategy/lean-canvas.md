# Lean Canvas — Pokemon Collection Manager (Working Title)

**Phase:** 4 — Strategy (Fast Track: Lean Canvas only)
**Project:** trading-card-collection-manager
**Date:** 2026-05-10
**Confidence:** Medium (grounded in research findings; pricing and customer-segment cells will firm up after Phase 8 validation experiments)

---

## Working Name

**"Pokébinder"** (placeholder — verify trademark, IP, and App Store availability before committing). Other candidates: "Pokévault", "CardIndex", "Trove TCG". The naming choice is deferred to a later branding phase, which is out of Fast Track scope.

---

## 1. Problem (top 3, with existing alternatives)

| # | Problem | Existing Alternatives |
|---|---------|----------------------|
| 1 | "I don't actually know what my Pokemon collection is worth right now, in real eBay sold-comp dollars." | Spreadsheet + manual eBay sold-listings filter (~70–85% prevalence among serious collectors) |
| 2 | "Manually entering 200+ cards is a nightmare and breaks my spreadsheet at scale." | Pokellector free tier (clunky); Collectr (multi-TCG, Pokemon-shallow); not bothering at all (~40–55%) |
| 3 | "I want alerts when a card I own actually moves on eBay — not when a TCGplayer 'ask' shifts." | eBay saved searches per card (impractical at scale); none of the major collection apps offer per-card eBay-sold alerts at price point |

**Anchor pain:** Pokemon-specific depth is missing from the polished apps; polish is missing from the Pokemon-specific apps.

(Cross-references `01-discovery/target-audience.md` Pain Hierarchy.)

---

## 2. Customer Segments

**Primary (early adopters):** **"Pokellector refugee"** — serious Pokemon collectors with 200–2,000 cards who currently use Pokellector or a spreadsheet, are frustrated with UX/lag, and have not yet committed to Collectr or have churned from Collectr free tier.

**Secondary (Y1 expansion):** **"Investor-curious hobbyist"** — Pokemon collectors with 500+ cards including some sealed product or PSA-graded, who care about appreciation tracking and would accept a $99/yr tier for serious analytics.

**Anti-segment (do not chase):**
- Casual TCG Pocket-only digital players (no physical collection)
- Competitive Standard-format players (need deck-building tools, not collection value)
- High-volume LCS dealers (need B2B inventory, different product entirely)
- Sub-50-card casuals (under free-tier threshold; will never pay)

(Cross-references `01-discovery/target-audience.md` Primary Persona.)

---

## 3. Unique Value Proposition

**Single-sentence formula** ("We help [customer] [solve problem] by [mechanism]"):

> *"We help serious Pokemon collectors know what their collection is actually worth — in real eBay sold-comp dollars — by scanning each card once and tracking real US market prices with custom alerts, in a Pokemon-native app built by an obsessive developer instead of a sports-card platform or grading service."*

**Tagline candidates** (to A/B test in Reddit/TikTok):
1. *"The Pokemon collection app that uses real eBay prices, not TCGplayer asks."*
2. *"Built for Pokemon. Not bundled with grading."*
3. *"Your binder, but it knows what it's worth."*

**The implicit promise stack:**
- Depth (Pokemon-only catalog, including Japanese sets and sealed)
- Realism (eBay sold-comps over TCGplayer asks)
- Independence (not feeding a grading-service upsell)
- Polish (Collectr-tier mobile UX)

---

## 4. Solution (top 3 features for top 3 problems)

| Problem | Solution |
|---------|----------|
| 1: "What's my collection worth?" | **Real-time portfolio valuation** using eBay sold-comp aggregation (last 30/60/90-day median of completed auctions for the same card + condition). Display methodology transparently — "this number comes from N actual sales in the last M days" — to build trust. |
| 2: "Manual entry is brutal." | **Camera scan + bulk CSV import.** Scanner identifies card; user confirms condition (rough self-tag, not AI-graded); card lands in collection. CSV import for users migrating from spreadsheets. CSV export always free, never gated. |
| 3: "Alert me when a card I own actually moves." | **Custom per-card price alerts** triggered by completed eBay sales (not list-price changes), with user-set thresholds (e.g., "alert me if a sale completes >10% above my last data point"). |

**Explicitly out of scope for v1:**
- Grading workflow integration (cedes that lane to PSA)
- AI-graded condition (commits to a quality bar the technology can't meet)
- Marketplace transactions (defer to v2 minimum)
- Multi-TCG breadth (cedes that lane to Collectr/CollX)
- Social feed / public collection sharing (privacy by default)
- Pokemon TCG Pocket digital-card tracking (handled as a separate small utility for top-of-funnel only)

(Cross-references `01-discovery/competitor-landscape.md` "Where to Compete / Where NOT to Compete".)

---

## 5. Channels

**Inbound (organic):**
1. **Reddit utility-posting** on r/pkmntcgcollections + r/pkmntcgtrades (90/10 rule, native showcase content) — primary
2. **Pokemon TCG Pocket trade-fairness sub-tool** posted on r/PTCGP + TikTok demo videos — top-of-funnel wedge
3. **Micro-creator gifting** (5K–50K-follower Pokemon TikTok/YouTube creators), Pro codes + beta access in exchange for honest review
4. **App Store Optimization** (Pokemon-specific keywords, screenshots, Pokemon-only positioning in store description)
5. **Long-tail SEO** ("how to track pokemon card collection", "pokemon collection app reddit") — slow but compounds

**Outbound (sales):** N/A. Consumer subscription product; no outbound.

**Avoided:**
- Paid Meta/Google/Apple Search Ads ($15–40/sub vs. <$30 LTV-derived ceiling)
- Generic "pokemon scanner" ASO category (10+ apps already on page 1)
- LCS partnerships (no successful comp; shop owners have no incentive)

(Cross-references `01-discovery/competitor-landscape.md` Channel Opportunity Map.)

---

## 6. Revenue Streams

**v1 (launch):**
| Tier | Price | Includes |
|------|-------|----------|
| Free | $0 | 50-card collection, manual entry, basic catalog browse, CSV import + export always free |
| Pro Monthly | **$5.99/mo** | Unlimited cards, scan, real-time eBay sold-comp valuation, 10 custom price alerts, basic analytics |
| Pro Annual | **$59.99/yr** (~17% saving) | Everything in monthly + unlimited price alerts |

**Note on pricing change from founder's pitch ($4.99/mo, $39.99/yr):** Research revealed structural cost from paid pricing-data APIs ($50–500/mo). To preserve gross margin at projected scale, the price floor must rise to $5.99/$59.99 minimum. **This must be validated against willingness-to-pay** — if Pokemon collectors push back hard, revisit by reducing the data-API spend (e.g., refresh prices once daily instead of real-time, or only refresh "watched" cards).

**v2 (after PMF, optional):**
- Pro Plus tier (~$9.99/mo or $99/yr): Investor-curious features (sealed-product tracking, set-completion ROI, time-series analytics, tax/insurance export)
- Marketplace fee (5–8%): Only after trust + community is established. Carries KYC/AML/payment-processing/dispute obligations and structural ops cost.

**LTV math (base case, mobile freemium benchmarks):**
- Annual sub: $59.99 × 1-year retention 36% (median, RevenueCat) → effective $59.99 × 1.4 multi-year LTV ≈ **$84/customer**
- Monthly sub: $5.99 × ~14 months @ 7% monthly churn ≈ **$72/customer**
- Blended LTV: **~$80/customer**

**Maximum sustainable CAC: $25–30** (per LTV/CAC ≥ 3:1 standard). **Confirms organic-only strategy.**

(Cross-references `01-discovery/market-analysis.md` Unit Economics Benchmarks.)

---

## 7. Cost Structure

**Recurring (monthly):**
| Item | Cost (Y1 estimate) | Notes |
|------|-------------------|-------|
| Pricing-data API (JustTCG / Scrydex / equiv.) | $50–200/mo | **Critical Y1 line item** — must be confirmed before MVP build |
| App store fees (Apple 15%, Google 15% small-business tier) | 15% of GMV | Net of small-business reduction |
| Backend hosting (Supabase / Firebase free tier extending into paid) | $0–50/mo | Scales with users |
| Push notification service (free tier) | $0 | Available |
| Analytics (PostHog / Mixpanel free tier) | $0 | Available |
| Domain + email | $5/mo | |
| **Total recurring (Y1)** | **$55–255/mo** | |

**One-time (Y0):**
| Item | Cost |
|------|------|
| Apple Developer Program | $99/yr |
| Google Play Developer | $25 one-time |
| Trademark search + filing (US, optional Y1) | $0–500 |
| Initial pricing-data ingestion + catalog seed | included in dev time |
| **Total one-time** | **$125–625** |

**Unit cost per active free user:** ~$0.05–0.20/mo (pricing API + hosting amortized)
**Unit cost per active paid user:** ~$0.20–0.50/mo (more API calls for alerts/refresh)
**Gross margin at scale:** ~75–85% (after 15% app-store fee + variable data costs) — healthy for consumer subscription

**Sweat equity (founder time, side project):**
- Y0 (months 1–4): ~10 hrs/week dev + 5 hrs/week customer dev — MVP build
- Y1 (months 5–12): ~10 hrs/week dev/maintenance + 5 hrs/week community/marketing
- This is a **material cost** even if not cash. At $100/hr opportunity cost, that's $30K–50K of unmonetized founder time in Y1. Founder must accept this is real.

---

## 8. Key Metrics (AARRR)

| Pirate metric | Y1 target | Y2 target |
|---------------|-----------|-----------|
| **Acquisition** — Monthly downloads | 500–2,500/mo by month 12 | 3,000–10,000/mo |
| **Activation** — % who scan first card within 24h | 40%+ | 50%+ |
| **Retention** — D30 free-user retention | 15–25% | 25%+ |
| **Revenue** — Free→paid conversion | 1.5–2.5% | 2.5–4.0% |
| **Revenue** — Annual ARR | $10–50K | $50–150K |
| **Referral** — % of paid users who refer 1+ friend | 10% (organic only) | 20%+ |

**North Star metric:** **Monthly active paid subscribers.** Not downloads (vanity), not free signups (vanity), not GMV (irrelevant pre-marketplace). Just "how many people pay this month."

**Operational guardrails:**
- Monthly subscription churn: keep below 8% (industry median 5–10%)
- Net Promoter Score (post-onboarding): >40 (signals organic referral potential)
- App Store rating: >4.5 stars (gating for organic ASO)
- Cost per paid sub: <$30 (confirmed organic-only)

---

## 9. Unfair Advantage

**Honest assessment first:** As of today, the founder has NO unfair advantage. Light-collector + bootstrapped + side-project pace + no domain authority + no community presence. This is the most uncomfortable cell in the canvas, and lying about it would defeat the purpose of the exercise.

**What can become an unfair advantage over 6–12 months (with deliberate effort):**

1. **Compounding community participation.** Daily 10-min participation in r/pkmntcgcollections + r/pkmntcgtrades, building reputation as "the indie dev who actually listens." This is unfakeable by Collectr (corporate brand), CollX (capital-funded), or PSA (institutional). Time-stacked credibility is a real asset.
2. **Pokemon-only depth as content.** A weekly "what just got added to the catalog" or "Japanese set spotlight" content stream. Multi-TCG competitors structurally cannot match Pokemon-specific content frequency.
3. **Execution speed on new sets.** When TPCi releases a new set, race to be the first app with full catalog support (English + Japanese). Multi-TCG competitors will be 1–2 weeks behind. This is a credibility flywheel.
4. **Privacy stance** with substance: local-first option, optional cloud, no public collection feed. PSA cannot match this (their business is identifying graded cards by serial); Collectr could but currently doesn't.
5. **No grading conflict-of-interest.** "Built independently of any grading service" is a real positioning advantage that PSA/Collectors cannot copy.

**The unfair advantage is buildable, not innate.** This is more honest than claiming "passion" or "execution" as a moat — it's not, until proven.

(Cross-references `01-discovery/market-analysis.md` Strategic Implications #5.)

---

## Lean Canvas at a Glance

```
+-------------------+----------------------+--------------------+----------------------+----------------------+
| PROBLEM           | SOLUTION             | UVP                | UNFAIR ADVANTAGE     | CUSTOMER SEGMENTS    |
| 1. Don't know     | 1. Real-time eBay-   | "The Pokemon       | Buildable, not       | Pokellector refugee  |
|    real value     |    sold-comp valuation|   collection app  | innate. Community    | (200-2000 cards,     |
| 2. Manual entry   | 2. Camera scan +     |  that uses real    | participation +      | $1K-$50K, frustrated |
|    nightmare      |    bulk CSV          |  eBay prices, not  | Pokemon-only depth + | with current tools)  |
| 3. No real        | 3. Per-card eBay-    |  TCGplayer asks.   | execution speed +    |                      |
|    price alerts   |    sold alerts       |  Built for Pokemon"| no grading conflict  | Anti: casuals,       |
|                   |                      |                    |                      | dealers, Pocket-only |
+-------------------+----------------------+                    +----------------------+----------------------+
                                            |                                            |
+-------------------+----------------------+|                   +----------------------+| 
| KEY METRICS       | CHANNELS             |                    |                      | 
| North Star: MAU   | r/pkmntcgcollections,|                    |                      | 
|   paid subs       | r/PTCGP, micro-      |                    |                      | 
| Y1: $10-50K ARR   | creator gifting,     |                    |                      | 
| Conv: 2-3%, churn | App Store ASO,       |                    |                      | 
|   <8%/mo, NPS >40 | long-tail SEO        |                    |                      | 
+-------------------+----------------------+--------------------+----------------------+----------------------+
| COST STRUCTURE                                | REVENUE STREAMS                                              |
| Pricing API: $50-200/mo (CRITICAL)            | Free: $0 (50 cards) | Pro: $5.99/mo or $59.99/yr             |
| Hosting: $0-50/mo                             | Future: $9.99/mo Plus tier; 5-8% marketplace fee (v2 only)   |
| Founder time: ~15 hrs/wk = $30-50K opp. cost  | LTV: ~$80 / max CAC: $25-30 / Margin: 75-85% at scale       |
+-----------------------------------------------+-------------------------------------------------------------+
```

---

## Strategic Connections

- **→ `01-discovery/market-analysis.md`** — TAM/SAM/SOM band, unit economics, data-access cliff all carry into this canvas without contradiction.
- **→ `01-discovery/competitor-landscape.md`** — Channels, problem-framing, and "where not to compete" stance directly inherited.
- **→ `01-discovery/target-audience.md`** — Customer Segments cell uses Primary + Secondary persona; "anti-segment" honors anti-persona.
- **→ Phase 7 Revenue Model** — $5.99/$59.99 pricing must hold through projections; LTV $80 anchor must drive CAC ceiling.
- **→ Phase 8 Validation** — Every Lean Canvas cell that contains an [Estimate] or [Assumption] becomes an experiment.

---

## Flags

**Red Flags:**
- "Unfair Advantage" cell is honestly empty today; must be deliberately built. If the founder is unwilling to do daily community participation for 6+ months, this canvas does not produce a viable business.

**Yellow Flags:**
- Pricing has been raised from founder's $4.99/$39.99 pitch to $5.99/$59.99 to absorb pricing-data API costs. Founder may push back; if so, revisit data-refresh cadence or feature scope.
- Pokemon TCG Pocket cross-promotion in Channels is structurally valuable but legally untested (third-party Pocket trackers have received takedowns).
- "Free tier 50 cards" matches Collectr's free tier exactly. Differentiation must come from paid features, not a more generous free tier.

## Sources

- All `01-discovery/` synthesized files
- Industry-benchmarks reference (mobile freemium benchmarks)
- April Dunford Positioning framework (used implicitly in UVP construction)
- Lean Canvas (Ash Maurya) framework
