# Assumptions Tracker

**Phase:** 8 — Validation
**Project:** ai-website-sg-restaurants
**Date:** 2026-05-11

---

This document tracks every critical assumption the business rests on. Update the **Status** column as validation data comes in. **Untested** assumptions are roadblocks until tested; **validated** ones lock in confidence; **invalidated** ones require a plan revision.

---

## Critical Assumptions

| ID | Assumption | Confidence (Today) | How to Test | Test Owner | Status |
|----|------------|--------------------|-------------|------------|--------|
| A1 | Pre-built spec sites lift cold-outreach close rate ≥3× in SG | Medium (US data; not SG) | Experiment 2 (walk-ins) + Experiment 4 (email A/B) | Founder 1 | **Untested** |
| A2 | Owner-operator persona present in venue 2-4pm | High (operator schedules) | Observed during Experiment 2 | Founder 1 | **Untested** |
| A3 | Per-site compute cost achievable at <SGD 2 in batch | Medium (vendor pricing supports it) | Experiment 1 (engineering spike) | Founder 2 | **Untested** |
| A4 | Standard tier (SGD 1,500) is acceptable without PSG | Medium (research says SG floor is SGD 2,500; we're undercutting) | Experiment 2 + 4 close rates | Founder 1 | **Untested** |
| A5 | Maintenance attach ≥20% at SGD 79/mo | Low (no SG data) | Offer maintenance to first 10 customers; track | Founder 1 | **Untested** |
| A6 | Walk-in close rate ≥5% in dense SG F&B clusters | Medium (US estimates) | Experiment 2 | Founder 1 | **Untested** |
| A7 | Cold-email reply rate ≥8% with personalized spec-site link | Medium (US data) | Experiment 4 | Founder 2 | **Untested** |
| A8 | PSG approval is achievable in <12 months | Low (depends on policy; no published timeline) | Experiment 5 (call EnterpriseSG + vendor founder lunch) | Founder 2 | **Untested** |
| A9 | AI-generated site quality is rated ≥7/10 by laypeople | Medium (Lovable/Bolt outputs are getting good) | Experiment 1 ratings | Founder 2 | **Untested** |
| A10 | Both co-founders can sustain 25 walk-ins/week each | Low (no prior agency experience) | Observed during Experiment 2 | Both | **Untested** |
| A11 | Customers will pay 50% upfront before delivery | Medium (typical SMB services pattern) | First close in Experiment 2 | Founder 1 | **Untested** |
| A12 | ~40-60% of SG independents have no owned website | Low (no clean stat) | 50-outlet Google Maps audit | Either | **Untested** |
| A13 | F&B operators understand "Google ranking loss" as a real cost | Medium (research says pain is latent) | Diagnostic conversation in Experiment 2-3 | Founder 1 | **Untested** |
| A14 | Singapore PDPA cold-email compliance is achievable at small scale | High (research: B2B legal w/ opt-out + ID) | Day-to-day operations | Founder 2 | **Assumed safe** — monitor |

## Supporting Assumptions (Lower-Stakes, Don't Block Launch)

| ID | Assumption | Status |
|----|------------|--------|
| B1 | Oddle/Chope will respond to partnership inquiry within 60 days | Untested |
| B2 | RAS allows non-operator vendor membership tier | Untested |
| B3 | AI tooling pricing remains stable through 2026 | Assumed |
| B4 | SG postal/transport costs remain stable | Assumed |
| B5 | Currency exchange (SGD/USD) remains within ±10% of current | Assumed |

---

## Validation Funnel

The 5 most load-bearing assumptions are **A1, A3, A6, A7, A8**. If any one of these is invalidated outright, the business model needs significant revision. The validation playbook is explicitly designed to test all 5 within 30 days.

### Pre-Test Confidence Profile

| Confidence | Count |
|-----------|------:|
| High | 1 (A14) |
| Medium | 7 (A1, A3, A4, A6, A7, A9, A11) |
| Low | 5 (A2, A5, A8, A10, A12, A13) |

**[Opinion] The "Low" cluster is uncomfortable — five critical assumptions with limited prior evidence. This is normal for early-stage validation but underscores why the 30-day sprint is non-negotiable.**

---

## How to Use This File

1. **Before each experiment:** Read the relevant assumption rows to clarify what you're testing.
2. **During each experiment:** Capture data in a spreadsheet (don't update this file every day).
3. **At the end of each experiment:** Update the Status column to **Validated**, **Invalidated**, or **Partially Validated**.
4. **Weekly review:** Re-read this file every Sunday. Untested assumptions older than 14 days are red flags — they mean you're operating on faith, not evidence.

## Status Definitions

- **Untested:** No data yet
- **Testing:** Experiment in progress
- **Validated:** Evidence confirms the assumption; lock in
- **Partially Validated:** Some evidence supports it but more is needed (e.g., n<5)
- **Invalidated:** Evidence directly contradicts the assumption; plan revision needed
- **Assumed safe:** Low-impact assumption, monitoring only

---

## Sources
- `01-discovery/*` for the original evidence base behind each assumption
- `06-validation/validation-playbook.md` for test specifications
