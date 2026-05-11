# Competitor Landscape — AI Customer Finder / AI Prospecting

**Phase:** Phase 3 — Market Research (synthesis)
**Project:** ai-customer-finder
**Date:** 2026-05-11
**Confidence:** Medium-High (funding/valuations well-sourced; ARR figures partly reported, partly estimated)

> Built from `raw/wave2-competitors.md` (12 web searches, ~30 competitors). Funding/valuation = Crunchbase/TechCrunch/The Information/SEC. ARR figures flagged where reported vs. estimated.

---

## The shape of the market

Money and momentum are concentrating in **two places — and neither is "autonomous cold-outbound AI SDR":**

1. **GTM-engineering infrastructure** — sits *above* the CRM, orchestrates data + AI, doesn't spam. **Clay** is the breakout: $100M Series C at **$3.1B** valuation (Aug 2025), ~**$100M ARR** in 2025 (~3x YoY), ~10K customers. [Data, TechCrunch/Crunchbase 2025]
2. **Cheap full-stack data + workflow for the masses** — **Apollo.io**: ~**$150M ARR** (May 2025, +~40% YoY), still carrying a stale $1.6B valuation from Aug 2023; acquired Pocus (signal/intent) early 2026. [Data, press 2025–26]

Meanwhile the **autonomous AI-SDR startups raised far less and are mid-correction** (11x reputational damage, Artisan facing platform enforcement, Unify tiny ARR), and the **public/legacy incumbents are flat-to-declining** (ZoomInfo revenue ~−1% 2024 and guiding down; Outreach valuation impaired, layoffs; Salesloft folded into Clari). The **bootstrapped cold-email tier** (Instantly, Smartlead, lemlist) is cheap and profitable but is exactly what the bulk-sender rules and AI-spray backlash are punishing.

## Comparison matrix

