# Industry Trends

**Phase:** 3 — Discovery
**Project:** pokemon-champions-team-workspace
**Date:** 2026-05-09
**Confidence:** Medium-High (macro trends well-documented; Pokémon-specific trends inferred from launch dynamics)

---

## Trend 1 — Esports Companion Tools as a Validated Category

**Signal strength: Strong.**

The market for "second-screen" prep and analytics tools for competitive games crossed a clear inflection in 2024-2025:

- [Data, Tier 1] **Mobalytics acquired by ESL FACEIT Group, March 2025** — first major exit in the category. Estimated $5-25M ARR.
- [Data, Tier 1] **Chess.com surpassed $100M annual revenue** with ~1% paid conversion, validating that prep/learning subscription works even in a "free dominates" community.
- [Data, Tier 2] **op.gg, Blitz.gg, U.GG** continue to ship paid tiers profitably across League of Legends, Valorant, and TFT.

**Implication for Pokémon:** The category playbook is validated in adjacent franchises. Pokémon competitive doesn't need a category to be invented — it needs the playbook applied to its specific tooling gaps. This *reduces* market-creation risk substantially.

**Counter-signal:** [Tier 2] Mobalytics took ~10 years to reach acquisition. The path is real but slow. Solo-founder side-project economics need to be sized for "modest win," not unicorn outcomes.

---

## Trend 2 — LLM-Powered Vertical Coaching Going Mainstream

**Signal strength: Medium-Strong.**

[Data, Tier 1] PokéLLMon (Hu et al., arxiv 2402.01118, 2024) demonstrated that retrieval-augmented LLMs grounded on Pokémon-specific knowledge bases reach 84% type-correctness on competitive Pokémon prompts — a substantial lift over base models. The pattern (LLM + simulator tool calls + structured retrieval) generalizes broadly.

