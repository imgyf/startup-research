# User Journey

**Phase:** 6 — Product
**Project:** pokemon-champions-team-workspace
**Date:** 2026-05-10
**Confidence:** Medium (journey is opinion-grounded; should be road-tested in closed beta)

---

## Persona

This journey is mapped for **Persona C — VGC Tournament Aspirant** (primary). Persona B (Smogon Veteran Crossing Over) follows a similar journey with a sharper rigor expectation at every step. Persona E (Casual Favorite-Builder) shows up via free-tier inbound and is not the primary journey to optimize.

---

## End-to-End Journey

### Stage 1 — Awareness

**How they hear about us:**
1. **Creator endorsement** — WolfeyVGC mentions in a video; CybertronVGC includes in onboarding video; Brady Smith mentions in a Patreon-tier post
2. **Reddit post** — founder's "I built this for Worlds prep" post on r/stunfisk or r/PokemonChampions
3. **Friend recommendation** — a training partner or Discord acquaintance shares a public team page link
4. **SEO long-tail** — searches like "VGC Reg G rain counter," "Pokemon Champions team builder," "VGC tournament prep" land on our archetype prep pages
5. **Twitter/X build-in-public** — founder's progress threads reach the comp Pokémon community

**Emotion:** Skeptical. They've seen 15+ tools launch in 30 days. "Why this one?"

**Drop-off risk:** First impression must signal **rigor and seriousness** within 3 seconds. Hero copy: *"The prep workspace VGC players actually use between tournaments."* No "AI revolutionizes Pokémon" energy.

**Mitigation:**
- Lead with social proof: founder name + advisor name + "built on @pkmn/sim — no hallucinations"
- Show, don't tell: hero animation showing version history diff and coach citing a damage roll

---

### Stage 2 — Consideration / Sign-up

**What they do:**
- Click through homepage; scan features; check pricing; read FAQ
- Read or watch the creator partner's content if discovery was creator-led
- Check the "About" page — looking for "is this a real person, are they competitive enough"

**Emotion:** Curious but cautious. Comparing mentally against Showdown + Pikalytics + their existing Discord-and-spreadsheet stack.

**Drop-off risk:** If they feel "this is just another AI tool," bounce. If they feel "I'd have to abandon Showdown," bounce. If pricing feels surprising, bounce.

**Mitigation:**
- Pricing is upfront, no dark patterns — Free tier is real, not a 7-day trial
- Hero subhead: "Imports from Showdown, exports to Poképaste — works alongside your existing tools"
- Founder + advisor names visible on About; testimonials from beta users with their Smogon ladder rating shown

**Sign-up:** Email + Google. No credit card required for Free.

---

### Stage 3 — Onboarding (the activation moment)

**Goal:** First saved team within 5 minutes; second saved team within 7 days.

**Onboarding flow:**

1. **Welcome screen:** "What are you prepping for?" — Three options: a tournament (with date picker), a goal ("climb to ladder rank X"), or "just exploring."

2. **Add your first team:**
   - **Easiest path:** "Paste a Showdown team" — instantly imports, populates workspace
   - **Alternative:** "Start from a template" — 6-8 curated sample teams from creator partners or Smogon samples (with credit)
   - **Skip option:** "I'll add later" — lands them on dashboard

3. **Try the AI coach (optional but heavily nudged):**
   - "Ask why this team is bad against rain" — pre-filled prompt against their imported team
   - First answer shows tool calls visibly: "Running 50 sim battles vs. typical rain leads..." → result with citations
   - Aha-moment goal: see the coach actually run a calc and cite Smogon stats

4. **Set up first matchup tag:**
   - "What archetype gave you trouble last week?" — quick chip selector
   - Auto-creates a tag, links to their team

5. **Optional: Set tournament target:**
   - If they came in via "prepping for a tournament," surface the days-to-event countdown
   - "Indianapolis Regional — 18 days away. Want me to keep your prep organized?"

**Drop-off risk in onboarding:**
- Empty state with no clear next step (mitigated by "What are you prepping for?")
- AI coach fails to deliver value on first use (mitigated by pre-filled prompt + visible tool runs)
- Mobile experience breaks (mitigated by mobile-responsive testing in Week 11)

**Activation metric:** ≥60% of signups save 2+ teams within 7 days.

---

### Stage 4 — First Week (the trust-building phase)

**What they do:**
- Add 2-3 teams to workspace (their current Champions team, a Showdown side project, maybe a sample they want to study)
- Tag a couple of archetype matchups
- Use AI coach 5-15 turns
- Maybe write their first journal entry after a frustrating ladder match

**Emotion:** Testing. "Is this actually useful or is it a toy?"

**Drop-off risk:** "I forgot it existed" — workspace value isn't yet compounding because they haven't been through a full prep cycle. We need to **bring them back in week 2-3**.

**Mitigation:**
- **Email cadence (light, calendar-aware):**
  - Day 1: "Welcome — here's how to get the most out of your first team"
  - Day 3: "Most users save a second team in week 1 — try one of these starting points"
  - Day 7: "How was your first week? Quick tip on matchup tags"
  - Day 14: "VGC tournament X is coming up — set it as your prep target"
- **In-product nudges:** small banner — "You haven't journaled this week. Just 2 lines after a hard match."

---

### Stage 5 — The First Tournament Cycle (the conversion moment)

**What they do (over ~2 weeks before a Regional):**
- Iterate on team — version history starts to feel useful when they realize they can compare v3 vs. v5
- Use coach more heavily — 30-100 turns over the prep cycle
- Tag matchups against expected archetypes from recent regional usage
- Journal after each ladder session
- Hit the team-slot limit on Free (5 teams) — most aspirants run 5-10 candidate teams in active prep

