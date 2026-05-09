# Brand Personality

**Phase:** 5 — Brand
**Project:** pokemon-champions-team-workspace
**Date:** 2026-05-09
**Confidence:** Medium (archetype + visual direction is opinion-grounded; designers should iterate)

---

## Brand Archetype

**Primary archetype: The Sage.** Secondary: **The Caregiver.**

### Why Sage

The Sage is about truth, knowledge, and competence — the brand of trusted advisors and reliable information sources. Examples: BBC, Britannica, Stack Overflow, Lichess, Stockfish.

This fits Champion's Notebook because:
- Persona C and B value rigor, citations, and earned expertise
- The product literally cites sources and refuses to bluff
- We carry the responsibility of *not misleading* serious players whose ranking depends on us being right
- The community trust currency is "do you actually know what you're talking about?"

### Why Caregiver Secondary

The Caregiver looks after the people who use it; quietly competent service. Examples: Notion's "we'll keep your work safe and organized," Patagonia's environmental concern, MailChimp's quirky helpfulness.

This fits the workspace half of the brand:
- A notebook is a service, not a product — it carries a custodial relationship with someone's prep work
- "We remember what you've learned, so you don't have to" is a Caregiver promise
- Tournament-prep urgency creates a moment where users are stressed; we're the calm helper, not the loud disruptor

### Archetypes we deliberately avoid

| Archetype | Why we don't use it |
|---|---|
| **The Hero** | "Conquer the meta!" energy — perfect for VGCCoach; wrong for our voice |
| **The Outlaw** | Wired-magazine "disrupting Pokémon prep!" — pulls toward marketing fluff |
| **The Magician** | "AI changes everything!" — the entire AI hype lane that Persona B mistrusts |
| **The Jester** | Light, playful, irreverent — fine for casual gaming brands; too unserious for tournament prep |
| **The Innocent** | Pokémon nostalgia / cartoon-y energy — pulls toward casual market |

---

## Emotional Attributes

What the brand should make users feel:

| Feeling | When | How we deliver |
|---|---|---|
| **Trust** | First time using the AI coach | Visible source citations; tool calls shown |
| **Calm preparedness** | Pre-tournament | Calendar awareness, organized workspace, restored context |
| **Quiet capability** | When working in the product | UX that respects vocabulary, doesn't over-explain |
| **Validation of seriousness** | Throughout | The brand treats them as a competitive player, not a casual fan |
| **Belonging** | Community touchpoints | Founder-voice content, beta credits, advisor visibility |

What we explicitly don't deliver:

