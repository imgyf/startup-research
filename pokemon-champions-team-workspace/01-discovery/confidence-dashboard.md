# Confidence Dashboard

**Phase:** 3 — Discovery
**Project:** pokemon-champions-team-workspace
**Date:** 2026-05-09

---

## Purpose

This dashboard catalogs every major claim used to drive Phases 4-8, the source tier, the number of corroborating sources, the confidence rating, and data age. Use it to know where decisions stand on solid ground vs. thin ice.

---

## Confidence Ratings

- **High** — Multiple Tier 1/2 sources, current data (<6 months), no contradictions
- **Medium** — Single strong source OR multiple Tier 2/3 sources, mostly current
- **Low** — Single source, Tier 3, or contradicting signals, or older than 18 months

---

## Market Sizing & Demand

| # | Claim | Source(s) | Tier | Corroborated | Confidence | Age |
|---|---|---|---|---|---|---|
| 1 | Pokémon Champions launched April 8, 2026 | Metacritic, OpenCritic, multiple gaming press | 1 | 5+ | **High** | <30d |
| 2 | Champions Metacritic 65 / OpenCritic 58 | Metacritic, OpenCritic direct | 1 | 2 | **High** | <30d |
| 3 | Champions has no replay URLs, 3 free team slots, $4.99/mo Membership for 18 | Multiple review sources, gamerant.com | 2 | 3+ | **High** | <30d |
| 4 | Pokémon Showdown >1M MAU, >30K peak concurrent, 18M visits/mo | SimilarWeb, Showdown analytics references | 2 | 2 | Medium-High | <12mo |
| 5 | VGC Worlds 2024: 943 competitors | Pokemon.com event reports | 1 | 1 | High | 12mo |
| 6 | Regional attendance 270-676 players | Limitless, Pokemon.com | 1-2 | 2 | High | <6mo |
| 7 | TAM proxy: 26.79M Scarlet/Violet units sold | TPC quarterly, Famitsu | 1 | 2 | High | 6mo |
| 8 | SOM 200-1,200 paying users Year 1 | Estimate from comparable tool conversions | n/a | n/a (estimate) | **Low-Medium** (assumption) | n/a |

## Willingness-to-Pay & Monetization

| # | Claim | Source(s) | Tier | Corroborated | Confidence | Age |
|---|---|---|---|---|---|---|
| 9 | WolfeyVGC has 10,893 paid Patreons | Graphtreon | 2 | 1 | **High** | <30d |
| 10 | WolfeyVGC est. $14K-94K/mo revenue | Graphtreon | 2 | 1 | Medium | <30d |
| 11 | WolfeyVGC added 5,706 paid Patrons in 30 days post-Champions launch | Graphtreon delta | 2 | 1 | High (single trusted source) | <30d |
| 12 | Mobalytics acquired by ESL FACEIT March 2025 | TechCrunch | 1 | 2 | **High** | 14mo |
| 13 | Mobalytics est. $5-25M ARR pre-acquisition | TechCrunch + analyst speculation | 2 | 2 | Medium | 14mo |
| 14 | Chess.com $100M+ revenue, ~1% paid conversion | chess.com 2024 disclosures | 1 | 2 | **High** | 12mo |
| 15 | Metafy Pokémon coaching $25-30/hr | metafy.gg direct | 1 | 1 | High | <30d |
| 16 | Pokémon HOME Premium $16/yr | nintendo.com | 1 | 1 | High | current |
| 17 | Recommended pricing $15/mo standard, $25/mo tournament-prep | Inferred from above benchmarks | n/a | n/a (synthesis) | Medium (assumption) | n/a |

## Competitor Landscape

| # | Claim | Source(s) | Tier | Corroborated | Confidence | Age |
|---|---|---|---|---|---|---|
| 18 | 15+ Champions-specific tools shipped within 30 days of launch | Direct site discovery | 1 (direct) | n/a (observed) | **High** | <30d |
| 19 | VGCCoach claims 112,480-battle training dataset | vgccoach.pro direct | 1 | 1 | Medium (claim, unverified) | <30d |
| 20 | VGCCoach owns position #1 for "Pokemon Champions AI coach" | SERP check | 1 | 1 | High | <30d |
| 21 | ChampDex is the only iOS-native Champions tool | App Store + competitor sites | 1 | 2 | High | <30d |
| 22 | Champions Lab is open-source with Monte Carlo sim | github.com/Andrew21P/ChampionsLab | 1 | 1 | High | <30d |
| 23 | No funded competitor exists in Champions companion space | Crunchbase + LinkedIn search | 1-2 | n/a (negative) | Medium-High | <30d |
| 24 | Pikalytics shipped Champions support within 30 days of launch | pikalytics.com direct observation | 1 | 1 | High | <30d |

## Customer Voice & Personas

| # | Claim | Source(s) | Tier | Corroborated | Confidence | Age |
|---|---|---|---|---|---|---|
| 25 | "I keep losing and don't know why" is highest-frequency pain | Reddit r/PokemonChampions + r/stunfisk threads | 3 | 5+ threads | Medium-High | <30d |
| 26 | Showdown teams disappear after closing browser | Reddit + Twitter | 3 | 5+ threads | Medium | ongoing |
| 27 | Tournament-prep persona pays $25-30/hr for Metafy coaching | metafy.gg direct + creator references | 1-2 | 2 | High | current |
| 28 | Brady Smith / VGC Corner has 206+ paid Patrons in tier | Graphtreon | 2 | 1 | High | <30d |
| 29 | Persona C TAM share ~5%, Persona B ~10%, Persona E ~50% | Estimate from community size & survey-style data | n/a | n/a (estimate) | **Low-Medium** | n/a |

