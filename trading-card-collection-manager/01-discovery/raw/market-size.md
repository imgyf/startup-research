# Market Sizing: Pokemon TCG Collector App Tools

> Research date: 2026-05-10. Founder context: side project, freemium mobile app, US-first, target = "200–2,000 card serious hobbyist with $1K–$50K collection."
>
> Labels used throughout: **[Data]** = directly cited figure from a source; **[Estimate]** = derived calculation from cited inputs; **[Assumption]** = reasonable judgment not directly sourced.

---

## TAM (global Pokemon TCG ecosystem in $)

### Global TCG market (umbrella)
- **[Data]** Global Trading Card Games market estimated at **$8.4B in 2025**, growing to ~$9.2B in 2026 → $16.9B by 2035 at ~6.9% CAGR. Source: GMInsights / Athlon Sports recap (Feb 2026). *Tier 2.*
- **[Data]** Competing estimate: **$13.28B in 2025 → $15.11B in 2026**, reaching $24.36B by 2031 at 10.03% CAGR. Source: Mordor Intelligence (2026). *Tier 2.*
- **Cross-reference note**: The two reputable analyst figures differ by ~60%. GMInsights likely counts cards-only/retail; Mordor likely includes accessories, sealed product wholesale, and possibly some secondary-market activity. Honest read: **TCG global retail = $8–15B, depending on definition.** No single Tier 1 (Gartner/SEC) figure was located.

### Pokemon's slice
- **[Data]** Pokémon TCG holds ~**12% share of the global TCG market in 2026** (GMInsights / Accio summaries, *Tier 2/3*). → Pokemon TCG global TAM = **~$1.0–1.8B in retail card sales** [Estimate, derived from the 12% of $8.4–15B range].
- **[Data]** The Pokémon Company produced **10.2 billion cards in fiscal year 2024–25** (April 2024 – March 2025), down 14.3% from 11.9B the prior year. Lifetime cumulative production: 75B+ cards. Source: PokéGuardian via TPCi annual data, May 2025. *Tier 2.*
- **[Data]** Pokémon was the **#1 US toy property in 2025 at $2.5B annual sales** (cards + merchandise combined). Source: Statista / Circana via Fortune (Jul 2025). *Tier 2.*
- **[Data]** Walmart trading-card sales **+200% YoY 2024→2025**; Pokémon-specific sales on Walmart Marketplace **10x growth YoY**. Source: VMFS USA market write-up (2025). *Tier 3* (single-source for the 10x figure — treat as directional).

### Secondary market (resale)
- **[Data]** eBay searches for "Pokémon" hit **~14,000 per hour in 2024**. Source: VMFS / eBay disclosure cited via Statista (2025). *Tier 2.*
- **[Estimate]** No clean published figure for Pokemon-specific secondary GMV exists. Founder verification needed; proxy = TCGplayer + eBay sold-listings volume. **[Assumption]**: Secondary market is at minimum 0.5–1.0x the size of primary card sales for an active franchise → roughly **$0.5–1.5B secondary Pokemon GMV** globally. This is a soft estimate — a Tier-1 source is not available.

### TAM verdict
- **Pokemon TCG global ecosystem (cards + secondary + grading + accessories)**: order-of-magnitude **$2–4B/year in 2026** [Estimate, anchored to: $1–1.8B primary cards + $0.5–1.5B secondary + grading/accessories].
- **The relevant TAM for a collector-tools app is NOT the card market itself** — it's the dollars collectors are willing to redirect into tools, software, sleeves, grading, and services. Realistically only a small fraction of card spend goes to tools.

---

## SAM (US Pokemon collectors with paid-tool willingness)

### Sizing the active US Pokemon collector base
- **[Data]** US trading card games market = **~$2.2B in 2025** (all TCGs, retail). Source: VMFS / Statista (2025). *Tier 2.*
- **[Estimate]** Pokemon ≈ 50–60% of US TCG share (higher US share than global because of cultural saturation and the Charizard halo) → US Pokemon retail ≈ **$1.1–1.3B** [Assumption, no direct US-Pokemon-only figure found].
- **[Data]** Average TCG collector annual spend = **$450/year**; average age 32; average household income $75K. Source: WiFi Talents trading-card stats compilation, 2026, reportedly from Helion Research. *Tier 3* — single secondary aggregator citing a primary survey we cannot directly verify. Treat as directional only.
- **[Estimate]** US Pokemon retail ($1.1–1.3B) ÷ $450/year per active collector ≈ **2.4–2.9M active US Pokemon collectors** [Estimate]. Cross-check: Collectr (multi-TCG, global) reports 4M+ users; Shiny reports 1M+ users; this is consistent with "low single-digit millions" of US Pokemon-specific collectors. **Treat 2–3M as the working number with low confidence.**

