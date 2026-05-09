# Lean Canvas

**Phase:** 4 — Strategy
**Project:** pokemon-champions-team-workspace
**Date:** 2026-05-09
**Confidence:** Medium-High (each cell traceable to Phase 3 research; assumptions explicitly labeled)

---

## Working Title

**Champion's Notebook** *(working name; brand work in Phase 5)*

A persistent prep workspace + grounded AI coach for serious *Pokémon Champions* competitive players.

---

## Lean Canvas

### 1. Problem (Top 3)

1. **Tool fragmentation under tournament pressure.** Serious players have teams in Showdown, notes in Discord, pastes in Google Docs, and screenshots on their phone — and lose hours of prep to context-switching before each Regional. *(Source: `target-audience.md` JTBD; verbatim Reddit pains)*
2. **Champions' broken save/version model.** 3 free team slots, $4.99/mo for 18 slots, no version history, EV/IV lock on import. Native game makes serious team iteration painful. *(Source: `market-analysis.md`)*
3. **Matchup uncertainty without explanation.** Players know they keep losing to rain/stall/setup but can't pinpoint *why*. Existing tools deliver data, not coaching. *(Source: `target-audience.md`, verbatim quote: "I keep losing and don't know why")*

### 2. Customer Segments

- **Primary:** **VGC Tournament Aspirant** — competitive ladder players preparing for Regionals/Internationals/Worlds; ages 19-32; US/CA/UK/EU; already paying for creator Patreons + Pokémon HOME Premium; 6-8 week prep cadence around tournaments.
- **Secondary:** **Smogon Veteran Crossing Over** — long-time Showdown ladder players also playing Champions; rigorous evaluators whose endorsement on r/stunfisk drives credibility.
- **Free-tier inbound only:** **Casual Favorite-Builder** — never paid acquisition; serves as SEO entry point and conversion funnel.

[See `target-audience.md` for full persona detail.]

### 3. Unique Value Proposition

> **The prep workspace serious VGC players actually use between tournaments — your teams, your matchup notes, your improvement journal, and an AI coach that knows your last 50 games. Built on the same simulator pros trust.**

High-concept pitch:

> ***Notion + Strava + a grounded AI coach — for competitive Pokémon.***

### 4. Solution

A web-based workspace (mobile-responsive at MVP, native iOS as Year-1 follow-up) with five core capabilities:

1. **Versioned team workspace** — save unlimited teams, branch/diff versions, tag teams ("for Indianapolis," "vs. rain decks"), with one-click Showdown packed-format import/export and Poképaste link generation.
2. **AI matchup coach** — grounded on @pkmn/sim + @smogon/calc + Smogon usage stats. Explains matchups in plain English, cites sources, refuses to bluff.
3. **Manual match journaling** — structured reflection prompts after a battle (no replay required). AI synthesizes patterns across N games.
4. **Tournament-prep mode** — calendar-aware: pulls Regional usage data into prep, helps build counter-cores, scouts likely opponent archetypes.
5. **Sharing & coach-mode** — share a team with a training partner or paid coach; collaborative read/comment on team versions.

### 5. Channels

**Launch (months 1-3):**
- Reddit organic on r/stunfisk and r/PokemonChampions (participate-first, content marketing)
- Direct creator partnership outreach: WolfeyVGC, CybertronVGC, Brady Smith / VGC Corner (Patreon-tier-locked Pro access + revshare)
- Pokémon Champions VGC Discord (~5K+, value-first participation)
- Founder content: weekly tournament-prep walkthroughs on YouTube/X

**Scale (months 4-12):**
- Programmatic SEO on archetype prep pages ("Reg G rain counter," "Indianapolis meta projections")
- Tournament sponsorship — Limitless community Champions tournaments
- Partnership with Smogon RMT mods (advisor program)
- Affiliate / creator marketplace for content packs

**Year 2:**
- Spanish localization via Victory Road partnership (Latam VGC)
- Native iOS app
- Eventual Japanese-market entry

[See `02-strategy/go-to-market.md` for full GTM playbook.]

### 6. Revenue Streams

| Tier | Price | Includes |
|---|---|---|
| **Free** | $0 | 5 saved teams, basic AI Q&A (10/day), Showdown import/export, public team pages, no version history beyond current |
| **Pro** | **$12/mo or $99/yr** | Unlimited teams, full version history, 100 AI coach turns/day, manual journaling + pattern synthesis, archetype matchup tags, tournament-prep mode (basic) |
| **Tournament Prep** | **$25/mo or $199/yr** | Everything in Pro + meta projection from recent regional data, counter-team builder, opponent scouting, 1-1 coach-mode sharing, priority support, early-access features |

