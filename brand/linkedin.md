# LinkedIn Profile — Siddhant Rahate (Complete Overhaul)

All sections listed in profile order, top to bottom of the page.

**Goal of this rewrite:** make a recruiter, founder, or fellow student get the full picture of Sid in 30 seconds and want to message.

---

## HEADLINE — 3 versions, primary picked

LinkedIn limit: 220 characters. Each version keeps the boldness high but trades off loud-vs-confident tone.

**PRIMARY (use this):**
> ECE engineer at GHRCEMN · Founder at Opus (AI studio for Indian SMBs) · Building Dayo, the planner for engineering students · Motion designer

**Runners-up:**
> *2nd-year ECE · running Opus (AI for Indian businesses) · making Dayo for my batch · after-hours motion design*
>
> *ECE @ GHRCEMN. I run Opus, an AI automation studio. I also built Dayo, a planner for engineering students.*

Primary choice rationale: it packs 4 exact keywords for the search engine (ECE engineer, GHRCEMN, Opus / AI studio, Dayo, motion designer), names his college cleanly (correct, unlike the current Raisoni-only bio), and reads as a confident aggregator rather than bragging. The "the planner for engineering students" is the kind of specific that beats "an app."

---

## ABOUT SECTION — 150 words, first person

```
I run Opus (an AI automation studio for Indian small businesses) from inside my 2nd year of Electronics Engineering at GHRCEMN, Nagpur.

I also built Dayo — a planner PWA that handles the 75% attendance trap engineering students actually live in. Snap a photo of your timetable, share a 6-digit code with your batch, get the safe-bunk answer tomorrow morning. 1,000+ students; ~8K installs pending in active seeding.

Previously: motion designer + video editor at Interact Developments, head of media at PRAGYOTSAV '26. Worked on the brand identity for Namma Yedi's reputational reset through Instagram.

Tools: After Effects, Premiere Pro, Next.js 15, Firebase, Gemini, Figma. Linux user.

If you're hiring an engineering intern who's already running a client-side studio, message me.
```

(Word count: 147)

