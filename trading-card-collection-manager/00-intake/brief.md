# Intake Brief — Trading Card Collection Manager

**Phase:** 1 — Intake
**Project:** trading-card-collection-manager
**Date:** 2026-05-10
**Confidence:** High (founder-stated; not externally verified)

---

## The Idea (founder-stated)

Mobile app that turns a phone camera into a trading card scanner. Point at a Pokemon (initial beachhead), MTG, or sports card and instantly get:

1. **Card identity** (set, name, edition, language, holo/non-holo)
2. **Current market value** aggregated across TCGplayer + eBay (sold listings)
3. **Condition assessment** (Near Mint / Lightly Played / etc.)
4. **Real-time portfolio tracking** (collection's total worth recalculates as the market moves)

## Target Customer

The "200–2,000 card serious hobbyist" with a $1K–$50K collection who is currently juggling spreadsheets and eBay tabs to manage value. Deliberately NOT the casual player and NOT the institutional grader/dealer.

## Business Model (founder-stated)

| Tier | Price | What's included |
|------|-------|-----------------|
| Free | $0 | Up to 50 cards, manual entry only |
| Pro | $4.99/month or $39.99/year | Unlimited cards, camera scanning, real-time valuation, price alerts, portfolio analytics |
| Future v2 | 5–10% marketplace fee | On trades facilitated through the app, after trust is established |

Founder-stated **realistic ceiling: $100–$500K/year** if the app becomes the standard tool for one specific TCG community.

## Founder Profile (confirmed via intake)

- **Domain:** Light collector. Some exposure but not deeply embedded in any TCG community.
- **Skill:** Experienced mobile developer.
- **Time:** Side project, evenings and weekends.
- **Budget:** Implied bootstrapped (not explicitly stated, side-project commitment implies low burn).

**[Yellow Flag]** Founder-market fit is moderate, not strong. Domain insight gap will need to be closed via customer development (interviews, community embedding) — and side-project pace makes this slower.

## Beachhead Choice

**Pokemon TCG**, chosen for largest market and demand signal. Note: also has the highest competitive density of any TCG segment (Collectr, Pokellector, TCGplayer's own app, plus the official Pokemon TCG Pocket / TCG Live ecosystems).

## Constraints

- Mobile-first by design (camera scanning is the core feature)
- Side-project pace → MVP must be small enough to ship in months, not years
- No stated regulatory exposure (consumer app, no payments at MVP — marketplace fees come later)

## Founder's Implicit Hypotheses (must be tested)

| # | Hypothesis | Risk if wrong |
|---|------------|---------------|
| H1 | Hobbyists with 200–2,000 cards will pay $40/year for scanning + valuation | Whole business model collapses |
| H2 | Camera scanning is meaningfully better than barcode/manual lookup for this user | Differentiation evaporates |
| H3 | TCGplayer + eBay aggregation is legally/technically feasible at scale | Core feature blocked |
| H4 | The "spreadsheet pain" is acute enough to drive paid conversion | Free tier becomes a graveyard |
| H5 | Price alerts + portfolio analytics are sticky enough to retain | High churn kills LTV |
| H6 | Marketplace trades will be transactable in v2 (trust, fees, dispute flow) | Future revenue layer never materializes |

## Hard Questions (deferred to validation phase)

- "Why are you the right person?" → Founder is execution-strong but domain-light. **Unfair advantage is currently unclear.** This must be closed by becoming embedded in one community OR by superior execution (better scanning accuracy, faster UX) than incumbents.
- "If TCGplayer or Pokemon Company launched this tomorrow, what would you do?" → No stated answer. Highest existential risk.
- "What's the strongest argument against?" → Crowded market, free alternatives (Pokellector, manual TCGplayer search), and the target user is already getting "good enough" with spreadsheets.
- "Have you talked to potential customers?" → Not stated. **Must happen in Week 1.**
- "What would make you walk away?" → Not stated.

---

## Flags

**Red Flags:**
- Founder-market fit is light + competitive density is high in Pokemon. Without a domain edge or a clear technical edge (e.g., dramatically better scanning), there is no obvious wedge.

**Yellow Flags:**
- Side-project pace vs. funded competitors (Card Ladder raised $50M+ in adjacent sports-cards space; multiple Pokemon-specific apps are funded teams).
- Stated revenue ceiling ($100–500K/year) implies a lifestyle business, not a venture-scale outcome — fine, but constrains funding options if the founder later needs capital.
- TCGplayer terms of service and eBay's developer access policies need to be checked. Aggregating their pricing data without authorization may violate terms.
- "Condition assessment" via phone camera is technically very hard. Even PSA/Beckett charge $20–$200 per card for grading because human eyes outperform. Setting buyer expectations matters.

## Sources

- Founder direct input (this conversation, 2026-05-10)
- AskUserQuestion responses (beachhead, founder fit, time commitment)
