# Validation Playbook — US Med Spa Pivot

**Phase:** Pivot validation
**Project:** ai-website-us-medspas
**Date:** 2026-05-11
**Confidence:** High (experiments are concrete; outcomes unknown by construction)

---

## Principle

The pivot's open questions are different from Singapore's. There, the question was "does the spec-site wedge convert at all in this market." Here, the wedge is more plausible (visual buyers) but the market is **saturated** and the team is **offshore** — so the validation must test: *can a 2-person Singapore team actually win deals against entrenched US agencies, on a partial-US schedule, before sinking real time into a US LLC?*

Run these in order. The first two cost almost nothing and can kill the pivot before you form an entity.

---

## Experiment 0 (Day 0–2): Desk Audit — "How saturated is one metro, really?"

**Cost:** 1 day, $0.
**Tests:** Is the addressable independent SAM real, and how bad are the incumbent sites?

1. Pull 60–100 med spas in Tampa + Orlando (and 40 in DFW for comparison) from Google Maps + the AmSpa member directory.
2. For each, record: independent vs franchise/chain vs PE-portfolio (exclude the latter two); current site quality (1–5: none/one-pager → dated template → decent → good → excellent); is it on Wix/Squarespace/GoHighLevel/custom; does it have a before/after gallery; does it embed Boulevard/Mangomint booking; any visible agency footer credit.
3. Count: how many *independent* spas with a 1–3 site = your real warm SAM in that metro.

**Success criteria:** ≥80 independent spas with a 1–3 site across Tampa+Orlando (enough to run a 200-prospect campaign over 2–3 months). **Kill signal:** <40 → the metro SAM is too thin; pick a different metro or reconsider the pivot.

---

## Experiment 1 (Day 1–3): Engineering Spike — "10 HIPAA-aware med spa spec sites in 1 day"

**Cost:** 1 day, < $30 compute + a Lovable Pro / Cursor seat.
**Tests:** Per-site cost, time, quality — for *med spa* sites specifically (before/after gallery, booking embed, compliance-aware structure).

