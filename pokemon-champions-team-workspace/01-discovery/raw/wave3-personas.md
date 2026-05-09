# Wave 3: Persona Segmentation — Pokémon Champions Workspace

**Research date:** 2026-05-09
**Method:** 8 web searches across Reddit, Smogon forums, Patreon, Metafy, Discord listings, GameFAQs, content creator audiences, and editorial coverage of Champions launch
**Goal:** Convert the binary "casual vs. competitive" framing into actionable, channel-mapped personas with WTP differentiation, and recommend a launch target.

---

## Cross-cutting demographic baseline

Anchor numbers used to size personas:

- **Pokémon player base average age:** 32 (Japanese consumer study cited by TheGamer); Nintendo's broader player base skews 20–30. Competitive Pokémon skews older still — VGC content creator audiences (WolfeyVGC 1M+ YT subs, CybertronVGC 232k) read as adults with disposable income.
- **r/stunfisk:** 257k subscribers — the dominant competitive subreddit (covers Smogon + VGC).
- **Pokémon Showdown:** 1M+ MAU (Wave 1 finding); the largest free competitive funnel.
- **Champions launch (Apr 8, 2026):** Metacritic 65; ships with 3 free team slots (15 paywalled), no in-game replay, no match history, no versioning. Reddit/Nintendo Life headline: "Feels like a fleshed-out beta." Devs publicly apologized for launch issues.
- **Co-purchased services already in wallet:** Patreon (WolfeyVGC, OsirusVGC, VGC Corner), Metafy ($25–30/hr 1:1 coaching, 4-week structured plans), Pokémon HOME ($16/yr), Discord Nitro, Switch Online. WTP for Pokémon-adjacent SaaS is **proven, not hypothetical**.
- **Geographic mix:** US-heavy English market, with material EU (esp. UK/Germany/Spain/Italy from Regional circuit) and Japan (separate ecosystem, less likely launch target). LatAm growing via Discord.
- **Device mix:** Switch / Switch 2 primary + secondary screen. Pikalytics, Trainer Tower, and Showdex are all laptop/desktop-first; mobile damage calc apps exist but adoption is split. **Assume desktop-primary, mobile-secondary** for serious prep.
- **Time of day patterns:** Pre-tournament weekends (Regionals are Sat–Sun); ladder reset cycles drive late-month surges. Evenings 7pm–midnight local time dominate ladder traffic.

---

## Persona A — "Bricked Champions Casual"