| Name | Category | What it does | Pricing (real) | Funding / valuation | Traction | Key strength | Key weakness |
|---|---|---|---|---|---|---|---|
| **Clay** | GTM-engineering infra | Data orchestration, enrichment waterfalls, AI research agents, list-building | $134–$800+/mo + credits; consultants charge $3K–$12K/mo to run it | $100M Series C @ **$3.1B** (Aug 2025) | ~$100M ARR, ~3x YoY, ~10K customers | Category-defining; CRM-agnostic; "infra" not "spam" | Steep learning curve ("need a Clay expert"); credit system punishes experimentation; not for solos sending <10K/mo |
| **Apollo.io** | Data + engagement, freemium | Contact DB (~275M), sequences, dialer, AI assist, now Pocus signals | Free tier; $49–$149/seat/mo paid | ~$1.6B (Aug 2023, stale); ~$150M ARR (May 2025) | Millions of users (freemium); G2 4.7 | Cheapest "ZoomInfo-lite + outreach"; huge top of funnel | Trustpilot ~2.9 — billing/credit complaints, data accuracy, deliverability; "sneaky games with credits" |
| **ZoomInfo** | Sales intelligence (public) | B2B contact/company data, intent, Copilot AI | ~$15K–$60K+/yr, annual contracts | Public (NASDAQ: GTM/ZI); ~$1.21B revenue 2024 (~−1%), guiding down 2025 | Large enterprise base; declining | Deepest enterprise dataset; intent data | "Absolutely scandalous" pricing; aggressive auto-renew enforcement; resented; shrinking |
| **6sense** | ABM / intent | Predictive intent, account ID, orchestration | Enterprise (opaque, ~$50K+/yr) | ~$5.2B (2021, stale); ~$200M revenue | Enterprise ABM leader | Expensive; enterprise-only; not for SMB |
| **Gong** | Revenue intelligence | Call recording/analysis, deal intelligence, some prospecting AI | ~$1,600/user/yr+ , platform fees | ~$7.25B (2021) → ~$4.5B secondary (2024); $300M+ ARR | Strong enterprise base | Adjacent (post-pipeline), not a "finder" — but expanding toward it |
| **Outreach** | Sales engagement | Sequences, AI agents, deal management | ~$100+/user/mo, annual | $4.4B (2021) — valuation impaired; layoffs 2023 & 2024; ~$300M revenue | Mid-market/enterprise base | Established engagement platform | Past its peak; valuation cut; not a "finder" |
| **Salesloft** | Sales engagement | Sequences, Drift conversational, Clari forecasting | ~$100+/user/mo | Vista bought for **$2.3B in 2021** (not 2024); merged into Clari Dec 2025; Drift sunset ~Mar 2026 | Large base, consolidating | Now part of a bundled GTM suite | Identity being absorbed; legacy engagement model |
| **11x.ai** | Autonomous AI SDR | "Alice" (outbound), "Jordan" (voice) | ~$5K–$45K/yr contracts | ~$350M post-money (a16z, Jan 2025) | **Reputationally damaged** — TechCrunch (Mar 2025): fake logos, ~$2–3M real ARR vs. ~$10M claimed, 70–80% churn; ZoomInfo said it underperformed humans | First-mover brand recognition | The cautionary tale of the category; trust deficit |
| **Artisan** | Autonomous AI SDR | "Ava" — finds + emails B2B prospects | ~$3K–$15K+/yr | $25M Series A (Apr 2025) | ~$5M ARR, ~250 customers; facing LinkedIn enforcement | "Stop Hiring Humans" attention | Data-source enforcement risk; horizontal me-too |
| **Regie.ai** | AI SDR / content | Auto-pilot prospecting, sequence content | ~$35K+/yr | $30M Series B (Feb 2025) | Mid-market | Content-quality focus | Horizontal; commoditization-exposed |
| **Unify** | Signal-based outbound | Intent signals + automated plays + AI agents | ~$700–$2K+/mo | $40M Series B @ $260M (Jul 2025) | **~$5.6M ARR** (small for the valuation) | Well-funded; "warm outbound" positioning | Valuation/ARR mismatch; horizontal; crowded "signals" space |
| **AiSDR / Jason AI (Reply.io) / B2B Rocket / Meetz / Salesforge (Agent Frank) / Bosh (Relevance AI)** | Autonomous AI SDR (long tail) | Variations on "AI does your outbound" | ~$500–$3K/mo; Salesforge ~bootstrapped (~$500K ARR) | Mostly small/seed or bootstrapped; Relevance ~$24M (May 2025) | Small | Cheap entry points | Indistinguishable from each other; "every tool is an AI agent now" |
| **Qualified (Piper)** | Inbound AI SDR | AI chat/SDR for *inbound* website traffic (Salesforce-centric) | Enterprise | Well-funded ($163M total) | Salesforce ecosystem | Different problem (inbound, not finding) | Salesforce-dependent |
| **Common Room / Pocus / Koala / Keyplay / Default** | Signal / intent / "lookalike" | Surface in-product + digital signals, score accounts, find lookalikes | ~$500–$2K+/mo (Common Room enterprise) | Various seed–B; Pocus acquired by Apollo (early 2026) | Mid-market PLG companies | The "right trend" tools | Horizontal; consolidating into bigger platforms |
| **Instantly.ai** | Cold-email infra (bootstrapped) | Sending infra, inbox rotation, lead DB, warmup | ~$30–$350+/mo | Bootstrapped; ~$35–45M ARR | Large SMB/agency base | Cheap, profitable, popular with agencies | "Warmup pool burns your domains"; the channel itself is depreciating; FTC/inbox-rule headwinds |
| **Smartlead / lemlist / la Growth Machine / Woodpecker** | Cold-email infra (bootstrapped) | Same space as Instantly | ~$30–$150+/mo | Bootstrapped; Smartlead ~$14M ARR | SMB/agency | Cheap | Same channel decay; deliverability arms race |
| **Lusha / Seamless.ai / RocketReach / LeadIQ / Cognism** | Commodity contact data | Email/phone lookup, Chrome extensions | ~$0–$100+/mo | Various (Cognism ~$120M+ raised; Seamless was public, struggled) | Large freemium funnels | Cheap data | Racing to zero; accuracy complaints; commoditized |
| **Salesforce Agentforce SDR Agent** | Incumbent platform AI | Native AI SDR inside Salesforce | ~$2/conversation or ~$0.10/action; $125+/user tiers | Salesforce (public) | Salesforce install base | Lives where the buyer already works | Salesforce-only; early; but a massive commoditization threat |
| **HubSpot Breeze (Prospecting Agent)** | Incumbent platform AI | Native AI prospecting inside HubSpot; bundling Apollo data | ~$1/qualified lead (≈2026); included in tiers | HubSpot (public) | Huge SMB/mid-market base | In the CRM SMBs already use; cheap | HubSpot-only; but directly squeezes standalone SMB AI-SDRs |
| **Microsoft / LinkedIn Sales Navigator + Copilot** | Incumbent platform AI | Lead/account discovery, AI account IQ inside LinkedIn | ~$100–$170/seat/mo | Microsoft (public) | The data source itself | Owns the graph; can choke off scrapers | LinkedIn-only; conservative pace |

### Vertical-specific incumbents (the wedge competition)

| Vertical | Incumbents | Gap |
|---|---|---|
| Staffing/recruiting BD (find client companies) | Bullhorn (ATS+), Loxo, Crelate, Recruiterflow (ATS/CRM); SourceWhale (recruiter outreach, $3K–$12K+/seat/yr); hireEZ/SeekOut (candidate side) | **BD is an afterthought** in candidate-centric ATSes; SourceWhale is outreach-execution, not "which companies, why now." Purpose-built "find me companies to staff for, ranked by hiring-distress signals" — **white space.** |
| Freight brokers finding shippers | DAT, Truckstop, FreightWaves SONAR (load/rate data); "shipper lists" (notoriously stale) | "Find me shippers to call, with intent" is **underserved by software** — mostly stale lists + cold calling. |
| Home services | Angi/HomeAdvisor/Thumbtack (lead marketplaces), Hover/Roofr (aerial), CompanyCam | Hated lead marketplaces, but the value there is *generating consumer demand* (media/arbitrage), not a "finder" — wrong business shape for this founder. |
| CRE brokers | CoStar, Crexi, Reonomy ($4.8K/yr) | Resented but it's an *assembled/licensed-data* business — wrong shape. |
| Construction subs | ConstructConnect (~$4.5K/yr), Dodge, BuildingConnected, PlanHub, BuildZoom | Pricey, but free options (PlanHub/Blue Book for subs) cap willingness to pay; private project intel is licensed. Mixed. |
| Insurance brokers | X-date data vendors, lead vendors ($424 blended CPL) | X-dates are proprietary/inferred + TCPA drag — data wall. |

