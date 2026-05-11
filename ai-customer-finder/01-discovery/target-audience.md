# Target Audience — AI Customer Finder

**Phase:** Phase 3 — Market Research (synthesis)
**Project:** ai-customer-finder
**Date:** 2026-05-11
**Confidence:** Medium (customer-voice grounded in forums/reviews — Tier 3; some Reddit quotes reconstructed from search indices)

> Built from `raw/wave3-customers.md` and `raw/wave4-vertical-distribution.md`. Pain language is sourced from r/sales, r/recruiting, r/SaaS, r/Entrepreneur, IndieHackers, HN, G2/Capterra/Trustpilot, vendor-critique blogs.

---

## Who we're actually building for

After the brainstorm + research, the recommended primary persona is **the owner/principal of a small staffing or recruiting agency** (and the senior recruiter/BD person inside one). Secondary/expansion persona: **independent freight brokers / small 3PLs finding shippers**. The generic "any small business" persona from the original idea is explicitly rejected — it's not a person you can build a product or a go-to-market for.

### Persona 1 (PRIMARY) — "Dana, the boutique recruiting agency owner"

- **Role:** Owner / managing director of a 1–15 person contingency or retained recruiting firm (or a solo "desk" recruiter). Often a former in-house recruiter or salesperson who went independent.
- **Specialization:** Places specific roles in a specific niche (e.g., "senior backend engineers at Series A–C startups," "RN travel nurses," "manufacturing plant managers in the Midwest," "Salesforce admins").
- **The job-to-be-done:** *"Keep my desk full of client companies who need the roles I place — and find them before my competitors do."* Candidate sourcing they're good at; **business development (winning client companies) is the bottleneck and the part they hate / are weakest at.**
- **Current workflow:** Manually scans LinkedIn Jobs / Indeed / company career pages for relevant openings; gets "job change" alerts; cold-calls/emails hiring managers; works referrals and their network; pays for Bullhorn/Loxo/Crelate (ATS), maybe SourceWhale or LinkedIn Recruiter; some buy stale "companies hiring" lists.
- **Pains:** It's reactive and slow ("by the time I see the job posting, 3 other agencies have called"); no good signal for *which* companies are in pain *now* (a role open 90 days, a reposted req, a hiring spike, fresh funding); the ATSes treat BD as an afterthought; lists are stale; outreach gets ignored.
- **Willingness to pay:** Solo recruiter ~$99–$299/mo on a card; agency (2–15 seats) ~$499–$1,500/mo. **Resists annual contracts** (the ZoomInfo experience scarred the broader market). Will pay more — even outcome-based — if it demonstrably produces booked client meetings.
- **Where to reach them:** r/recruiting (~150K), r/staffing, agency-owner Facebook groups, recruiting Slack communities, the Recruiting Brainfood newsletter (Hung Lee), RecruitingDaily, podcasts (Secrets of Staffing Success, The Elite Recruiter, RecruiterCast, The RAG). Highly clustered — a solo founder *can* reach them with content + community + a data report.
- **Buying behavior:** Pragmatic, ROI-driven, time-poor, somewhat tool-fatigued, allergic to lock-in. Trusts peer recommendations and visible domain credibility over slick marketing. Will try a free trial; will churn fast if it doesn't produce.

### Persona 2 (EXPANSION) — "Marco, the independent freight broker"

- **Role:** Solo or small-team freight broker / 3PL agent.
- **JTBD:** *"Find shippers who have freight to move and aren't locked into a broker — and get to them before the next guy."*
- **Current workflow:** DAT/Truckstop for loads, cold-calling from stale "shipper lists," referrals.
- **Pains:** "Find me shippers" is essentially un-tooled; lists are garbage; it's a grind.
- **WTP:** Similar band ($99–$299/mo solo). Reachable via r/FreightBrokers, FreightWaves, broker training programs.
- **Note:** Validate *after* Persona 1; don't split focus at MVP.

