# Wave 1 — Market Landscape (Raw Findings)

Research agent: A1 — Market Sizing & Economics
Compiled: 2026-05-09
Search rounds: 12 web searches + 4 direct page fetches across pokemon.com, Wikipedia, Pokemon Showdown, Graphtreon, PlayTracker.

Tier rating legend:
- **Tier 1** — analyst/industry report (SimilarWeb, Crunchbase/Tracxn financial profiles, official corporate press releases with numbers, peer-reviewed)
- **Tier 2** — established tech press, official game/company announcements without numbers, Wikipedia citing primary sources
- **Tier 3** — blog, forum, social media, fan wiki, SEO-content site

---

## 1. Pokémon Champions Launch Status

### Release date & platforms (CONFIRMED — single source of truth: pokemon.com)
- **Released April 8, 2026** on Nintendo Switch and Nintendo Switch 2 (free-to-start). Source: pokemon.com — "Pokémon Champions Releases on Nintendo Switch and Nintendo Switch 2 on April 8, 2026" — **Tier 1** (official).
- **Mobile (iOS / Android) coming "later in 2026"** — confirmed in same official article, exact date NOT yet announced as of 2026-05-09. **Tier 1**.
- **PC: NOT supported.** Game8 — "Can You Play Pokemon Champions on PC?" — confirms unavailable on PC. **Tier 2**.
- **Cross-platform play between Switch and mobile is confirmed.** **Tier 1** (pokemon.com).
- **Switch 2 free graphical-upgrade patch confirmed.** **Tier 1**.
- Game was announced at **Pokémon Presents on Feb 27, 2025**, alongside Legends: Z-A. **Tier 2** (Wikipedia, Bulbapedia).
- **Play! Pokémon competitive series transitioned to Champions** in April–May 2026 — pokemon.com press release. **Tier 1**.

### Critical reception (anchor for "is this a hit?")
- **Metacritic 65 / OpenCritic 58** at launch. Source: ResetEra review thread + Nintendo Life review round-up. **Tier 2**.
- IGN review-in-progress: "struggling to find the hook." **Tier 2**.
- Game Rant (5/10), Nintendo Life (5/10), Dexerto (6/10), GameSpot (7/10). **Tier 2**.
- Common criticism phrasing: "feels like a title that suddenly had to launch due to chasing a specific quarterly report." (paraphrased across multiple reviews). **Tier 2**.
- Backlash drivers per multiple reviews: poor animation, technical bugs, cut Pokémon (no Amoonguss, Rillaboom), cut items (no Rocky Helmet, Life Orb), grindy progression, microtransactions. **Tier 2**.

### Native team management features — CRITICAL FOR PRODUCT GAP ANALYSIS

| Feature | Native in Champions? | Source | Tier |
|---|---|---|---|
| Team save slots (default) | **3 slots only** | Nintendo Life "In-Game Purchases" guide; gametyrant; insider-gaming | T2 |
| Team save slots (premium) | **18 total** with $4.99/mo or $49.99/yr Membership | Nintendo Life | T2 |
| Replica Team rental codes | Yes — up to **10 simultaneously**, 10-character code | The Gamer, GAMES.GG, Serebii | T2 |
| Replica Team caveat | You must **already own the Pokémon + items** in your box; not a true rental | The Gamer | T2 |
| Matchup notes / team annotations | **Not native** — third parties (Porygon Labs, ChampionsMeta) provide this | Multiple T3 builder sites | T3 |
| Version history / team revisioning | **Not native** | Inferred from absence in all reviews; no contradicting source found | — |
| Replay system / saved match VOD | **NOT IN GAME at launch** — actively requested feature | GameFAQs board "Do you think this game will ever receive a replay feature?"; multiple reviews call this out | T2/T3 |
| In-app teambuilder analysis (defensive/offensive coverage, role warnings) | **Limited** — basic type checker plus image/URL export, but third-party tools (PikaChampions, ChampionsMeta, Porygon Labs, Champions Lab, ChampDex) already filling deeper analysis gap | game8 Team Builder page | T3 |
| Match history with opponent archetype tagging | **Not native** | Reviews + third-party tool feature lists (Porygon Labs advertises this) | T3 |

**Headline product gap:** No native replays + only 3 free team slots + no annotations or version history = exactly the product surface area for a team workspace tool.

