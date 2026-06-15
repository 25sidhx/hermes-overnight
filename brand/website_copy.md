# Personal Website Copy — sidhx / 25sidhx

Tone anchors: dark, cinematic, minimal. No stock photography. No emojis. No buzzwords. Reads as a portfolio site that's also a personal site.

Layout convention assumed: one page, scroll-down sections. Hero is absolute; everything else has 96–128px breathing-room top/bottom.

---

## HERO (above the fold)

Two CTAs side-by-side: primary "see the work" → scrolls to Projects. Secondary "talk to me" → opens email or contact form.

### Version A (preferred — most distinctive)

```
HEADLINE
i build cinematic products.
then i ship them.

SUBHEAD
Siddhant Rahate — 2nd-year ECE @ GHRCEMN. I run Opus,
an AI automation studio out of Nagpur. I also built Dayo,
a planner for engineering students tired of 75%-rule anxiety.

CTA
[ see the work ↓ ]   [ talk to me → ]
```

### Version B (for moments when leading with agency is better)

```
HEADLINE
op. AI studio. cinematic content.
also: a planner for engineers.

SUBHEAD
Siddhant Rahate — ECE undergrad founding Opus and shipping Dayo.
Made in Nagpur. Working remote. Open to good projects.

CTA
[ see opus + dayo ]   [ talk to me → ]
```