- Excitement (cheaper feeling than capability)
- Awe (sets expectations the AI can't meet)
- Amusement (wrong tone for tournament prep)
- Fanboy nostalgia (alienates Persona B/C; pulls toward Persona E)

---

## Visual Direction (input to design phase)

This is *direction*, not a design system. A designer should iterate.

### Adjectives

- Calm
- Spacious
- Dense-where-it-needs-to-be
- Serif-and-mono mixed (serious + technical)
- Restrained palette
- Functional first

### Visual references

- **Lichess.org** — calm, dense, respects the user's vocabulary, lets the chess pieces (or in our case, Pokémon names) carry visual weight
- **Linear's marketing site** — quiet confidence, mono details, generous white space
- **Notion's app interface** — workspace metaphor, hierarchical, neutral palette
- **Hey.com** — earnest copy with a strong typographic anchor
- **Are.na** — research-feel, restrained, scholarly
- **Substack reader** — long-form-respect, comfortable reading

### Visual references we explicitly avoid

- **Mobalytics** — too gamer-RGB; over-stimulating UI
- **Pikalytics** — functional but visually noisy; Pokémon-fan-aesthetic
- **Pokémon official sites** — bright primaries, mascot-driven; would invite trademark issues
- **VGCCoach** — busy gradient gaming aesthetic
- **op.gg** — dense data dashboard; too gamer-pro

### Color direction

- **Foundation:** Neutral, slightly warm white or off-black background; high-contrast text
- **Accent:** A single restrained accent color — recommended consideration: a deep teal or muted indigo (avoid Pokémon-brand red/blue/yellow primaries)
- **Functional colors:** Standard semantic — green for confirm, amber for caution, red sparingly for destructive
- **No gradients except for very specific states** (loading, AI thinking)
- **Type-color contrast:** Always WCAG AA+ for body, AAA for primary text

### Typography direction

- **Display / hero:** A serious serif (e.g., Tiempos, Source Serif, Spectral) for warmth without playfulness
- **Body:** A neutral humanist sans (e.g., Inter, Söhne, IBM Plex Sans)
- **Code / data:** A clean mono (e.g., IBM Plex Mono, Berkeley Mono) — used for EV spreads, damage rolls, sim outputs to signal "this is real data"
- **Avoid:** Display sans-serifs designed for tech-startup vibe (Söhne is fine; Söhne Breit is too loud)

### Layout principles

- **Workspace dominance:** The product tab is the home tab; the marketing page is one click away
- **Density that respects expertise:** EV spreads and team data should be readable at-a-glance, not buried under chrome
- **Calm scaffolding:** Generous spacing in marketing/onboarding; tight spacing in expert workflows
- **Mobile-responsive at MVP, not mobile-equivalent:** The phone is for "look at my team while away from the keyboard," not for deep editing

### Logo direction

- **Mark:** A simple, geometric symbol — possibilities: a stylized notebook spine, a small tag/bookmark glyph, a Greek letter or chess-piece-like icon (no Pokémon imagery)
- **Wordmark:** Pair the mark with a wordmark in the chosen serif or a refined sans
- **No Pokémon imagery, no Champion's-style logo type, no resemblance to TPC marks** — this is a non-negotiable trademark guardrail
- **Test with a competitive player:** does it feel pro-grade or fan-grade?

---

## How the Brand Compares to Competitors

| Brand | Energy | Where they live | Where we live |
|---|---|---|---|
| Pokémon Showdown | Spartan-functional, retro | "We're the simulator" | "We're the workspace" |
| Pikalytics | Fan-aesthetic, dense | "We're the data" | "We're the prep notebook" |
| Smogon | Forum-classic | "We're the canon" | "We respect the canon" |
| VGCCoach | Modern gaming-AI | "We're the AI coach" | "We're grounded craft" |
| ChampDex | App-store-Pokémon | "We're the iOS app" | "We're cross-format prep" |
| Notion (analog) | Calm workspace | (broad SaaS) | (vertical Pokémon prep) |
| Lichess (analog) | Calm chess | (chess world) | (VGC equivalent) |

The closest aesthetic + ethos analogues are **Lichess** and **Notion**. Neither competes in our category, but borrowing their seriousness-of-craft is on-mission.

---

## Brand Risks to Monitor

- **Inflation by AI feature buzz:** When AI features ship, easy to drift toward "AI-powered" copy. Audit voice quarterly.
- **Casual-market pull:** Persona E's vocal feedback ("make Charizard work!") could pull brand toward fan-aesthetic. Resist.
- **Trademark drift:** Logo, color, name proximity to Pokémon official assets. Trademark search before lock-in; designer briefed on guardrails.
- **Founder-leaving-stage growth:** When founder hires designers, marketers, the voice and personality must be documented enough to survive. This file + tone-of-voice.md + values are that record.

---

## Flags

**Red Flags:**
- None.

**Yellow Flags:**
- "Champion" in the name lives close to TPC's "Champions" mark. Trademark / domain check is mandatory before brand work locks in.
- Sage archetype requires the product to actually be correct. If AI coach hallucinates regularly, the archetype collapses to fraud. Phase 6 + Phase 8 quality enforcement is the brand's foundation, not a separate workstream.
- Lichess-aesthetic references depend on disciplined design. Easy to slip into "Pokémon-fan dense UI" if an inexperienced designer interprets "dense" too literally.

## Sources

- `02-strategy/positioning.md` — brand-adjacency requirements
- `03-brand/mission-vision-values.md` — values that drive personality
- `03-brand/tone-of-voice.md` — voice that personality animates
- Carl Jung / Mark & Pearson archetype framework (industry standard)
- Lichess.org, Linear, Notion, Hey.com, Are.na — visual reference set