### Narrowing to the founder's ICP ("200–2,000 cards, $1K–$50K collection")
- **[Assumption]** This is the "serious hobbyist" tier — neither casual openers nor whales. Based on classic hobby distributions (long-tail / 80-20), this segment is roughly **15–25% of active collectors**.
- **[Estimate]** US ICP = 2.5M × 20% = **~500K serious US Pokemon hobbyists** [Estimate, ±50%].
- **[Data]** Helion-cited 35% of trading card buyers are 35+ with disposable income — supports a meaningful "high-intent adult" subset. *Tier 3.*

### Willingness to pay for tools
- **[Assumption]** Of serious hobbyists, ~30–50% would consider paying $4–10/mo for a portfolio + scanning tool, based on the existence of paid tiers at Card Ladder (~$10–30/mo) and Collectr Pro (similar tier) sustaining real revenue.
- **[Estimate]** Paid-willingness pool in US = 500K × 40% = **~200K paying-eligible serious collectors** [Estimate].
- **[Estimate]** SAM in revenue terms: 200K × $60 ARPU/year (mid of $4–8/mo blend with annual discount) = **~$12M ARR addressable in the US** [Estimate]. Generous extension to "all US Pokemon collectors who'd buy a tool" (not just the strict ICP) widens this to **$25–40M ARR**.

### SAM verdict
- **Tight (ICP-only) US SAM ≈ $10–15M ARR.**
- **Loose (all serious US Pokemon collectors) SAM ≈ $25–40M ARR.**
- This is small. It is not VC-scale — it IS side-project-scale, and matches the thesis. Honest read: this is a profitable lifestyle business at the high end, not a unicorn.

---

## SOM (realistic Year 1 capture for a side-project app)

### Comp anchors
- **[Data]** Collectr: 4M+ global users, 8-figure ARR (so $10M+ ARR), zero ad spend, multi-TCG, bootstrapped. Took several years to reach this. Source: BetaKit profile (2024). *Tier 2.*
- **[Data]** Shiny (TCG Card Scanner): 1M+ users, scanner + TCGplayer/eBay pricing. Source: Google Play listing copy. *Tier 3* (self-reported install count).
- **[Data]** PokeScope: 50K+ users. Source: site copy. *Tier 3.*
- **[Data]** Card Dealer Pro / Ludex: smaller, specialty-focused. *Tier 3.*

### Year-1 funnel for a solo side-project entrant
- **[Assumption]** A side-project Pokemon-only scanner with no paid acquisition realistically reaches **5K–25K downloads in Year 1** (Reddit r/PokemonTCG, r/pkmntcgcollections, TikTok organic, hobbyist Discord — all viable channels; Collectr hit 5K users in 24 hours from forum posts but had a multi-product team).
- **[Data]** Median freemium download-to-paid conversion = **2.18%** (RevenueCat State of Subscription Apps 2025, *Tier 2*). Top-quartile freemium = 5%. Hobby/utility apps trend toward the higher end because intent is high.
- **[Estimate]** Y1 paid users = 15K downloads × 3% = **~450 paying users**.
- **[Estimate]** Y1 ARR = 450 × $60 = **~$27K** [Estimate]. Optimistic case (50K downloads, 5% conversion): 2.5K × $60 = **~$150K ARR**. Pessimistic (5K downloads, 2%): **~$6K ARR**.

### SOM verdict
- **Realistic Y1 SOM: $10K–$50K ARR.** Stretch case to $100K+ ARR if a single viral moment hits (TikTok creator picks it up; pack-opening influencer endorses).
- This is appropriate for a side project. **Crossing $250K ARR in Y1 would require something unusual** — paid acquisition, a hit influencer, or B2B side (LGS / dealer plans).

---

## Unit Economics Benchmarks (mobile freemium ARPU, conversion, churn)

