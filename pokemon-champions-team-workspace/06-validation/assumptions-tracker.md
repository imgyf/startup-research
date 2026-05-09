# Assumptions Tracker

**Phase:** 8 — Validation
**Project:** pokemon-champions-team-workspace
**Date:** 2026-05-10
**Status:** Living document — update after every experiment

---

## How to Use

Each row is a critical assumption underlying the business plan. **Status:** untested / testing / validated / invalidated. **Confidence:** Low / Medium / High. After every experiment, update affected rows.

---

## Critical Assumptions

| # | Assumption | Confidence | Status | How to test | Validation experiment |
|---|---|---|---|---|---|
| **A1** | VGC tournament aspirants (Persona C) are reachable through Reddit + creator partnerships | Medium | Untested | Track Free signup source-attribution after launch | E4 + E6 + E9 |
| **A2** | Persona C will pay $12/mo for Pro tier | Medium | Untested | Pricing test on landing page; closed-beta WTP survey | E5 + E8 |
| **A3** | Persona C will pay $25/mo for Tournament Prep | Low-Medium | Untested | Pricing test variants | E5 + E8 + E9 |
| **A4** | Tool fragmentation under tournament pressure is the top pain | Medium-High | Untested directly | Customer-discovery interviews | E1 |
| **A5** | "I keep losing and don't know why" is the strongest single wedge | Medium-High | Untested directly | Customer-discovery interviews | E1 |
| **A6** | Manual journaling adoption is high enough (≥30%) to support pattern synthesis | Low-Medium | Untested | Closed-beta usage observation | E8 |
| **A7** | Grounded AI coach feels meaningfully different from VGCCoach / ChatGPT | Medium | Untested | Wizard-of-oz prototype | E7 |
| **A8** | At least 1 of top-3 creators agrees to a Patreon-locked partnership | Low-Medium | Untested | Direct outreach | E3 |
| **A9** | A credible competitive-player advisor is recruitable | Medium | Untested | Direct outreach | E2 |
| **A10** | r/stunfisk + r/PokemonChampions communities accept our framing without hostility | Medium | Untested | Reddit testing post | E6 |
| **A11** | Y1 free signups can reach 12K (Base) via organic + creator | Low-Medium | Untested | Track signup growth | E9 |
| **A12** | Free → Pro conversion of 2.5% (Base) | Low-Medium | Untested | Public-launch cohort | E9 |
| **A13** | 4-week paid retention ≥70% in Base scenario | Low-Medium | Untested | Cohort retention | E9 + E10 |
| **A14** | Off-season (Sept-Nov) churn is manageable (<25%/month) | Low | Untested | Q2 metrics | E10 |
| **A15** | TPC will not C&D our companion tool | High | Validated by 15-year historical pattern | Monitor for any TPC contact | Ongoing |
| **A16** | AI coach hallucination rate can be held below 5% with grounding | Medium | Untested | Sample-audit of coach responses | E7 + E8 |
| **A17** | LLM cost per Pro user stays under $3/mo at typical usage | Medium | Untested | Daily cost dashboard | E7 onwards |
| **A18** | TPC won't ship native team management within 6 months | Medium | Untested | Patch-note monitoring | Quarterly |
| **A19** | Pikalytics won't ship workspace features that obsolete our wedge before MVP | Medium | Untested | Competitor monitoring | Monthly |
| **A20** | Founder velocity holds at 15-25 hrs/week for 12 weeks | Medium-High | Untested | Self-tracked time logs | Ongoing |
| **A21** | Showdown packed-format imports cleanly for >95% of real-world team paste inputs | Medium | Untested | Test against 50+ real teams | Pre-public-launch |
| **A22** | Mobile-responsive web is sufficient for MVP (no need for native iOS) | Medium | Untested | Beta tester feedback | E8 |
| **A23** | Tournament-cycle hook (calendar awareness) drives meaningful retention | Medium-High | Untested | Q1-Q2 retention data | E10 |
| **A24** | Persona share % (5% C, 10% B, 50% E) approximately holds in real signups | Low | Untested | Survey of new signups | E1 + E9 |
| **A25** | Brand name "Champion's Notebook" is trademark-clear and domain-available | Medium | Untested | USPTO + WHOIS check | Pre-launch (Week 0-1) |

---

## Status Summary

- **Validated (1):** TPC enforcement posture (A15)
- **Untested but supported by adjacent data (10):** A1, A2, A4, A5, A7, A9, A16, A20, A23, A25
- **Untested with weaker support (14):** Everything else

After Week 1: Most A1-A10 should move to "testing" or "validated" via interviews + outreach.
After Week 6: A6, A7, A16, A21, A22 should be validated/invalidated by closed beta.
After Week 12: A11, A12, A13, A14, A24 should have first-month data.

---

## Decision Triggers

| Trigger | Action |
|---|---|
| A4 or A5 invalidated by interviews | Pivot positioning before building anything |
| A8 invalidated (no creator partnerships) | Rebuild GTM around content + tournament sponsorships |
| A9 invalidated (no advisor) | Recruit panel of 3-5 informal advisors as Plan B |
| A2 invalidated (Pro $12 too high) | Test $9 in next pricing variant |
| A3 invalidated (TP $25 too high) | Restructure tier — fold TP into Pro at $15-18 |
| A6 invalidated (journaling too low) | Replace with quick-tag voting; restructure synthesis |
| A12 invalidated (Free→Pro <1%) | Major product or market mismatch; consider pivot |
| A14 invalidated (off-season collapse) | Accept seasonal-business model; cap ambitions |
| A18 invalidated (TPC ships native) | Lean hard into AI + cross-format moats; possibly pivot to Showdown-primary |

---

## Update Log

| Date | Update |
|---|---|
| 2026-05-10 | Initial creation. All assumptions in baseline state from Phase 3 research. |

---

## Flags

**Red Flags:**
- None.

**Yellow Flags:**
- The list of low-confidence assumptions is long (~14). This is normal pre-validation. The point is to reduce the count by half within 6 weeks via the playbook experiments.
- A24 (persona share %) is hard to validate cheaply; partial validation via survey is acceptable.

## Sources

- `01-discovery/research-gate.md`
- `06-validation/validation-playbook.md`
- `06-validation/risk-analysis.md`
- All Phase 3 research deliverables
