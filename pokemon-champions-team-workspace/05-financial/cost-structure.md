# Cost Structure

**Phase:** 7 — Financial
**Project:** pokemon-champions-team-workspace
**Date:** 2026-05-10
**Confidence:** Medium-High (fixed costs well-bounded; LLM variable cost estimated from current API pricing)

---

## Founder Time (Opportunity Cost)

Not cash — but the largest real cost of the project.

- 15-25 hrs/week × 52 weeks = **780-1,300 hrs/year**
- Founder time-value (hobbyist+technical, market rate): **$50-100/hr**
- **Annual opportunity cost: $39K-130K**

This is the cost the project is competing against. It frames every cash decision below.

---

## Fixed Monthly Costs

### Pre-Launch (Months 1-3, build phase)

| Line | Provider | Cost | Notes |
|---|---|---|---|
| Hosting | Vercel Hobby (free) or Cloudflare Pages (free) | $0-10 | Free tiers cover pre-launch traffic |
| Database | Supabase Free or Pro starter | $0-25 | Free tier OK during build |
| Domain (incl. .com + .gg or .io) | Cloudflare Registrar | $1-2/mo amortized | One-time annual fee |
| Auth | Built into Supabase or Clerk Hobby | $0-25 | Free tier covers small user count |
| Email (transactional) | Resend Free | $0 | <3K emails/mo free |
| Stripe | Pay-per-transaction | $0 | No fixed cost; 2.9% + $0.30 per transaction |
| Analytics | Plausible Hobby | $9 | Privacy-respecting; or use Vercel Analytics |
| Error monitoring | Sentry Hobby (free) | $0 | |
| LLM API | Anthropic Claude API | $20-50 | Light dev/test usage; founder testing |
| **Total pre-launch monthly** | | **~$30-120** | |

Pre-launch total: ~$90-360 over 3 months.

### Launch & Early Growth (Months 4-6)

| Line | Cost | Notes |
|---|---|---|
| Hosting | $20-50 | Move to paid plan as traffic grows |
| Database | $25-50 | Supabase Pro or equivalent |
| Auth | $25 | Clerk Pro if Supabase auth doesn't fit |
| Email | $20 | Resend paid for transactional volume |
| Analytics | $9-19 | Plausible / Vercel |
| Error monitoring | $26 | Sentry Team |
| Domain + DNS + Cloudflare | $10 | Annualized |
| LLM API (variable, see below) | $50-200 | Light usage at <100 paid users |
| Backup / observability | $10-20 | Logflare or similar |
| **Total launch-phase monthly** | **~$200-450** | |

### Steady-State (Months 7-12, ~200-400 paid users)

| Line | Cost | Notes |
|---|---|---|
| Hosting | $50-100 | Scaled |
| Database | $50-100 | More storage and connections |
| Auth | $25-50 | More users |
| Email | $50-100 | More transactional + marketing |
| Analytics | $19-50 | Higher tier |
| Error monitoring | $26-80 | More events |
| LLM API (variable) | $400-1,200 | At ~300 paid users avg |
| Domain + DNS | $10 | |
| Backup / observability | $30 | |
| **Total steady-state monthly** | **~$650-1,700** | |

---

## Variable Costs

### LLM API (Anthropic Claude)

The single largest variable cost — and the most volatile.

**Per-Pro-user assumptions:**
- 50 coach turns/month average (heavy users hit 100; light users 10-30)
- Avg input: 2K tokens (system prompt + retrieval context + history)
- Avg output: 800 tokens
- Smart routing: 70% Sonnet 4.6, 30% Haiku 4.5 for cheaper queries
- Tool call overhead: ~30% additional tokens

**Per-turn cost (blended):**
- Sonnet 4.6: ~$0.04-0.07/turn
- Haiku 4.5: ~$0.01-0.02/turn
- Blended: ~$0.03/turn

**Per-user/month cost: 50 turns × $0.03 = ~$1.50/mo Pro**

**Per-Tournament-Prep-user/month cost:** 150 turns × $0.03 = ~$4.50/mo

**At 300 paid users (Base scenario steady state):**
- 200 Pro × $1.50 = $300
- 100 Tournament Prep × $4.50 = $450
- **Total: ~$750/mo** (within the $400-1,200 range above)

**Risk: 5x cost spike from runaway usage.** A user with broken automation (or bad prompt design on our side) could 10x token use overnight. Mitigation: per-user daily quotas, per-turn token caps, monthly cost ceiling alarm.

### Stripe Transaction Fees

- Pro $12/mo: $0.65 fee per transaction (2.9% + $0.30) = ~5.4% effective
- Pro annual $99: $3.17 fee = ~3.2% effective
- TP $25/mo: $1.03 fee = ~4.1% effective
- TP annual $199: $6.07 fee = ~3.0% effective

**Effective payment processing cost: ~3-5% of paid revenue.**

### Other Variable

