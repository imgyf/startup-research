# Tone of Voice

**Phase:** 5 — Brand
**Project:** pokemon-champions-team-workspace
**Date:** 2026-05-09
**Confidence:** Medium (voice is opinion; should be road-tested in beta with real users)

---

## Brand Personality (Adjectives)

Four traits that define how Champion's Notebook sounds and behaves:

### 1. **Earnest** — sincere, no marketing voice
We don't say "delight" or "experience." We don't write product copy that sounds like a sales deck. When we mean "save your team," we say "save your team." Persona C is allergic to corporate fluff.

### 2. **Capable** — quietly confident
We know the meta. We know the mechanics. We don't perform expertise — we demonstrate it. We use the right vocabulary (EVs, IVs, Trick Room, Tera, Reg G, Reg H) without over-explaining and without showing off.

### 3. **Grounded** — citations and humility
We refuse to bluff. When we say "Bisharp counters Iron Hands," we cite a damage roll or a tournament dataset. When we don't know something, we say so. This is the single most important voice trait — it's why Persona B will trust us.

### 4. **Calm** — measured, not hype-y
The Pokémon AI category is full of breathless "GAME CHANGER" copy. We're the opposite. We use plain words. We keep paragraphs short. We let the product carry the weight.

---

## Voice Principles

### We Are / We Are Not

| We are | We are not |
|---|---|
| Players who happen to be building a tool | A startup that happens to make a Pokémon product |
| Specific (EV spreads, item slots, tier letters) | Generic (Pokémon-flavored marketing) |
| Honest about limitations | Optimistic about everything |
| Brief | Wordy |
| Citing sources | Asserting authority |
| Conversational | Corporate |
| Pro-community | Pro-disruption |
| Quietly confident | Loudly confident |

### Vocabulary Guide

**Use freely (Persona C/B vocabulary):**
- EVs, IVs, Tera type, Trick Room, Choice band, Assault Vest, Reg G, Reg H, archetype, matchup, pivot, sweep, hazards, setup, paste, ladder, top-cut, regional, win condition, speed tier

**Use carefully (jargon that excludes Persona E):**
- Min-max, 252 Atk / 0 Def, EV optimization, role compression — fine in deep-feature copy, avoid in onboarding

**Avoid (marketing fluff):**
- "delight," "experience," "magical," "next-gen," "powered by AI" (instead: "uses our grounded coach"), "revolutionize," "game-changing"

**Avoid (TPC trademark territory):**
- Don't claim "official" anything
- Don't use "Pokémon" in the brand name
- Don't reference Pokémon types/moves/abilities in brand visuals (text references in product/tools are fine; trademark logos are not)

---

## Writing Samples — How We Sound

### Homepage hero

❌ **Wrong (marketing voice):**
> "Revolutionize your Pokémon Champions experience with the world's first AI-powered VGC coaching platform. Build the perfect team. Crush the meta. Win every match."

✅ **Right (our voice):**
> **The prep workspace VGC players actually use between tournaments.**
> Save your teams, version what works, journal what doesn't, and ask an AI coach that cites its work. Built on @pkmn/sim — no hallucinations.

### Onboarding microcopy

❌ Wrong:
> "Welcome to your AI-powered Pokémon journey! Let's build something amazing together!"

✅ Right:
> **What are you prepping for?**
> Pick a tournament — or just a goal — so we can keep your work organized.

### Feature description

❌ Wrong:
> "Our state-of-the-art AI matchup analyzer leverages cutting-edge machine learning to deliver unparalleled insights."

✅ Right:
> **Matchup coach.** Ask why a matchup is hard. We run real damage calcs and check Smogon usage stats, then explain what's pressuring your team in plain English. Every claim cites a source. If we don't know, we say so.

### Error message

❌ Wrong:
> "Oops! Something went wrong. Please try again later."

✅ Right:
> **Couldn't save that team.** The Showdown import had a malformed item line on slot 3 — usually a typo. Want to look at it?