| Metric | Benchmark | Source / Tier |
|---|---|---|
| Median freemium download→paid conversion | **2.18%** | RevenueCat State of Subscription Apps 2025 *(Tier 2)* |
| Top-quartile freemium conversion | 5–8% | RevenueCat / First Page Sage 2026 *(Tier 2)* |
| Hard-paywall conversion (no free tier) | 12.11% median | RevenueCat 2025 *(Tier 2)* |
| Trial → paid (opt-out, card required) | 49–60% | RevenueCat 2025 *(Tier 2)* |
| Trial → paid (opt-in, no card) | 18–25% | RevenueCat 2025 *(Tier 2)* |
| Median ARPU, mobile subscription apps (global) | **$5.65/mo** | RevenueCat 2025 *(Tier 2)* |
| Mean ARPU mobile subscription apps | $8.41/mo | WinSavvy aggregator *(Tier 3)* |
| Typical sub-app ARPU range | $3–$9/mo | BusinessDojo (Oct 2025) *(Tier 3)* |
| Avg monthly churn, consumer subscription apps | **5–10%** | RevenueCat / SubJolt 2026 *(Tier 2/3)* |
| First-month cancel rate | ~30% of annual subs | Marketing LTB stats roundup *(Tier 3)* |
| Annual plan retention (1 year) | ~36% | RevenueCat 2025 *(Tier 2)* |
| Weekly plan churn vs monthly | 3x faster | RevenueCat 2025 *(Tier 2)* |

### Implications for a Pokemon collector app
- **[Estimate]** Target ARPU should be **$6–8/mo** ($60–80/yr with annual discount) — defensible vs. Card Ladder Pro / Collectr Pro pricing and within mobile subscription median.
- **[Estimate]** Realistic blended monthly churn = **6–8%** at scale (collectors are sticky when actively buying, but lapse fast in cooling markets — see headwinds below).
- **[Estimate]** Implied LTV at $7 ARPU and 7% monthly churn = **~$100/customer**. CAC must stay under ~$30 to be healthy → effectively organic/community only for a side project.
- **[Assumption]** Hobby utility apps tend to outperform median freemium conversion (3–5%) because users with $1K+ collections have explicit ROI for a tool.

---

## Market Headwinds & Risks

### Macro: Pokemon TCG cooling cycle (REAL but not fatal)
- **[Data]** Pokemon card production fell **14.3% YoY** in fiscal 2024–25 (10.2B vs 11.9B). *Tier 2.*
- **[Data]** Modern card prices fell **5–15% across the board** in late 2025; some chase cards (Mega Gardevoir ex Hyper Rare, Mega Lucario ex) dropped **30%+** in months. Sources: PokéWallet, PokeInsider, TCGplayer blog (Nov 2025–Feb 2026). *Tier 2/3.*
- **[Data]** Industry consensus: this is a **correction, not a crash**. Vintage PSA 9/10 has held or appreciated. Collectors stay, speculators leave. Sources: Card Chill, Indigo Plateau TCG, PokéWallet (multiple). *Tier 3 each, but converging.*
- **Implication for the app**: a price-tracking tool is **more, not less, valuable in a cooling market** because losses hurt and users want visibility. But ARPU and willingness-to-pay decline if the asset class is shrinking. Net: neutral-to-mildly-negative for the next 12–24 months.

### Competitive moats already built
- **[Data]** Collectr has ~4M users, 8-figure ARR, multi-TCG, no ads spend. Source: BetaKit. *Tier 2.* This is the dominant incumbent.
- **[Data]** Shiny: 1M+ users on the same value prop (scan + TCGplayer/eBay pricing). *Tier 3.*
- **[Data]** TCGplayer's own mobile app does scanning natively. *Tier 2.*
- **[Data]** eBay launched a card-scanning tool in its mobile app (currently buggy per community reports). *Tier 3.*
- **Implication**: the "scan a card, see prices" feature is **commoditized**. Differentiation must come from: condition assessment quality, portfolio analytics, social/trading features, sealed-product tracking, or a niche the incumbents underserve (e.g., LGS dealer mode, Japanese-card focus).

### App store & platform risk
- **[Assumption]** Apple/Google take 15–30%. TCGplayer/eBay APIs/affiliates may change terms. eBay has historically restricted price scraping. Pokemon Company is litigious about IP — using card art at scale may invite cease-and-desists.

