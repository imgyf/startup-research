# Risk Analysis

**Phase:** 8 — Validation
**Project:** pokemon-champions-team-workspace
**Date:** 2026-05-10
**Confidence:** Medium-High (risks identified across phases; likelihood/impact ratings are opinion-grounded)

---

## Risk Matrix

Likelihood: Low / Medium / High. Impact: Low / Medium / High / Critical (kills the business).

### Market Risks

| Risk | Likelihood | Impact | Detection signal |
|---|---|---|---|
| **TPC ships native team management in Champions update** | Medium | High | Patch notes mentioning team slots / version history |
| Pokémon Champions player population decays faster than expected | Low | High | Monthly Pikalytics traffic decline; r/PokemonChampions activity drop |
| Casual market is the only WTP segment we reach (Persona C unreachable) | Low | Critical | Free signups skewed toward Persona E by survey data |
| Major competitor with venture funding enters Q3-Q4 2026 | Medium | High | Crunchbase + new tool launch with cohesive marketing |
| Pokémon Champions tournament scene fails to mature | Low | Medium | Regional attendance flat or declining 2027 vs 2026 |

### Product Risks

| Risk | Likelihood | Impact | Detection signal |
|---|---|---|---|
| **AI coach hallucinates on competitive Pokémon facts** | Medium | High | User complaints; sample audit reveals errors |
| Manual journaling adoption is below 30% (kills synthesis feature substrate) | Medium | Medium | Closed-beta journal entry count |
| Showdown packed-format edge cases break import for new users | Medium | Medium | Error logs from import endpoint |
| Mobile-responsive feels broken on tournament day | Medium | Medium | Closed-beta mobile testing reports |
| LLM cost runaway from broken feature | Low | High | Daily cost dashboard alarm |

### Business Risks

