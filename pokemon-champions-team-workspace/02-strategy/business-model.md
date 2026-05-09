# Business Model

**Phase:** 4 — Strategy
**Project:** pokemon-champions-team-workspace
**Date:** 2026-05-09
**Confidence:** Medium (pricing benchmarks strong; conversion + churn assumptions need validation)

---

## Model Type

**Freemium SaaS.** Three-tier vertical:

| Tier | Price (monthly) | Price (annual) | Annual Discount |
|---|---|---|---|
| Free | $0 | $0 | — |
| **Pro** | **$12** | **$99** | ~31% (1.7 months free) |
| **Tournament Prep** | **$25** | **$199** | ~34% (2 months free) |

Pricing rationale traced to Phase 3 benchmarks (`01-discovery/market-analysis.md`):
- Mobalytics LoL premium $7.99/mo — closest direct adjacency, but for a much larger audience. Our smaller, more concentrated market supports 50% premium pricing at standard tier.
- Wolfey Patreon $5-10/mo — proves the community-pays-for-prep ceiling at this tier.
- Metafy human coaching $25-30/hr — Tournament Prep tier sits at "10x cheaper than one coaching session per month" framing.
- Pokémon HOME Premium $16/yr — confirms the community will commit to annual subscriptions at $15-20 range.

---

## Tier Feature Map

### Free Tier
*Goal: hook serious players, deliver enough value that Pro feels worth it after one tournament cycle.*

- 5 saved teams (max)
- Showdown packed-format import + export
- Poképaste-style public team pages (with our branding)
- Basic AI Q&A (10 turns/day)
- Public archetype tag library (read-only)
- No version history (current version only)
- Community-paste browse

### Pro Tier — $12/mo or $99/yr
*Goal: the tournament-prep persona's daily-driver workspace.*

Everything in Free, plus:
- Unlimited saved teams
- Full version history with diff views
- 100 AI coach turns/day
- Manual match journaling — structured reflection prompts after a battle
- Pattern synthesis across last N games
- Personal archetype matchup tags ("for Indianapolis," "vs. rain decks")
- Calendar-aware tournament-prep mode (basic): single tournament target
- Smogon usage stats live integration
- Showdown packed-format round-trip with no data loss

### Tournament Prep Tier — $25/mo or $199/yr
*Goal: the highest-WTP segment's pre-Regional/Worlds prep stack.*

Everything in Pro, plus:
- Meta projection from recent Regional/International data
- Counter-team builder — runs simulator battles to preview matchup tradeoffs
- Opponent scouting (publicly known teams from VGC tournament results)
- 1-1 coach-mode sharing — invite a training partner with read/comment access
- Multiple concurrent tournament targets
- Priority AI coach quota (500 turns/day)
- Early-access to new features
- Direct support from founder

---

## Unit Economics

All numbers are estimates anchored on Phase 3 benchmarks. Bracketed labels mark assumptions.

### Per-User Economics (assuming Pro tier, monthly)

**Revenue per Pro user:** $12.00/mo

**Variable cost per Pro user:**
- LLM API (Sonnet 4.6 with smart routing, ~50 coach turns/mo avg): **$1.50-3.00** [Estimate, from Wave 4 benchmarks]
- Database I/O + storage: $0.05
- Email + transactional: $0.05
- Payment processing (Stripe ~2.9% + $0.30): $0.65 monthly fee
- **Total variable: ~$2.25-3.75/mo**

**Gross margin: ~$8-10 per Pro user/mo (~70-80%)**

### Per-User Economics — Tournament Prep tier

**Revenue:** $25.00/mo
**Variable cost (heavier AI usage, ~150 turns/mo):** $4-6/mo
**Gross margin: ~$19-21 per user/mo (~80%)**

### CAC (Customer Acquisition Cost)

[Estimate — not yet validated]

- **Organic Reddit + creator-partner traffic:** CAC essentially $0 in volume; capped by reach.
- **Founder time as acquisition:** 5-10 hrs/wk on content creation (cost = founder time, ~$0 cash but real opportunity cost).
- **Direct paid acquisition (Reddit ads, YouTube creator-paid placements):** $15-30 per paid signup [Estimate, from gaming-tool benchmarks]. Should not be primary channel given the founder's budget.

**Target CAC: $0-15 per paid signup** — achievable through organic + creator partnerships in Year 1.

### LTV (Lifetime Value)

**Working assumption [Assumption to validate]:**
- Avg Pro user retention: **6 months** (driven by VGC tournament cycle — many players are seasonal)
- Tournament Prep retention: **8 months** (more committed players)

**Pro LTV** = $12 × 6 × 0.75 (gross margin) = **$54**
**Tournament Prep LTV** = $25 × 8 × 0.80 = **$160**

[Yellow Flag] These retention figures are inferred from creator Patreon patterns, not validated. The most important unknown in the financial model.

### LTV:CAC Ratio (Target)

- Pro: $54 / $15 = **3.6x** (acceptable; above 3x threshold)
- Tournament Prep: $160 / $15 = **10x** (excellent if achievable)

---

## Free → Paid Conversion

**Industry benchmarks:**
- B2C SaaS / consumer freemium: 1-3%
- Highly-targeted vertical tools: 3-8%
- Mobalytics-class gaming companion tools: ~1-2% [Estimate, Tier 2]