### Pokémon HOME integration
- **Confirmed.** Pokémon HOME v4.0.0 added Champions support alongside Legends: Z-A. Source: pokemon.com / Game8 / Serebii. **Tier 1**.
- Uses a **"Visit" model**: Pokémon transferred from HOME are **locked in HOME** while visiting Champions; cannot release/transfer/mark elsewhere until returned. **Tier 2** (TheGamer, GamerBraves).
- **EVs/IVs are overhauled in Champions** — stats look different from S/V; once accepted into Champions, stats are **locked permanently within Champions** and external EV training does not carry over. **Tier 2** (TheGamer guide, GenPKM).
- This means there is **no clean cross-format team portability** between HOME's stored teams and Champions' tuned competitive builds. Builds are effectively format-pinned to Champions.

### Competitive transition
- VGC switched to Champions as the standard tournament platform with the April 8 launch — confirmed by official pokemon.com transition press release (April–May 2026). **Tier 1**.

---

## 2. Player Population Sizing

### Pokémon Showdown (the dominant simulator)
- **>1 million monthly active visitors**, sustained for years. Source: Wikipedia article on Pokémon Showdown citing usage data — **Tier 2**. Independently corroborated in Smogon Development docs ("over a million monthly active users") — **Tier 3**.
- **>30,000 concurrent users at peak.** Same Wikipedia citation. **Tier 2**.
- **18.03M visits in February 2026** per Semrush/SimilarWeb (pokemonshowdown.com); -9.51% MoM. Average session **21 minutes** — extreme engagement. **Tier 1**.
- 82.47% of traffic is direct (loyal repeat users), 10.7% Google, audience top-1 USA then Spain, India. **Tier 1** (SimilarWeb).
- Note: 18M visits ≠ 18M unique users — likely 1–3M MAU with very high session repetition, consistent with the >1M monthly active figure.
- **No public registered-user count** published by Smogon/Showdown after multiple searches.

### VGC / Play! Pokémon competitive ladder
- **2024 Worlds final attendance (verified Twitter from Victory Road, the canonical VGC stats account):**
  - Masters: **694 players**
  - Seniors: **130 players**
  - Juniors: **119 players**
  - Total: **943 VGC competitors at Worlds 2024**. **Tier 2** (canonical community account).
- **2026 Regional sample sizes** (post-Champions launch, from the Limitless/Victory Road network):
  - Orlando Regional: **676 players**
  - Prague Regional: **558 players**
  - Querétaro Regional: **270 players**
  - Pattern: **typical regional = 250–700 players Masters Division.** **Tier 2/3**.
- Play! Pokémon runs **dozens of regionals + multiple internationals + Worlds** per season — order-of-magnitude estimate: **15,000–30,000 unique tournament-attending VGC players globally per season** (assumes ~30 regionals × ~400 avg, with overlap). **Estimated, no public consolidated number found.**
- **2025 Worlds was held at Anaheim Convention Center, Aug 17, 2025; finals stream began ~4pm PDT.** **Tier 2**.

### Pikalytics (the leading public stats site, comparison anchor)
- **SimilarWeb estimate: 223.2K monthly visits** to pikalytics.com. **Tier 1** (SimilarWeb).
- HypeStat estimate **82,256 monthly visits / 2,662 daily uniques** — substantially lower; sources disagree by ~2.7x. **Tier 1** (HypeStat is generally a less reliable sampler than SimilarWeb).
- **Contradiction flagged:** SimilarWeb 223K vs HypeStat 82K monthly. SimilarWeb tends to be higher because it counts repeat visits more aggressively. Conservative read: **80K–225K MAU range** for pikalytics.com.