### Empty state

❌ Wrong:
> "No teams yet! Start your epic journey by creating your first team."

✅ Right:
> **No teams here yet.**
> Import a Showdown paste, start fresh, or copy a sample team to get going.

### Email — tournament reminder

❌ Wrong:
> "🔥 Indianapolis is HEATING UP! 🔥 Don't miss your chance to dominate the meta!"

✅ Right:
> **Indianapolis Regional is in 10 days.**
> You have 3 candidate teams in the workspace and notes on 4 archetypes. Want to set this Regional as your active prep target?

### Social — launch post on r/stunfisk

❌ Wrong:
> "Excited to announce our amazing new tool! Try it free today!"

✅ Right:
> **I built a notebook for VGC prep — looking for sharp feedback.**
> Background: I kept losing track of my own teams between Reg G and Reg H. So I built a workspace that holds team versions, matchup notes, and a coach that cites its sources. Free tier; closed beta for serious feedback. AMA, and please try to break it.

### Social — X/Twitter follow-up

❌ Wrong:
> "🚀 Big news! Our AI coach just hit a new accuracy milestone! Try it now! 🚀"

✅ Right:
> Updated the matchup coach this week — it now runs Trick Room sim variants when you ask about TR matchups. Tested against 200 ladder games; corrected hallucinations on Choice Band Iron Hands EVs (was off by ~12%). Ship notes:

---

## Voice Across Touchpoints

| Touchpoint | Tone modifier |
|---|---|
| Homepage / landing | Earnest, brief, capable |
| Onboarding | Welcoming but precise; no over-explaining |
| In-product copy | Quiet, functional |
| Tooltips / help | Specific, no fluff |
| Error states | Honest, give the user what to do next |
| Email — feature announcements | Restrained ("we shipped X"), not breathless |
| Email — tournament reminders | Calm, calendar-aware, informative |
| Reddit posts | Participatory, "I built / I'm building" voice |
| Twitter/X | Conversational, build-in-public, technical when natural |
| Discord | Founder voice; first-person; participatory |
| Marketing page copy | Minimal hype; measurable claims only |
| Pricing page | Direct, no dark patterns |
| Footer / legal | Clear, no legalese where avoidable |
| Job postings (when we hire) | Honest about scope and stage |

---

## How to Pass the "Persona B Smell Test"

Before publishing any external copy, ask: **Would a 1700+ Smogon ladder player roll their eyes at this?**

- Does it use precise vocabulary correctly?
- Does it avoid claims it can't back up?
- Does it credit the open-source / community sources it depends on?
- Is there *no* "powered by AI" energy?
- Would a top-cut Regional player share it without embarrassment?

If any answer is "no," rewrite.

---

## What to Watch For As We Grow

### Voice drift signals
- Marketing copy starts using "delight," "experience," "journey," "amazing"
- Feature descriptions get longer and louder
- Product tweets get more emoji-heavy
- We start describing the product in the third person to investors more than in the first person to users

### Counter-rituals
- Quarterly voice audit — re-read homepage, onboarding, last 10 emails
- Run all major launch copy past one beta-tester Persona C/B before publishing
- Founder reads at least 3 r/stunfisk threads/week to keep voice calibrated
- If we hire marketing, the brief is "imitate the founder, don't optimize for clicks"

---

## Flags

**Red Flags:**
- None.

**Yellow Flags:**
- This voice requires founder discipline. The moment we hire marketing without strong voice guidelines, drift is likely. Document and audit.
- Earnest + grounded sets a high bar for the AI coach. Any feature that ships with hallucinations directly contradicts the voice and damages the brand.

## Sources

- `02-strategy/positioning.md` — anti-positioning, voice implications
- `02-strategy/value-proposition.md` — verbatim language map
- `03-brand/mission-vision-values.md` — values that resolve voice decisions
- `01-discovery/target-audience.md` — Persona B's allergy to manufactured authority