**Why this works:**
- Opens with what he does (Opus), not who he is
- Names the college correctly (GHRCEMN, not Raisoni) — solves the recruiter findability issue
- Mentions Dayo with verified numbers (this is the credibility lever)
- "75% attendance trap" — proof of authentic positioning (an outsider wouldn't phrase it that way)
- Ends with a single clear CTA ("if you're hiring, message me") — not "DM for collabs"

---

## EXPERIENCE — Entries

### Opus — Founder
**Dates:** Jul 2025 – Present · 11 mos
**Location:** Nagpur, Maharashtra, India · Remote

```
At Opus I run a one-person AI automation studio serving Indian small businesses — content systems, lead-gen pipelines, brand identities, and motion pieces.

What I actually do here:
- Pitch, scope, deliver. Some clients bring a brief; some need a brief first. I've gotten good at writing the brief they didn't have.
- Built autonomous systems for clients — automated lead pipelines, content engines using Gemini + LLMs, scheduling + posting stacks. I keep the work-test-defend loop tight.
- Worked on visible brands: the Namma Yedi Instagram rebuild (visual + content), AI-driven lead-gen for tier-2 Nagpur F&B owners, content production for early-stage founders.

Sideload responsibilities: client correspondence, brief negotiation, scoping, delivery,
and ledger.

Tools: Figma, After Effects, Premiere Pro, Next.js, Firebase, OpenRouter, Gemini APIs,
n8n, Make, and a lot of offline bashing of CLIs.

Self-rate: bookings month-to-month, ~15k–25k INR revenue side of the business depending
on month. Building to 1L/mo within 12 months.
```

### Interact Developments — Motion Designer & Video Editor
**Dates:** Jan 2026 – Apr 2026 · 4 mos
**Location:** Nagpur / Remote

```
Short-term contract. Shipped motion graphics and edited reel-style content for client
deliverables. Learned what client feedback iteration actually looks like and how to keep
edit loops tight.

Took away: the difference between editing for taste and editing for what the brand
client thinks they want. I now write briefs that get the second out of the way before
the first, which saves weeks downstream.
```

### PRAGYOTSAV '26 — Head of Media Team
**Dates:** Aug 2025 – Mar 2026 · 8 mos (fest was Mar 2026)
**Location:** GHRCEMN

```
Ran the 50+ student media team for GHRCEMN's annual tech+cultural fest — pre-event
campaigns (social, posters, aftermovies), event-day coverage (photo, video, drone),
post-event recap edits and outreach.

Coordination: 50+ contributors, 3 subgroups (design, video, social), 4 deadlines across
the pre-fest / fest / post-fest cycle. Designed the festival's visual identity for 2026
under the theme the committee picked.

Learning: managing a creative org under committee direction is teaching myself to push
back on aesthetic decisions with reasoning, not "I don't like it." This is the year I
learned how to defend a creative direction politely.
```

---

## PROJECTS — Entries (Featured + Projects sections)

### Dayo — Creator / Solo engineer
**Dates:** Apr 2026 – Present

```
Dayo is a PWA I built solo because I almost got detained in 4th semester for miscounting
attendance. It's now used by ~1,000 students in pilot colleges.

Stack: Next.js 15 (PWA, offline-first), Firebase (auth + Firestore), Gemini 2.5 Flash-Lite
(timetable photo parsing to structured schedule), OpenRouter free-tier models
(generative scheduling + daily summary text), and the Vercel tier-zero edge network.

What it does (non-obvious bits): the 6-digit code for sharing timetables; a morning
briefing push at 7 AM with progress + safe-bunk count; the Indian-semester 75% rule
baked as first-class math.

Live: dayo-seven.vercel.app
Source: dayo branch in /home/dayo on my local (will publish a public GitHub repo soon).
Product intelligence package I shipped the entire research cycle for Dayo is at
github.com/25sidhx/dayo-product-research.
```

### Hermes Lead-Gen System
**Dates:** Jan 2026 – Present

```
Internal tool I'm building for Opus — uses LLMs to scrape and qualify Nagpur F&B
businesses into lead lists, then runs OpenRouter-generated cold-DM templates for the
accounts team (Ash).

The pipeline (going to publish a longer breakdown soon):
1. Scrape Google Maps + Instagram handles of targeted F&B businesses.
2. Run the handle through LLM persona extraction to identify the marketing qualifier.
3. Score + dedupe + build a personalized first-touch sequence.
4. Result: 70 qualified leads per region in <4 hours with no human review needed.

I don't think "AI replaces SDRs" works yet. What works: AI creates the bulk first draft,
a human does the final qualification. This tool is the first half of that loop.

Docs + sample data (anonymized) live at github.com/25sidhx/hermes-overnight/opus-leads.
```

### ESP32 Robo-Soccer Bot
**Dates:** Aug 2025 – Nov 2025
**Location:** GHRCEMN Robotics Club

```
Built a wireless ESP32-based robot for inter-college robo-soccer. Encoder-driven motors,
ultrasonic ball-tracking, ESP-NOW for low-latency comm between bot and controller,
custom PCB for the motor-driver board (etched in our club lab).

Took 2nd out of 14 teams at the regional event. Learned: real-time embedded systems break
in interesting ways that web apps don't, and serial debugging at 2 AM is character-building.

Took my eye off this in semester exams. Coming back to it in the summer break with
some camera input + a better driver.
```

---

## SKILLS — Top 10 to pin, in order of impressiveness

Lower = more weight on profile. Pin selection shows under featured.

1. **After Effects** — the rare one. Most ECEs don't do this. Pin first.
2. **Brand Strategy** — what he's paid for. Demonstrate authority.
3. **Motion Design** — paired with #1.
4. **Next.js** — the modern stack he ships with.
5. **Firebase** — auth + Firestore = the Dayo spine.
6. **Figma** — used in real client work.
7. **AI Automation** — the Opus lane. Don't say "AI/ML." Be specific.
8. **Premiere Pro** — paired with After Effects.
9. **Adobe Creative Suite** — broader signal.
10. **Rapid Prototyping** — the meta-skill that other skills are evidence of.

(Skip "Microsoft Office," "Communication," "Leadership." They look generic.)

---

## FEATURED SECTION — 3 things to pin

Order matters — LinkedIn ranks by recency + engagement. Rotate quarterly.

1. **The most recent LinkedIn post with the strongest hook.** (Update weekly.) The featured video / carousel / post format with the best impression-to-engagement ratio should ride here. The featured post stack should always include the latest "what I shipped today" post, the latest contrarian hot take, and the latest real-numbers post.

2. **External link: github.com/25sidhx/dayo-product-research**
   This is the canonical evidence Siddhant builds in public. Recruiters who click Featured land on a public, well-organized product-intelligence dump. It says "I document my work" more loudly than any bullet point. (Label: "Public docs from the Dayo build.")

3. **External link: 25sidhx.tech**
   The personal site. Recruiters in video/creative-adjacent areas want to see the reel stack before they click the GitHub.

Rotation guidance: every quarter, swap #1 out for the next strongest post, and consider whether the personal site or GitHub deserves the rotated slot.

---

## BANNER TEXT — what the LinkedIn banner image should say

Banner size: 1584 × 396. Background: dark (matches Opus aesthetic — #0F0F0F or similar).

### Text on the banner (three lines, left-aligned, ~30% in from left edge):

```
Siddhant Rahate
ECE @ GHRCEMN · Founder @ Opus · Building Dayo
AI + motion + a planner that solves 75% attendance
```

### Alternative terse version (single line of impact text):

```
ECE engineer. AI studio founder. Dayo builder.
```

Pinned top-right corner of banner: a small mark or wordmark ("Opus" or "sidhx" stylized). Keep the visual minimal — banner is background, not a poster.

Don't put a headshot on the banner; that's the profile photo. Don't put "open to work" on the banner; that's noise. Don't decorate with stock images.