### Pokémon Scarlet/Violet — the "competitive-curious" install base anchor
- **26.79 million units sold globally** as of March 31, 2025. **Tier 1** (The Pokémon Company / Nintendo financial via Pokémon Blog citing Nintendo's annual report).
- Second best-selling mainline Pokémon game ever, behind Red/Blue (~31.4M). **Tier 1**.
- This is the addressable "owns a recent mainline Pokémon game on Switch" pool. Champions transfers from HOME, which itself bridges S/V → Champions.
- **Pokémon HOME premium subscriber count: NO public data found after 2 searches.** Nintendo/TPC do not disclose this. Pokémon HOME premium is $16/year (Nintendo direct).

### Estimated TAM for "competitive-curious team-prep tool"
Triangulating:
- Hard core: ~30K Pokémon Showdown peak concurrent → implies ~300K–1M committed laddering players globally.
- Medium core: ~1M Showdown MAU + ~80K–225K Pikalytics MAU + tournament attendees.
- Soft core: % of 26.79M S/V owners who would consider team-prep tools — even 1% = 268K additional curious users.
- **Reasonable TAM band: 1.0M–3.0M competitive-curious Pokémon players globally** who already use a team simulator, stats site, or tournament platform; **expanded TAM 5M–10M** if Champions actually onboards casual S/V owners into competitive play.
- **All TAM figures are estimates. No published industry analyst report on competitive Pokémon TAM was found.**

---

## 3. Companion-Tool Monetization Benchmarks

### Within Pokémon
- **Pikalytics**: free; ad-supported; no public revenue figure. **Has a paid iOS app** ("Pikalytics: Battle Strategy") — but no public ARR. **Tier 2**.
- **Pokémon Showdown**: free; non-commercial; no monetization (per Sportskeeda analysis, this is a key reason TPC has not enforced against it). **Tier 3**.
- **Smogon**: free; volunteer-run; no premium tier exists. **Tier 3**.
- **Trainer Tower**: free, 15-person community-driven content org, founded Nov 2016. **No revenue/traffic data published.** **Tier 3**.
- **Victory Road**: free coverage org, founded Sept 2015. **No revenue/traffic data published.** **Tier 3**.

### Pokémon content creators (Patreon — proxy for willingness-to-pay in this fandom)
- **WolfeyVGC (Wolfe Glick, 2016 World Champion):**
  - **10,893 paid Patreon members** + 20,704 total (free + paid). Source: graphtreon.com — **Tier 1** (third-party Patreon analytics, scraped).
  - **Estimated $14K–$94K/month** Patreon-only earnings. **Tier 1** (graphtreon range).
  - **Ranked 80th overall** of all Patreon creators; 26th in Video category.
  - Tiers: Gym Trainer $5/mo, Gym Leader $10/mo. Benefits include tournament prep notes, exclusive analysis videos.
  - Gained **+5,706 paid members in last 30 days** (the Champions launch period).
  - **Implication:** competitive Pokémon content is a real economy. ~11K paid subs at $5+ ARPU at a single creator → ~$650K–$1.3M/yr lower bound, easily above.
- **Aaron Zheng (CybertronVGC):** Stanford GSB grad 2024, podcast (Trainers Lounge), 10x Worlds qualifier — **no Patreon revenue figure surfaced**. **Tier 2**.

### Adjacent gaming companion-tool businesses (the comp set)

| Company | Game | Users | Revenue / Funding | Pricing | Tier |
|---|---|---|---|---|---|
| **OP.GG** | LoL et al. | ~28M MAU; ~75M monthly visits (some sources) | $29.35M raised across 4 rounds; latest Series B $20M Jun 2021 | Free + ads + premium | T1 (Crunchbase, Tracxn) |
| **Mobalytics** | LoL/multi | not disclosed | Acquired by ESL FACEIT Group **March 17, 2025**; est. ARR **$5–25M**; ~53 employees; **$13.8M raised** | Free + Premium subscription | T1 (Tracxn, Owler) |
| **U.GG** | LoL | ~30.7M monthly visits (SimilarWeb); rank ~#1,823 globally | Not disclosed | Free + ads + premium | T1 (SimilarWeb) |
| **Blitz.gg** | Multi (LoL, Valorant, Dota etc.) | On track for ~10M MAU | "Blitz Pro" + "Blitz Enterprise" subscription tiers; saw +39% ad revenue lift via Aditude case study | Freemium | T1 (Aditude case study, SimilarWeb) |
| **Porofessor** | LoL | "nearly 9M users" cited | Not disclosed | Free with premium | T2 |
| **Metafy** | Multi (esports coaching) | not disclosed | **$25M Series A** led by Tiger Global + Seven Seven Six | Marketplace | T2 |

### MTG deck-builder comp set (closest culturally to "team workspace")
- **Moxfield**: completely free, no ads visible to logged-in users, supported by donations/Patreon; community-leading deck builder. **Tier 2** (EDHRec, Draftsim).
- **Archidekt**: completely free, ad + Patreon supported. All features free. **Tier 2** (Archidekt FAQ).
- **EDHRec**: free aggregator/recommender. **Tier 2**.
- **Net read:** the **MTG companion-tool category is overwhelmingly free**. No major MTG deck-builder has flipped to a successful paid SaaS model. Patreon supplements but does not replace ads.

### Chess comp set (huge subscription business)
- **Chess.com**: **150M members** at $100M+ revenue (per 20VC podcast / Sherwood News, 2024); **250M members** by early 2026; **11M DAU** (April 2023 figure). **~1–1.5% conversion to paid** per public estimates. Three tiers, six monthly/yearly options. **Tier 1/2** (Sherwood News reporting).
- **Lichess**: **non-profit**, no ads, no paywall; 1B games played. **Tier 2** (Wikipedia, Lichess directly).
- **Net read:** in chess, the dominant for-profit player has built a 9-figure subscription business at ~1% conversion against a similarly-sized hobbyist population. The free non-profit alternative coexists.

### LLM-powered gaming coach comps (newer category)
- **iTero**: LoL AI coach. Primary revenue = ads. Has **iTero+ at $2.99/mo** to remove ads + unlock customization. **Tier 2/3** (iTero blog, Substack updates).
- **HakkoAI**: claims 10M users, "VLM tech," real-time tactical advice. **Tier 3** (their own site).
- **Statup.gg**: real-time AI voice coaching. **Tier 3**.
- **Meeko.ai**: 24/7 LoL AI coach; Discord/desktop. **Tier 3**.
- **RiftCoach**, **League Copilot**, **Omnic.AI**: all in market 2025–2026.
- **Pricing pattern:** mostly freemium, $3–10/mo subscriptions. **No public ARR/MAU disclosed by any of these AI coaches** after multiple searches.

---

## 4. Industry Trends

- **Esports VC funding fell ~40% in 2023 then rebounded in 2024** per Esports Insider / Finalis. **Tier 2/3**.
- **ESL FACEIT Group acquired Mobalytics on March 17, 2025** — strongest signal that companion-tool category has strategic exits even after a contraction. **Tier 1** (Tracxn).
- **Konvoy Ventures**, **Benchmark** active in gaming infra/analytics. **Tier 2/3**.
- **AI gaming coach category is crowded but unmoated** — at least 6+ direct competitors in LoL alone, all freemium, all with thin pricing ($3/mo). No clear winner has reported MAU > 10M with pricing power.
- **The pattern from Mobalytics, OP.GG, Blitz, U.GG**: tens of millions of MAU + ad-driven revenue + thin premium tier. None became a Chess.com-tier subscription business; instead they exited via M&A in mid-eight-figure to nine-figure ranges (Mobalytics range $5–25M ARR implies <$200M valuation pre-acquisition).

---

## 5. Regulatory & IP Posture

### TPC enforcement record
- **Pokémon Showdown has NEVER received a C&D from TPC/Nintendo** despite using Pokémon names, sprites, mechanics for ~15 years. **Tier 2/3** (Sportskeeda, Quora discussion citing Cale Michael of Sports Illustrated; absence is well-documented in the community).
- **Smogon has never received a C&D** despite hosting all Pokémon names/data. **Tier 3** (community knowledge).
- **Pikalytics, Trainer Tower, Victory Road, Limitless TCG/VGC, Porygon Labs, ChampionsMeta, ChampDex, Champions Lab — all currently active in 2026 with no public C&D events found.** **Tier 3** (live sites, no contradicting source).
- The cited common-sense framing: TPC tolerates fan tools that **(a) don't sell or distribute game software, (b) don't host ROMs, (c) don't compete with TPC's own commerce**. Showdown does charge nothing; this is repeatedly cited as why it has been left alone.

### TPC enforcement actions that DID happen 2024–2026 (for contrast)
- **Palworld (Sept 18, 2024)**: TPC + Nintendo **patent infringement lawsuit** against Pocketpair in Tokyo District Court. **Tier 1** (Dexerto, court filings reported in multiple outlets).
- **Palworld Pokémon-style mods**: Nintendo issued DMCAs against ToastedShoes' mod video, fan merch. **Tier 2** (Kotaku, Windows Central, Insider Gaming).
- **Relic Castle (fan-made game forum)**: shut down in 2024 due to copyright issues from Nintendo + TPC. **Tier 2** (GamesRadar+).
- **Pokémon Essentials**: shut down 2018 (older event, pattern reference). **Tier 2** (Nintendo Life).
- **Pokémon ROM hacks (Prism, Uranium)**: historically C&D'd before release. **Tier 2**.

### Has TPC shipped its own competitive tools historically?
- **Pokémon Stadium / Pokémon Battle Revolution (Wii)**: rental teams, online battles — historic precedent.
- **Pokémon Sword/Shield, Scarlet/Violet**: **Battle Stadium** mode, ranked online ladder, basic team registration, very limited team-prep features. No matchup notes, no version history, no annotations.
- **Pokémon HOME**: storage + transfer; **NOT a teambuilder** in any robust sense. Has basic competitive team builder UX but heavily limited.
- **Pokémon Champions itself**: this is now TPC's flagship competitive companion product. **It only has 3 free team slots, no replays, no match history with annotations, no team versioning** — confirmed gaps as of launch.

### Risk matrix for a third-party "team workspace"
- **Lower risk ingredients** (well-tolerated for 15+ years): Pokémon names, sprites/icons referenced via official-looking links, usage stats, type charts, damage calc, team-import/export via PokePaste-style codes.
- **Higher risk** (would attract enforcement based on TPC pattern): redistributing game ROMs/binaries, hosting playable battle clones, fan game distribution, monetizing trademark itself (selling merch with Pokémon names), simulating gameplay competitive with paid TPC products.
- **Key strategic note:** Champions launching has shifted the dynamic vs Showdown — community speculates risk is "less certain than ever" (Cale Michael, Sports Illustrated, paraphrased). However, no actual enforcement action against simulators or team tools has materialized in the 2 months since Champions launch (per searches as of 2026-05-09).

---

## Key Quantified Findings

- Pokémon Champions launched **April 8, 2026** on Switch + Switch 2; mobile "later in 2026"; PC: not supported. (pokemon.com — T1)
- Champions free tier: **3 team slots**; Membership $4.99/mo or $49.99/yr unlocks **18 total slots**; Replica Team rental codes allow **10 saved** but require already owning the Pokémon. (Nintendo Life — T2)
- Champions launch reception: **Metacritic 65 / OpenCritic 58**, Game Rant 5/10, GameSpot 7/10, Nintendo Life 5/10, IGN review-in-progress critical. (review aggregators — T2)
- Champions explicitly **lacks a replay system** at launch; widely cited as a missing feature by reviewers. (multiple T2 reviews + GameFAQs T3)
- Pokémon Champions Pokémon transfers: **EV/IV stats locked permanently** when Pokémon enters Champions; no clean cross-format portability. (TheGamer — T2)
- Pokémon Showdown: **>1M MAU**, **>30K concurrent peak**, **18.03M total visits Feb 2026 (-9.51% MoM)**, **21-min average session**. (Wikipedia, Semrush — T1/T2)
- Pikalytics: **80K–225K MAU** depending on source (HypeStat vs SimilarWeb disagree). (T1)
- 2024 Pokémon World Championships VGC: **694 Masters + 130 Seniors + 119 Juniors = 943 competitors**. (Victory Road Twitter — T2)
- Recent VGC regionals: **270–676 player Masters fields**, e.g., Orlando 676, Prague 558, Querétaro 270 (2026). (Victory Road / Limitless — T2/3)
- Pokémon Scarlet/Violet sold **26.79M units** lifetime through Mar 31, 2025. (Nintendo financial — T1)
- WolfeyVGC Patreon: **10,893 paid + 20,704 total members**, **est. $14K–$94K/month**, **#80 overall on Patreon**, +5,706 paid in 30 days post-Champions-launch. (graphtreon — T1)
- OP.GG: ~28M MAU; **$29.35M total funding** ($20M Series B June 2021). (Crunchbase — T1)
- Mobalytics: **$13.8M raised**; estimated **$5–25M ARR**; **acquired by ESL FACEIT Group March 17, 2025**; ~53 employees. (Tracxn — T1)
- Blitz.gg: ~10M MAU on track; subscription tiers Blitz Pro / Blitz Enterprise; +39% ad-rev lift case study. (Aditude — T1)
- Chess.com: **~250M members** early 2026; **$100M+ revenue** (2024); **11M DAU** (Apr 2023); **~1–1.5% paid conversion**. (Sherwood News — T1/T2)
- Lichess: **non-profit, fully free, 1B+ games played**. (Lichess + Wikipedia — T2)
- iTero (LoL AI coach): **iTero+ at $2.99/mo**, otherwise free + ads. (iTero — T2)
- Metafy esports coaching: **$25M Series A** led by Tiger Global + 776. (Esports Insider — T2)
- Palworld (TPC enforcement target): patent lawsuit filed **Sept 18, 2024** in Tokyo District Court. (Dexerto — T1)
- Relic Castle (fan game hub) shut down in 2024 from TPC/Nintendo copyright pressure. (GamesRadar+ — T2)
- Pokémon Showdown has operated for **~15 years (since Oct 2011) with zero C&D from TPC**. (Wikipedia, Sportskeeda — T2/3)

---

## Source Inventory

### Tier 1 (analyst / industry / official with numbers)
- pokemon.com — "Pokémon Champions Releases on Nintendo Switch and Nintendo Switch 2 on April 8, 2026"
- pokemon.com — "Play! Pokémon Competitions Transition to Pokémon Champions on April and May 2026"
- pokemon.com — "Pokémon Champions Is Now Available on Nintendo Switch and Nintendo Switch 2"
- Pokémon Blog / Nintendo financial summary, May 8, 2025 — S/V at 26.79M units sold (cites Nintendo's annual financials)
- Semrush / SimilarWeb — pokemonshowdown.com Feb 2026 traffic
- SimilarWeb — pikalytics.com / op.gg / u.gg / blitz.gg traffic profiles
- HypeStat — pikalytics.com (lower-bound estimate)
- Crunchbase — OP.GG funding ($29.35M, Series B $20M Jun 2021)
- Tracxn — Mobalytics ($13.8M raised, ESL FACEIT acquisition Mar 17 2025), OP.GG profile
- graphtreon.com/creator/WolfeyVGC — paid member count 10,893; range $14K–$94K/mo
- Aditude — Blitz.gg case study (39% ad-rev lift)
- Sherwood News — Chess.com $100M+ rev / 150M members 2024
- Statista — Pokémon S/V global unit sales 2025

### Tier 2 (tech press / official without numbers / Wikipedia)
- Wikipedia — Pokémon Showdown (>1M MAU, >30K concurrent peak)
- Wikipedia — Pokémon Champions
- Wikipedia — Chess.com
- Bulbapedia — Pokémon Champions
- Nintendo Life — "Pokémon Champions: In-Game Purchases - Membership & Battle Pass Explained"
- Nintendo Life — "Round Up: The Reviews Are In For Pokémon Champions"
- TheGamer — "Pokemon Champions: Complete Guide To Replica Teams"
- TheGamer — "Pokemon Champions: How To Transfer Pokemon From Pokemon Home"
- TheGamer — "Pokemon Champions Fails Both Hardcore And Casual Players"
- GameSpot — Pokemon Champions review (7/10)
- ScreenRant — "Pokémon Champions Review: Not Quite Champion Material"
- Dualshockers — Pokémon Champions review
- Gamereactor — Pokémon Champions review
- ResetEra — Pokémon Champions review thread
- Insider Gaming — Champions team slots; Palworld Pokémon mod DMCA
- Kotaku — "Nintendo DMCAs Palworld Mod That Makes Everything Pokémon"
- Windows Central — Palworld Pokémon mod takedown
- Dexerto — Nintendo + TPC sue Palworld (Sept 18, 2024)
- GamesRadar+ — Relic Castle 2024 shutdown
- Esports Insider — esports VC trends 2023–2025; GIANTX iTero standalone
- Serebii — Pokémon Champions Replica Teams; Pokémon HOME subscription
- Pokémon Blog / GamesRadar+ — Pokémon HOME Premium ($16/yr)
- Substack — iTero fundraising update
- Kotaku — "A Fan-Made Browser Game Is Pro Pokémon Players' Secret Weapon" (Showdown)
- 51st.news — WolfeyVGC profile (3,000+ Patreon members at $5/mo previously)
- Liquipedia — Cybertron, Trainer Tower, Victory Road profiles
- Victory Road Twitter — 2024 Worlds VG attendance numbers (canonical community source)
- Sherwood News — Chess.com revenue/membership

### Tier 3 (blog / forum / SEO / fan wiki / social)
- Sportskeeda — "How has Pokemon Showdown avoided Nintendo ban hammer?"
- Quora — Showdown shutdown discussion
- GameFAQs — "Do you think this game will ever receive a replay feature?"
- Game8 — Champions team builder, replica codes, platform questions
- GAMES.GG — Champions team slots, replica codes guides
- gametyrant — Champions team slots
- pokebase / pokemondb — Showdown account count question
- The Knowledge Base (theknowledgebase.net) — Pokémon Showdown overview
- finalboss.io — "is it secretly a pay-to-play tax?"
- HakkoAI / RiftCoach / Statup.gg / Meeko.ai homepages
- ChampionsMeta, Porygon Labs, Champions Lab, ChampDex, PikaChampions third-party sites
- Reddit/Twitter posts cited via search (e.g., MathematicalBoi tweet)
- pokemonchampions.us (SEO)

---

## Confidence Notes

### Strong (multi-source corroborated)
- Champions launch date, platforms, F2P model, 3-slot/Membership monetization, HOME integration via Visit model, EV/IV lock — all confirmed via primary pokemon.com + multiple independent reviews.
- Showdown ~1M MAU + 30K concurrent peak — Wikipedia citation + Smogon Development docs + SimilarWeb 18M visit corroboration.
- WolfeyVGC Patreon scale — graphtreon (third-party Patreon scraper, generally accurate within ~10%).
- Mobalytics ESL FACEIT acquisition — Tracxn primary financial profile.
- TPC's enforcement pattern (no action against Showdown/Smogon/Pikalytics; aggressive against ROM hacks/Palworld/fan games).

### Medium confidence (single source or estimated)
- Pikalytics MAU — SimilarWeb (223K) and HypeStat (82K) disagree by ~2.7x. Real number likely between.
- VGC global tournament-attending player population — only event-by-event data, no consolidated TPC figure published. Triangulated estimate of 15–30K worldwide per season is mine.
- Mobalytics $5–25M ARR — Tracxn provides a wide range, not a precise figure.
- Champions player counts post-launch — PlayTracker has zero data; no concurrent/MAU figure surfaced after multiple searches.
- AI gaming coach revenue/MAU — virtually no public ARR/MAU disclosed by iTero/HakkoAI/Meeko/etc. HakkoAI's "10M users" claim is self-reported and unverified.

### Thin / NOT FOUND (gaps for future research)
- **Pokémon Showdown registered (vs active) account count** — no published number after multiple searches.
- **Pokémon HOME global premium subscriber count** — Nintendo/TPC do not disclose; not found.
- **Pokémon Champions launch downloads / DAU / concurrent** — not yet published (game is ~1 month old at time of research; PlayTracker has empty record).
- **Aaron Zheng / CybertronVGC Patreon revenue** — not surfaced.
- **Pikalytics revenue or app revenue** — not disclosed.
- **U.GG and Porofessor exact revenue** — not disclosed.
- **Trainer Tower / Victory Road / Limitless traffic or revenue** — not disclosed.
- **Dollar value of competitive Pokémon tools market specifically** — no industry analyst report exists.
- **TPC's official posture on AI/ML-powered companion tools** — no public statement found.

### Contradictions flagged
- Pikalytics monthly visitors: SimilarWeb 223.2K vs HypeStat 82.3K (factor 2.7x). Use range, not point.
- Mobalytics revenue: Tracxn says $5–25M ARR (a 5x range — extremely wide). Use as order-of-magnitude.
- LoL MAU figures vary 33M–180M depending on source/period — not directly relevant here, but illustrates the noise in any "active player" companion-tool comp.

### What I deliberately did NOT estimate
- Did not invent any TAM dollar figure — the $-denominated sizing exercise belongs in a separate financial-model wave once unit economics inputs are picked.
- Did not estimate WolfeyVGC's exact monthly revenue inside the $14K–$94K band — the band itself is what graphtreon publishes.
- Did not estimate Champions' actual installed base — too early post-launch and no public data exists.
