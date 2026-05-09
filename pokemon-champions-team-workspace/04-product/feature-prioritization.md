# Feature Prioritization

**Phase:** 6 — Product
**Project:** pokemon-champions-team-workspace
**Date:** 2026-05-09
**Confidence:** Medium-High (RICE estimates are inferred; should be re-scored after closed beta)

---

## Method

We use **RICE prioritization** (Reach × Impact × Confidence ÷ Effort) for major features, with a parallel **MoSCoW classification** (Must/Should/Could/Won't) to drive scope discipline. Reach is scored 1-5 (% of target audience reached). Impact 0.25-3 (massive = 3, minimal = 0.25). Confidence 0.5-1 (gut-feel = 0.5, validated = 1). Effort in person-weeks (1 person-week = 20-30 hrs).

---

## RICE Scores (Sorted)

| Feature | Reach | Impact | Confidence | Effort (pw) | RICE | MoSCoW |
|---|---|---|---|---|---|---|
| **Team workspace + Showdown import/export** | 5 | 3 | 1.0 | 3 | **5.00** | Must |
| **AI Matchup Coach (grounded)** | 5 | 3 | 0.8 | 5 | **2.40** | Must |
| **Version history + diff** | 5 | 2 | 1.0 | 2 | **5.00** | Must |
| **Free / Pro / Tournament Prep billing** | 5 | 3 | 1.0 | 1.5 | **10.0** | Must |
| **Matchup tags (manual)** | 4 | 1.5 | 1.0 | 1 | **6.00** | Must |
| **Match journal + AI synthesis** | 3 | 2 | 0.7 | 3 | **1.40** | Must |
| **Tournament prep mode (basic)** | 3 | 2 | 0.8 | 2 | **2.40** | Must |
| **Mobile-responsive web** | 5 | 1 | 1.0 | 1 | **5.00** | Must |
| **Public team page (Poképaste-style)** | 4 | 1 | 1.0 | 1 | **4.00** | Should |
| **Coach-mode (collaborative sharing)** | 2 | 2 | 0.7 | 2 | **1.40** | Should — v1.1 |
| **Counter-team builder (sim-based)** | 2 | 3 | 0.6 | 4 | **0.90** | Should — v1.1 |
| **Meta projection from Regional data** | 2 | 2 | 0.7 | 3 | **0.93** | Should — v1.1 |
| **Native iOS app** | 3 | 2 | 0.8 | 6 | **0.80** | Could — v1.1/v1.2 |
| **Spanish localization** | 1 | 2 | 0.7 | 2 | **0.70** | Could — v1.2 |
| **Opponent scouting (top-cut teams)** | 1 | 2 | 0.7 | 2 | **0.70** | Could — v1.2 |
| **Public team explore feed** | 3 | 1 | 0.7 | 2 | **1.05** | Could — v1.2 |
| **Streamer overlay / OBS integration** | 0.5 | 2 | 0.4 | 2 | **0.20** | Won't — Y2 |
| **Custom archetype tag system (admin)** | 1 | 1 | 0.7 | 2 | **0.35** | Won't — defer |
| **Battle simulator UI** | n/a | n/a | n/a | huge | n/a | **NEVER** (Showdown's job) |
| **Casual team-builder mode** | n/a | n/a | n/a | small | n/a | **NEVER** (anti-positioning) |
| **Auto-replay analysis** | n/a | n/a | n/a | infeasible | n/a | **NEVER** (no Champions replay data) |

[Effort columns are point estimates. Confidence in estimates is moderate.]

---

## MoSCoW Summary

### Must-Have (MVP — v1.0 ships by late June 2026)

1. Account + team workspace foundation
2. Showdown packed-format I/O
3. Version history + diff
4. Matchup tags (manual taxonomy + free-text)
5. AI Matchup Coach (grounded on @pkmn/sim + @smogon/calc + Smogon stats)
6. Match journal + AI pattern synthesis
7. Tournament prep mode (basic — set target, days countdown, prep checklist)
8. Free / Pro / Tournament Prep billing
9. Mobile-responsive web
10. Public team page (Poképaste-style, branded)

### Should-Have (v1.1 — September-October 2026)

1. Coach-mode (read/comment sharing)
2. Counter-team builder (sim-based matchup tradeoff preview)
3. Meta projection from Regional usage data
4. Public team explore feed (with attribution; light social)

### Could-Have (v1.2-v1.3 — Q4 2026 / Q1 2027)

1. Native iOS app
2. Spanish localization (Latam unlock via Victory Road partnership)
3. Opponent scouting (publicly known top-cut teams)
4. Custom archetype tag system

### Won't-Have (Year 2+)

1. Streamer overlay / OBS integration
2. Tournament organizer tools
3. Pokémon GO / mainline ranked / TCG support
4. Casual fun-team-builder mode
5. Battle simulator UI
6. Auto-replay analysis (technically infeasible)

---

## Dependency Map (Build Order)

```
M1 Account + Workspace ──┬─→ M2 Version History ──┬─→ M3 Matchup Tags
                         │                        │
                         ├─→ M7 Billing           ├─→ M5 Journal
                         │                        │
                         └─→ M4 AI Coach ─────────┴─→ M6 Tournament Mode
                                                      (depends on M2, M3, M5)
```

**Critical path:** M1 → M4. The AI Coach is the differentiator and is gated by Workspace foundation. If M1 slips, M4 slips, MVP slips.

**Parallelizable:** M2 + M3 + M7 can be built mostly in parallel after M1 is stable. M5 depends on M1 + M3 conceptually. M6 sits at the end.

---

## Recommended 12-Week Build Order

| Week | Focus | Deliverables |
|---|---|---|
| 1-2 | M1 foundation + Showdown I/O | Working teambuilder + import/export |
| 3 | M2 version history | Save versions, diff view |
| 4 | M3 matchup tags | Tag system + filtering |
| 5-6 | M4 AI coach grounding stack | LLM + sim + calc + stats RAG; first coach turns working |
| 7 | M4 polish + citations | Citation discipline, refusal behavior |
| 8 | M5 match journal | Structured prompts + entries |
| 9 | M5 AI synthesis + M6 tournament mode | Pattern synthesis + tournament target |
| 10 | M7 billing + Pro/TP gating | Stripe live; quotas enforced |
| 11 | Polish, mobile-responsive, onboarding | Closed-beta-ready |
| 12 | Closed beta + iteration | 30-50 invited users; final fixes |

**Public launch target: end of Week 12 — late June 2026.**

If schedule slips by 2 weeks, public launch lands mid-July, still within Worlds-prep window.

---

## Re-Scoring Schedule

RICE scores are estimates. Re-score after:
- Closed beta (Week 11-12) — Confidence levels for AI Coach + Match Journal will firm up
- 30 days post-launch — Reach + Impact for v1.1 features informed by real usage data
- After first creator partnership goes live — channel-driven reach estimates change

---

## Anti-Pattern Watch

Based on common founder pitfalls flagged in Phase 1 hard questions:

- **"Boiling the ocean"** — Resist the urge to ship Coach-mode + Counter-team builder + Mobile native in v1.0. Each is a "should-have," not a "must."
- **"Premature optimization"** — Don't build a meta-projection algorithm until we have usage data; static usage stats from Smogon are enough at MVP.
- **"Vanity features"** — A "battle predictor" or "team grader" feels exciting but doesn't change retention; cut.
- **"Solution looking for a problem"** — Auto-replay analysis was the original "exciting" feature; cutting it is correct because the problem (player learning) is solved better by manual journaling given data constraints.

---

## Flags

**Red Flags:**
- None.

**Yellow Flags:**
- Match Journal is the most novel feature — its RICE confidence is 0.7 because adoption isn't validated. If users don't journal in closed beta, the AI synthesis feature has no substrate. **Plan B: if journal adoption is below 30% in beta, replace pattern-synthesis with simple quick-tag voting on individual battles, then synthesize from tags.**
- AI Coach effort (5 person-weeks) is the largest single block and the biggest schedule risk. Founder should architect grounding stack first, then layer in features — not the other way around.
- Counter-team builder is a v1.1 feature that competitor Pikalytics or VGCCoach could ship before us. If they do, our v1.1 differentiation narrows. Mitigation: ship coach-mode (collaboration) and meta projection in v1.1 instead of leading with counter-team builder.

## Sources

- `04-product/mvp-definition.md` — must-have scope
- `02-strategy/lean-canvas.md` — tier-feature alignment
- `01-discovery/raw/wave4-technical.md` — effort estimates
- `02-strategy/go-to-market.md` — launch timeline
