# Operational Reality — A Singapore 2-Person Team Selling Web Services to US Med Spas

Research date: 2026-05-11. Prefer 2025–2026 data. Labels: **[Data]** / **[Estimate]** / **[Assumption]** / **[Opinion]**.

Context: 2-person team, currently Singapore, < USD 4k working capital, willing to relocate *or* operate remotely. Selling AI-built websites (USD 4,000–8,000 + optional retainer) to US med spas in DFW or Tampa/Orlando.

---

## 1. Can a non-US team sell web services to US med spas remotely?

**[Opinion]** Yes — this is a *normal* arrangement in 2026. Web/marketing services are routinely delivered remotely; clients increasingly don't care where the team sits as long as communication is good. **[Data]** ~54% of small US companies outsource ≥1 core function in 2025; ~83% plan to hold/grow outsourcing budgets; digital marketing is one of the most-outsourced; failed outsourcing is overwhelmingly blamed on "cultural misalignment / passive communication" (74% per a cited Deloitte 2025 study), not on offshore-ness per se. (abroadworks.com/blog/outsourcing-popularity; kdci.co/outsourcing-blog/...; parallelhq.com/blog/offshore-web-design-services) — rating B- (industry/vendor blogs, directionally solid).

**Timezone — the real friction. [Data/Assumption]** DFW = CST/CDT, UTC−6/−5. Singapore = UTC+8. Gap ≈ **13h (CDT) / 14h (CST)**. US business hours 9am–5pm CT ≈ **10pm–6am Singapore** (during CDT). Tampa/Orlando = ET, UTC−5/−4 → ~12–13h gap, US hours ≈ 9pm–5am SG. **[Opinion]** Async work (building sites, email, LinkedIn) is fine. *Synchronous* work (cold calls, discovery calls, kickoff calls, "can we hop on a quick call") forces at least one founder onto a partial-US schedule (e.g., 8pm–2am SG = 7am–1pm CT). Doable for two people splitting shifts; brutal solo. This is the single biggest operational tax of staying in SG.

**Payment rails / banking — see §2.** Invoicing US clients: standard — issue USD invoices via Stripe Invoicing / Wise / QuickBooks. US clients pay by ACH or card; collect a 40–50% deposit upfront (essential for cash-poor team). **[Opinion]** Med spas care about *the work and responsiveness*, not your passport — but a US LLC, US phone number, US-looking email domain, and US business address (registered-agent or virtual office) all reduce friction and "are you legit?" hesitation. Worth the ~$500–1k/yr.

---

## 2. Cost & process to form a US entity from Singapore