- Email per-user: ~$0.001/transactional email; $0.01/marketing email — negligible at our scale
- Database I/O: included in Supabase Pro fixed price up to ~10K paid users
- CDN egress: included in Vercel/Cloudflare free tier up to >100K MAU

---

## One-Time / Episodic Costs

| Item | Estimated Cost | When |
|---|---|---|
| Logo + brand design (contractor) | $300-1,500 | Pre-launch (Month 2-3) |
| Visual/UI design help (contractor) | $1,000-3,000 | Optional, if founder velocity slips |
| Legal: TOS + Privacy Policy review | $300-800 | Pre-launch |
| Trademark search + brand check | $200-500 | Pre-launch |
| Domain costs (.com + .gg or .io) | $50-200/yr | Year 1 |
| Initial creator partnership "investment" — free Pro for top tier patrons | $0 (no cash) | Pre-launch / launch |
| Limitless tournament sponsorship | $200-500 prize pool | Month 3+ |
| Founder content production (camera/mic if needed) | $200-500 | Pre-launch |
| **Total one-time** | **~$2,250-7,000** | Spread over 6-9 months |

---

## Marketing Budget

The founder's budget is ~$500-2K/mo. Realistic Y1 marketing spend:

| Line | Monthly | Y1 Total |
|---|---|---|
| Founder content (no cash) | $0 | $0 |
| Reddit/X creator collabs (rev share, no cash) | $0 | $0 |
| Limitless community tournament sponsorship | $50-100 | $300-600 |
| Programmatic SEO content (writers if outsourced) | $100-300 | $1,200-3,600 |
| Paid creator placements (selective, post-launch) | $0-200 | $0-1,200 |
| **Total Y1 marketing cash** | **~$150-600/mo** | **~$1,500-5,400** |

---

## Break-Even Analysis

**Steady-state monthly cost: ~$1,000-1,800** (including LLM at 300 paid users + marketing).

**Break-even paid users:**
- All Pro tier ($12, ~70% margin = ~$8.40 net per user): **~120-220 paid users**
- All TP tier ($25, ~80% margin = ~$20 net per user): **~50-90 paid users**
- Realistic blend (75% Pro, 25% TP): **~100-180 paid users**

**Base scenario Year 1 reaches break-even around month 4-5** (300 paid by month 6).

---

## Total Year 1 Cash Flow

| Line | Y1 Total |
|---|---|
| **Revenue (Base)** | **+$60,000** |
| Hosting + infra (avg $400/mo × 12) | -$4,800 |
| LLM API (avg $500/mo × 12) | -$6,000 |
| Stripe fees (~4%) | -$2,400 |
| Marketing | -$3,000 |
| One-time (logo, legal, trademark) | -$3,500 |
| Founder time (opportunity cost — not cash) | $0 cash, -$39K-65K opportunity |
| **Net Y1 cash flow (Base)** | **+$40,000** before founder opportunity cost |
| **Net Y1 economic profit (Base)** | **-$15K to +$5K** after founder opportunity cost |

**At Base, the project breaks even economically within Year 1**, but barely. Optimistic clears it cleanly. Conservative loses $20-30K of founder time.

---

## Cost Risks

| Risk | Likelihood | Impact | Mitigation |
|---|---|---|---|
| LLM cost runaway from buggy feature | Medium | High | Per-user quotas + per-turn caps + monthly ceiling alert |
| Anthropic price increase | Low | Medium | Multi-provider abstraction (OpenAI, Anthropic, Google) at code level |
| Spam signups inflating LLM cost | Medium | Medium | Email verification + rate limiting on Free tier |
| Stripe dispute/chargeback storm | Low | Medium | Reserve 2-3% of revenue; clear refund policy |
| One-time costs balloon (e.g., visual design) | Medium | Low | Cap at $5K total; escalate before exceeding |
| Server cost surprise from viral moment | Low | Medium | Use Cloudflare's edge caching; set spend caps in Vercel |

---

## Flags

**Red Flags:**
- None.

**Yellow Flags:**
- LLM costs are the most volatile single line. A poorly designed feature could 5x the bill overnight. Per-user quotas at MVP are non-negotiable.
- Founder opportunity cost is the largest "cost" and is invisible to traditional accounting. Conservative scenario is *economically* a loss after this. If the project is tracking Conservative at month 6, founder should seriously reassess.
- One-time costs are bounded but logo + legal + trademark together can hit $3K-5K. Budget for that upfront.

## Sources

- `01-discovery/raw/wave4-technical.md` — LLM cost estimates
- Anthropic API pricing (Tier 1, 2026)
- Stripe pricing (Tier 1)
- Supabase, Vercel, Cloudflare pricing (Tier 1)
- `02-strategy/business-model.md` — tier pricing
- `04-product/mvp-definition.md` — feature scope and effort estimates
- `05-financial/revenue-model.md` — revenue scenarios