[Tier 2] In 2025-2026, vertical coaching products in chess (Chess.com's GM-tutor features), in fitness (Whoop, Strava AI summaries), and in code review have proven that LLM-grounded coaching that *cites its sources* and *runs real simulations* dramatically outperforms generic ChatGPT-style coaching.

**Implication for Pokémon:** The window for a vertical Pokémon AI coach is open. Generic ChatGPT/Claude get Pokémon mechanics wrong at high rates without grounding (Wave 4 mining shows community is openly mocking generic LLM Pokémon advice). A simulator-grounded, calc-grounded vertical coach has a real edge.

**Counter-signal:** [Tier 3] The community is sensitive to AI hype. Cheap "AI coach" branding without rigor will be called out fast — Persona B (Smogon Veteran) is allergic to it.

---

## Trend 3 — Live-Service Game Companion Tooling Compressed Cycle

**Signal strength: Strong.**

[Data, observed] When *Pokémon Champions* launched April 8, 2026, **15+ companion tools shipped within 30 days**. This is a much faster build cycle than the 12-24 month historic norm in the Pokémon community (e.g., Pikalytics took years to mature).

**Drivers:**
- Modern web stacks (Next.js, Vercel, Cloudflare) reduce time-to-launch for companion tools to under a month.
- LLM-assisted coding accelerates solo-founder velocity 2-3x.
- The audience expectation is "if there's a game, there's a tool tomorrow" — formed by adjacent communities (Mobalytics for LoL, op.gg for Valorant).

**Implication:** First-30-days post-launch was the easy land grab. Now (~30 days post-launch) the differentiation game has begun. **Late entrants that ship by Worlds-prep season (June-Aug 2026) can still win on quality**, but late entrants that miss Worlds-prep slip into a much weaker Sept-Nov environment.

---

## Trend 4 — Creator Economy as Distribution Layer

**Signal strength: Strong.**

[Data, Tier 2] **WolfeyVGC's Patreon added 5,706 paid Patrons in the 30 days following Champions' April 8 launch** — direct evidence that the creator economy converts viewer attention into prep-content WTP at scale.

[Tier 2] In adjacent communities, creator-tool partnerships have become standard:
- Mobalytics × top League streamers (Patreon-tier-locked tool access)
- Chess.com × Hikaru Nakamura, Levy Rozman (Gotham Chess) — co-promotion + tool integrations
- op.gg × Korean pro teams

**Implication:** Creator partnerships are the highest-leverage acquisition channel for Pokémon companion tools. WolfeyVGC, CybertronVGC, Brady Smith / VGC Corner are the top three targets. **A locked-tier deal (free Pro for the creator's top Patreon tier + revshare) is a textbook play.**

---

## Trend 5 — Tournament-Calendar Driven Demand Cycles

**Signal strength: Strong (Pokémon-specific).**

Pokémon competitive has a predictable demand calendar:

| Event | 2026 Date | Effect on tool demand |
|---|---|---|
| Indianapolis Regional | May 29-31 | First post-launch major; high prep spike |
| North America International | June 12-14 | Major demand spike |
| Multiple Regionals (June-July) | Various | Sustained elevated demand |
| **Worlds 2026** | **Aug 28-30** | **Peak demand of the year** |
| Off-season | Sept-Nov | Significant trough |
| Reg H meta announcements | Late 2026 | Demand re-spike on format change |
| Worlds 2027 build-up | Q1-Q2 2027 | Annual cycle repeats |

**Implication:** Build cadence and marketing cadence must align with this calendar. Missing the Worlds-prep window (June-Aug) drops a launch into a trough. Conversely, an MVP that ships meaningful value by July gets the late-Worlds-prep audience for free.

---

## Trend 6 — TPC's Slow Native Tooling Velocity

**Signal strength: Medium.**

The Pokémon Company has a documented pattern of:
- Shipping minimal competitive features at launch
- Iterating on cosmetics and balance, but slowly on workflow features
- Letting the community build the missing infrastructure (Showdown, Smogon, Pikalytics) and tolerating it

[Inference, Tier 3] Champions is more competitive-focused than any prior TPC product, which *might* mean faster native tooling velocity than historical baseline. But the launch state (no replay URLs, 3 free slots, EV/IV lock on import) suggests they haven't broken the pattern.

**Implication:** Plan for TPC to eventually ship a basic team-versioning + cloud-save feature in Champions within 6-12 months. Build moats (AI coaching, longitudinal memory, tournament-prep workflow, Showdown cross-sync) that TPC won't ship as a side feature.

---

## Trend 7 — Mobile Companion Apps Becoming Default Expectation

**Signal strength: Medium.**

ChampDex's iOS-native app within 30 days of launch demonstrates that mobile-native is now an expected category for serious Pokémon tools. Pokémon HOME is mobile-first. Younger competitive players skew mobile-first for non-battle interactions.

**Implication:** Mobile-responsive web is **table stakes for MVP**. Native iOS app is a Year-1 follow-up — not Day-1 scope, but a clear roadmap milestone.

---

## Trend 8 — Free-Tool Cultural Norms Eroding (Slowly)

**Signal strength: Medium.**

The Pokémon competitive community has a deep "free tools" culture (Showdown, Smogon, Pikalytics — all free). But:

- [Data, Tier 2] WolfeyVGC's 10,893 paid Patrons proves the community pays for *content*.
- [Data, Tier 2] Pokémon HOME Premium ($16/yr) has sustained adoption.
- [Tier 2] Metafy 1-1 Pokémon coaching exists at $25-30/hr — the high-end of WTP for prep-related services.

**Implication:** The community pays when value is concentrated in a recognized brand or person, less so for plain SaaS utility. **A workspace tool likely needs creator-brand assistance to monetize at meaningful scale**, or else needs a defensible utility deep enough to overcome the free-tool default. We bake both into the GTM (creator partnerships) and product (cross-format sync, longitudinal memory, AI coaching).

---

## Strategic Implications Summary

| Trend | Implication | Affects which phase |
|---|---|---|
| 1. Esports companion category validated | Reduce market-creation risk; apply playbook | Strategy (Phase 4) |
| 2. LLM vertical coaching window open | AI coach is a real wedge if grounded | Product (Phase 6) |
| 3. Compressed launch-cycle land grab | Speed-to-meaningful-MVP matters; July 2026 deadline | Validation, GTM |
| 4. Creator economy is the distribution layer | Wolfey/Cybertron/Brady partnerships are top priority | GTM (Phase 4) |
| 5. Tournament calendar drives demand | Align build/launch cadence to calendar | All execution phases |
| 6. TPC slow on native tooling | Build moats TPC won't ship | Product, Strategy |
| 7. Mobile is expected | Responsive web at MVP, native iOS Y1 | Product (Phase 6) |
| 8. Free-tool culture | Need brand assist OR defensible utility for paid tier | Strategy, Brand |

---

## Flags

**Red Flags:**
- None.

**Yellow Flags:**
- **Tournament-calendar dependence creates concentration risk.** If the founder misses the July 2026 ship target, the next strong demand window is February-March 2027 (Reg H season ramp). That's a 7-month cold-start risk.
- **Macro trend toward LLM coaching means more entrants will arrive throughout 2026.** Defensibility must come from data + community + workflow — not from "we have an AI."

## Sources

- `01-discovery/raw/wave1-market.md`, `wave2-champions-competitors.md`, `wave2-gtm.md`, `wave3-personas.md`, `wave4-technical.md` — full source detail with URLs
- TechCrunch — Mobalytics acquisition coverage (Tier 1)
- arxiv 2402.01118 — PokéLLMon paper (Tier 1)
- Chess.com 2024 financials (Tier 1)
- WolfeyVGC Patreon, Graphtreon (Tier 2)
- Pokemon.com event calendar 2026 (Tier 1)
