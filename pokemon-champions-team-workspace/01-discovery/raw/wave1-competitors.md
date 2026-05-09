# Wave 1 — Competitor Deep-Dive: Pokémon Champions Team Workspace

**Research agent:** A2
**Date:** 2026-05-09
**Scope:** Direct + indirect competitors for a "persistent team workspace" web app targeting Pokémon Champions (TPC's standalone competitive battler, launched on Switch 2026-04-08, with iOS/Android ports later in 2026; replaced Scarlet/Violet as the official VGC platform starting with Indianapolis Regionals 2026-05-29).

**Source-tier legend:**
- **T1** — Primary / official (the company itself, gov filing, the operator's own statements). High confidence.
- **T2** — Reputable third-party measurement (Similarweb, Semrush, Social Blade, Wikipedia citing primary, Liquipedia).
- **T3** — Community-curated reference (VGCpedia, Smogon forum threads, fan wikis, Reddit).
- **T4** — Inferred / extrapolated / single-anecdote.

---

## A. Comparison Matrix — Direct Competitors

| # | Product | Pricing | Target user | Funding | Traction (latest) | Workspace? | AI? | Mobile? | Strength | Weakness |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | **Pokémon Showdown** (play.pokemonshowdown.com) | Free | All competitive PKM players (sim + teambuilder) | Personally funded by Smogon founder Chris "chaos" Monsanto; volunteer-maintained, MIT-licensed | ~13.88M monthly visits to smogon.com (the parent), Showdown ranks #2020 globally / #10 Games-Other on Similarweb (Mar 2026); web traffic +19.89% MoM | Partial — server-side team save (`/teams`) exists since 2022, browser cookie fallback; folders by tier; no real "workspace" (no comments, versioning, AI, multiplayer collab) | No | Browser-only (mobile web works; no iOS app due to App Store policy; Android APK only) | Default tool of the entire competitive scene; full sim + teambuilder + ladder in one place; deep format coverage; open-source ecosystem (Showdex extension, etc.) | Owned by Smogon (Scarlet/Violet/Smogon-tier focus); Champions support is community-driven, not first-party; UX dated; no AI; no native mobile; teams stored as flat list, not as a versioned project |
| 2 | **Smogon University** (smogon.com) | Free | Smogon-tier players, RMT seekers, theorycrafters | Donations / Smogon Premier League sponsorships; volunteer mods | ~13.88M monthly visits (Semrush Jan 2025); 45% organic search, 43% direct; "RMT of the Year 2025" award shows active forum culture | No — RMT is forum threads, not a workspace; sample teams are static articles | No | Mobile web only | Strongest organic SEO moat in competitive PKM (ranks for nearly every Pokémon name + tier query); 20+ year community trust; the canonical "Smogon-tier" rule body | Forum UX from 2010s; primary focus is Smogon singles tiers, not VGC/Champions; no AI, no team versioning, no personal workspace; RMT feedback is human + slow |
| 3 | **Pikalytics** (pikalytics.com) | Free, ad-supported (assumed); "Support Us" link visible | VGC players checking usage stats + matchups | Solo / tiny team (founder operates @Pikalytics on Twitter; not publicly disclosed funding) | Featured site in VGCpedia; sole canonical destination for "[format] usage stats" SEO; shipped full Champions support (Pokédex, damage calc with Champions ruleset toggle, team builder, top teams, calc-quiz) within weeks of game launch | Partial — has a team builder (pikalytics.com/team) with suggested sets, but it's a stateless builder, not a versioned workspace | Damage calc + meta data is data-driven, not AI; no LLM coaching layer | Mobile web; no native app located | Fastest to ship Champions content; the trusted source for usage/meta data; calc + builder + meta in one site is a strong bundle | No persistent user accounts visible; no team history/versioning; ads are noisy; not a coaching tool |
| 4 | **Poképaste** (pokepast.es) | Free, optional donations | Anyone sharing teams via URL | Solo dev (Felix Phew); BSD/MIT-licensed | ~300K+ pastes in DB (creator's own statement); de facto URL-sharing standard across Showdown/Smogon/Twitter/VGC | No — anonymous, write-once paste hosting; intentionally has no accounts (URLs are cryptographic) | No | Mobile web works | Universally adopted "share team" primitive; trivially embedded in every other VGC site; zero friction | By design has no analysis, no accounts, no comments, no editing — pure pastebin |
| 5 | **VGCPastes** (vgcpastes.com / @VGCPastes) | Free | VGC players hunting tournament-proven teams | Volunteer-curated (community contributors via Twitter/Discord) | 1,150 teams logged for Reg H; 63 teams already curated for Reg I; cross-format repos for SV Series 1, Reg G, Reg H, Reg I | Curated repository, not a workspace — exports paste links | No | Mobile web | Single best library of *meta-validated* team archetypes; community-trusted curation | Read-only spreadsheet feel; depends on Poképaste; nothing personal/private/AI |
| 6 | **Limitless TCG / VGC** (play.limitlesstcg.com, limitlessvgc.com) | Free for players; tournament organizer pricing not public | Tournament organizers + players; tournament data consumers | Self-funded / sponsorship-funded (run by Eddy "Limitless" Cheung & team) | The de facto Swiss tournament-running platform; tracks every tour result for VGC 2025-26 season; supports Champions tournaments from day 1 | No — tournament management + result database, not a personal teambuilding workspace | No | Mobile web; functional | Owns competitive *tournament* infrastructure end-to-end (registration, decklist, results, decklist-archives); irreplaceable for TOs | Not a player-facing teambuilding tool; no team workspace, no analysis layer for personal prep |
| 7 | **Trainer Tower** (trainertower.com) | Free content; damage calc free | English-speaking VGC players, intermediate-to-advanced | Volunteer collective (~15 people, founded Nov 2016 to fill the NuggetBridge gap); revenue source not publicly disclosed (likely zero/donation) | Hosts the most-cited damage calc fork (damagecalc.trainertower.com); runs the "World Cup of VGC" annually | No (calc is stateless; articles are content) | No | Mobile web | Strongest English-language *long-form* VGC analysis brand; the canonical VGC damage calc | No product, no accounts, low ship velocity (volunteer-run); no AI, no workspace; competition for the calc from Pikalytics and the Showdown calc |
| 8 | **Victory Road** (victoryroad.pro) | Free; Twitch/YT monetization; sponsorships | International VGC players (started Spanish, English since 2018) | Founded 2015 by Ruben Yanguas + David Olivar; ad/sponsorship + Twitch sub revenue (assumed); not a funded startup | The community's go-to VGC "season hub" (rules, calendar, regulations, resources, regional coverage) | No — content + tournament coverage hub | No | Mobile web | The canonical VGC season-information site; first to publish Champions regulations breakdowns; bilingual reach | Editorial not product; no team workspace; revenue model is creator-economy not SaaS |
| 9 | **Damage calculators** (calc.pokemonshowdown.com, trainertower calc, NCP, vgcmulticalc, pikalytics calc) | All free | Every competitive player | Smogon-funded for the official one; volunteer forks for the rest | The Showdown calc (`@smogon/calc`) is the canonical engine; Showdex extension (4.7★, integrates calc into Showdown live) is widely installed | No | Embedded — Showdex syncs with live Showdown battles | No | Calc engine is a commodity (open-source, well-tested) | Stateless tool; no team memory, no versioning, no personalization |

### A.1 New Champions-era entrants (already shipped before A2's research date 2026-05-09)

These appeared in the ~30 days between game launch (2026-04-08) and now — direct evidence the founder has competition already in their exact niche.

| Product | URL | What it does | Workspace? | AI? | Mobile? |
|---|---|---|---|---|---|
| **VGCCoach** | vgccoach.pro | "Trained on 112,000 real VGC battles"; instant team-score 0-10 + AI coaching in <3s | Some (team analysis, articles) | **Yes — explicit AI coach product** | Web |
| **ChampTeamAI** | champteamai.com | AI builds full team (moves/EVs/items/abilities) scoped to Champions | Generative, not persistent | **Yes** | Web |
| **Champions Lab** | championslab.xyz | Team builder + battle simulator + meta analysis | Builder only | Unclear | Web |
| **Champions Builder** | championsbuilder.com | Team builder w/ SP calc, damage calc, mega evos, Showdown export | Builder only | No | Web |
| **Champions Team Builder** | championsteambuilder.app | Coverage checker + speed tiers + 6-mon recommendations | Builder only | Pattern-based, not LLM | Web |
| **ChampDex** | apps.apple.com/us/app/champdex | "Build smarter teams, calculate damage, track meta" | Some | Unclear | **Native iOS** |
| **Pokébase Champions** | pokebase.app/pokemon-champions | Team builder + damage calc | Builder only | No | Web + app |
| **Porygon Labs** | porygonlabs.com | Champions damage calc + team builder | Builder only | No | Web |
| **Poké Team Builder** | poketeambuilder.app | Generic AI Pokémon team builder (Showdown/VGC) — not Champions-exclusive | Generative | **Yes** | Web |

**Critical implication:** the "AI VGC coach" wedge is already crowded with 2+ shipped products (VGCCoach, ChampTeamAI) and the "Champions team builder" wedge has 5+ shipped competitors as of week 4 post-launch. The founder is not first; the question is differentiation.

---

## B. Deep-dives

### 1. Pokémon Showdown — the 800-lb gorilla
- **Maintained by:** Smogon University, originally written by Guangcong "Zarel" Luo, server funded by Smogon founder Chris "chaos" Monsanto. Volunteer-maintained, MIT-licensed (T2: Wikipedia + GitHub).
- **Traction:** Similarweb has Showdown ranked #2020 global / #10 in Games-Other as of March 2026, with a 19.89% MoM traffic bump (T2). Smogon.com (the parent) drew ~13.88M monthly visits in Jan 2025 (T2: Semrush). Audience skews 68.7% male, largest cohort 18-24 (T2: Similarweb). The community runs trivia comps, multi-tier leagues, and custom format cups year-round.
- **Team save capacity:** Server-side team storage was added in 2022 ("Teams can now be stored server-side!" official news post #175). Teams are accessible via `/teams` slash command across logged-in devices. The teambuilder also auto-organizes folders by tier (T1: official news + T3: PokeBase Q&A). I couldn't confirm an explicit per-account team count cap; in practice users routinely store dozens.
- **2025-2026 product moves:** Continued adding format support, but no public roadmap signaling a workspace pivot. The product remains a battle simulator with a teambuilder bolted on. Champions support is community-effort (as Champions is not Smogon-tier-derived). The Showdex extension (4.7★ Chrome rating) is the de facto "calc inside Showdown" overlay — a third party is filling the in-app analysis gap.
- **Monetization:** None. No premium tier. No ads. No plans signaled.
- **Threat to founder:** **HIGH for sim/teambuilder use case, LOW for AI-workspace use case.** Showdown will not ship AI coaching, native mobile, or rich workspace features any time soon — that's the gap.

### 2. Smogon University — the SEO moat
- **Acquisition engine:** Google organic search drives 45.21% of Smogon's traffic, direct another 42.59% (T2: Similarweb). Smogon ranks for virtually every "[Pokémon] competitive set" / "[Pokémon] moveset" / "[tier] sample teams" query. Over 20 years of accumulated content + interlinking is a near-impossible moat to replicate.
- **Community:** "RMT of the Year 2025" awards ran successfully (T1: smogon forum thread). RMT forums by generation/tier are extremely active.
- **2025-26 product moves:** None of consequence. Forum software is the same. No app. No AI. No premium tier.
- **Workspace-style features:** Effectively zero — RMT is forum threads, sample teams are static articles. No team versioning, no private notes, no personal dashboard.
- **Threat to founder:** **MEDIUM via SEO (any new tool will struggle to outrank Smogon for generic Pokémon queries) but LOW as a product.** The founder needs to win on long-tail Champions-specific + workspace-feature queries, not head-on against Smogon SEO.

### 3. Pikalytics — fastest mover, biggest threat in the data layer
- **Owner / team:** Solo or very small team behind @Pikalytics. Not publicly funded; no disclosed investors.
- **Monetization:** Display ads + "Support Us." No premium tier identified.
- **Champions response:** Within ~30 days of Champions launch, Pikalytics shipped: full Champions Pokédex, Reg M-A meta stats, Champions damage calc with Champions-specific ruleset toggle (weather/terrain/screens/Helping Hand/Intimidate stacking), team builder, top teams, "calc-quiz" gamified learning tool. This is the fastest-moving incumbent in the space (T1: pikalytics.com/champions, /calc, /team, /calc-quiz, /topteams).
- **Workspace-style features:** Has a builder, but stateless — no accounts visible, no team versioning, no AI coaching layer.
- **Mobile:** Web-only as of research date.
- **Threat to founder:** **HIGH.** Pikalytics already owns the data + meta + calc moat AND is shipping fast. If they add accounts + AI, they own the category. The founder's only viable wedge is that *Pikalytics is data-first, not workspace-first*, and there's no sign they're building team versioning, comments, or coaching memory.

### 4. Poképaste — the unkillable primitive
- Solo dev (Felix Phew), open-source (BSD/v3 written in Go), 300K+ pastes (T1: creator's own README + Smogon thread), free, donation-backed.
- Anonymous by design — URLs are cryptographically derived; the creator considered publishing aggregate stats but explicitly *won't* break user anonymity (T1).
- **Threat:** **LOW as a competitor, HIGH as a substrate.** The founder must integrate with Poképaste (import/export) — fighting it is futile; embracing it is table stakes.

### 5. VGCPastes — community curation
- Volunteer-run (Twitter/Discord-driven). Latest counts: 1,150 teams for Reg H, 63 teams for Reg I, 54 teams from 29 creators for Reg G (T1: @VGCPastes posts).
- Effectively a Google Sheet that powers off Poképaste links.
- **Threat:** **LOW.** It's a content source, not a workspace. The founder could ingest these as starter templates.

### 6. Limitless TCG / VGC — owns the tournament rails
- Run by Eddy "Limitless" Cheung & team. Free for players; TO pricing not public.
- Already supports Champions tournaments. Maintains every result + decklist for VGC 2025-26 (T1: limitlessvgc.com, play.limitlesstcg.com).
- **Threat:** **LOW direct, HIGH as a partnership / data source.** They are not a teambuilding workspace. The founder could plug into Limitless's decklist API to feed "tournament-winning teams this week" into their workspace.

### 7. Trainer Tower — content brand + the canonical calc
- 15-person volunteer collective since Nov 2016 (T2: VGCpedia + Liquipedia).
- Damage calc (damagecalc.trainertower.com) is the most-forked VGC calc lineage (8+ public forks on GitHub, including Chinese localization).
- No paid tier. Content cadence is moderate (post-event reports, occasional analysis pieces).
- **Threat:** **LOW.** They have brand and calc but no product engine and no funding; they will not build a workspace.

### 8. Victory Road — content + season hub
- Founded 2015 by Ruben Yanguas + David Olivar. Bilingual ES/EN since 2018.
- Already shipped a Champions Regulations page and 2026 Season Calendar/Structure (T1: victoryroad.pro/champions-regulations, /2026-season-calendar, /2026-season-structure).
- Revenue: ad/sponsorship + creator-economy (Twitch/YT) — *not* a SaaS.
- **Threat:** **LOW.** They make content, not products. Potential partner for distribution.

### 9. Damage calculators — commodity layer
- The `@smogon/calc` engine is open-source and embedded in nearly every third-party tool (Showdex, Pikalytics, ChampDex, Champions Builder, Porygon Labs, Pokébase, etc.).
- Showdex (Chrome extension, 4.7★ avg rating) integrates the calc directly into live Showdown battles — strong product-led growth.
- **Threat:** **LOW as a competitor, MUST-HAVE as a feature.** The founder shouldn't try to out-build a calc; they should embed `@smogon/calc` and focus value above it (workspace, AI, memory).

---

## C. Indirect Competitors

### Generic AI assistants (ChatGPT, Claude, Gemini)
- **Prevalence in 2025-26:** Multiple custom GPTs exist ("Poké Team Builder" by Mark Mandell on chatgpt.com; FlowGPT competitive PKM bots; ai4chat.co/yeschat.ai variants). These have low traction individually but signal that *informal* AI prep usage is normalized in 2026.
- **Why they're a real threat:** Players already paste team text into ChatGPT/Claude and ask "what's this team weak to?" Free, no signup beyond their existing AI sub. The founder's product must beat the *combined* experience of "ChatGPT + Showdown + Pikalytics tabs," not just Showdown alone.
- **Why they lose:** Generic AI hallucinates moves/abilities, doesn't know latest Reg M-A meta, has no calc engine, no persistent team memory.
- **Tier:** T2 (multiple shipped GPTs visible) / T4 (no usage data).

### Discord servers + spreadsheets — the "informal stack"
- 10+ VGC-tagged Discord servers on Discodus alone; "Pokémon Champions" Discord server cited as a notable growing community (T2: Disboard listing). Servers facilitate team-building, EV/IV optimization, Showdown practice rooms, replay sharing, draft leagues.
- Discord+Sheets is *the* prep stack for most active players: a Google Sheet for personal notes, a Discord channel for sharing pastes, a notepad for matchup notes.
- **Threat:** **HIGH and underrated.** This is the actual baseline. A workspace product must replace 3-4 ad-hoc tools at once or it loses to the zero-CAC habit of "just paste in #team-help."

### Creator economy (Wolfey, CybertronVGC, Aaron Zheng)
- **WolfeyVGC:** 2.14M YouTube subscribers (Mar 2026), ~1.25M monthly views, 694M lifetime views, ~1,300 videos (T2: Social Blade / vidiQ / HypeAuditor).
- **CybertronVGC (Aaron Zheng):** ~130K+ subscribers (T3: youtubers.me); 7-time worlds qualifier (T2: Liquipedia).
- They are not building products; they're shaping what players *expect* prep to look like. Their tutorials normalize: "watch a 30-min team explanation video → import the paste → tweak in Showdown."
- **Threat to founder:** **LOW direct, HIGH for distribution.** A creator partnership is the cheapest acquisition channel in VGC (Wolfey's audience alone is ~10× Smogon's monthly visits). Conversely, if a creator shipped their own coach app, they'd dominate overnight (this is essentially what VGCCoach is positioning as).

---

## D. Go-to-Market Analysis (how rivals acquire)

| Competitor | Primary acquisition channel | Why it works | Replicable? |
|---|---|---|---|
| Smogon | Organic SEO on Pokémon names + tiers (45% of traffic) | 20+ years of indexed long-tail content; deep interlinking from forums/articles | **No** for head terms; **Yes** for long-tail Champions-specific queries |
| Pokémon Showdown | Direct (returning users) + word-of-mouth in Discord/Twitter | It's the only full sim; retention via tournaments/ladder | **No** — single-product moat |
| Pikalytics | Organic SEO on "[format] usage stats" / "[Pokémon] usage" + Twitter (@Pikalytics, @VGCdata) | Owns the meta-data SEO niche; Twitter posts data graphs that get reshared | **Partial** — could build "Champions [Pokémon] best partners" long-tail pages |
| Poképaste | Embedded everywhere (every Twitter team share, every Smogon RMT, every Discord) | Network effect — it's the link format | **No** — but *use* it (embed/import) |
| VGCPastes | Twitter (@VGCPastes) — curated team drops after every regional | Active on Twitter where VGC players already live | **Yes** — Twitter is high-leverage for VGC |
| Limitless | Tournament organizers list it on event pages → players land via brackets | Captive audience (you must use it to enter the tournament) | **No** — hard to compete with TO infra |
| Trainer Tower / Victory Road | YouTube + Twitter creator audiences + niche Google ranking for VGC season-info | Authority-built brand | **Slow** — takes years |
| Wolfey / Cybertron / Zheng | YouTube algorithm + Twitch + Twitter | Personality-driven, evergreen tutorial content | **Via partnership only** |
| Discord servers | Word-of-mouth in adjacent Discords + Disboard listings | Zero-friction — already where players hang out | **Yes** — found a Discord *alongside* a workspace product |
| Generic AI (ChatGPT) | Habitual usage; users opportunistically paste teams | Zero CAC for OpenAI; pre-existing daily-active habit | **Yes** — must beat ChatGPT-tab as the path of least resistance |

---

## E. White Space — Unowned Territory

What no one in this matrix currently owns:

1. **Versioned, named team history with notes.** Showdown has a flat list. Poképaste is anonymous + immutable. No one has "v3 of my Calyrex-Shadow team — I swapped Trick Room for Tailwind because of the Indianapolis Reg M-A meta shift; here's why."
2. **AI coaching with *memory of your specific team and your specific gaps*.** VGCCoach and ChampTeamAI score teams or generate teams, but neither (per their public surface) maintains a longitudinal player profile that learns "this player keeps losing to Tailwind teams; suggest a Tailwind-counter slot."
3. **Native iOS/iPadOS app for serious teambuilding.** ChampDex is the only listed iOS native, and it's positioned as a meta-tracker/calc, not a full workspace. Showdown can't ship an iOS app (App Store policy on emulators-adjacent IP). Pikalytics is web-only.
4. **Multiplayer / squad workspace.** No competitor offers shared editing of a team between training partners. Discord+Sheets is the workaround — vulnerable to disruption.
5. **Matchup-prep workflow specifically.** Damage calcs are stateless. No one has "save this matchup analysis against this opponent's archetype, revisit before next regional."
6. **Pokémon Champions-native UX.** Most current builders are Showdown-mental-model retrofits. None deeply use Champions' specific mechanics (cross-platform play, Pokémon Home routing, Mega in Reg M-A) as first-class concepts.

What no one will likely build (don't bother trying to own):
- A better damage-calc engine (commodity; integrate `@smogon/calc`).
- A better tournament platform (Limitless's moat).
- A better paste-sharing primitive (Poképaste is the standard).
- A better content site (Smogon/Victory Road/Trainer Tower own this).
- A better usage-stats site (Pikalytics is too far ahead).

---

## F. Things the founder might be missing entirely

1. **VGCCoach (vgccoach.pro)** — *direct AI-coach competitor already shipped*, claims training on 112K real ladder battles, sub-3-second team grade. Likely the founder's #1 competitive threat. Worth a deep separate audit.
2. **ChampTeamAI (champteamai.com)** — *AI generative team builder for Champions*, also already shipped.
3. **Champions Lab, Champions Builder, Champions Team Builder, ChampDex, Porygon Labs, Pokébase** — six more Champions-specific tools shipped in the first ~30 days post-launch. The land grab is already underway.
4. **Showdex (4.7★ Chrome extension)** — proves players will install browser extensions for analysis; potential *form factor* the founder hasn't considered (extension vs. standalone web app).
5. **`@smogon/calc` open-source engine** — embedding it is table-stakes; trying to write a calc from scratch would be wasted engineering.
6. **The Discord+Sheets baseline** — the real "default" the founder must displace, not Showdown.
7. **iOS App Store policy reality** — Showdown can't ship iOS, but Pokémon Champions is *officially* on iOS in 2026. A third-party Champions companion app *can* live on the App Store as long as it's a teambuilder/analysis tool (ChampDex already proves this). Significant moat opportunity.
8. **Pokémon Home integration** — Champions connects to Pokémon Home; no competitor surveyed has signaled API integration for "import my actual box."
9. **Aggregate damage-roll learning across users** — Pikalytics has aggregate usage. Showdown has aggregate ladder. No one has aggregate *teambuilding decisions* (e.g., "82% of top-cut players run Modest over Timid on Calyrex-Shadow this week" with reasoning notes).

---

## G. Source Index (with tiers)

- **T1 official:** champions.pokemon.com; pokemonshowdown.com/news/175 (server-side team save); pikalytics.com/champions, /team, /calc, /calc-quiz; pokepast.es; @VGCPastes Twitter; victoryroad.pro/champions-regulations; play.limitlesstcg.com; pokemon.com VGC transition announcement (Apr/May 2026); apps.apple.com/ChampDex.
- **T2 third-party measurement:** Similarweb pokemonshowdown.com (Mar 2026); Semrush smogon.com (Jan 2025); Social Blade / vidiQ / HypeAuditor for WolfeyVGC; Wikipedia (Pokémon Showdown, Pokémon Champions, Wolfe Glick); Liquipedia (Cybertron, Victory Road); Nintendo Life coverage of Champions transition (Mar 2026); Game8 Champions release coverage.
- **T3 community-curated:** VGCpedia (Pikalytics, TrainerTower, VictoryRoad entries); Smogon forum threads (RMT 2025, PokePaste programming thread, Showdex thread); Disboard / Discodus VGC server listings; PokeBase Q&A; us.youtubers.me CybertronVGC stats.
- **T4 inferred:** discord+sheets prevalence (anecdotal from forum/disboard signals); AI-tab usage in 2026 (signal: many shipped custom-GPTs but no usage stats published); VGCPastes ownership (Twitter handle only).

