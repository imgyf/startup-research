# Experiment Design — Top 3 Detailed

**Phase:** 8 — Validation
**Project:** ai-website-sg-restaurants
**Date:** 2026-05-11

---

## Experiment 1 (Detailed): Engineering Spike — 10 spec sites in 1 day

### Hypothesis
A 2-person team can produce production-quality spec restaurant websites at ≤SGD 2/site compute cost and ≤45 min wall-clock per site at small batch.

### Method

**Pre-work (2 hours):**
1. Sign up for Lovable Pro (USD 25), v0 (USD 20), Cursor (USD 20)
2. Set up Vercel deployment pipeline for preview URLs
3. Build a base prompt template:
   ```
   Build a 4-page mobile-first restaurant website for [RESTAURANT NAME]:
   - Hero with restaurant name, tagline, hero photo
   - Menu page (parse from [MENU IMAGE URL or LIST])
   - Reservations page with embedded Chope/booking link
   - Contact page with address, hours, phone, WhatsApp click-to-chat
   Style: clean, modern, fast-loading, mobile-first. Use the restaurant's existing brand colors from [LOGO/HERO].
   Output: deployable React + Tailwind, no external dependencies.
   ```
4. Create a tracking spreadsheet: restaurant name, time started, time finished, AI tool used, prompt tokens, output tokens, compute cost (USD/SGD), final preview URL, quality rating (1-10)

**Execution (8 hours):**
1. Pick 10 SG restaurants from a Google Maps random sample (Joo Chiat or Tanjong Pagar). Mix of cuisines.
2. For each: scrape menu image, hero photo, business hours from their existing Google Business Profile or website (5 min)
3. Run prompt template through Lovable / v0 / Bolt — measure time and cost (30-40 min)
4. Customize: replace template logo, fix obvious AI mistakes, add restaurant photo (5-10 min)
5. Deploy to `tryaisite.sg/preview/[restaurant-slug]` and screenshot
6. Have a non-founder (partner, friend, parent) rate each on 1-10 visual appeal — without telling them it's AI-generated

### Metrics
| Metric | Target | Stretch |
|--------|--------|---------|
| Compute cost per site (SGD) | ≤2 | ≤1 |
| Wall-clock time per site (min) | ≤45 | ≤30 |
| Non-founder quality rating (1-10) | ≥7 average | ≥8 average |
| % sites that work on mobile without bugs | ≥80% | 100% |

### Success Criteria → Decision
- **All 4 metrics hit target:** Proceed to Experiment 2 with confidence. Document the pipeline.
- **3/4 hit, 1 marginal:** Proceed but flag the gap; revisit before scaling.
- **2/4 hit or fewer:** Don't scale. Either invest more in tooling/template work, or rethink the model — if compute is the bottleneck, walk-in-only at higher ACV may be the right answer.

### Timeline
Days 1-2 (parallel with founder admin setup).

### Templates / Tools Needed
- Spreadsheet: `experiment-1-tracking.csv` with columns above
- Base prompt above
- Spec-site URL slug convention: `tryaisite.sg/preview/[normalized-restaurant-name]`
- A `.sg` domain ASAP (~SGD 30/yr at Vodien or Webvisions)

---

## Experiment 2 (Detailed): Walk-In Pilot — 20 restaurants

### Hypothesis
At least 5% of SG independent restaurant owners walked into during 2-4pm will engage with a pre-built spec-site pitch within 6 weeks, and at least 1-2 will convert to paying customers.

### Method

**Pre-work (1 day):**
1. Use the 10 sites from Experiment 1, plus generate 10 more (now that the pipeline is built — should take 4-5 hours)
2. Prepare a sales conversation script (≤90 seconds):
   ```
   "Hi, I'm [name]. I build websites for SG restaurants. I noticed [Restaurant Name] doesn't have a website — actually, I went ahead and built you a sample of what one could look like. Can I show you for 60 seconds on this tablet?"

   [Show preview]

   "I built this in about 30 minutes using AI. We'd ship you the final, customized version in about a week. The price is SGD 1,500 for the full site, or SGD 750 for a basic 3-page version — no monthly fee unless you want one. We're SG-based, you'd own the domain. Want me to leave a card and the link to this preview so you can think about it?"
   ```
3. Print 50 simple business cards (~SGD 30 at Vistaprint) with URL to spec site live
4. Prepare a 5-question intake form for hot prospects: Are you the owner? Do you have a current site? What's frustrating about your online presence? What's your timeline if you do this? What budget would feel right?

**Execution (1 week, 4 walk-in days):**
1. Cluster by neighborhood — one day each: Joo Chiat / Tanjong Pagar / Tiong Bahru / Telok Ayer
2. Visit 5 restaurants per day, 2-4 PM window
3. Open with the script. Track every visit in spreadsheet
4. After each visit: 60-second debrief note (what they said, their face)
5. Send follow-up email same evening to anyone who looked at the tablet ("here's the link again, here's what we discussed, ready when you are")
6. Follow up at 48 hours, 1 week if no response

### Metrics
| Metric | Target | Stretch |
|--------|--------|---------|
| Owner present and willing to look at tablet | ≥60% of visits | ≥75% |
| Engaged conversation 2+ min after tablet view | ≥30% of viewers | ≥50% |
| Asked about price (buying signal) | ≥40% of engaged | ≥60% |
| Committed to a follow-up call/meeting | ≥15% of engaged | ≥25% |
| Paying customer within 30 days of first contact | ≥2 of 20 (10%) | ≥4 of 20 (20%) |

