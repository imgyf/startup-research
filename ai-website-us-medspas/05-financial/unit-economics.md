# Unit Economics — US Med Spa Website Agency (Pivot)

**Phase:** Pivot financial pass
**Project:** ai-website-us-medspas
**Date:** 2026-05-11
**Confidence:** Medium (ACV and tooling cost well-grounded; conversion rates and channel mix are estimates pending a live pilot)

---

## Pricing Model

| Tier | Price (USD) | Includes | Margin |
|------|-------------|----------|--------|
| **Core build** | 5,000–7,000 one-time | 6–10 page custom site, HIPAA-aware hosting, before/after gallery (consent-tracked CMS), booking-widget embed (link-out to spa's Boulevard/Mangomint/Vagaro), FTC-compliant testimonials, WCAG-AA pass, Google Business Profile refresh, on-page SEO, 30-day support | ~80% gross |
| **Lite build** | 3,000–4,000 one-time | 4-page site, GBP, booking embed, basic SEO — for budget objectors / brand-new spas | ~70% gross |
| **Maintenance retainer** | 200–400/mo | Content updates, new-treatment pages, photo uploads, monthly review responses, GBP management, light SEO | ~70% margin |
| **Premium retainer (optional, later)** | 1,000–2,500/mo | + paid ads management, monthly content, conversion optimization — competes head-on with Growth99/PatientGain (only attempt once you have case studies) | ~50% margin |
| **Add-ons** | 500–2,500 | Pro photo/video shoot (subcontract), copywriting, additional landing pages, online-store setup | 50–80% |

**Reasoning:** US med spa website builds run $4–10k from competent shops (up to $10–20k creative-led). Pricing at $5–7k for the core build is mainstream — *not* a discount play (unlike SG). The maintenance retainer at $200–400/mo is the realistic LTV ladder; the premium retainer is the "become a real agency" path but means competing directly with entrenched incumbents.

## Cost Structure

| Line | Cost (USD) | Notes |
|------|-----------:|-------|
| AI tooling per site (Lovable/v0/Cursor seat amortized + API) | 30–80 | Avoid Bolt (no HIPAA/SOC2) |
| HIPAA-aware hosting + domain (Year 1, prepaid) | 50–120 | Compliant host or compliant form/booking embed |
| Founder time per build at $40/hr blended × 12–25 hr | 480–1,000 | The real cost — includes QC, client revisions, compliance setup |
| Stripe fees on a $6k invoice (~2.9% card / cheaper ACH) | 30–175 | Push ACH for the deposit |
| **Total COGS per core build** | **~600–1,400** | → **gross profit $3,600–6,400 per build (60–90%)** |

**Fixed monthly costs (months 1–6):**
| Line | USD/mo |
|------|-------:|
| Cold email infra (Instantly/Smartlead + warmed domains) | 100–250 |
| Data/enrichment (Apollo/Clay low tier) | 50–150 |
| AI tooling subscriptions (Lovable Pro + Cursor ×2) | 65–130 |
| AmSpa membership (annualized) | 35–70 |
| US LLC registered agent + accountant (annualized) | 35–60 |
| LinkedIn Sales Nav (optional) | 0–100 |
| **Total** | **~320–810/mo** |

Plus one-time: US LLC formation + EIN (~$500–1,000), business cards / brand basics (~$100), accountant setup consult (~$200–400). **All-in launch cost ~$1,000–1,800** — within the ~USD 3.7k budget, with the EIN's 4–8 week wait being the schedule constraint.

## Customer Acquisition Math

**Cash CAC:** very low — < $300/client, near-zero ad spend. The constraint is *time*, not money. Good fit for a cash-poor team.

**Time CAC (the real number):**
- Pre-build a spec site + research a prospect ≈ 1–3 hr ≈ $50–150 of founder time
- To land 1 client: ~5–10 demos → ~50–150 spec sites sent → ~50–150 hr ≈ **$2,500–7,500 of founder time per client** if you pre-build every prospect
- If you only pre-build for *warm replies* (send a "want me to mock yours up?" first, build on yes): time CAC drops to **~$500–1,500/client**
- **Recommendation: hybrid** — pre-build a small batch (~20–30) to seed the pilot and prove the wedge, then switch to build-on-warm-reply once you have demo conversion data

**Sales cycle:** ~2–6 weeks from first touch to signed (SMB, owner-decision, mid-4-to-low-5-figure ticket). Expect ghosting and "after Q3" delays from busy clinician-owners. The spec site compresses the cycle (decision = "do I like this?" not "should I get a website?").

## LTV

- Core build only: ~$6,000
- + 30% maintenance attach × $300/mo × 18-mo avg life: **+$1,620 blended LTV**
- + 50% attach: +$2,700 blended LTV
- **Blended LTV (30% attach): ~$7,600** → vs cash CAC < $300 → **LTV/CAC > 25× on cash**; on *fully-loaded* time CAC ($3,000–7,500 build-every-prospect) it's ~1–2.5× early, improving to ~5–15× once you switch to build-on-warm-reply

**The honest read:** unit economics per deal are *excellent* (60–90% gross margin, $3.6–6.4k gross profit per build). The bottleneck is **deal volume in a saturated market with a 2-person offshore team** — not margin.

## Revenue Scenarios — 12 Months

Assumptions: closes/month ramp from a cold start; ~$5,500 blended ACV (mix of Core/Lite); 30% maintenance attach; both founders selling part-time on a partial-US schedule.

| Scenario | Closes/mo (M1→M12) | Total Y1 closes | Y1 build revenue | Y1 maintenance (annualized exit) | Total Y1 revenue |
|----------|---------------------|----------------:|-----------------:|--------------------------------:|-----------------:|
| **Conservative** | 1 → 3 | ~22 | ~$121k | ~$24k | **~$145k** |
| **Base** | 2 → 6 | ~45 | ~$248k | ~$50k | **~$298k** |
| **Optimistic** | 3 → 10 | ~70 | ~$385k | ~$120k | **~$505k** |

**Comparison to SG-restaurants base case (~SGD 266k ≈ USD ~200k):** the US-medspas base case (~$298k) is **~1.5× the SG base case in revenue terms** — the higher ACV does show up. But it's a wider range (saturation makes the conservative case more likely) and the gross-margin dollars per founder-hour are similar once you account for the heavier compliance/revision load on US med spa builds and the timezone tax.

## Break-Even

Fixed costs (incl. modest founder draw of ~$2,500/mo each = $5,000) + ~$600/mo variable infra ≈ **~$5,600/mo**. At ~$4,500 gross profit per blended build, break-even ≈ **~1.3 closes/month** — easily cleared by the base case from month 2–3, and even the conservative case clears it by ~month 4. The ~$3.7k starting buffer must absorb months 1–2.

## Sensitivity (±30% on key variables, base case)

| Variable | Base | −30% Y1 revenue | +30% Y1 revenue |
|----------|------|----------------:|----------------:|
| Close rate | | ~$209k | ~$387k |
| Blended ACV ($5,500) | | ~$209k | ~$387k |
| Maintenance attach (30%) | | ~$283k | ~$313k |
| Time CAC (build-every-prospect vs build-on-warm) | | margin ±10% | margin ±10% |

**Worst-case stress (all −30%): ~$130k Y1 revenue** — cash-positive but thin founder draws. **Best-case (+30%): ~$480k** — funds a first hire by month 6.

---

## Flags

**Red Flags:**
- **Per-deal economics are great; deal flow is the risk.** In a saturated market, the conservative scenario (~$145k) is at least as likely as the base case. A 2-person offshore team's volume ceiling — bounded by spec-site production capacity *and* a partial-US selling schedule — is the binding constraint.

**Yellow Flags:**
- Time CAC of $2.5–7.5k/client (if pre-building every prospect) eats most of the gross profit on the first deal — the hybrid (seed batch, then build-on-warm-reply) is essential, not optional.
- All conversion rates are estimates from general B2B benchmarks — no med-spa-specific data. A 200-prospect pilot must measure the real numbers before scaling.
- Premium retainer revenue (the bigger LTV) means competing head-on with Growth99/PatientGain — don't model that as easy money.

## Sources
- `01-discovery/findings-synthesis.md` and `raw/*` (this project)
- AmSpa marketing-spend data (5–12% of revenue; ~$3–7k/mo median) — Tier 1/2
- US web build pricing $4–10k+ — Tier 2 triangulated
- Cold-outreach benchmarks (Instantly/Belkins 2025–26) — Tier 2
- `../ai-website-sg-restaurants/05-financial/revenue-model.md` — comparison baseline