1. Pick 10 of the 1–3-rated independent spas from Experiment 0.
2. Build each: 6-page site, real menu of treatments scraped from their current presence, before/after gallery as an owner-editable CMS with a consent field, a *placeholder* booking-embed slot (don't wire real PHI), FTC-style testimonial section, WCAG-AA basics. Use Lovable/v0/Cursor — **not Bolt** (no HIPAA/SOC2).
3. Measure: time/site (target ≤90 min — med spa sites are heavier than restaurant sites), compute cost/site (target ≤$3), and have a non-founder rate visual quality (1–10, target ≥7.5) *and* a quick "would a med spa owner think this looks more premium than [their current site]?" yes/no.

**Success criteria:** ≤90 min/site, ≤$3/site, ≥7.5/10 quality, ≥8/10 "more premium than current." **Kill signal:** >2.5 hr/site or quality <6 → delivery isn't fast/good enough to make the volume math work; fix tooling or reconsider.

---

## Experiment 2 (Day 3–21): Cold-Outreach Pilot — "Does the wedge beat the noise in a SMMA-saturated vertical?"

**Cost:** ~$200 (email tool month + data) — no US LLC needed yet; send from a `@yourbrand.com` you already control or a cheap secondary domain.
**Tests:** Real reply rate, demo-booking rate, and whether the spec site beats a generic pitch *for med spas who already get pitched constantly*.

Build 60 more spec sites (capacity test). Split into three cohorts of 40 prospects each, matched on site quality:
- **A — Generic pitch:** "We build conversion-focused med spa websites, here's our portfolio."
- **B — Diagnostic pitch:** "Your site is missing X, Y, Z that's costing you bookings — here's a 3-min Loom showing the gaps." (no spec site)
- **C — Spec-site pitch:** "I rebuilt your site. Here's the live preview: [link]. Built it in an afternoon — want the real, customized version?"

Same subject-line variants, same send window, same domain reputation. Channel: email primarily; mirror a smaller LinkedIn version (20 owners per cohort) for the metros' larger practices.

**Track:** open, click-to-preview, reply, demo booked, and (over the following 4 weeks) signed. **Success criteria:** Cohort C reply rate ≥2× Cohort A *and* ≥1.3× Cohort B (i.e., the *built site* adds meaningfully over just a diagnostic); ≥3 demos booked from C; ≥1 signed from C within 6 weeks. **Kill signal:** Cohort C ≈ Cohort A → in this vertical the wedge is theatrical, not real; or all cohorts < 1% reply → med spa owners are too pitch-fatigued to reach cold — reconsider the channel or the vertical.

---

## Experiment 3 (Day 7–25): Trust Test — "Will a US med spa hire an unknown offshore 2-person team?"

**Cost:** founder time + ~$30 for coffees-equivalent (gift cards for interviews).
**Tests:** The offshore-trust discount — the biggest unmeasured operational risk.

1. From Cohort C demos (and any warm replies), run the demo calls on a partial-US schedule (one founder, 8pm–1am SG = 7am–noon CT).
2. On each call, deliberately surface "we're a Singapore-based studio" early and watch the reaction. Ask non-buyers afterward: "was the location a factor? what would have made you comfortable?"
3. Tag objections: PRICE / TRUST-OFFSHORE / TRUST-SMALL-TEAM / TIMING / DON'T-NEED-IT / ALREADY-HAVE-AGENCY.

**Success criteria:** "TRUST-OFFSHORE" is <30% of objection weight *and* at least one client signs knowing you're offshore. **Kill signal:** TRUST-OFFSHORE >50% → you need a US-based face (a US contractor doing sales calls, a US co-founder, or relocation) before this is viable — a much bigger lift.

---

## Experiment 4 (Day 4–25, parallel): Partner & Compliance Probe

**Cost:** founder time + AmSpa Basic membership ($395) + a $200–400 accountant consult.
**Tests:** The two slow-burn realities — partner channels and the US-tax/entity setup.

1. Join AmSpa Basic; list in the vendor directory; DM 5–10 med spa consultants/coaches on LinkedIn about referral arrangements.
2. Book a 30–60 min consult with a US international-tax accountant: confirm the Wyoming LLC + EIN + Wise/Stripe setup, the ECI/Form-5472 obligations, and a realistic timeline.
3. Confirm Wise/Relay will approve you with the business address you'll actually use (not a registered-agent address — Mercury and others reject those now).

**Success criteria:** ≥2 consultants express willingness to refer; accountant confirms the setup is clean and ~$300–600/yr ongoing; Wise/Relay pre-qualifies. **Kill signal:** tax treatment is messy/expensive for this exact setup, or you can't get a US business bank account → operational friction may outweigh the ACV upside.

---

## Decision Framework — End of ~30 Days

| Outcome | Action |
|---------|--------|
| Exp 0–3 all pass (real SAM, fast delivery, wedge beats noise, offshore-trust OK), ≥1 signed | **GO** — form the Wyoming LLC, scale Cohort-C-style outreach across Tampa+Orlando |
| Wedge works (Exp 2) but offshore-trust fails (Exp 3) | **Conditional** — find a US-based sales face before scaling; or pivot to selling *through* US consultants/agencies as a white-label spec-site sub-vendor |
| SAM is thin (Exp 0) but wedge works | Add metros (Scottsdale, Nashville, Charlotte) or broaden to adjacent cash-pay healthcare (dermatology, plastics, dental — but those are *more* saturated) |
| Delivery too slow (Exp 1) | Fix tooling/templates, re-test; if still slow, the volume math doesn't close — drop the pivot |
| Wedge ≈ generic pitch (Exp 2) | **Drop the pivot.** In a SMMA-saturated vertical with no wedge advantage and offshore friction, this is worse than the SG idea — and the SG idea was already only CONDITIONAL. Go back to brainstorming a category that isn't "another website agency." |
| Operational/tax friction too high (Exp 4) | Reconsider — maybe a non-US English market (Australia: Gold Coast/Sydney med spas — same wedge, far less SMMA saturation, dense enough for occasional in-person, AUD strong, friendlier timezone) |

---

## What This Plan Costs

| Line | USD |
|------|----:|
| Email tool + data (1 month) | ~200 |
| AI tooling seats (1 month) | ~100 |
| AmSpa Basic membership | 395 |
| Accountant consult | 200–400 |
| Domains (secondary, warmed) | ~45 |
| Interview gift cards | ~30 |
| **Total** | **~$1,000–1,200** |

You spend ~$1k and ~30 days to learn whether the pivot is better than the thing you already had. The US LLC (~$500–1k more) only happens *after* Exp 0–3 pass.

---

## Flags

**Red Flags:**
- The kill signal on Experiment 2 (wedge ≈ generic pitch) is a real possibility in this vertical — and if it triggers, the honest conclusion is that *both* the SG and US versions of "AI website agency" are weak, and the team should brainstorm a fundamentally different idea rather than pivot-shopping for a better city.

**Yellow Flags:**
- Running demo calls on a partial-US schedule during the pilot is itself a test of whether the team can sustain that for a year — watch for burnout signals, not just conversion data.

## Sources
- `01-discovery/findings-synthesis.md`, `01-discovery/raw/*`
- `05-financial/unit-economics.md`
- `../ai-website-sg-restaurants/06-validation/*` — prior validation design