### Success Criteria → Decision
- **Owner-look rate ≥60% AND ≥2 paying:** Wedge works. Scale Experiment 2 → 80 walk-ins in month 2.
- **Owner-look rate 40-60% OR <2 paying:** Pitch needs refinement; redo with revised diagnostic frame (lead with FoodPanda commission math, not "I built you a site"). Re-run 20 walk-ins.
- **Owner-look rate <40%:** Wedge is broken in SG. Stop or pivot to Variation C (different vertical).

### Timeline
Days 3-9.

### Templates / Tools Needed
- Tracking spreadsheet: `experiment-2-walkins.csv` (date, time, restaurant name, address, owner-name-if-given, tablet-look Y/N, engaged-2min Y/N, asked-price Y/N, committed-followup Y/N, paying Y/N within 30d, notes)
- Tablet (iPad or Android tablet — use a personal one to save SGD 250-400)
- Business cards (SGD 30)
- Mobile data plan for tablet (SGD 20-40/month if not piggybacking on phone)
- Sales conversation script (above)
- Follow-up email template

---

## Experiment 3 (Detailed): No-Sale Interviews

### Hypothesis
The objections of non-buyers cluster into ≤3 categories (trust / price / timing), each addressable with a specific tactical change. >50% of objections are NOT "I don't see the need" (which would indicate the pain is too latent for this wedge).

### Method

**Pre-work (1 hour):**
1. List every walked-in restaurant from Experiment 2 who did NOT buy within 14 days
2. Categorize: those who saw the tablet but didn't buy (interesting), those who didn't look (less interesting — they didn't engage at all)
3. Prepare a 10-minute interview guide:
   - "I'm not selling you anything today. I just want to understand."
   - "When I showed you the sample, what was your first thought?"
   - "If you were ever going to commission a website, what would have to be true for you to feel confident saying yes?"
   - "What's your gut on websites in general — necessary, optional, luxury?"
   - "If you had to put a number on it, what would feel like a fair price?"
   - "Were you put off by anything I said or did?"

**Execution (1 week, ~5 hours):**
1. WhatsApp or walk-back to 15 restaurants. "Hi, I'm the guy who showed you the website sample last week — can I buy you a kopi/teh and ask you 10 minutes of questions? I'm not selling, just trying to learn."
2. Expect ~7-10 to say yes (asking for nothing earns goodwill)
3. Conduct 10-min interviews. Record on phone (with permission) or take notes
4. Tag every objection: TRUST / PRICE / TIMING / FEATURE / DON'T-SEE-NEED / OTHER

### Metrics
| Metric | Target | Stretch |
|--------|--------|---------|
| Interviews completed | ≥5 | ≥8 |
| "Don't see the need" share of objections | <50% | <30% |
| Objection categories represented | ≤3 dominate | ≤2 dominate |
| Found ≥1 systematic improvement to pitch | Yes | Yes |

### Success Criteria → Decision
- **"Don't see the need" <30% AND clear 1-3 objection clusters:** The pain is reachable. Refine the pitch around the dominant objection (e.g., if 60% say "timing not now," add a "lock in 2026 pricing today, deliver Q3" promo).
- **"Don't see the need" 30-50%:** Mixed. The diagnostic frame may need to be stronger before the spec site is shown.
- **"Don't see the need" >50%:** The pain is too latent for this wedge to work at scale. Either pivot to Variation C (different vertical with more vocal pain) or significantly raise the diagnostic muscle of the pitch.

### Timeline
Days 8-14 (overlap with end of Experiment 2).

### Templates / Tools Needed
- Interview guide (above)
- Recording tool (phone voice memo)
- Coffee/kopi budget: ~SGD 30 for 5-8 interviews
- Tagging spreadsheet: `experiment-3-objections.csv`

---

## Coordination Across Experiments

```
Day:  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 ... 30
       [E1: ENG SPIKE]
                [E2: WALK-INS         ]
                                  [E3: INTERVIEWS ]
                                              [E4: COLD EMAIL                ]
                [E5: PSG PROBE                              ]
```

**Founder roles (suggested):**
- Founder 1 (sales-lead): owns E2 and E3
- Founder 2 (tech-lead): owns E1 and E4 setup + spec-site production
- Both: contribute to E5, weekly review

**Weekly review cadence:**
- Every Sunday 7pm, 60 minutes
- Review assumption tracker, pull latest spreadsheet data
- Make go / pivot / kill calls for upcoming week
- Update PROGRESS.md with status

---

## What's NOT Being Tested in 30 Days

Deliberate omissions — these are month 2-3 problems:
- Partnership channel (Oddle, Chope, RAS) — start outreach in week 4 but don't expect closes
- Long-tail SEO content — defer to year 2
- LinkedIn outreach — only run if pivot to multi-outlet ACV
- Hawker / coffeeshop segment — separate SKU, year 2
- International expansion — irrelevant at this stage

## Sources
- `06-validation/validation-playbook.md`
- `06-validation/assumptions-tracker.md`
- `01-discovery/raw/distribution.md`
