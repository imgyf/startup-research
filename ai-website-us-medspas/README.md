# US Med Spa Website Agency — Pivot Validation Summary

**Project:** ai-website-us-medspas (pivot of `../ai-website-sg-restaurants/`)
**Date:** 2026-05-11
**Mode:** Focused validation pass (not a full 8-phase run)
**Verdict:** **CONDITIONAL — Score 5.0/10. A lateral move, not the upgrade you'd want. Validate before committing.**

---

## One-Paragraph Overview

Same model as the Singapore project — pre-build an AI-generated spec website for a named prospect, cold-outreach showing it, full build on conversion — but pivoted to **US med spas / aesthetic clinics** (target: Tampa + Orlando cluster, not Dallas–Fort Worth) at **USD 3,000–7,000 per build + USD 200–400/mo maintenance retainer**. The pivot was proposed to escape Singapore's two structural drags: low ACV (~USD 1,000/restaurant site) and the Productivity Solutions Grant rising to 70% (which lets subsidized SG competitors match the unsubsidized price).

## Key Findings

1. **The pivot fixes the right things.** US med spa website builds sell for $4–10k+ (vs ~$1k in SG), there's no subsidy distortion, med spa owners are visually obsessed (the spec-site wedge should land harder), and — unlike restaurants/Oddle — med spa booking SaaS (Boulevard, Mangomint, Zenoti) *overlays* booking on your site rather than replacing it, which helps a web vendor. Med spa customers are cash-rich ($1.4M avg revenue, 15–30% mature margin, 5–12% of revenue on marketing).

2. **But the US med spa web/marketing market is closer to a bloodbath than an opening.** 10+ specialized agencies (Growth99, PatientGain $999–1,999/mo, MyAdvice, Influx, Aesthetic Conversion, ClinicGrower, The Med Spa Agency, …) plus a huge invisible long tail of GoHighLevel white-label "med spa marketing" sub-agencies. Almost none sell a website as the product — they sell **monthly marketing retainers with the site as a loss-leader**. A standalone "$5–7k site once" play is a *weaker* business than what incumbents run, and they'll happily build a free site to win a retainer.