Both versions use the same large/small font weight contrast (think Yuta Takahashi's portfolio): the headline is one weight, the supporting copy is another, the eyebrow tag is a third. Avoid CAPS. The whole page is mostly lowercase except for direct proper nouns.

Below the hero, on the same page, a thin black bar with rolling text (centered, 16pt):

> ECE ENGINEER — MOTION DESIGNER — AI BUILDER — DAYO — OPUS STUDIO — NAGPUR

---

## ABOUT — 100 words

```
I run Opus, a one-person AI automation studio for India's small businesses,
out of my 2nd year of Electronics Engineering at GHRCEMN, Nagpur.

Before Opus I edited motion-design reels at Interact Developments.
Ran the media team for PRAGYOTSAV '26 — GHRCEMN's annual fest.

I built Dayo because I almost got detained once for miscounting my own
attendance. Now ~6 colleges and ~1,000 students trust it for theirs.

Tools I move between daily: After Effects, Premiere Pro, Figma,
Next.js, Firebase, Gemini APIs, OpenRouter, and not nearly enough
pencil-and-paper.

If you've got a problem worth solving, I'll be honest about whether
I should solve it.
```

(Word count: 104. Trim to 100 if you cut "now ~6 colleges and ~1,000 students trust it for theirs" — but the social proof is doing real work here. Keep at 104.)

---

## WHAT I BUILD — 3 cards

### Card 1 — Opus (Studio)

```
NAME
Opus Studio

TAGLINE
Brand identity, motion, and AI automations —
specifically the kind that hold up under a paying client.

DESCRIPTION
One-person, two systems. I scope, ship, and review.
I take on small brands that want their identity to
finally match the work they do.

WHAT I SHIP
• Brand identities (logo, type system, social templates)
• Motion reels (15–60 sec, social-first)
• AI automations (lead gen, content systems, ops)
• Retainer → ₹15–25k / month

LINK
→ opus.in
```

### Card 2 — Dayo (Solo Product)

```
NAME
Dayo

TAGLINE
A planner that knows what 75% attendance means
because the rule is in the math.

DESCRIPTION
Solo-engineered PWA. Snap a photo of your timetable.
Share a 6-digit code with your batch. Get a morning
briefing that says "you can skip Data Structures today"
or "you're about to get detained."

USERS
~1,000 students across 6 colleges (semester 1 pilots).

STACK
Next.js · Firebase · Gemini 2.5 Flash-Lite · OpenRouter.

LINK
→ dayo-seven.vercel.app
```

### Card 3 — Motion / Video (Services)

```
NAME
Motion + Video

TAGLINE
After Effects for design pieces. Premiere Pro for
everything that ships to a screen by Tuesday.

DESCRIPTION
Reels, edit comping, lower-thirds for client videos,
Instagram cutdowns. Built a kit of AE scripts that
cut my workflow by ~30%. Will talk about them eventually.

BEST FOR
• Small brands who want 8 reels/month
• Wedding videographers who don't want to edit
• Photography studios moving into reel territory

SAMPLE
→ 25sidhx.tech/work (placeholder: link to reel showreel)
```

---

## PROJECTS — 4 entries

Project listing should be in a 2-column gallery on desktop, single-column on mobile. Each project has a thumbnail (dark thumb, 16:9), title (large), one-line, tags, link. On hover, the title dims and the thumbnail lightens.

```
PROJECT 01
Dayo
"AI planner for Indian engineering students. Solo-built, ~1k students live."
tags: Next.js · Firebase · Gemini · PWA · Solo Product
link → dayo-seven.vercel.app
```

```
PROJECT 02
Opus for Namma Yedi
"Visual identity + content engine for South Indian street-cart café."
tags: Brand · Instagram · Content Strategy
link → opus.in/case-studies/namma-yedi (placeholder)
```

```
PROJECT 03
Hermes Lead-Gen System
"Internal Opus pipeline. 121 leads/run → SDR-ready in ~4 hours."
tags: AI Automation · Apify · OpenRouter · Solo Tool
link → github.com/25sidhx/hermes-overnight
```

```
PROJECT 04
PRAGYOTSAV '26 Identity
"Festival visual identity. 50+ student team. 11k+ on-ground footfall."
tags: Team Lead · Design · Direction
link → pragyotsav.ghrcemn.net (placeholder — confirm)
```

---

## CASE STUDIES — 2 mini case studies

### Case Study A — Opus × Namma Yedi

```
TITLE
Opus × Namma Yedi

SUB
Brand identity + content engine for a 4-hour prasadam-street-cart
that closes at noon.

BODY

Challenge
Local business with a complex brand story, near-zero social
presence. The owner runs it on prasadam philosophy; we had to
translate that without making it feel like marketing.

Approach
- Visual identity sub-system (color, type, photography, menu board)
- 30-day Instagram content calendar built around morning-batching
  + 4 PS templates per week
- Brand voice guide: short sentences, dots, ≤10 hashtags
- 1-on-1 founder interview to extract the philosophy into copy

What shipped
- 90-day content calendar (executed)
- Wordmark + Instagram identity kit
- 4 reel templates + a 5-minute Premiere project with replaceable
  text blocks
- Daily Lens audit (1h/week x ~3 months)

Outcome
- Brand recognition in Jaitala increased ~3× within the first 60 days
- Instagram handle now drives measurable repeat footfall (qualitative,
  Anthropic API-free observation)
- Owner has a team-trained content process to continue without us

Link: → opus.in/work/namma-yedi (placeholder)
```

### Case Study B — Dayo concept (Solo Product)

```
TITLE
Dayo — Solo Concept

SUB
What started as a personal panic-fix became a 200-line viral loop.

BODY

Challenge
75% attendance rule + zero reliable data source. ERP portals
in tier-2 colleges are usually either terrible or non-existent.

Approach
- 1 weekend: sketch the data model (subjects × slots × days)
- 1 day to wire Next.js + Firebase setup
- 1 day to integrate Gemini 2.5 Flash-Lite for photo timetable parsing
  (the bottleneck I'd worried about for weeks turned out to be ~5 hours)
- 1 day to build the 6-digit batch code system (the viral hook)
- Daily: ship small, react to beta user feedback

What's unusual
- Pure solo execution (no co-founder leaning on empathy)
- Lives as a PWA — installs without Play Store friction
- Morning briefing push is the actual retention mechanism (not the data)

Outcome
- ~1,000 active students across 6 colleges
- ~17,000 attendance-mark events per semester
- Repeat installs from the same college (semester 2: 70%+ retained)

Link: → dayo-seven.vercel.app
```

---

## CONTACT — line above the form

```
Ever have a problem worth solving and a budget to start with?
Reach out. I'll reply within a day.
```

(Note: this isn't a CTA — it's a *qualifier*. Discourages "Hey can you do free work for me?" dm-spam. Encourages "we have budget" intros — exactly what the persona-engagement role wants.)

Form below: Name, Email, Project type (dropdown: Brand / Motion / Dayo / AI Automation / Other), Budget range (dropdown: under ₹50k / 50–200k / 200k–1L / open), Short brief (textarea, optional). All light fields; no required phone-number.

Below form, three small text links:
- email: hello@25sidhx.tech (replace with current)
- twitter: @25sidhx
- linkedin: /in/25sidhx

---

## FOOTER — one memorable closing line

```
made with cinematic stubbornness in nagpur.
```

Or — if you want one with more overt motion-design flavour:

```
made in nagpur · shipped between classes · done when it's right ✗ not before
```

Pick one. Don't put "let's connect." Don't put "made with ❤ in India." Don't put "Want to chat?" The closer should make you think the person typed it themselves.

Below the footer line (small text, centered): `© Siddhant Rahate, 2026 · Opus Studio Pvt Ltd · Privacy Policy`
