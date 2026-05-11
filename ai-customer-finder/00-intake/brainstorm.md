# Brainstorm — AI Customer Finder

**Phase:** Phase 2 — Brainstorm
**Project:** ai-customer-finder
**Date:** 2026-05-11
**Confidence:** Medium (idea-space exploration; not yet validated by research)

---

## Why this phase matters here

The raw idea ("AI finds any business its customers") is too broad to build. The job of this phase is to generate sharper, *narrower* variations and find the one where a solo technical founder on nights/weekends has a real chance — i.e., where "technical + fast + cheap" is actually an edge, the data is gettable without licensing deals, and the buyer pays for leads today.

## Variations

### V1 — Horizontal "AI prospecting agent for everyone" (the original)
Describe what you sell → agent returns a list of matching companies/people, enriched, with intent signals; optionally drafts outreach.
- **Exciting:** Biggest TAM; simple pitch.
- **Risky/hard:** Direct collision with Apollo, ZoomInfo, Clay, 11x, Artisan, Instantly, Smartlead, Unify, AiSDR, etc. — all funded ($50M–$1.6B). No data moat, no distribution edge. **Verdict: do not build.** Kept only as the baseline.

### V2 — Vertical AI BD agent for **staffing & recruiting agencies** ("find me companies to staff for")
Recruiting/staffing firms make money when they fill client roles. Their "customers" = companies with open reqs. Job-posting data is abundant and publicly scrapable; the *candidate-side* is well-served (SeekOut, hireEZ, Loxo) but the *business-development side* (winning new client companies) is underserved. Agent monitors job boards + company signals, surfaces "this company just posted 4 roles you specialize in, here's the hiring manager + a tailored pitch," tracks which agencies already have the contract.
- **Exciting:** ~20k+ US staffing firms, they live and die on BD, they already pay for tools, ICP is crisp, data is scrapable, "technical + fast" matters because the signal-engineering is the product.
- **Risky/hard:** Agencies are price-sensitive and notoriously cheap on software; some overlap with Loxo/Crelate CRMs adding "BD" modules; job-posting scraping is an arms race.

### V3 — Vertical AI prospecting agent for **B2B service agencies & consultants** (marketing agencies, dev shops, fractional execs)
"Find companies that just [raised a round / hired a VP Marketing / launched a product / lost a key person / are running broken ads]" → warm-trigger prospect lists + drafted outreach, tuned to what the agency sells.
- **Exciting:** Millions of solo consultants & small agencies; acute, recurring pain (pipeline); will pay $50–200/mo on a card; self-serve.
- **Risky/hard:** This is *exactly* what Clay, Unify, Common Room, and "signal-based selling" tools already do (just not packaged for tiny agencies); low switching cost; churny segment.

### V4 — Vertical AI lead agent for the **construction / trades supply chain** (subs finding GCs & projects; suppliers finding contractors)
Aggregate permits, bid boards, plan rooms, project announcements, contractor licensing data → "these 7 upcoming projects in your trade + radius, here's the GC and the estimator to call."
- **Exciting:** Enormous, fragmented industry; incumbents (ConstructConnect, Dodge, BuildingConnected/Autodesk, PlanHub) are expensive ($3k–15k/yr) and widely disliked; buyers already pay big for leads.
- **Risky/hard:** Data acquisition is genuinely hard and partly licensed/regional; sales cycle is slow; field-heavy onboarding — **a poor fit for nights/weekends, limited cash.** Strong business, wrong founder/resourcing.

### V5 — Vertical AI lead agent for **home-services contractors** (roofing, solar, HVAC, remodeling)
Find homeowners with intent: storm/hail events, old roofs (aerial imagery), recent home purchases, permit filings, expiring warranties → ranked door-knock / call lists.
- **Exciting:** Contractors spend heavily on leads (Angi, HomeAdvisor, lead brokers at $30–150/lead); intent data exists; high willingness to pay.
- **Risky/hard:** Crowded with lead-broker incumbents and storm-tracking tools; consumer-PII/TCPA exposure on outreach; needs imagery/property data partnerships; local-sales motion. Not a clean solo-bootstrapper play.

