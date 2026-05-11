# Indirect Competitors, Substitutes & Platform Risk
## Pokémon TCG Collection Manager — Mobile App

**Research date:** 2026-05-10
**Wave:** 1 (Discovery)
**Search budget used:** 8/9
**Scope:** US Pokémon serious-hobbyist segment ≈ 200K paying-eligible (carried from Wave 1)

---

## 1. Status Quo Solutions (Substitutes)

These are non-app workflows that the 200K-collector base actually uses today. The relevant question is not "could an app beat them on features" — it's "why do collectors still use them."

### 1.1 Spreadsheets (Excel / Google Sheets)

- **Prevalence:** ~30–40% of serious hobbyists maintain at least one spreadsheet **[Estimate]**, often *in addition* to an app. Multiple community-shared templates exist on PokéBeach, PokéCommunity, Elite Fourum, Scribd, and Reddit (e.g., u/konekode's TCG Pocket sheet has been cross-posted across Threads / Facebook / Reddit) **[Data]**.
- **Why it sticks:**
  - Total schema control — collectors invent custom columns (sleeve type, trade history, bought-from, condition notes, "for trade" flag) **[Data, from forum threads]**.
  - Free, portable, no vendor lock-in, no shutdown risk.
  - Formulas + Bulbapedia/takharii.com set-list scrapes give "% complete per set" tracking that most apps don't expose well **[Data]**.
- **Where it breaks:**
  - Pricing is stale — collectors copy/paste TCGplayer prices manually, which decays daily.
  - Mobile UX is brutal (Sheets on phone is unusable for batch entry).
  - No image, no scan, no auto-set-detection — you type every card by hand.
  - Becomes "quite a task as the collection grows" **[Data, multiple Reddit/forum posts]** — typically breaks past ~500–1,000 cards.
- **Threat level to a new app:** **HIGH** as a substitute (free, sticky, customizable), **LOW** as direct competition (no mobile ergonomics).

### 1.2 eBay Sold-Listings Tab + TCGplayer Search (Manual Lookup)

- **Prevalence:** ~70–85% of serious hobbyists use eBay sold-listings as their *price-check* workflow for higher-value cards (>$20) **[Estimate, triangulated from Wave 1 research that eBay/TCGplayer dominate price discovery]**. This is the de-facto "comp" tool.
- **Why it sticks:** Free, real-time, ground-truth signal. eBay sold = what a card *actually* transacted at, including BIN vs auction spread. No app fully replaces this for high-value collectors.
- **Where it breaks:** Per-card; no portfolio view, no aggregate value, no historical chart, no condition-adjusted comp filtering at scale.
- **Threat:** **MEDIUM** substitute — coexists with apps; collectors use both. The app value-add is *aggregation*, not lookup.

### 1.3 Reddit / Discord / Community-Tracked Value

- **Prevalence:** ~50–60% of serious hobbyists are active in r/pkmntcgcollections, r/pkmntcgtrades, or Discord servers (FlipsideGaming, Elite Trainer, set-specific servers) **[Estimate]**.
- **Why it sticks:** Trade reputation, "what's-this-worth" social validation, deal-spotting — these are *not* app-replaceable functions. Trade reputation systems on r/pkmntcgtrades are the closest thing to escrow many collectors use **[Data]**.
- **Where it breaks:** Not a tracker; no inventory, no portfolio. Pure community layer.
- **Threat:** **LOW** as a direct substitute, but **HIGH** as a switching anchor — collectors won't leave their community even if an app is better at tracking.

### 1.4 PSA Set Registry / Pop Reports (Graded-Card Collectors)

- **Prevalence:** Mandatory for graded-card collectors. Likely ~15–25% of the 200K paying-eligible segment treats PSA Set Registry as their primary tracking tool **[Estimate]**.
- **Why it sticks:** Official population data, set-completeness leaderboards (rank/competition layer), and PSA Premium membership ($199/yr) bundles in **Card Ladder Pro ($200 value)** **[Data]** — this is a meaningful giveaway.
- **Where it breaks:** Graded-only; raw cards invisible. Web-first, mobile experience is weak for inventory entry.
- **Threat:** **HIGH** for graded-card subsegment (20-25% of TAM); **LOW** for raw-card collectors.

### 1.5 Physical Binders + Memory ("Lazy" Baseline)

- **Prevalence:** ~40–55% of collectors at the lower end of "serious" track *nothing* digitally and rely on binders/photo albums **[Estimate]**.
- **Why it sticks:** Zero friction. The hobby is tactile; many collectors actively *don't want* the spreadsheet experience.
- **Where it breaks:** Insurance loss, theft, no liquidity, no value awareness. Almost no upgrade trigger until a "wake-up" event (move, divorce, theft, trying to sell).
- **Threat:** **HIGH** — this is the dominant "competitor." The hardest user to convert because they don't experience the pain until something goes wrong.

### 1.6 LCS (Local Card Shop) Printouts / Consignment Systems

- **Prevalence:** ~5–10% **[Estimate]**, mostly older collectors and consignment sellers.
- **Why it sticks:** Trust relationship; LCS handles pricing + sale.
- **Where it breaks:** LCS spreads (typically 30–50% of retail) are punitive; no real-time visibility.
- **Threat:** **LOW** to a digital app.

---

## 2. Adjacent Products & Platform Risk

Per-threat ratings: likelihood that the platform absorbs/eliminates the wedge within stated timeline.

### 2.1 eBay (existing app, owns TCGplayer)
- **Capability:** Watchlist already gives portfolio-lite. Sold-comps are unmatched. Following eBay's TCGplayer acquisition, pricing data is in-house **[Data — Wave 1]**.
- **Likelihood of absorption: MEDIUM-HIGH**
- **Timeline: 18–36 months** for a serious "collection portfolio" feature, given eBay's slow cadence on consumer features. **[Estimate]**
- **Mitigation:** Be better at *non-eBay* workflows — community trades, set completion, condition notes, multi-source pricing. Avoid being a thin wrapper on eBay data.

### 2.2 TCGplayer App (eBay-owned, owns the pricing data)
- **Capability:** Already has the canonical pricing dataset and a card identifier. Could trivially add scan-to-collection with portfolio valuation. The fact that they *haven't* — despite 5+ years of opportunity — suggests strategic disinterest, not inability **[Assumption, but strong].**
- **Likelihood of absorption: HIGH** (they have everything they need)
- **Timeline: 12–24 months** if eBay decides to push it; 36+ months if it remains a marketplace-only app **[Estimate]**.
- **Mitigation:** Speed; community features; cross-platform pricing (don't be locked to TCGplayer-only data, integrate eBay sold + Cardmarket).

### 2.3 PSA / Collectors (owns Card Ladder, Beckett)
- **Capability:** Already has the **PSA app with card scanner + digital inventory + real-time pricing** in production **[Data]**. Owns Card Ladder Pro for analytics. Acquired Beckett (further consolidation) **[Data]**. Premium tier ($199/yr) bundles Card Ladder Pro at zero marginal cost.
- **Likelihood of absorption: HIGH** for the graded-card subsegment — they're already doing it.
- **Timeline: NOW** for graded; **12–18 months** to extend to raw-card portfolio at scale.
- **Mitigation:** This is the most credible existential threat. Differentiate aggressively on raw-card UX, community/trades, and set-completion features that don't serve PSA's grading-funnel agenda. Avoid head-on collision with graded-card tracking.

### 2.4 Pokémon TCG Pocket / TCG Live (TPCi/Nintendo official)
- **Capability:** Could in theory ship a physical-card scan/track tool. They have the brand, but their priorities are digital game monetization, not collection management. **[Assumption]**
- **Likelihood of absorption: LOW**
- **Timeline: 36+ months** if ever; physical-card features are off-strategy.
- **Mitigation:** Minimal action needed; monitor only.

### 2.5 Apple Wallet / Google Wallet (collectibles passes)
- **Capability:** Speculative. No public roadmap on collectibles passes for trading cards. **[Assumption]**
- **Likelihood of absorption: LOW**
- **Timeline: Unknown / 36+ months**
- **Mitigation:** Not a near-term concern.

### 2.6 Generic Portfolio Trackers (Kubera, Empower, etc.)
- **Capability:** Could add a collectibles asset class but historically have stayed in liquid financial assets. Even Kubera's "alternative assets" feature is manual entry.
- **Likelihood of absorption: LOW** — TCG is a niche with idiosyncratic data needs (set/number/condition/grade) that don't map to a generic asset row.
- **Timeline: 36+ months**
- **Mitigation:** None needed. Different buyer.

### 2.7 Sports-Card Platforms Entering TCG (Goldin, PWCC, Fanatics Collect)
- **Capability:** These are auction/marketplace plays, not collection-management plays. Fanatics has the deepest pockets and could acquire a TCG-tracking app to bundle with their auction flow.
- **Likelihood of absorption: MEDIUM** via acquisition; **LOW** via build.
- **Timeline: 24–36 months** for acquisition appetite; depends on category economics.
- **Mitigation:** Build to be acquirable (clean data model, defensible community, real DAU) — possibly an *exit path* rather than a threat.

### 2.8 Existing collection-app incumbents (NOT the question, but adjacent)
- Collectr, PKMN.GG, TCG Collector, PokeDATA, Pricecharting Collection Tracker, Shiny, PokeScope all already exist and have varying traction **[Data]**. These are *direct* competitors and are covered in a separate Wave 1 deliverable; flagged here only to note that the "obvious app" space is already crowded.

---

## 3. Open-Source / Free / DIY Alternatives

### 3.1 Open-Source Card Recognition

There are **10+ active GitHub repos** for Pokémon card scanning **[Data]**:

| Repo | Approach | Maturity |
|------|----------|----------|
| `prateekt/pokemon-card-recognizer` | Pre-built refs all major sets, GPU-accelerated | Most mature |
| `1vcian/Pokemon-TCGP-Card-Scanner` | TCG Pocket-specific | Active |
| `em4go/PokeCard-TCG-detector` | OpenCV + Pokémon TCG API | Active |
| `t-sinclair2500/pokemon-scanner` | OpenCV + Tesseract + pricing | Active |
| `xavidop/cardex` | "All-in-one AI platform" | Active |
| `NolanAmblard/Pokemon-Card-Scanner` | OpenCV + MySQL, single-set | Demo |
| `iFan13/Pokemon_TCG_Scanner` | CV + ML OCR | Demo |
| `KLuml/CardScanner`, `luisquint/Pokemon-Card-Detector`, `jmtrafny/card-scanner` | Various | Demo |

**Founder implication:** Card recognition is **NOT a moat**. A weekend integration of `prateekt/pokemon-card-recognizer` + Pokémon TCG API gets to ~90% accuracy. The moat must be elsewhere (UX, pricing aggregation, community, trades, or completeness).

### 3.2 Paid Recognition API: Ximilar
- **Pricing:** ~10 credits per card scan; Business 100k Plan ≈ 10,000 cards **[Data]**. Custom pricing for higher volume.
- **Coverage:** 15+ TCGs including Pokémon, MTG, Yu-Gi-Oh!, One Piece, Lorcana **[Data]**.
- **Cost implication:** At ~$0.001–0.01 per scan depending on tier, recognition is a cheap commodity. **Not a meaningful cost barrier.**

### 3.3 Pricing API Access (CRITICAL FOUNDER DECISION)

**TCGplayer API:** **CLOSED to new developers as of late 2024.** Existing keys being deprecated; no public timeline to reopen. eBay acquisition shifted strategy to "data stays in-ecosystem." **[Data]**

**eBay Finding API:** Decommissioned Feb 5, 2025. `findCompletedItems` deprecated since Oct 2020. **License terms forbid storing results or using for "market research."** Marketplace Insights API restricted to "high-end developers (like Terapeak)" with eBay Business approval. **[Data]**

**Pokémon TCG API (pokemontcg.io / now part of Scrydex):** Free, no key = 1,000 req/day & 30 req/min; with key = higher; pricing data sourced from **Cardmarket** (European, not US-primary). **[Data]**

**Third-party paid alternatives that have emerged:**
- JustTCG
- TCG API (tcgapi.dev / tcgapis.com)
- PokeWallet.io
- pokemon-api.com
- Scrydex (the new owner of pokemontcg.io)

**Founder implication:** This is the **single largest non-obvious risk in the build**. The canonical US pricing dataset (TCGplayer Market Price) is now legally walled off. Options:
1. Pay for a third-party aggregator (introduces dependency + recurring cost).
2. Use Cardmarket-priced data via Pokémon TCG API (US collectors will complain — Cardmarket prices ≠ TCGplayer prices).
3. Scrape (legal grey zone, fragile, ToS violation).
4. User-contributed pricing (requires scale to be useful).

### 3.4 Browser Extensions
- Search did not surface a single category-leading TCGplayer Chrome extension **[Data — null result]**. This is either an opportunity (low entry into desktop workflow) or a signal that desktop is not where the user is. **[Assumption: desktop irrelevance]**

---

## 4. Switching Cost Analysis — What Moves a Collector Off Their Spreadsheet?

A serious collector with a working spreadsheet has **switching costs ≈ 4–10 hours of re-entry** plus **loss of custom schema** plus **trust transfer to a new vendor**. The triggers that overcome this:

| Trigger | Strength | Notes |
|---------|----------|-------|
| **Bulk scan-and-import** of an existing collection (CSV → app, or photograph-binder → recognized cards) | **HIGHEST** | The single largest unlock. Eliminates the 4–10 hour re-entry tax. **[Estimate]** |
| **Live pricing that beats stale spreadsheet values** | HIGH | But only if the pricing source is *credible* (TCGplayer/eBay sold) — Cardmarket-only will be dismissed. |
| **Mobile-first batch entry** (scan 10 cards in 60 seconds) | HIGH | Spreadsheets are unusable on mobile; this is the Achilles heel. |
| **Set-completion tracking with visual %** | MEDIUM-HIGH | Spreadsheets do this with formulas; an app must do it *better* with set imagery. |
| **Trade workflow / community integration** | MEDIUM | Reddit r/pkmntcgtrades + Discord are sticky; an in-app trade flow with reputation is a real wedge but hard to bootstrap. |
| **Insurance / loss documentation** (photos + values + serial #s, exportable PDF) | MEDIUM | Latent need; few collectors say it but many would value it post-event. |
| **Graded-card sync with PSA cert lookup** | MEDIUM | Already partially solved by PSA app for the graded subsegment. |
| **Ability to *export* to a spreadsheet anytime** | UNDERRATED | Lock-in fear is the silent killer. Apps that don't offer clean CSV export lose the spreadsheet-power-user persona. |

**Verdict:** The path off a spreadsheet is **bulk-import + mobile scan + credible US pricing + clean export**. Miss any one and the collector keeps the spreadsheet. The first three are achievable; **credible US pricing is the structural risk** because of TCGplayer API closure.

The "lazy baseline" (binders + memory, ~40–55% of segment) has a *different* switching trigger: a **wake-up event** (insurance, sale, theft, move). The app that captures this user must be present *at the event* (search, recommendation, friend referral) — they don't pre-shop for collection apps.

---

## 5. Platform-Risk Verdict

**Single biggest existential threat:** **PSA / Collectors.** They already ship a card-scanner + digital-inventory + real-time-pricing app, they own Card Ladder (analytics), they bought Beckett (consolidation), and they bundle Card Ladder Pro free with their $199/yr Premium membership. For the **graded-card subsegment** (~20-25% of the 200K) they are not a future threat — they are the incumbent. For the **raw-card subsegment**, the threat is 12-18 months out and motivated, because every raw-card-tracker user is a future grading-submission lead in PSA's funnel — meaning PSA is willing to operate this product at *negative margin* to feed their core business. Any startup serving the raw segment must build a wedge that PSA structurally cannot copy: cross-grader-neutral (PSA + CGC + Beckett + raw all equal), trade-community-first (PSA has no community asset), or non-US-pricing-aware (PSA is US-graded-centric). The TCGplayer-API closure compounds this — PSA's pricing pipeline is internal and won't break, while the startup's depends on a fragile third-party data layer.

**Secondary platform threat:** TCGplayer/eBay, lower urgency (12-36 months), but if they ship, they win pricing decisively.

---

## 6. Data Gaps

| Gap | Severity | How to close |
|-----|----------|--------------|
| Actual % of 200K paying-eligible using each substitute (spreadsheet/eBay/binders/etc.) | HIGH | Wave 2 survey; r/pkmntcgcollections poll |
| Whether PSA has a *raw-card* tracking roadmap (vs. graded-only focus today) | HIGH | Wave 2: PSA earnings calls, exec interviews, App Store update notes |
| TCGplayer API reopening probability + timeline | HIGH | Wave 2: developer.tcgplayer.com FAQ monitoring; eBay developer forums |
| Whether Scrydex/JustTCG/TCG API can serve as a stable canonical US-pricing source at startup-affordable cost | HIGH | Wave 2: founder direct outreach for pricing + ToS review |
| Reddit/Discord true active-collector size (not just subscriber count) | MEDIUM | Subreddit traffic stats, Discord member counts via DiscordLookup |
| Existing-app churn rates (Collectr, PKMN.GG, TCG Collector) — do users leave, and to where? | MEDIUM | App Store/Play Store review mining, Reddit complaint threads |
| Insurance-as-trigger frequency (theft + claim events) | LOW-MEDIUM | Insurance industry reports; collectibles riders data |
| Whether Fanatics Collect has signaled TCG-acquisition appetite | MEDIUM | News monitoring; Fanatics earnings/M&A activity |
| Founder's own time-budget for community moderation (community is the strongest moat against PSA, but founder is light-collector + side project) | HIGH — INTERNAL | Founder self-assessment in Wave 2 |

---

## Sources

- [PokéBeach forum: How I Catalog My Card Collection](https://www.pokebeach.com/forums/threads/how-i-catalog-my-card-collection.150917/)
- [PokéCommunity: Master Card Inventory Spreadsheet](https://www.pokecommunity.com/threads/master-card-inventory-spreadsheet.273714/)
- [Elite Fourum: Pokemon TCG Collection Tracker Excel](https://www.elitefourum.com/t/pokemon-tcg-collection-tracker-excel-document/34382)
- [Elite Fourum: How do you keep track of value](https://www.elitefourum.com/t/how-do-you-keep-track-of-the-value-of-your-collection/41383)
- [Pokemon TCG Spreadsheet V3.2 (Scribd)](https://www.scribd.com/document/825230180/Pokemon-TCG-Spreadsheet-V3-2)
- [JustTCG: Definitive TCGplayer API Alternative for Developers in 2025](https://justtcg.com/blog/the-definitive-tcgplayer-api-alternative-for-developers-in-2025)
- [TCG API: Best TCGplayer API Alternative 2026](https://tcgapi.dev/blog/tcgplayer-api-alternative/)
- [TCGAPIs: TCGplayer API Alternatives 2026](https://tcgapis.com/blog/tcgplayer-api-alternatives)
- [TCGplayer Developer Docs](https://developer.tcgplayer.com/)
- [eBay Developers — findCompletedItems (deprecated)](https://developer.ebay.com/Devzone/finding/CallRef/findCompletedItems.html)
- [eBay sold items documentation (GitHub)](https://github.com/colindaniels/eBay-sold-items-documentation)
- [Pokémon TCG API rate limits](https://docs.pokemontcg.io/getting-started/rate-limits/)
- [Pokémon TCG API (now part of Scrydex)](https://pokemontcg.io/)
- [PSA app on App Store](https://apps.apple.com/us/app/psa-card-scanner-grading/id996239729)
- [PSA Apps page](https://www.psacard.com/info/apps)
- [PSA support: app card scanner](https://support.psacard.com/s/article/psa-app-card-scanner)
- [Sports Collectors Daily: PSA acquires Card Ladder](https://www.sportscollectorsdaily.com/psa-acquires-card-laddere/)
- [PSA: Collectors Universe Acquires Card Ladder](https://www.psacard.com/articles/articleview/10556/collectors-universe-acquires-card-ladder-card-grading-values)
- [Sportico: Collectors Universe Buys Card Ladder](https://www.sportico.com/business/commerce/2021/collectors-universe-buys-card-ladder-1234647703/)
- [Yahoo: Collectors acquires Beckett](https://sports.yahoo.com/articles/led-psa-collectors-corners-even-230000416.html)
- [Card Ladder Pro and PSA integration overview](https://www.oreateai.com/blog/card-ladder-pro-and-psa-elevating-your-card-collecting-game/0e38a0e6d87f2853e562eba72d9fe51b)
- [Sports Collectors Daily: PSA app card identification & grading](https://www.sportscollectorsdaily.com/psa-card-grading-app-update-scanning-grading/)
- [GitHub: prateekt/pokemon-card-recognizer](https://github.com/prateekt/pokemon-card-recognizer)
- [GitHub: 1vcian/Pokemon-TCGP-Card-Scanner](https://github.com/1vcian/Pokemon-TCGP-Card-Scanner)
- [GitHub: em4go/PokeCard-TCG-detector](https://github.com/em4go/PokeCard-TCG-detector)
- [GitHub: t-sinclair2500/pokemon-scanner](https://github.com/t-sinclair2500/pokemon-scanner)
- [GitHub: xavidop/cardex](https://github.com/xavidop/cardex)
- [GitHub: NolanAmblard/Pokemon-Card-Scanner](https://github.com/NolanAmblard/Pokemon-Card-Scanner)
- [Ximilar Plans & Pricing](https://www.ximilar.com/pricing/)
- [Ximilar Collectibles Recognition API](https://docs.ximilar.com/collectibles/recognition)
- [Ximilar: How to Automate Pricing of Cards & Comics via API](https://www.ximilar.com/blog/how-to-automate-pricing-of-cards-comics-via-api/)
- [TCG Collector](https://www.tcgcollector.com/)
- [PKMN.GG](https://www.pkmn.gg/)
- [PokeDATA](https://www.pokedata.io/portfoliolanding)
- [Pricecharting Collection Tracker](https://www.pricecharting.com/page/collection-tracker)
- [Collectr app](https://app.getcollectr.com/)
- [CardPriceIQ: 7 Best Card Scanner Apps 2026](https://cardpriceiq.com/news/best-card-scanner-apps-2026)