## Positioning map

Two useful axes:

- **Horizontal ↔ Vertical** (who it's built for): almost everything clusters at the *horizontal / "B2B SaaS selling to B2B SaaS"* pole. The *vertical* pole is nearly empty.
- **Data-provider ↔ Workflow-agent ↔ Send-engine**: ZoomInfo/Apollo/Lusha = data; Clay/Unify/Common Room = orchestration/workflow; 11x/Artisan/AiSDR/Instantly = send. The durable middle (orchestration) is owned by Clay at the high end; the low end (cheap send) is being killed by deliverability rules.
- **DIY ↔ Done-for-you, by price**: a chasm sits between *$0–50/mo DIY tools* (Apollo free, Lusha) and *$1–2K/mo opaque "AI SDR"* — the *$100–300/mo done-for-them* band, and *outcome-based pricing*, is barely served.

**Where a new entrant can stand:** the **vertical pole**, in the **orchestration/insight middle** (not the send-engine), at the **$100–500/mo done-for-them price band**, optionally with **outcome-based pricing** and a **warm-path** angle. That is empty space — because the funded players have bigger fish and the platforms won't build a staffing-specific (or freight-specific) tool.

## Platform & commoditization risk: HIGH for horizontal cold-outbound AI SDRs

HubSpot Breeze (~$1/qualified lead), Salesforce Agentforce SDR (~$2/conversation), Apollo (cheap freemium + Pocus signals), and LinkedIn Copilot are bundling "find + email prospects" into the tools buyers already own. Standalone *horizontal* AI SDRs — especially ones whose only home is inside HubSpot/Salesforce — get squeezed hard. Commodity contact-data tools (Lusha/Seamless/RocketReach/LeadIQ) race to zero.

**What survives the squeeze:** (1) CRM-agnostic orchestration infra with real data depth (Clay), (2) **vertical depth the platforms won't bother to build**, (3) **warm-path / network-sourcing engines** immune to the cold-email decay, (4) **outcome-based pricing** for the long tail that can't afford seats. Our wedge is deliberately built on #2 + #3 + (#4 optional).

## Vulnerability analysis — who we'd actually be up against in the wedge

- **Bullhorn / Loxo / Crelate / Recruiterflow** — could add a "BD signals" module, but it's not their focus and their customers complain BD is neglected; they're integration *partners* more than threats short-term.
- **SourceWhale** — closest analog (recruiter outreach tooling), but it's execution, not "which accounts / why now"; possible "use us together" partner, possible eventual competitor. Watch closely.
- **Clay / Apollo / Unify** — *could* be configured to do staffing BD, but it requires the user to be a power-user and assemble the job-data themselves. Our edge: it's pre-built, opinionated, and the data plumbing is done. The risk: a savvy Clay consultant packages a "staffing BD template" — defensible only if we go deeper (integrations, proprietary signal scoring, the warm-path graph).
- **"AI SDR for recruiters" startups** — none prominent yet; this could change in 12 months. Speed matters.

---

## Flags

**Red Flags:**
- Horizontal AI-SDR entry faces direct platform commoditization (HubSpot Breeze, Salesforce Agentforce, Apollo) — do not enter here.
- The category's flagship products (11x, ZoomInfo, Apollo) are also its *most-criticized* — "AI SDR" carries a trust deficit a new entrant inherits unless deliberately distanced from it.
- Contact-data accuracy (15–35% bounce on scraped data) is a moat the incumbents have and we don't — our wedge must minimize reliance on a maintained contact DB (lean on signal + integrations + lighter-touch enrichment).

**Yellow Flags:**
- SourceWhale and the staffing ATSes (Bullhorn/Loxo/Crelate) could move into the BD-signals space — competitive moat is "deeper, faster, more opinionated," which a side-project pace makes harder.
- A "staffing BD template" on Clay/Apollo is a plausible low-effort competitor — differentiation must be product depth + integrations, not just "we did the prompt for you."
- Several reported ARR figures (11x, Artisan, Unify, Instantly, Smartlead) are estimates/leaks, not audited — treat as directional.

## Sources
- `raw/wave2-competitors.md` — Crunchbase, TechCrunch, The Information (Tier 1–2) for funding/valuations; SEC filings (Tier 1) for ZoomInfo; vendor pricing pages, G2/Capterra/Trustpilot (Tier 2–3) for pricing/ratings; press releases (Tier 3) for incumbent AI feature launches. All 2023–2026; pre-2024 valuations flagged "stale" inline.
- `raw/wave4-vertical-distribution.md` — vertical incumbent pricing and ASA/SIA data.