**% of TAM:** ~50–55% of total Champions ranked players, ~30–35% of *tool-buyer* TAM (most won't pay). The most numerous, but pricing-sensitive.

**Signal:** Operation Sports, TheGamer, and Game8 all run "what Champions doesn't tell you" articles. Reddit/GameFAQs threads about replay feature, team slot paywall, and Hisuian Zoroark confusion are top-voted. Editorial: "you don't lose because your team is bad; you lose because you don't know the matchup yet."

**Pain hierarchy:**
1. "I keep losing and don't know why" (no replay, no match history)
2. Only 3 free team slots; can't experiment
3. Doesn't know which loss is bad luck vs. bad play vs. bad teambuilding
4. Doesn't know the meta vocabulary (Trick Room, redirection, speed control)

**JTBD:** "When I lose 4 ladder games in a row in Champions, I want to know whether my team is broken or my decisions are broken, so I can stop ladder-tilting and actually climb."

**Channels:** r/PokemonChampions, r/stunfisk crossposts, GameFAQs Champions board, casual Discord servers, YouTube comment sections on Wolfey/Cybertron videos. **Not** Smogon forums (too intimidating).

**WTP:** **$0–5/mo.** This persona converts best on free tier with very visible upgrade triggers ("save more than 3 teams," "see your full match history"). Whales here are rare; volume strategy.

**Top 3 features they'd use:**
1. Unlimited team slots (#1 paywall pain — directly translates Nintendo's $-trigger)
2. "Why did I lose?" automated post-game explanation in plain English
3. Beginner archetype library ("Trick Room for dummies," "What is redirection")

**Churn triggers:** Stops losing (graduates to B/D), or quits Champions entirely (~30–40% likely within 6 months given Metacritic 65). Also churns if tool feels "too sweaty."

---

## Persona B — "Smogon Veteran Crossing Over"

**% of TAM:** ~10–15% of tool-buyer TAM. Smaller count, very high engagement and WTP.

**Signal:** Smogon forums "Pokémon Champions — releasing April 8, 2026" thread is multi-page, meta-analytical. Showdex (auto-updating damage calc embedded in Showdown) has cult adoption. Smogon stats infra (pkmn/smogon, asanrom) is run by power users. National Dex player surveys exist but no public age data.

**Pain hierarchy:**
1. Champions has *worse* tooling than Showdown (no replay, fewer slots, no robust teambuilder export)
2. Workflow split: builds on Showdown, has to re-enter on Champions
3. Showdown teams not saving (cookie storage bug — Wave 1 confirmed pain, server-side `/teams` is workaround but not adopted by all)
4. Wants to track meta shifts across both platforms simultaneously

**JTBD:** "When I build a team for Smogon OU/VGC ladder, I want to also test it on Champions ranked without re-entering everything, so my prep effort compounds across both ecosystems."

**Channels:** Smogon forums (esp. Stadium / SS OU / VGC subforums), r/stunfisk, Showdown chat rooms, X (formerly Twitter) competitive Pokémon network, GitHub (smogon/damage-calc, pkmn org).

**WTP:** **$8–15/mo.** Already pays Patreons. Will pay for cross-platform sync, advanced calc, replay parsing. Sensitive to "is this rigorous?" — won't tolerate hand-wavy AI.

**Top 3 features they'd use:**
1. Showdown ↔ Champions team sync + format conversion
2. Replay parser that extracts decision-tree analysis (since Champions has no native replay, this means clip-from-VOD or screen-grab)
3. Advanced damage calc + EV/SP optimizer that beats Showdex's UX

**Churn triggers:** If product feels "AI slop" or unrigorous; if Smogon adds first-party Champions support; if calc accuracy is wrong even once.

---

## Persona C — "VGC Tournament Aspirant"

**% of TAM:** ~8–12% of tool-buyer TAM. Smallest count, deepest pockets, shortest sales cycle.

**Signal:** Trainer Tower, Victory Road, Pikalytics, VGC Helper, Limitless VGC, VGCStats — entire infrastructure built for this person. Play! Pokémon transitioned VGC to Champions Apr–May 2026 (officially the ranked competitive platform now). Active Discord servers (Pokémon Champions VGC Discord ~451 members in first 4 months — small but quality, growing). Pre-Regional weekends are peak tool traffic.

**Pain hierarchy:**
1. Need to ingest Pikalytics meta data, build counter-teams, test on Showdown, then port to Champions — manual workflow
2. No replay = can't review tournament losses (huge regression vs. previous gens that had replay codes)
3. Need to track multiple teams across regulation sets (M-A now, future rotations)
4. Pre-tournament prep is high-stress, time-boxed (Sat–Sun events)

**JTBD:** "When I'm prepping for a Regional 10 days out, I want a single workspace that holds my candidate teams, the current meta usage data, my practice match notes, and counter-team analysis, so I can show up confident instead of frantic."

**Channels:** Trainer Tower, Victory Road, Pikalytics user base, VGC-specific Discords, Limitless tournament organizers, X comp Pokémon Twitter, Patreons (Wolfey, Osirus, VGC Corner — Brady Smith's Patreon shows 206 paying members at multi-year track record), Metafy ($25–30/hr coaching).

**WTP:** **$15–25/mo, or $50–100/event** for tournament-prep mode. Highly elastic upward for proven ROI ("got me to Day 2 of Regionals"). Already paying Metafy + 2-3 Patreons + travel costs.

**Top 3 features they'd use:**
1. Tournament prep mode: meta snapshot + candidate team comparison + matchup matrix
2. Match notes + decision-log replay (manual or screen-recorded since no native replay)
3. Team versioning with diff view ("what changed between v3 and v7?")

**Churn triggers:** Bad Regional weekend (will blame the tool); tool fails right before event; doesn't qualify for Worlds and quits VGC.

---

## Persona D — "Returning Lapsed Player"

**% of TAM:** ~10–15% of tool-buyer TAM. Re-activated by Champions launch + IV/EV removal lowering the on-ramp.

**Signal:** Champions removed IVs entirely (all 31), replaced EVs with Stat Points — explicitly framed in coverage as "lowering the gatekeeping mechanics." Special Roster (31 mons vs 229 full) marketed as on-ramp. Editorial coverage emphasizes "if you stopped playing in Gen 6/7, the breeding wall is gone." Reddit/r/PokemonChampions has heavy "hadn't played since Sun/Moon" threads.

**Pain hierarchy:**
1. Meta vocabulary has changed (Tera, Paradox mons, regulation sets are new concepts post-Gen 7)
2. Build muscle memory for team-building is rusty
3. Doesn't know who the current creator authorities are (last knew Aaron Zheng, may not know newer voices)
4. Has more disposable income than 10 years ago (now in 30s with jobs)

**JTBD:** "When I come back to competitive Pokémon after 5+ years away, I want a guided 'what's changed since Gen 7' onboarding plus a team I can trust, so I can start having fun on ladder this weekend, not three weekends from now."

**Channels:** YouTube (Wolfey/Cybertron meta primer videos), r/PokemonChampions, casual Discords. Re-enters via passive content consumption first, then active tools.

**WTP:** **$5–10/mo.** Adult disposable income, but lower engagement frequency than C; converts on "structured comeback" framing.

**Top 3 features they'd use:**
1. "Catch me up: what's changed since Gen 7" curriculum
2. Pre-built rental teams with explanations of *why* each pick
3. Match history with annotated turns ("this is a Tera trick — here's how to spot it")

**Churn triggers:** Falls back out of the hobby (lifecycle); gets discouraged after 2-3 weeks of grinding back to old skill level.

---

## Persona E — "Casual Favorite-Builder"

**% of TAM:** Largest player count (~30–40% of *all Champions players*), but **<5% of tool-buyer TAM**. Largest TAM, lowest WTP — generally NOT the buyer.

**Signal:** TheGamer "Champions Fails Both Hardcore and Casual," Pokémon Forums casual rants, TVTropes Casual-Competitive Conflict. Quote: "wants to run a team they love without optimized teams destroying their experience." Champions has no PvE mode; this segment is currently uncatered.

**Pain hierarchy:**
1. Wants to use Charizard / their starter / their childhood favorite, gets stomped
2. Doesn't speak tier language (S/A/B), finds Smogon culture alienating
3. Casual mode has no skill-based matchmaking
4. Doesn't think of themselves as needing a "tool"

**JTBD:** "When I bring my favorite Pokémon to ranked and lose, I want to find ways to make my favorites work, so I don't have to abandon my identity to play this game."

**Channels:** Pokémon subreddits (r/pokemon, r/PokemonChampions but not r/stunfisk), Pokémon Forums, YouTube casual content, TikTok Pokémon clips. **Almost never** Smogon or VGC Discords.

**WTP:** **$0–3/mo** if anything. Mostly free-tier user; converts on cosmetic / identity framing not analytical framing.

**Top 3 features they'd use:**
1. "Make my favorite work" — auto-build the most viable shell around any chosen Pokémon
2. "Will I have fun" matchmaking-style guidance (avoid the OHKO experience)
3. Lore/identity content (move flavor, why Garchomp is good, stories)

**Churn triggers:** Realizes their favorite genuinely can't compete; quits ranked; goes back to PvE games.

**Strategic note:** This is the persona to *acquire for free, not target with paid tier*. They drive top-of-funnel SEO traffic and word-of-mouth. Using them as the launch persona would be a mistake — they don't pay and they don't have urgency.

---

## Persona F — "Coach Buyer"

**% of TAM:** ~1–2% of tool-buyer TAM. Tiny, ultra-high LTV.

**Signal:** Metafy 1:1 sessions $25–30/hr; structured 4-week plans (8 sessions = $200–500). VGC Corner Patreon shows ~206 paying members at established creators. Wolfey/Osirus Patreons have multi-tier paid memberships. This person is already spending $50–500/mo on human guidance.

**Pain hierarchy:**
1. Coach availability — coaches sell out, especially pre-Regional
2. Coach session prep — wants to come prepared with team data, replay annotations
3. Coach session retention — wants to retain notes/lessons across sessions

**JTBD:** "When my coach and I review my last tournament, I want my replays and notes pre-organized so I don't waste 20 minutes of my $30 hour setting context."

**Channels:** Metafy directly, coach-specific Patreons, VGC Discord coach-channels, X DMs.

**WTP:** **$20–50/mo** in addition to coaching spend. Spending elasticity is high because this is already an "investment in performance" mindset.

**Top 3 features they'd use:**
1. Coach-shareable workspace (export team + replays + notes to coach)
2. Pre-session prep template
3. Lesson library (what we worked on, retention)

**Churn triggers:** Drops coach (rare); finds in-person training group instead.

**Strategic note:** Tiny segment, but **pairs perfectly with C** — most Coach Buyers ARE Tournament Aspirants. Build for C and F naturally satisfies.

---

## Persona G — "Content Creator / Streamer"

**% of TAM:** ~0.5–1% of tool-buyer TAM. Tiny direct revenue, **massive distribution multiplier**.

**Signal:** Active streamer overlay tools (Cobold's overlay, Pokemon-Stream-Tool, pkmn.gg stream tools, Readek's GitHub) — proven category. WolfeyVGC 1M+ YT subs, CybertronVGC 232k. Wolfey's Patreon 10,893 paying members at $5–10/mo (Wave 1 — confirms aggregate creator-economy spend). Stream-tool ecosystem is currently fragmented and ugly.

**Pain hierarchy:**
1. Stream overlay tools are clunky, often Windows-only, manual
2. Wants to show team, sets, damage calcs live without alt-tabbing
3. Wants to share builds with audience seamlessly
4. Wants creator-attributable content (their builds, tracked usage)

**JTBD:** "When I stream Champions ladder, I want my workspace, team display, damage calc, and audience build-share to all run from one tool, so I look polished and my audience can actually copy what I'm doing."

**Channels:** Twitch, YouTube, X, creator Discords. Reached via creator-program outreach, not paid acquisition.

**WTP:** **Free in exchange for visibility, OR $20–50/mo for "creator pro."** Direct revenue minor; influence outsized.

**Top 3 features they'd use:**
1. Stream-ready overlay (OBS browser source) that mirrors their team/notes
2. "Share build to chat" one-click with QR/code
3. Creator analytics (which builds the audience copied)

**Churn triggers:** Tool gets unreliable on stream (one mid-stream crash kills it); a competitor offers a cleaner overlay.

**Strategic note:** Critical for distribution. Free creator tier should be in MVP scope, even if monetization is deferred.

---

## Buying behavior signals (cross-persona)

**Trigger moments — when do players reach for tools?**
- **Pre-Regional weekends** (Sat-Sun events) — peaks Mon–Fri before. C, F, B.
- **Mid-month meta shifts** (new Pikalytics data, balance patches) — A, B, C.
- **Loss streaks** — A, D, E.
- **Ladder reset / season start** — all personas, especially A.
- **Champions feature gap moments** — every time a player hits the 3-team-slot wall, that's a trigger.

**Decision criteria — what makes them try a tool?**
- Creator endorsement (Wolfey/Cybertron/Osirus) — strongest signal across all paying personas
- Reddit thread (r/stunfisk, r/PokemonChampions) — strongest for B, A, D
- SEO ("Pokemon Champions team builder," "why did I lose Champions") — A, D, E
- Discord word-of-mouth — C, F
- "It works with Showdown" claim — B, C

**Conversion-from-free triggers:**
- Hit the 3-slot Champions wall (A) → unlimited slots upgrade
- Lost a tournament that could have been won with better prep (C) → tournament mode upgrade
- Coach asked "do you have your replays?" (F) → workspace export upgrade
- Got humiliated on ladder and want to know why (A, D) → "explain my loss" pro feature

**Retention/churn triggers:**
- Lifecycle exits: Champions itself losing players (A, D, E most exposed)
- Better free alternative emerging from Smogon-org (B is the biggest risk)
- One bad mid-tournament moment (C, G — high stakes)
- Meta stagnation killing engagement (all personas)

---

## The "First 100 Customers" Question

**Fastest to convert in 90 days:** **Persona C (VGC Tournament Aspirant).**
- Already paying Patreons + Metafy; have established WTP behavior
- Have urgent, calendar-driven need (Regionals every 6–8 weeks)
- Concentrated in 5–10 Discords + Trainer Tower / Victory Road readership = reachable
- Will adopt a tool that *measurably* helps their prep workflow

**Highest LTV:** **Persona F (Coach Buyer)** in absolute terms, but they overlap heavily with C. **Effective answer: C-with-F-overlap.** Treat F-features (coach-share, lesson retention) as upsell within C tier.

**Best word-of-mouth multiplier:** **Persona G (Content Creator)** — 1 streamer with 50k followers > 1,000 paid users for top-of-funnel.

**Are these the same person?** Mostly. C, F, G overlap in ~40–60% of cases (the same VGC tournament aspirant who pays for coaching is also the person small-streaming on Twitch). The convergence is real and design-able.

---

## RECOMMENDED LAUNCH TARGETS

### Primary Launch Persona: **C — VGC Tournament Aspirant**

**Why:**
1. **Proven WTP** — already paying $25–30/hr coaching + multi-Patreons. The wallet is open.
2. **Reachable** — concentrated in Trainer Tower / Victory Road / Pikalytics / VGC Discords. <10 distribution channels cover 80% of them.
3. **Urgent JTBD** — calendar-driven Regional prep, not vague self-improvement.
4. **Best evangelists** — when they win, they post about their tools (organic Pikalytics-style growth).
5. **Forces feature rigor** — building for C means accuracy, versioning, replay-handling that benefits everyone downstream.
6. **Champions-specific gap is acute** — no replay + no versioning + 3 slots is *most painful* for the prep-heavy aspirant.

**Initial pricing test:** $15/mo standard, $25/mo "pro/tournament prep mode." Annual discount.

### Secondary Target: **B — Smogon Veteran Crossing Over**

**Why:**
- They will *evaluate* the tool with the most rigor and become the credibility signal on r/stunfisk and Smogon.
- Cross-platform (Showdown↔Champions) sync is a moat feature only achievable by serving B properly.
- Their endorsement converts D and skeptical C buyers.
- Build for B's rigor standard, charge them slightly less than C ($8–12/mo), use them as case studies and beta testers.

### Persona to EXPLICITLY NOT CHASE at launch: **E — Casual Favorite-Builder**

**Why not:**
1. **WTP is near zero.** They will use a free tier and rarely upgrade. CAC will exceed LTV.
2. **No urgency.** They don't have a Regional next weekend. They have a vague feeling of frustration.
3. **Feature requests pull product away from rigor.** "Make Charizard work" features are at odds with the data-rigor needs of C and B, and force product toward "vibes" away from "performance."
4. **They're the largest TAM, which is seductive.** Going broad-first kills startup focus.
5. **Capture them later, free-tier, via SEO** — they will arrive organically once C/B are evangelizing. Don't *target* them; *welcome* them when they show up.

**Acquisition order:** C → B → G (creator partnerships) → F (upsell from C) → D (catch-up curriculum once core tool is mature) → A (free-tier inbound) → E (free-tier inbound, never paid focus).

---

## Sources

- [Pokémon Champions Beginner Guide 2026 — DTGRE](https://www.dtgre.com/2026/04/pokemon-champions-beginner-guide-pvp-meta-teams.html)
- [Pokemon Champions Tips: Master the Competitive Ladder 2026](https://www.pokemonchampions.wiki/guide/Pokemon-Champions-tips)
- ["Feels Like A Fleshed Out Beta" — Nintendo Life](https://www.nintendolife.com/news/2026/04/feels-like-a-fleshed-out-beta-fans-are-unhappy-with-pokemon-champions-at-launch)
- [The Pokémon Champions Backlash — Kotaku](https://kotaku.com/pokemon-champions-backlash-reaction-response-switch-2000691772)
- [Pokemon Champions Has No IVs: Competitive Player's Guide 2026](https://genpkm.com/blog/pokemon-champions-no-ivs-stat-points-competitive-guide-2026)
- [Pokémon Champions: What The Game Doesn't Tell Casual Players — Operation Sports](https://www.operationsports.com/pokemon-champions-what-the-game-doesnt-tell-casual-players/)
- [Pokemon Champions Fails Both Hardcore And Casual Players — TheGamer](https://www.thegamer.com/pokemon-champions-dead-on-arrival-competitive-vs-casual/)
- [Pokémon Champions Guide: How to Get More Free Team Slots — GAMES.GG](https://games.gg/pokemon-champions/guides/pokemon-champions-how-to-get-more-free-team-slots/)
- [Do you think this game will ever receive a replay feature? — GameFAQs](https://gamefaqs.gamespot.com/boards/517117-pokemon-champions-81134751)
- [More team slots in Pokemon Champions — Pokémon Forums](https://community.pokemon.com/en-us/discussion/23896/more-team-slots-in-pokemon-champions)
- [Play! Pokémon Competitions Transition to Pokémon Champions — Pokemon.com](https://www.pokemon.com/us/pokemon-news/play-pokemon-competitions-transition-to-pokemon-champions-on-april-and-may-2026)
- [Resources for Pokémon VGC — Victory Road](https://victoryroad.pro/resources/)
- [Trainer Tower — Resource Hub](https://www.trainertower.com/resource-hub/)
- [Pikalytics — VGC 2026 Pokemon Champions Competitive Stats](https://www.pikalytics.com/)
- [Showdex — Auto-Updating Damage Calculator Built into Showdown! — Smogon Forums](https://www.smogon.com/forums/threads/showdex-an-auto-updating-damage-calculator-built-into-showdown.3707265/)
- [Smogon damage-calc — GitHub](https://github.com/smogon/damage-calc)
- [pkmn/smogon — GitHub](https://github.com/pkmn/smogon)
- [Showdown — Teams Lost (Not A Bug) — Smogon Forums](https://www.smogon.com/forums/threads/teams-lost.3752384/)
- [Showdown Desktop App not saving Teams — GitHub Issue #4850](https://github.com/smogon/pokemon-showdown/issues/4850)
- [Frequently Asked Questions — Pokémon Showdown](https://pokemonshowdown.com/pages/faq)
- [Metafy — Pokémon Scarlet and Violet Sessions](https://metafy.gg/pokemon-scarlet-and-violet/sessions)
- [Metafy — VGC Coaching ($25/hr session)](https://metafy.gg/@ammodee/sessions/vgc-coaching-qAjKzwMIKUt)
- [Metafy — Comprehensive VGC Mastery Program](https://metafy.gg/@relicsongrickstar-/sessions/comprehensive-vgc-mastery-program-8BOPF3UcJHs)
- [WolfeyVGC Patreon](https://www.patreon.com/WolfeyVGC/membership)
- [OsirusVGC Patreon](https://www.patreon.com/OsirusStudios)
- [VGC Corner — Brady Smith Patreon (206 members)](https://www.patreon.com/vgccorner/about)
- [Wolfe Glick — Wikipedia](https://en.wikipedia.org/wiki/Wolfe_Glick)
- [Aaron "Cybertron" Zheng — Liquipedia](https://liquipedia.net/pokemon/Cybertron)
- [r/stunfisk Subreddit Stats — 257k subscribers](https://subredditstats.com/r/stunfisk)
- [Pokémon Champions Discord — CommunityOne (~451 members)](https://communityone.io/servers/1457350549216432295/pokemon-champions-vgc/)
- [Japanese study average player ages — TheGamer](https://www.thegamer.com/japanese-survey-study-results-average-age-final-fantasy-mario-pokemon/)
- [VGC Helper](https://vgchelper.com/)
- [VGC MultiCalc](https://vgcmulticalc.com/)
- [Pokemon Team Stream Overlay — Cobold](https://coboldthefox.itch.io/pokemon-team-stream-overlay)
- [Pokemon Stream Tool — Readek GitHub](https://github.com/Readek/Pokemon-Stream-Tool)
- [pkmn.gg Stream Tools](https://www.pkmn.gg/stream-tools)
- [Casual-Competitive Conflict — TV Tropes](https://tvtropes.org/pmwiki/pmwiki.php/Main/CasualCompetitiveConflict)
- [Just another casual player rant — Pokémon Forums](https://community.pokemon.com/en-us/discussion/7687/just-another-casual-player-rant-about-this-game-thats-getting-worse-every-day)
- [What is a "good" ladder rating? — VGC guide](https://www.vgcguide.com/what-is-a-good-ladder-rating)
- [Pokémon VGC Competitions Officially Transition To Champions — Nintendo Life](https://www.nintendolife.com/news/2026/03/pokemon-vgc-competitions-officially-transition-to-pokemon-champions)
- [Smogon Forums — Pokémon Champions thread](https://www.smogon.com/forums/threads/pok%C3%A9mon-champions-releasing-april-8-2026.3779617/page-5)