### Why prior TCG apps die (pattern, not specific evidence)
- **[Assumption, no clean Tier-1/2 source found]** Common failure modes: (1) unsustainable scraping infra costs vs. small revenue, (2) ML accuracy collapses on new sets, requiring ongoing labeling spend, (3) founder burnout when revenue stays sub-$10K MRR for 18+ months, (4) market correction shrinks willingness to pay.

---

## Source Quality Assessment

| Source | Used For | Tier |
|---|---|---|
| RevenueCat State of Subscription Apps 2025 | ARPU, churn, conversion | **Tier 2** (industry-standard, large dataset) |
| Statista (Pokemon topic page, US TCG market, Pokemon TCG Pocket) | TAM, US sizing | **Tier 2** |
| BetaKit (Collectr profile) | Comp data | **Tier 2** (established trade press) |
| Mordor Intelligence | TCG market size | **Tier 2** (analyst firm; methodology opaque) |
| GMInsights / Athlon Sports | TCG market size | **Tier 2** |
| PokéGuardian (TPCi production) | Card volume | **Tier 2** (cites primary TPCi disclosure) |
| Fortune (Gen Z collector behavior) | Demographics | **Tier 2** |
| First Page Sage | SaaS conversion | **Tier 2/3** |
| Helion Research (cited via WiFi Talents) | Collector spend ($450/yr) | **Tier 3** (secondary aggregator citing a primary survey we did not directly access) |
| VMFS USA / Accio | US TCG market, Pokemon trends | **Tier 3** (single-source business blogs) |
| Card Chill, PokéWallet, PokeInsider, Indigo Plateau TCG | Market correction narrative | **Tier 3** (hobbyist blogs, but consistent across 5+ sources → directionally reliable) |
| Google Play / App Store install counts | Comp user numbers | **Tier 3** (self-reported, Google Play install bands are wide) |
| No Tier 1 source (SEC filing, IBISWorld, Gartner) located for any figure. | — | — |

---

## Data Gaps (what couldn't be found, with proxies + suggested founder verification)

1. **Exact count of US Pokemon-specific collectors.** No published figure. Proxy used: US TCG retail $2.2B × Pokemon's ~50% US share ÷ $450/yr avg spend ≈ 2.4–2.9M. **Founder action**: run a Reddit poll on r/PokemonTCG and r/pkmntcgcollections; query Census/Pew leisure spending tables; commission a 200-respondent Prolific survey (~$400) for ground truth.

2. **Pokemon secondary-market GMV (TCGplayer + eBay sold) globally and US-only.** TCGplayer is owned by eBay (acquired 2022) but I couldn't find a disclosed Pokemon-specific GMV figure. Proxy: search-volume data, sold-listings sampling. **Founder action**: scrape 30 days of TCGplayer + eBay sold listings for a representative 100-card basket, extrapolate. eBay sometimes discloses category GMV in earnings calls — worth searching transcripts.

3. **Card Ladder revenue and user count.** Not publicly disclosed. Public signals only (pricing page, feature set). **Founder action**: SimilarWeb traffic estimate; LinkedIn employee count as proxy for stage.

4. **Hobby-vertical-specific subscription churn.** Benchmarks here used pan-utility-app numbers. Pokemon hobby churn could be materially higher in a cooling market. **Founder action**: reach out to indie devs of Card Ladder, Collectr, MTG/sports-card competitors via DM; many indie founders share metrics on Indie Hackers / X.

5. **Conversion rates specifically for "scanner + portfolio" apps.** General freemium benchmarks were used as a proxy. **Founder action**: ask incumbents directly; build minimum viable product and instrument from Day 1.

6. **Real cost of card-recognition ML at scale.** Not researched in this round. **Founder action**: separate technical due-diligence sprint — labeling cost per new set, GPU inference cost per scan, accuracy drop-off on Japanese / damaged / glare cards.

7. **Active vs. lapsed collector ratio.** "Active" definitions vary widely across sources. **Founder action**: define active = 1+ purchase in last 90 days, validate via own user telemetry post-launch.

8. **Pokémon Company licensing posture toward third-party collector apps.** No explicit guidance found. **Founder action**: review TPCi Brand Guidelines; check whether competitors (Collectr, Shiny) operate under formal license or quietly tolerated. Plan a fallback if a takedown ever lands.