**Emotion:** Engaged. The product is starting to feel like **the place where my prep lives**.

**Conversion trigger:** Hitting team-slot limit, hitting AI coach quota, or wanting full version history. Stripe checkout is one click; pricing is honest.

**Conversion target:** ≥2% Free → Paid within 30 days for Persona C-aligned users.

**Mitigation for those who don't convert:**
- Don't aggressively nag — Persona B/C will resent it
- Surface upgrade in context: when they hit team-slot limit, modal explains *what they unlock*
- Annual pricing prompt: "Tournament Prep $199/yr saves you $101 vs. monthly — and our roadmap takes you through Worlds 2026"

---

### Stage 6 — Tournament Day & Aftermath (the retention moment)

**What they do:**
- Reference team paste from phone in lobby (mobile responsive critical here)
- Optional: log results and quick-journal each round during breaks
- Post-tournament: write a longer journal entry; ask AI coach to "synthesize what hurt me this weekend"
- Make notes for the next tournament — "next time bring more Tera Steel"

**Emotion:** Cathartic. The product becomes the place where the lesson is stored, not where it evaporates.

**Retention metric:** Did they come back the week after the tournament? Did they create another version of their team within 14 days?

**Risk:** If no upcoming tournament is on their calendar, demand drops. **Off-season retention is the hardest single product challenge.**

**Mitigation:**
- Surface "what other tournaments are upcoming" — pull Pokemon.com event calendar
- Encourage Showdown ladder grind during off-season — workspace works for that too
- Creator content drops keep the workspace relevant (e.g., "Wolfey's Reg G analysis after Worlds — import the team")

---

### Stage 7 — Long-Term (multi-tournament, multi-season)

**What we hope happens:**
- They build 30-50 teams over a year
- They have 200+ journal entries
- The AI synthesis becomes more valuable than first-time use because it has more data
- They share teams with a training partner via coach-mode (v1.1)
- They renew annual at the next Worlds-prep cycle

**Risk:** They graduate to advanced needs (counter-team builder, opponent scouting) faster than v1.1 ships. Lose them to a sharper competitor.

**Mitigation:** v1.1 ship by October 2026 is the next gate. Don't slip past Q1 2027 spike.

---

## Key Touchpoints — Emotion Map

| Touchpoint | Emotion | Risk | Top mitigation |
|---|---|---|---|
| First creator mention | Curious | "Yet another AI tool" | Hero copy + advisor names |
| Homepage hero | Skeptical | "Doesn't look serious" | Lichess-aesthetic; numbers visible (battles run, sources cited) |
| Sign-up | Cautious | Friction | Email/Google; no credit card |
| First team save | Hopeful | Empty workspace | Showdown paste import + sample teams |
| First AI coach turn | Tense | "Will it bluff?" | Visible tool calls + citations |
| First journal entry | Awkward | "Why am I doing this?" | Structured prompts; one entry, not a novel |
| Hit team-slot limit | Frustrated then converted | Hard sell | Honest modal explaining unlock |
| Tournament prep day -3 | Anxious | Disorganized | Days-to-event banner; prep checklist |
| Post-tournament journal | Reflective | "What did I learn?" | AI synthesis prompt: "what hurt you this weekend?" |
| Off-season week | Disengaged | Forget about us | Email re-engagement; creator content |

---

## The "Aha Moment"

The single moment where Persona C feels: *"OK, this is different."*

We hypothesize the aha moment is **the first time the AI coach runs a sim battle live and shows the tool call output before answering** — turning a generic-LLM-coaching expectation ("ChatGPT for Pokémon") into a grounded-engineering experience ("oh, it's actually running my team in the simulator").

Goal: get every new user to that moment within their first 5 minutes.

**How to achieve it:**
- Pre-fill a prompt against their imported team
- Show the tool call running with a small "Running 50 sim battles..." indicator
- Show the citations clearly when the answer arrives
- Don't hide the engineering behind chat-style UX

---

## Failure Modes

| Mode | What it looks like | Frequency |
|---|---|---|
| **Lurker** | Free signup, never returns | Common — accept ~30-40% of Free signups never activate |
| **Tourist** | Saves one team, never engages with coach | 15-20% — these likely Persona E that came in via free-tier inbound |
| **Skeptic** | Tries coach once, sees a hallucination, leaves | The most dangerous — Persona B in particular. Mitigation: hard rigor in coach grounding |
| **Off-season churner** | Engaged before tournament, gone after | Expected — accept some seasonal churn; aim for 70% paid retention through 4-week post-tournament window |
| **Graduator** | Outgrows MVP, wants v1.1 features now | Risk after 4-6 weeks if v1.1 slips |

---

## Flags

**Red Flags:**
- None.

**Yellow Flags:**
- The "aha moment" depends on AI coach grounding being visibly impressive AND correct. If Week 11 closed-beta testing reveals the citations are confusing or the tool calls feel slow (>5s), we may need to invest in UX polish before public launch.
- Off-season retention is the single hardest journey challenge. If 4-week post-Worlds retention drops below 50%, the LTV model breaks.
- Mobile-responsive is "must-have" but solo founders typically under-invest. Real device testing across iPhone + Android sizes in Week 11 is non-negotiable.

## Sources

- `01-discovery/target-audience.md` — Persona C JTBD, channels, triggers
- `04-product/mvp-definition.md` — feature scope that journey depends on
- `02-strategy/value-proposition.md` — substitution equation, gain creators
- `03-brand/tone-of-voice.md` — copy patterns at each touchpoint