**Working target:** **3% free-to-paid conversion within 30 days** for Persona C-aligned signups; lower (~0.5-1%) for Persona E (casual) inbound.

**Conversion levers:**
- Hitting team-slot limit (free capped at 5)
- Tournament announcement (we surface Tournament Prep upsell)
- AI coach quota exhaustion (free capped at 10/day)
- Version history limit hit (free has none)
- Public team page → "want to keep this in your private workspace?"

---

## Revenue Lines (Year 2+)

**Creator content marketplace (Year 2)**
- Named players publish team packs, prep guides, archetype primers
- Rev share — 70/30 to creator
- Anchor partner: WolfeyVGC, CybertronVGC, Brady Smith / VGC Corner
- Estimated incremental ARR: $20-50K Year 2

**Team / club seats (Year 2)**
- $X/mo per seat for training-partner squads (3-8 person clubs)
- Pricing target: $8/seat/mo on top of Pro
- Estimated incremental ARR: $10-30K Year 2

**API access (Year 2)**
- Tournament organizers, content sites integrate our team-data and meta-projection feeds
- Pricing target: $50-200/mo per integrator
- Estimated incremental ARR: $5-20K Year 2

---

## Scalability

- **Engineering:** Solo-founder MVP feasible (Wave 4: ~315 hours within 235-390 hour 6-mo envelope). Beyond ~500 paid users, will need part-time second engineer or contractor for sustained product velocity.
- **Operations:** Stripe handles payments. Resend handles email. Cloudflare/Vercel scale automatically.
- **Customer support:** Founder direct in Year 1; community Discord becomes primary support channel by month 3.
- **AI cost scaling:** LLM costs scale linearly with users; ~$3/mo/user variable. Becomes a meaningful cost line at >1000 paid users; revisit caching, smaller models, retrieval optimization at that point.

[Yellow Flag] LLM cost is the most volatile cost line. A bad prompt design or runaway feature could 5x AI cost overnight. Phase 6 product spec must include explicit per-user AI quotas and graceful degradation.

---

## Key Partnerships

**Critical (must close in first 6 months):**
1. **Top-3 creator partnership** — WolfeyVGC primary; CybertronVGC + Brady Smith / VGC Corner alternates. Patreon-tier-locked Pro access + revshare. *Validation Week 1-2.*
2. **Competitive-player advisor** — name with credibility on r/stunfisk and Smogon forums. Equity, comp, or revshare TBD. Non-negotiable for Persona C credibility. *Validation Week 1-2.*

**Strategic (year 1):**
3. Smogon RMT moderator advisor — informal credibility
4. Limitless community Champions tournament sponsor — "Presented by Champion's Notebook"
5. Victory Road bilingual partnership (Latam) — Spanish unlock

**Optional (year 2+):**
6. Pokémon Champions Twitch streamer integrations
7. Tournament organizer integrations (auto-import top-cut teams)

---

## Dependencies (Risks Carried Into Phase 8)

1. **WolfeyVGC partnership viability** — unvalidated. If declined, Plan B is CybertronVGC + Brady Smith.
2. **Advisor recruitment** — unvalidated. Must close before launch.
3. **TPC native team management** — could ship within 6-12 months and erode 30% of value prop. Mitigation: AI coaching + longitudinal memory + cross-format sync are moats.
4. **Pikalytics expansion into workspace** — could ship a workspace layer at any time. Mitigation: speed-to-meaningful-MVP + creator partnership lock-in.
5. **LLM API cost stability** — Sonnet 4.6 pricing is current; provider could change. Multi-provider abstraction at code level.

---

## Three Financial Scenarios (Year 1 ARR)

[Detail in `05-financial/projections.md`. Quick preview here:]

| Scenario | Free signups Y1 | Pro paying | TP paying | ARR Y1 |
|---|---|---|---|---|
| **Conservative** | 5,000 | 100 | 30 | **$23K** |
| **Base** | 12,000 | 300 | 100 | **$66K** |
| **Optimistic** | 25,000 | 700 | 250 | **$159K** |

Conservative does not cover even the founder's part-time opportunity cost. Base is meaningful side-project revenue. Optimistic implies bootstrap-business viability and the start of a hire-someone runway.

---

## Flags

**Red Flags:**
- None.

**Yellow Flags:**
- LTV/retention assumptions are inferred from adjacencies, not validated for this specific market. Phase 8 retention measurement is the single most important post-launch metric.
- LLM cost variability could destabilize unit economics if not capped per-user.
- Conservative scenario doesn't return a positive net for the founder's time investment. The model needs at least Base to be worth pursuing.
- Tournament Prep tier's $25/mo pricing is the riskiest single number — if it lands at $15 instead, optimistic ARR drops by ~$30K.

## Sources

- `01-discovery/market-analysis.md` — pricing benchmarks (Mobalytics, Wolfey, Metafy, HOME Premium)
- `01-discovery/raw/wave3-personas.md` — Persona C WTP signals
- `01-discovery/raw/wave4-technical.md` — LLM cost estimates
- `02-strategy/lean-canvas.md` — pricing-tier feature breakdown
- `02-strategy/value-proposition.md` — substitution equation