### Personas explicitly NOT targeted (and why)
- **"Any small business owner"** — not a coherent buyer; no shared workflow, channel, or data. (The original idea's fatal flaw.)
- **Solo consultants / fractional execs / indie SaaS founders** — feel the pain most acutely but have ~$0–50/mo budget and want *outcomes*, not tools. Worst monetization. (Possible *much* later, as a self-serve down-market product.)
- **Mid-market RevOps teams** — already served (Clay, Apollo, ZoomInfo, Unify); we can't out-data or out-fund them.
- **Marketing/dev agencies finding their own clients** — that's the horizontal market wearing a costume; no data moat; too-noisy channel.

## Pain hierarchy (ranked, from the research)

1. **"Finding the customers" is the real bottleneck** — not closing them. ("Most indie founders doing $0 aren't distribution-constrained — they're *specificity*-constrained." — IndieHackers.) For recruiters specifically: candidate sourcing is solved, *client* sourcing isn't.
2. **Prospecting is emotionally corrosive and low-yield** — ~95% of cold emails get zero reply; "brutal," "crickets," "soul-crushing."
3. **The tools bought to fix #1/#2 don't deliver and burn money/domains** — AI SDR churn ~50–70%/yr; "0 meetings in 6 months on a $45K contract"; "warmup pool burned my domains"; ZoomInfo "scandalous" pricing + auto-renew traps; Clay "needs an expert"; Apollo "sneaky credit games."
4. **Stale / shared / commoditized leads** — list vendors sell garbage; Angi sells the same lead to 3–8 contractors ("race to the bottom").
5. **No signal for *timing*** — buyers know *who* their ICP is; they don't know *who's in pain right now* or *how to get a warm intro*.

## Language map (use these words; avoid the others)

| They say (use) | They don't say / dislike (avoid) |
|---|---|
| "keep my desk full," "fill my pipeline," "find me clients/companies," "who's hiring for X" | "go-to-market motion," "ICP orchestration," "revenue engine" |
| "warm intro," "someone who already raised their hand," "a reason to call" | "cadence," "sequence," "spray," "blast" |
| "before my competitors," "first to the hiring manager" | "10x your outbound," "scale your outreach" |
| "is this thing actually going to get me meetings?" | "AI agent," "autonomous SDR" (← *especially* avoid — the 11x stink is on this phrase) |
| "month to month," "no contract," "let me try it" | "annual commitment," "talk to sales," "enterprise plan" |
| "stop wasting my time on dead accounts" | "data enrichment waterfall" |

**[Opinion]** The product's marketing language should sound like a sharp recruiter peer, not a sales-tech vendor. Lead with "we tell you which companies to call this week and why" — not "AI-powered prospecting agent."

## "Tried and hated" (verbatim / near-verbatim)

- *"Used 11x for six months, but they had 0 meetings to show for it."* / *"Only 1 lead after 6 months"* on a ~$45K/yr contract (≈ $22.5K per lead) — Trustpilot / Iliya Valchanov public post. [Tier 3]
- ZoomInfo *"aggressively insisted on enforcing another 12-month contract"* after a missed 60-day cancellation window, *"despite the product not being a good fit"*; pricing *"absolutely scandalous."* [Tier 3, paraphrase]
- *"It has a steep learning curve... if you're sending under 10k emails per month I don't think it's worth it"* — on Clay. Plus the credit system *"can punish experimentation."* [Tier 3]
- *"[Apollo] arbitrarily started to charge us the full amount... had to dispute via Amex"*; *"plays sneaky games with credits to force you to upgrade."* (G2 4.7 vs Trustpilot 2.9.) [Tier 3]
- *"the warming-up pool is burning your domains"*; deliverability *"dropped 30–40% after switching to shared warmed accounts"* — Instantly/Smartlead. [Tier 3, paraphrase]
- *"159 contacts, 0 meaningful replies so far... cold outreach being brutal"* — IndieHackers. [Tier 3]
- Home services: effective CAC *">$1,400 per booked job on Angi"*; leads sold to *"3–8 contractors simultaneously."* [Tier 2/3]

## What actually works (so we build the right thing)

In rough order of effectiveness reported by practitioners:
1. **Referrals** and **strategic referral partners**.
2. **Warm email to people who already engaged** (event attendees, content responders, past contacts) — not cold strangers.
3. **Community participation** ("help first, mention second" — find people "raising their hand").
4. **Visible expertise / content** in the niche.
5. **Vertical specialization** (generalists lose).
6. **Owned SEO / Google LSA** (for contractors).
7. **Cold outbound — only if hyper-segmented + a real offer** (SaaStr's 6.7% reply rate came from ~100 micro-segments across ~1,000 contacts, not a 50K blast).

**Pattern: warm + specific + intent/community-sourced wins; cold + generic + high-volume AI spray fails.** The product should optimize for *the right 20 accounts this week and the warmest way in*, not *5,000 emails sent*.

## Jobs-to-be-done summary

| When... | I want to... | So that... |
|---|---|---|
| my pipeline of client companies is thinning | know which companies in my niche are hiring (or distressed: reposted/aged reqs, hiring spikes, funding) *right now* | I have warm reasons to reach out before competitors do |
| I'm about to reach out | get the right hiring-manager contact + a tailored, non-generic opener + a warm path if one exists | I actually get a reply / a meeting |
| I'm deciding where to spend my limited selling time | see accounts ranked by "likelihood they need me now," not an undifferentiated list | I stop wasting hours on dead accounts |
| I want to know it's working | see meetings booked / replies, not "emails sent" | I can justify the spend and not churn |

## Channels to reach this audience (preview — full plan in Phase 4 go-to-market)

Dogfood the product as outbound (target growth-mode staffing agencies) → niche communities (r/recruiting, agency-owner FB groups, recruiting Slacks) → industry newsletters/podcasts (lead with a "State of Agency BD" data report from aggregate job data) → SEO/programmatic ("companies hiring [role] in [city]," "SourceWhale alternative") → partnerships (Loxo/Crelate/Recruiterflow/Bullhorn marketplace, ASA) → marketplaces (ATS app directories, G2/Capterra) → small disciplined paid tests last. GTM here is mostly *time*, not *money* — which fits a nights/weekends technical founder.

---

## Flags

**Red Flags:**
- The audience that feels the pain *most* (solo consultants, indie founders) has the *least* budget and wants outcomes, not tools — do not build for them first; it's a monetization trap.
- The word "AI SDR / AI agent" is damaged with this audience — using it in positioning inherits the 11x trust deficit.

**Yellow Flags:**
- This audience is tool-fatigued and churns fast — onboarding-to-first-value must be very short or retention collapses.
- They resist annual contracts hard — pricing/packaging must be month-to-month-friendly, which hurts cash predictability.
- Customer-voice evidence is mostly Tier 3 (forums/reviews) and some Reddit quotes are reconstructed from search indices — directionally sound, but the founder should confirm with 20–30 real conversations (Action Plan Week 1) before betting the product on it.

## Sources
- `raw/wave3-customers.md` — Reddit (r/sales, r/recruiting, r/SaaS, r/Entrepreneur, r/msp, r/FreightBrokers), Hacker News, IndieHackers, G2/Capterra/Trustpilot reviews, vendor-critique blogs — Tier 3, treated as sentiment evidence not hard data; flagged inline where reconstructed.
- `raw/wave4-vertical-distribution.md` — ASA/SIA staffing data (Tier 1), community/newsletter/podcast inventory (Tier 2–3), vendor pricing.
