# Risk Analysis

**Phase:** 8 — Validation
**Project:** ai-website-sg-restaurants
**Date:** 2026-05-11
**Confidence:** Medium (risk likelihood is estimated; impact is grounded in unit economics)

---

## Risk Matrix

Likelihood: L = Low (<25%), M = Medium (25-60%), H = High (>60%)
Impact: 1 = minor delay, 2 = quarter-scale setback, 3 = year-scale setback, 4 = existential

### Market Risks

| Risk | Likelihood | Impact | Mitigation | Early warning signal |
|------|:----------:|:------:|------------|----------------------|
| Spec-site wedge doesn't lift conversion in SG | **M** | **4** | Run Experiment 2+4 in month 1 before scaling | Walk-in tablet-look rate <40% |
| Wix Aria / Squarespace ship "cold-outreach with samples" feature | **M** | **3** | Move up-market into managed services + PSG | Wix product announcement; competitor traffic spike |
| F&B closure rate spikes (recession-like) | **L** | **3** | Diversify into adjacent verticals (clinics, salons) | F&B closures >400/month sustained 2+ quarters |
| PSG support reduced post-2027 budget | **L** | **2** | Build non-PSG sales muscle in parallel | Annual SG budget announcement |
| Owners' pain stays latent — they never feel acute need | **M** | **4** | Diagnostic pitch ("here's what you're losing"); demo at events | Interview Exp 3 shows >70% "don't see the need" |

### Product Risks

| Risk | Likelihood | Impact | Mitigation | Early warning signal |
|------|:----------:|:------:|------------|----------------------|
| AI-generated sites look generic / non-professional | **M** | **3** | Custom theme library + human design review per site | Non-founder ratings <6/10 in Exp 1 |
| Per-site compute cost exceeds SGD 5/site | **M** | **3** | Cache prompts, batch generation, template reuse | Cost-per-site tracker in dashboard |
| Customer asks for ordering checkout (out of scope) | **H** | **1** | Pre-empt in pitch: "we link to your FoodPanda/Oddle, we don't rebuild" | Repeated objection in interviews |
| Generated sites break on edge content (long menu, weird fonts) | **M** | **2** | Manual QC step; refund policy 14-day | Customer complaints in first 30 days |
| Hosting outages / domain issues | **L** | **2** | Use Vercel/Cloudflare; document handoff | Uptime <99% on monitoring |

### Business Risks

| Risk | Likelihood | Impact | Mitigation | Early warning signal |
|------|:----------:|:------:|------------|----------------------|
| Can't sustain founder draws at SGD 4k each | **M** | **3** | Either of: (a) raise pricing to SGD 1,800+, (b) co-founder takes parallel contract work, (c) accept 2-3 month dip | Bank balance trajectory |
| Maintenance attach <15% | **M** | **2** | Bundle maintenance into Standard tier at SGD 1,800 ("we keep it updated for the first year") | Attach rate after first 10 closes |
| PSG approval takes 18+ months | **M** | **2** | Don't bet on it; treat as upside | EnterpriseSG initial response |
| One-time pricing limits scale to founder hours | **H** | **2** | Bake maintenance tier and product upsells from day 1 | Revenue plateau at SGD 15k/mo |
| Founders disagree on direction | **M** | **3** | Written founder agreement; equal walk-in target/week to share pain | Inter-founder communication breakdown |

### Team Risks

| Risk | Likelihood | Impact | Mitigation | Early warning signal |
|------|:----------:|:------:|------------|----------------------|
| Walk-in burnout for co-founders | **M** | **3** | Rotate days; cap at 25 walk-ins/week each; weekly reset | Reduced output, missed days |
| One founder skill gap (sales OR engineering) | **M** | **2** | Clear role split; outsource gaps to contractors at SGD 40-80/hr | Output gap visible by week 2 |
| Co-founder exit | **L** | **4** | Vesting/cliff agreement; mutual-deck buyout terms | Pre-defined exit triggers |

### Financial Risks

| Risk | Likelihood | Impact | Mitigation | Early warning signal |
|------|:----------:|:------:|------------|----------------------|
| Month-1 revenue <SGD 3k (below break-even) | **M** | **2** | SGD 5k buffer absorbs; both founders take contract work | Week-2 sales count |
| Restaurant goes under between contract + delivery | **M** | **1** | Take 50% upfront, 50% on delivery; non-refundable spec-site | Refund requests |
| AI tooling pricing rises 50%+ | **L** | **2** | Multi-tool fluency (Lovable + v0 + Bolt); switching cost is low | Vendor pricing announcements |
| Cold email tools/email account gets banned | **L** | **2** | Multi-domain sending; reputation hygiene | Bounce rate, spam complaint rate |

---

## Top 3 Risks to Actively Manage

These have the worst likelihood × impact and need explicit mitigation work, not just monitoring:

### #1: Spec-site wedge fails to lift SG conversion (M × 4 = 12)
**Why this is #1:** The entire business thesis depends on this. If pre-built sites don't convert better than generic pitches in SG specifically, every other piece of the plan is irrelevant.
**Mitigation:**
- Experiment 2 (walk-ins) and Experiment 4 (cold email A/B) explicitly test this in month 1
- Pre-commit kill criteria: if walk-in tablet-look rate <40% AND Cohort B email reply rate <2× Cohort A, the wedge is dead — pivot
- Don't spend more than SGD 1,500 on tooling/marketing until validated

### #2: Owners' pain stays latent (M × 4 = 12)
**Why this is #2:** Customer voice research found pain is real but unvocalized. Cold outreach that asks "do you want a website?" will mostly hear "no" even when the answer should be yes.
**Mitigation:**
- Pitch must lead with a **diagnostic** (here's your Google ranking vs competitors; here's your FoodPanda monthly commission cost) before showing the spec site
- Spec site shouldn't be the opener — the *loss* should be the opener
- Test variant in Experiment 2: with vs without diagnostic frame

### #3: AI commoditization (M × 3 = 9)
**Why this is #3:** Wix Aria, Squarespace Blueprint, Durable, and others are all moving toward "AI generates a sample for prospects." Window is 6-18 months.
**Mitigation:**
- Move the value claim from "AI-built" (a feature) to "ranked on Google by Friday" (an outcome)
- Build SG-specific moats: PayNow QR templates, Oddle handshake integration, local domain registry, .sg domain expertise
- Apply for PSG approval as a long-term moat that AI tools can't replicate (regulatory not technological)

---

## Risks Explicitly Accepted (Not Mitigated)

- **High customer mortality (60% 5-year survival):** Match it with one-time pricing; accept churn as feature not bug.
- **Restricted founder draw early:** Founders have agreed to lean months 1-3 — this is a feature of bootstrap.
- **Limited venture-scale upside:** This is a bootstrapped lifestyle business in its current form. If venture-scale matters, pivot to Variation B (subscription) or Variation C (different vertical) after first 50 customers.

---

## Flags

**Red Flags:**
- **Two simultaneous M×4 risks** (spec-site lift, latent pain) make this a higher-risk validation than a typical SMB-services play. Both are testable cheaply within 30 days — that's the saving grace.

**Yellow Flags:**
- **Founder burnout risk is medium-impact and medium-likelihood** — meaningful, but typical for any 2-person bootstrap. Pre-defined rest cadence and rotation are mitigations, not eliminations.

## Sources
- `01-discovery/*` (all research files)
- Internal analysis