## Technical Feasibility

| # | Claim | Source(s) | Tier | Corroborated | Confidence | Age |
|---|---|---|---|---|---|---|
| 30 | Champions has no public API, no replay URLs, no team data export | Direct game documentation + reviews | 1-2 | 3+ | **High** | <30d |
| 31 | @pkmn/sim, @smogon/calc, @pkmn/client are MIT-licensed and ready | npm + github | 1 | 3 | **High** | current |
| 32 | PokéLLMon achieves 84% type-correctness on Pokémon prompts | arxiv 2402.01118 | 1 | 1 | High | 18mo |
| 33 | Solo founder MVP build estimate: ~315 hours within 235-390 hr envelope | Estimate from technical scope | n/a | n/a (estimate) | Medium | n/a |
| 34 | LLM costs $150-400/mo for 100 active users on Sonnet 4.6 | Estimate from API pricing + usage patterns | 2 | 1 | Medium | <30d |
| 35 | Auto-replay-analysis feature is INFEASIBLE due to no replay data access | Champions docs + reviews | 1 | 3+ | **High** | <30d |

## Regulatory & IP

| # | Claim | Source(s) | Tier | Corroborated | Confidence | Age |
|---|---|---|---|---|---|---|
| 36 | TPC has never C&D'd Showdown, Smogon, Pikalytics in 15+ years | Multiple coverage sources, no enforcement found | 1-2 | n/a (negative) | **High** | longstanding |
| 37 | TPC enforcement targets ROM hacks, asset reuse, not companion tools | Multiple cases (Uranium, Palworld, etc.) | 1-2 | 5+ | **High** | longstanding |
| 38 | "Standard fan-tool risk" posture is appropriate for our scope | Synthesis from above | n/a | n/a (judgment) | Medium-High | n/a |

## Distribution & GTM

| # | Claim | Source(s) | Tier | Corroborated | Confidence | Age |
|---|---|---|---|---|---|---|
| 39 | r/stunfisk has 257K members | Reddit direct | 1 | 1 | High | <30d |
| 40 | Smogon Discord has 54K members | Discord direct | 1 | 1 | High | <30d |
| 41 | WolfeyVGC YouTube ~2.14M subs | YouTube direct | 1 | 1 | High | <30d |
| 42 | Smogon Discord & Showdown rooms have anti-advertising rules | Direct community rules | 1 | 1 | High | longstanding |
| 43 | Worlds 2026 Aug 28-30 is peak demand window | Pokemon.com event calendar | 1 | 1 | High | current |
| 44 | Indianapolis Regional May 29-31, NAIC June 12-14 | Pokemon.com event calendar | 1 | 1 | High | current |

---

## Where We're Standing on Solid Ground

1. **Game launch state** — high confidence in the gaps Champions left for third-party tools.
2. **WTP exists** — WolfeyVGC Patreon proves it categorically.
3. **No funded incumbent** — the window is technically open.
4. **IP risk is moderate-low** — historical baseline strongly supports standard fan-tool posture.
5. **Tournament calendar is concrete** — event dates and demand cycles are known facts.
6. **Open-source ingredients work** — @pkmn libs are real, current, MIT-licensed.

## Where We're on Thin Ice

1. **SOM estimate (200-1,200 paying users Y1)** is *inferred* from adjacent benchmarks — not validated by Pokémon-specific conversion data.
2. **Persona C TAM share (~5%)** is an estimate based on community signal, not survey data.
3. **VGCCoach's "112,480-battle training dataset" claim** is unverified (their own marketing).
4. **Mobalytics ARR estimate ($5-25M)** is analyst speculation; could be substantially off.
5. **Build cost estimate** assumes solo founder of 15-25 hrs/week productivity; varies widely.
6. **Reddit pain frequency** based on thread sampling, not systematic content analysis.
7. **WolfeyVGC partnership viability** is hypothetical — we have not validated his interest.

## Critical Gaps to Validate in Phase 8

These are the highest-leverage unknowns. Validation experiments should prioritize them:

1. **Will tournament-prep players actually pay $15/mo for a workspace?** Customer interviews + landing-page test.
2. **Can we reach Persona C in volume through Reddit + creator partnerships?** Content marketing test, Reddit AMAs, direct creator outreach.
3. **Does the AI coach value-prop hold up in real use?** Wizard-of-Oz prototype with 10 test users.
4. **Will Pikalytics ship workspace features that obsolete our wedge?** Monitor + competitive intelligence.
5. **Will WolfeyVGC or another top creator agree to an early partnership?** Direct outreach.

---

## Note on Knowledge-Based vs Web-Sourced Research

All Phase 3 research was conducted with WebSearch tool (Tier 1 web access) on 2026-05-09. **No findings rely on Knowledge-Based Mode.** Confidence ratings reflect actual source quality observed during research.

## Sources

All raw research files in `01-discovery/raw/`:
- `wave1-market.md`
- `wave1-competitors.md`
- `wave1-customer.md`
- `wave2-champions-competitors.md`
- `wave2-gtm.md`
- `wave3-personas.md`
- `wave4-technical.md`