**[Data]** Options: Stripe Atlas, Firstbase, doola, or DIY via a registered-agent service (Northwest, etc.).
- **Stripe Atlas**: ~$500 one-time (Delaware C-corp or LLC, formation docs, EIN application, registered agent free year 1 then ~$100/yr). Atlas does *not* handle Form 5472 or ongoing tax compliance. (docs.stripe.com/atlas; stripe.com/resources/more/how-to-register-a-us-business-as-a-nonresident-...) — rating A- (Stripe's own docs).
- **DIY**: state filing fee (Wyoming ~$100–150, Delaware ~$90–110 + ~$300/yr DE franchise tax; Wyoming ~$60/yr report) + registered agent ~$100–300/yr ≈ ~$300–600 year 1.
- **EIN for non-residents (no SSN)**: file Form SS-4 by fax/mail → commonly **4–8 weeks** (some report 6–9 weeks). Atlas now lets you accept Stripe payments *before* the EIN arrives.

**[Estimate]** All-in to be "formed + EIN + bank + Stripe live": **~$500–1,000 one-time + ~$300–600/yr ongoing**, timeline **~4–8 weeks** (EIN is the bottleneck). Well within < $4k capital, though it's a meaningful chunk.

**[Opinion]** Wyoming LLC is cheapest/simplest for a 2-person service business; Delaware C-corp only if they plan to raise US VC (they're not — skip it). LLC = pass-through, simpler.

**Compliance landmine [Data]**: a foreign-owned single-member US LLC must file **Form 5472 + pro-forma 1120 every year** — **$25,000 penalty** for late/missed filing. Atlas/Firstbase don't do this for you. Budget ~$200–500/yr for an accountant who does. (globalsolo.global/blog/what-happens-if-you-miss-form-5472-...) — rating B+.

---

## 3. Should they relocate?

**[Data]** Singapore *is* an E-2 treaty country — Singaporean citizens are E-2-eligible. But E-2 requires a "substantial" investment with no fixed minimum; in practice consular officers expect roughly **$100k–200k+** for a small business, and a **one-person/self-employment model gets rejected** ("marginality" rule — must show capacity to hire US workers). (uscis.gov/working-in-the-united-states/temporary-workers/e-2-treaty-investors; usimmigrationadvisor.sg/e2-visa-guide/; joorney.com/news/e2-visa-advertising-agencies/) — rating B+ (USCIS + immigration-law sources).

**[Opinion]** With < $4k capital, **E-2 is not realistic** — they're ~25–50x short of a credible investment, and the marginality test kills a 2-person shop with no employees. Other paths:
- **O-1** (extraordinary ability): high bar, needs a portfolio/awards/press — not yet.
- **L-1**: requires an existing foreign company with ≥1 year of operations + a qualifying US affiliate — premature.
- **B-1 (business visitor)**: allows *attending meetings/conferences*, NOT performing productive work or "running a business" — fine for an occasional conference trip, not for relocating to operate.
- **ESTA/Visa Waiver (Singapore qualifies)**: 90-day visits for business meetings only — same limits as B-1.

**Verdict [Opinion]**: They almost certainly **cannot move to the US** at current resources, and shouldn't try. Operate remotely from Singapore (or anywhere) with a US LLC. Re-evaluate E-2 only if they bootstrap to ~$100k+ in retained earnings and want to hire US staff — a 2027+ question, not now.

---

## 4. Contracts / liability

**[Opinion/Estimate]**:
- **Client contracts**: use a written services agreement (SOW + MSA) — many free/cheap templates exist (e.g., from web-design communities, Bonsai, etc.). Governing law: pick the LLC's state (Delaware/Wyoming) or the client's state; for sub-$10k projects either is fine. Include scope, milestones, deposit, IP-transfer-on-final-payment, limitation of liability, and a "no PHI / not a HIPAA business associate" clause.
- **HIPAA / BAA**: only needed if you *create, receive, store, or transmit PHI*. A marketing/brochure website + booking-widget *link-out* (to the spa's own HIPAA-compliant booking tool — Boulevard, Mangomint, etc.) means **you never touch PHI** → **no BAA needed**. Explicitly architect it that way and say so in the contract. (hipaajournal.com/hipaa-compliance-for-email/; paubox.com/blog/hipaa-marketing-rules-email) — rating A-.
- **Insurance**: US general liability + professional liability (E&O) for an agency runs roughly $400–1,200/yr; **not strictly required** for sub-$10k web projects but some sophisticated clients ask for a COI. **[Opinion]** Skip at launch; add once a client requires it or revenue justifies it.
- **ADA / web accessibility**: med spa sites should be WCAG-2.1-AA-ish to limit drive-by ADA lawsuits (real risk in the US) — bake accessibility into the build; it's a selling point, not a cost.

---

## 5. Tax (one paragraph — consult an accountant)

**[Data/Opinion]** A foreign-owned US LLC that *provides services* may be treated as engaged in a US trade or business, generating **Effectively Connected Income (ECI)** taxed at US graduated rates on net profit — *but* whether a USTB exists turns on whether activities (especially personal services) are "considerable, continuous, regular" *and performed in the US*. Services performed *from Singapore* for US clients are frequently argued to be **non-ECI / no USTB** (no US-based personnel, no US office, no dependent agent) — meaning potentially **no US federal income tax**, only the Form 5472 + pro-forma 1120 information filing (and possibly state franchise fees). This is genuinely fact-specific and the IRS position can bite if you later put a person/office in the US, hire US contractors as agents, or attend the US closely. **Flag: consult a US international-tax accountant before the first invoice — getting this wrong (or missing Form 5472) is a $25k+ mistake.** (irs.gov/individuals/international-taxpayers/effectively-connected-income-eci; 1040abroad.com/blog/foreign-owned-llc-reporting-and-taxes-explained/; acciyo.com/us-llc-non-resident-tax-...) — rating B (mix of IRS + tax-advisory blogs; the "services-from-abroad = likely no ECI" framing is a common-but-not-guaranteed position).

Singapore side **[Opinion]**: SG taxes on a remittance/territorial basis for some income; the founders likely owe SG tax on their share of profits as residents. Also an accountant question. Net: probably a *low* total tax burden if structured cleanly, but get advice.

---

## 6. Pricing / collecting in USD from Singapore

**[Opinion/Estimate]** Straightforward:
- **Stripe** (via Atlas + US LLC) for card payments and invoicing; ~2.9% + $0.30 per card txn (less for ACH). USD settles to your US business account.
- **Wise Business** — easiest non-resident account to get approved (vs Mercury, which **tightened in 2025 and now rejects registered-agent addresses** and some founder countries — have a real business address ready). Wise gives USD/SGD/EUR balances, cheap FX (~0.3–0.6% spread), local US ACH details for clients to pay into. (Wise is an EMI, not a bank — funds not FDIC-insured; fine for an operating float, don't park large reserves there.) (devanta.us/us-llc-banking-for-nonresidents-mercury-financial/; support.mercury.com/hc/en-us/articles/28770467511060-Eligibility; wise.com/gb/blog/how-to-open-a-us-bank-account-for-llc-as-a-non-resident) — rating B+.
- **Relay** — another non-resident-friendly US business bank (FDIC via partner bank) worth considering alongside Wise.
- **FX**: revenue in USD, costs partly in SGD (living costs) + partly USD (tools). USD/SGD has been ~1.28–1.36 range recently — **[Assumption]** budget some volatility; convert in tranches via Wise; keep a USD buffer for US obligations (franchise tax, accountant).
- **[Opinion]** Charge a **40–50% non-refundable deposit** on signing and the balance on delivery — non-negotiable for a team with < $4k runway; it also funds the per-project AI/tooling spend.

---

## Confidence summary
- **High**: remote delivery is normal and clients won't reject it for being offshore; US LLC formation cost/timeline (~$500–1k, ~4–8 wks); E-2 is not realistic at < $4k; no BAA needed if no PHI; Wise/Relay viable for non-residents, Mercury got harder; collecting USD is easy.
- **Medium**: exact tax treatment (the "services-from-SG = no ECI" position is common but fact-specific); insurance need; the precise EIN timeline.
- **Low**: how much med spa owners *actually* discount an offshore agency in practice (no hard data — assumed minimal but unproven); SG-side personal tax exposure.

## Biggest gaps
1. No definitive answer on ECI / US tax for *this exact setup* without a paid accountant opinion — and the downside of getting it wrong is large (Form 5472 = $25k penalty).
2. No data on med spa owners' real-world willingness-to-pay $4k–8k *to an unknown foreign agency* vs a local one — could be a meaningful discount or trust barrier (untested).
3. Banking approval is increasingly fickle for non-residents — Wise/Relay *probably* work but it's not guaranteed; need a real (non-registered-agent) US business address lined up.
4. Whether splitting US-hours synchronous work across 2 founders is sustainable for 6–12 months — operationally unproven; could cause burnout.

Word count ≈ 1,650.