| Risk | Likelihood | Impact | Detection signal |
|---|---|---|---|
| **All 3 top creators decline partnership** | Medium | High | Outreach replies + scheduled meetings count |
| Free→paid conversion lands at <1% | Medium | High | Public-launch month-1 cohort data |
| Off-season retention drops below 40% | Medium | High | Q2 (Oct-Dec '26) churn rate |
| Tournament Prep tier WTP is half what we modeled ($12 actual vs $25 plan) | Medium | Medium | Pricing test results + landing page tier-interest survey |
| Annual contracts don't renew at expected rate | Low | Medium | First annual renewals around month 12 |

### Team Risks

| Risk | Likelihood | Impact | Detection signal |
|---|---|---|---|
| **Founder credibility gap (no advisor) makes Persona C reject the product** | Medium | High | Beta tester comments mentioning "who are you?" |
| Founder velocity drops below 15 hrs/wk for >4 weeks | Medium | High | Build cadence missed milestones |
| Founder burns out on solo development | Medium | Medium | Slipping deliverables, reduced engagement signals |
| Skill gap on AI grounding architecture | Low-Medium | Medium | Build delays on M4 module |

### Financial Risks

| Risk | Likelihood | Impact | Detection signal |
|---|---|---|---|
| **Conservative scenario plays out (Y1 ARR <$25K)** | Medium | Critical | Month 6 milestone — see kill criteria |
| LLM costs exceed $1500/mo before paying users cover it | Low | Medium | Monthly cost vs MRR trend |
| Stripe dispute / chargeback storm | Very Low | Medium | Stripe dashboard alerts |
| One-time costs balloon past $5K | Low | Low | Bookkeeping tracker |

### Legal / IP Risks

| Risk | Likelihood | Impact | Detection signal |
|---|---|---|---|
| TPC issues C&D against the workspace (despite historical pattern) | Very Low | Critical | Any communication from TPC legal |
| Trademark conflict with brand name | Low | Medium | USPTO search; cease-and-desist from holder |
| Showdown / Smogon community openly criticizes us as "exploiting" their work | Low-Medium | Medium | Reddit/Discord sentiment monitoring |
| Privacy / data handling complaint (esp. EU users) | Low | Medium | User complaint or regulator inquiry |

---

## Top 5 Risks — Detailed Mitigation Plans

### Risk 1 — Founder credibility gap

**Likelihood:** Medium **Impact:** High

**Mitigation:**
- **Week 1-2:** Advisor recruitment is non-negotiable. Target 1 named competitive player.
- **Backup plan:** If no single advisor lands by Week 4, recruit a "panel" of 3-5 mid-tier ladder players as informal advisors with quarterly stipends ($50-100/each per quarter).
- **Brand safeguard:** Always credit advisor visibly on About page, footer, AI coach citations.
- **Validation experiment:** E1 interviews surface whether the credibility issue is real or anticipatory.

**Early warning signal:** Beta testers in E8 mentioning "who are you" or "what are your credentials" 3+ times.

### Risk 2 — TPC ships native team management

**Likelihood:** Medium **Impact:** High (could erase 30% of value prop)

**Mitigation:**
- **Build moats they can't easily replicate:** AI coaching grounded on @pkmn/sim + @smogon/calc; longitudinal memory; cross-format sync.
- **Quarterly competitive intelligence:** monitor Champions patch notes, TPC PR releases.
- **Product agility:** keep workspace abstraction format-agnostic so we can pivot to Showdown-only or new-format if Champions native tools narrow our wedge.

**Early warning signal:** Pokémon Champions roadmap leaks; patch notes preview; TPC PR mentions team-related features.

### Risk 3 — Creator partnership all 3 decline

**Likelihood:** Medium **Impact:** High

**Mitigation:**
- **Backup pool:** smaller-creator network — VGC Corner / Brady Smith is already in our top 3 and may be more reachable than Wolfey.
- **Content-led acquisition:** if no creator partnerships materialize, founder content + SEO becomes the primary channel. Slower ramp but feasible.
- **Tournament sponsorship as alternative reach:** Limitless community Champions tournaments are buyable for $200-500.

**Early warning signal:** No replies to Tier 1 creator DMs within 14 days.

### Risk 4 — AI coach hallucinates on competitive Pokémon facts

**Likelihood:** Medium **Impact:** High (brand-killing if Persona B amplifies on Reddit)

**Mitigation:**
- **Hard rule:** every AI response must either cite a tool-call result OR refuse to answer. Enforced at the prompt-engineering and architecture level.
- **Audit cadence:** founder samples 20 random AI responses weekly; hallucinations logged and root-caused.
- **Red-team in closed beta:** invite Persona B beta testers specifically to try to break the coach.
- **Public commitment:** "If we hallucinate, refund the month" — possible policy that signals seriousness.

**Early warning signal:** Even one hallucination caught in closed beta is reason to delay public launch until grounding is hardened.

### Risk 5 — Conservative scenario plays out (Y1 ARR <$25K)

**Likelihood:** Medium **Impact:** Critical (founder opportunity cost not covered)

**Mitigation:**
- **Hard kill criterion at Month 6** (see `kill-criteria.md`)
- **Pivot options if metrics fail:** (a) free utility with creator content marketplace as monetization; (b) AI coach as standalone tool, sell to coaching marketplaces; (c) wind down, write retrospective.
- **Don't sunk-cost:** revisit the kill decision at every milestone.

**Early warning signal:** Month 3 free signups <2,000 OR closed-beta Pro WTP commitments <30%.

---

## Risk-Adjusted Posture

The honest summary: this project carries **moderate execution risk and moderate-low market risk**. The market is real, the WTP is real, the IP risk is low, the technical feasibility is established. The risks concentrate on **execution** (founder velocity + advisor + creator partnerships) and **product quality** (AI grounding + journal adoption + retention).

This is **a manageable risk profile for a side-project bootstrap**. It is **not** a venture-scale opportunity given the small TAM and likely Year 2 ARR ceiling of $200-500K. Founder should not pursue this expecting a unicorn outcome — pursue it expecting a meaningful side income and a portfolio piece, with a small probability of a $1-5M ARR business by Year 3.

---

## Risk Review Cadence

- **Weekly:** AI hallucination samples; LLM cost dashboard
- **Monthly:** Free signup growth; conversion rate; competitor monitoring; founder velocity
- **Quarterly:** Competitive intelligence (Champions patch notes, new tools); TPC enforcement scan; creator partnership health
- **Pre-launch:** Trademark + privacy + legal review

---

## Flags

**Red Flags:**
- None at the risk-portfolio level.

**Yellow Flags:**
- Founder credibility gap is the highest-leverage risk because it's addressable in Week 1. If not addressed, it compounds across all other risks.
- TPC native-feature risk is the hardest to mitigate fully. Build moats that survive their potential moves.
- The risk register depends on founder honesty in self-assessment at each milestone. Sunk-cost continuation past kill criteria is the single most expensive failure mode of side projects.

## Sources

- `01-discovery/competitor-landscape.md` — competitor risk
- `01-discovery/raw/wave4-technical.md` — feasibility risks
- `02-strategy/business-model.md` — dependency list
- `02-strategy/go-to-market.md` — channel risk
- `05-financial/revenue-model.md` — financial risk