**Future revenue lines (Year 2+):**
- Creator content marketplace (rev-share with named players publishing team packs)
- Team / club workspaces ($X/mo per seat for training-partner squads)
- API access for tournament organizers / content sites

### 7. Cost Structure

**Fixed monthly:**
- Hosting (Cloudflare/Vercel): $20-50
- Database (Supabase or similar): $25-50
- Domain + email + auth (Supabase Auth or Clerk): $25-50
- Marketing budget (early): $100-300/mo

**Variable monthly:**
- LLM API costs (Sonnet 4.6 with smart routing): $150-400 per 100 active paid users
- Email (Resend): $20-50

**One-time:**
- Founder time at 15-25 hrs/wk × 6 months MVP build = ~315-625 hours (opportunity cost only — no salary)
- Logo / brand design: $300-1,500
- Legal review of TOS / terms: $300-800

**Total monthly burn at launch: ~$200-500/month. Total at 100 paid users: ~$500-900/month.**

[See `05-financial/cost-structure.md` for detail.]

### 8. Key Metrics

**North Star:** **Weekly Active Paid Users (WAP)**

Why: Tournament prep is a *recurring* workflow. Daily active is irrelevant; monthly active hides drop-offs. WAP captures the "do they come back this week" loop that determines retention.

**Activation:** % of new free signups who save 2+ teams within 7 days
**Conversion:** Free → paid within 30 days
**Retention:** Month-2 paid retention (after first tournament cycle)
**Engagement:** Avg AI coach turns / paid user / week
**Quality:** AI hallucination rate (sampled audit; target <5% on Pokémon-specific facts)
**Revenue:** MRR, ARPU, churn

### 9. Unfair Advantage

[Honest assessment — this is the weakest cell on the canvas]

**What we have:**
- Open-source ingredients (@pkmn/sim, @smogon/calc, Showdown packed format) make the technical build feasible and cheap.
- Live-game gap awareness — Champions' specific limitations are clear and not changing tomorrow.
- LLM-coding velocity advantage that the broader incumbent set (Smogon, Pikalytics — volunteer / single-operator) lacks.

**What we lack and must address:**
- **Founder is hobbyist, not tournament-tier.** Persona C will sniff this out. **Mitigation: recruit a competitive-player advisor with name recognition before launch.** This is treated as a non-negotiable Phase 8 Week-1 task.
- **No creator partnership locked yet.** Mitigation: outreach to WolfeyVGC + 4 alternates in Week 1-2.
- **No data moat at launch.** Becomes a moat over time as the AI coach accumulates anonymized matchup patterns from paying users — but this is a flywheel, not a starting position.

[Yellow Flag] The unfair advantage is *thin at launch*. The strategy depends on building it through advisor partnership + creator deal + accumulated coaching data over the first 6 months. If those three don't compound, the moat doesn't form.

---

## Lean Canvas Risk Heat Map

| Cell | Confidence in our framing | Biggest risk |
|---|---|---|
| Problem | **High** | None |
| Customer Segments | **Medium-High** | TAM share % is estimated |
| UVP | **Medium** | "AI coach" is crowded; positioning must be sharper than the headline |
| Solution | **High** | None — feasibility validated |
| Channels | **Medium** | Creator partnership unvalidated |
| Revenue Streams | **Medium** | $25/mo tier WTP is inferred from Metafy + Patreon, not validated |
| Cost Structure | **High** | None |
| Key Metrics | **High** | None |
| **Unfair Advantage** | **Low** | Thin at launch — depends on flywheels forming |

---

## Flags

**Red Flags:**
- None.

**Yellow Flags:**
- Unfair Advantage is the weakest cell. The strategy is "build it as we go" via advisor + creator + data flywheel. If any of those don't materialize, defensibility erodes.
- $25/mo Tournament Prep tier WTP is inferred, not validated. Phase 8 must include a direct pricing test in Week 2-3.
- The Lean Canvas assumes the three Pivots from Phase 3.5 are accepted (tournament-prep primary, manual journaling, premium pricing). If any are reverted, the canvas collapses.

## Sources

- `01-discovery/research-gate.md` — three-pivot decision
- `01-discovery/market-analysis.md` — WTP benchmarks, market sizing
- `01-discovery/competitor-landscape.md` — positioning gaps
- `01-discovery/target-audience.md` — persona JTBDs
- `01-discovery/raw/wave4-technical.md` — feasibility constraints