### V6 — "**Lookalike-from-your-best-customers**" agent (any B2B, but the wedge is the *input*, not the vertical)
User connects their CRM / uploads their 20 best customers → agent reverse-engineers the real ICP (firmographic + technographic + behavioral patterns the user can't see) → finds the closest matches + explains *why* each is a match. Niche down later by being the best at "what does my actual best customer look like, and who else looks like that."
- **Exciting:** Differentiated *angle* (insight, not just a list); demos well; "AI/ML founder" is genuinely the edge here (it's a modeling problem); CRM-connected = stickier.
- **Risky/hard:** Still needs an underlying contact/company dataset (buy from a reseller, or scrape) — that's the expensive/risky part; Clay, Keyplay, Common Room, Pocus, and ZoomInfo "lookalikes" already exist; "explain the match" is a feature, not a moat, for long.

### V7 — Narrow it by *channel* not industry: **"AI customer finder for people who hate cold email"** — i.e., warm-intro & community-signal sourcing
Instead of "scrape + spam," the agent finds prospects via paths the user can actually open: mutual LinkedIn connections, alumni overlap, customers of your customers, people active in relevant communities/subreddits/Slack groups, podcast guests, conference attendees → "here are 12 reachable buyers and the exact warm path to each."
- **Exciting:** Sidesteps the deliverability death-spiral that's hurting the whole cold-email category; differentiated; aligns with where buying is actually going (referrals, communities); could pick a vertical later.
- **Risky/hard:** Warm-path data is hard to get at scale (LinkedIn graph is walled, anti-scraping); narrower per-user value; harder to prove ROI quickly.

### V8 — Productized service first, software later: **done-for-you "we'll find & book you 10 meetings" for one niche, run by your AI under the hood**
Pick one vertical (say, B2B service agencies). You operate it as a service — your AI does the prospecting/personalization, you do the human glue — at $1.5–3k/mo. Use it to learn the vertical, then productize what's repeatable.
- **Exciting:** Revenue in weeks, not quarters; forces customer contact; de-risks the "I'm a builder, not a seller" gap by making you sell *outcomes*; classic path to a vertical SaaS.
- **Risky/hard:** It's a job, not (yet) a startup; doesn't scale on nights/weekends; you become an agency competing with 10,000 agencies — unless you ruthlessly productize.

## Convergence — what resonates / recommended direction

The brutal facts: (1) the horizontal version is dead on arrival; (2) the founder's edge is *building*, not *selling* — so the wedge must be one where smart data/signal engineering is the moat and the buyer self-serves at low ACV (no field sales); (3) nights/weekends + <$10k rules out anything needing data-licensing deals or local sales (V4, V5 — good businesses, wrong fit).

That points the spotlight at **V2 (staffing/recruiting BD agent)** and **V6 (lookalike-from-your-best-customers, applied to one starting vertical)**, with **V8 (productized-service-first)** as the *go-to-market motion* for whichever product wedge wins, and **V7's "warm path, not spam"** ethos baked in to dodge the deliverability cliff.

**Recommended idea to carry into research:** A **vertical AI prospecting agent for B2B staffing & recruiting agencies** — "point it at your specialties and territory, it watches the job market + company signals and hands you a ranked list of *companies you should be staffing for*, the right contact, why now, and a tailored opener; tracks who already has the contract so you don't waste a pitch." Start with a productized-service / high-touch beta (V8) to learn the vertical, then self-serve SaaS at ~$99–299/mo per recruiter.

Why this and not the others: crisp ICP, scrapable data, real recurring pain, segment already pays for tools, "technical + fast" is the actual edge (it's a signals/ranking problem), and it's small enough that the funded horizontal players won't bother — yet there are ~20k+ US staffing firms and tens of thousands more globally, so it's not a toy.

**Open questions for research (Phase 3):** Is staffing-firm BD genuinely underserved, or do Loxo/Crelate/Bullhorn already own it? What do recruiters actually pay for BD tooling today? Is there a *better* underserved vertical with the same shape (e.g., commercial insurance brokers, MSPs/IT services, freight brokerage, wholesale/distribution)? And — does the founder even *want* to spend nights/weekends learning the staffing world? (If not, V3/V6 self-serve for consultants/agencies is the fallback.)

## Brief update needed?

No fundamental change to `00-intake/brief.md` yet — the original idea is intact, just sharpened. If research confirms a specific vertical, add a "Refined Idea" section to the brief at the start of Phase 4.

---

## Flags

**Red Flags:**
- V1 (horizontal) remains a no-go — do not let it creep back in as the "real" product "once we have traction." That's the boiling-the-ocean trap.

**Yellow Flags:**
- Every vertical option still depends on an underlying company/contact dataset the founder must either buy from a reseller (cost, ToS) or scrape (legal/maintenance risk). This data-acquisition question is the make-or-break feasibility item — it must be answered before any building. (Phase 3 + Phase 6.)
- Recommending a vertical the founder has zero affinity for risks low motivation on a nights/weekends timeline. Founder should sanity-check the staffing pick against "would I enjoy obsessing over this for 18 months?"

## Sources
- Analyst synthesis of founder intake + prior knowledge of the sales-tech / lead-gen landscape. All competitive and market claims here are **[Opinion]/[Assumption]** pending Phase 3 verification.