3. **Moxie ([joinmoxie.com](https://joinmoxie.com)) eats the warmest leads.** Venture-backed all-in-one med spa OS for *launching* new med spas — bundles "customized website creation with online appointment booking" + back office + coaching, performance-priced. New openings (no site, no agency) are the best warm leads, and Moxie is aggressively chasing them.

4. **The spec-site wedge is not novel here.** Webware.ai, Workee.ai, Webflow's med-spa template gallery, and template shops already do free demos/mockups. "We'll show you a demo" is *standard practice*. A *fully personalized production-ready spec site for a named prospect before any contact* is mildly more differentiated — but it's an execution tactic copyable in a day, not a moat.

5. **Pitch fatigue is a real risk.** Med spas are *the* canonical SMMA-agency target vertical — owner inboxes/DMs are likely already saturated with web/marketing pitches.

6. **Per-metro independent market is small.** ~81% of US med spas are single-location, but you must exclude franchises (LaserAway, Milan Laser, Ideal Image, SEV Laser, OrangeTwist — corporate sites) and PE roll-ups (MedSpa Partners 40+ clinics, Advanced MedAesthetic Partners — centralized web). Realistic independent SAM per metro: ~150–350 med spas, switchable fraction smaller. DFW specifically may have *higher* roll-up density (home of Leon Capital / AMP) → **lean Tampa + Orlando together over DFW**. Fine for a 2-person lifestyle agency; not VC-scale.

7. **Offshore operations are workable but taxed.** A Singapore 2-person team *can* do this: Wyoming LLC (~$500–1k one-time, ~$300–600/yr), EIN (4–8 week bottleneck for non-residents), Wise/Relay banking (Mercury got stricter in 2025), Stripe for USD, **Form 5472 annual filing — $25k penalty if missed**, and a paid US international-tax accountant opinion before the first invoice (the ECI/USTB question is fact-specific; "services-from-SG = likely no US income tax" is a common but not guaranteed position). Relocation is **off the table** (E-2 needs ~$100–200k+ and bars no-employee micro-teams). **The biggest operational tax is timezone** — DFW business hours ≈ 10pm–6am Singapore; any synchronous work (discovery calls, kickoffs, cold calls) forces a founder onto a partial-US schedule. Med spa sites also need HIPAA-aware hosting/forms, consent-tracking photo galleries, FTC-compliant testimonials, and ADA/WCAG accessibility — all real, none fatal, and all selling points against cheap DIY sites.

## Verdict

**Score 5.0/10 — CONDITIONAL. The pivot is roughly a wash vs the Singapore idea (which itself scored 5.5).** It trades low ACV + subsidy distortion for a saturated market + offshore friction, and slightly *worsens* competitive advantage and founder-market fit. Per-deal economics are genuinely better ($3.6–6.4k gross profit per build, 60–90% margin); the binding constraint shifts from "will the wedge convert at all" to "can a 2-person offshore team win deals against entrenched US agencies on a partial-US schedule."

**Recommendation:**
- **Do not form a US LLC yet.** Run the ~$1,000, ~30-day validation pilot in [`06-validation/validation-playbook.md`](06-validation/validation-playbook.md) first. The deciding tests are Experiment 2 (does the spec-site pitch beat a generic pitch in this SMMA-saturated vertical?) and Experiment 3 (will US med spas hire an unknown offshore micro-team?).
- **If both pass:** the pivot is worth pursuing — form the Wyoming LLC, scale Cohort-C-style outreach across Tampa + Orlando.
- **If Experiment 2 fails:** stop pivot-shopping. The honest conclusion is that "AI website agency" is a structurally weak category for this team — go to a fresh brainstorm, not a third city.
- **If forced to pick right now without the pilot:** marginally prefer **staying with SG-restaurants** — not because it's better, but because the team has location/timezone/operational advantages there and a lower-cost validation path already mapped. *Best of all: validate before deciding — $1k and 30 days answers it.*

## The Bigger Picture (Read This Before Pivoting Again)

Both ideas land at ~5/10, and that's the category, not bad luck. "AI builds a spec site → we cold-outreach with it → they pay for the real one" has a wedge that's a tactic not a moat, AI tooling commoditizing under it, and an inverse relationship between ACV and market openness. **If the team wants a >7/10 idea, the move isn't a better city — it's pairing the website build with something incumbents do poorly *and recurringly* (a retained service, not a one-shot project), in a vertical that isn't SMMA-saturated.**

Candidates worth a fresh look — high-ish budgets, dated web presence, recurring update needs, far less agency saturation than med spas / dental / legal / home services:
- **Private preschools / Montessori / independent K-12** — parents judge enrollment partly on the website; owners are educators not techies; annual enrollment cycles = recurring updates; low SMMA saturation; ~$3–8k builds.
- **Senior living / assisted living facilities** — families choose based on the website; high LTV per resident placement; facilities often have dated corporate sites; less SMMA-targeted.
- **Veterinary specialty / emergency hospitals** — good margins, dated sites, less SMMA-targeted than general vet.
- **Custom home builders / high-end remodelers** — huge project values ($200k–$2M+), often weak web presence, less saturated than HVAC/roofing.
- **Country clubs / private golf clubs** — members judge by the site, real budgets, dated sites, almost no SMMA competition.

A focused validation pass on one of these (same method as this doc) would likely beat both the SG and US med spa scores.

## Documents

- [`00-intake/pivot-brief.md`](00-intake/pivot-brief.md) — pivot context, what carries over, decision frame
- [`01-discovery/findings-synthesis.md`](01-discovery/findings-synthesis.md) — the meat: what's better, what's worse, channel reality, best metro
- [`01-discovery/raw/`](01-discovery/raw/) — agent research outputs (competitors, market, gtm, operations)
- [`05-financial/unit-economics.md`](05-financial/unit-economics.md) — pricing, COGS, CAC, LTV, 12-month scenarios, SG comparison
- [`06-validation/validation-playbook.md`](06-validation/validation-playbook.md) — 5 experiments (0–4) to run before forming an LLC
- [`06-validation/kill-criteria.md`](06-validation/kill-criteria.md) — 7 pre-committed stop/pivot conditions + the meta-kill
- [`06-validation/scorecard.md`](06-validation/scorecard.md) — scored 5.0/10, dimension-by-dimension vs SG

**Not done (focused pass — out of scope):** brand, product spec, full strategy docs, 30-day calendar. If the pilot passes, expand to a full run then.

---

## Flags

**Red Flags:**
- The US med spa web/marketing market is a mature, crowded vertical, not greenfield — and the pivot doesn't escape the core weakness that "AI website agency" is a structurally weak category for a 2-person bootstrap.

**Yellow Flags:**
- Per-metro independent SAM is small (~150–350) and the switchable fraction smaller; metro counts are estimates pending a manual audit.
- Spec-site lift for med spas specifically is unproven (all evidence is general B2B from vendor sources).
- Offshore-trust discount is unmeasured; timezone tax is real and its 6–12-month sustainability untested.
- Form 5472 / ECI tax treatment needs a paid accountant opinion before the first invoice — $25k+ mistake if mishandled.

## Sources
- `01-discovery/raw/competitors.md`, `raw/market.md`, `raw/gtm.md`, `raw/operations.md` — full citation lists
- AmSpa State of the Industry (2024 report / 2023 data); PatientGain pricing; joinmoxie.com; joinblvd.com; mangomint.com — Tier 1
- Instantly / Belkins / Expandi cold-outreach benchmarks 2025–26 — Tier 2
- Stripe Atlas docs; IRS ECI page — Tier 1; tax-advisory blogs — Tier 2
- `../ai-website-sg-restaurants/` — prior project (model mechanics, wedge evidence, baseline scores)
