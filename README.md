# Hermes Overnight — Product Intelligence Drop

Solo product research package — this is a parallel mirror of the work done for **Dayo** (an AI-powered PWA daily planner for Indian engineering students, https://dayo-seven.vercel.app).

The same 5 documents were also published at the canonical Dayo mirror: https://github.com/25sidhx/dayo-product-research

This repo (`hermes-overnight`) exists as the long-term research-dump location for any overnight / autonomous intelligence runs done via Hermes Agent. The Dayo materials are the first such drop.

## Repo layout

```
.
├── README.md                          ← you are here
└── docs/
    ├── competitor_analysis.md         ← Phase 1 + Phase 3
    ├── student_pain_points.md         ← Phase 2
    ├── dayo_v2_spec.md                ← Phase 4  (V2 feature spec)
    ├── dayo_ux_copy.md                ← Phase 5  (in-app UX copy)
    └── dayo_launch_kit.md             ← Phase 6 + Phase 7 (GTM + launch copy)
```

## Document index

### 1. `docs/competitor_analysis.md`
Deep-dive profiles for 8 apps — Indian direct (Bunk it, BunkWise, Bunk Manager, Ajack, College Attendance Tracker) and global comparators (My Study Life, Structured, iStudiez Pro, Engross), plus Notion (student use) and Classplus (institutional) as foils. Each profile: features, rating + downloads, pricing, top 3 praises, top 3 complaints, and a 6-axis checklist. Ends with full 20×9 Feature Gap Matrix + "Dayo's Moat" section.

### 2. `docs/student_pain_points.md`
32 raw student comments mined from r/Btechtards, r/Indian_Academia, r/developersIndia, r/IndianEngineers, Quora, MouthShut, Play Store reviews. Clustered into 8 themes with quotes + app-failure attribution + top-3 virality quotes for marketing.

### 3. `docs/dayo_v2_spec.md`
17 V2 feature proposals, each with: pain-cluster reference, build difficulty (Easy/Medium/Hard for Next.js 15 + Firebase), impact (1-10), differentiator flag. Grouped into MUST ship / Nice to have V2 / Save for V3, sorted by impact.

### 4. `docs/dayo_ux_copy.md`
Production-ready UI copy for every Dayo V1 surface: onboarding, schedule builder, morning briefing, attendance tracker, timetable sharing, error/edge states, push notifications. Tone: smart college senior, casual Indian English, no startup-speak.

### 5. `docs/dayo_launch_kit.md`
GTM strategy + 30-day launch calendar + all launch copy: Product Hunt (tagline, description, 5 features, hunter comment), 8-tweet Twitter thread, Instagram caption, 3 angle-specific one-liners, peer-voice WhatsApp class-group message.

## Key findings (TL;DR)

1. **Real direct competition = 1.** Bunk it is the only Indian-built app in the same lane. Its weakness is the paste-into-Another-AI flow (it admits 95% OCR). Dayo's native Gemini photo parser is the real wedge.

2. **Two pain clusters dominate.** "I got detained and didn't see it coming" + "Why do I retype my entire timetable every semester." Dayo V1 addresses both; V2 should reinforce via widgets + WhatsApp share.

3. **Strategic reframe.** Don't compete on "mass-bunk community" — Bunk it owns it and it's ethically sketchy. Pitch Dayo as the **consensual safety app** ("safe to bunk today") to align with parents and college admin, opening institutional channels later.

## Caveats from the original research

- Numbers in the 30-day calendar are direction-style estimates, not data projections
- Theme-clusters are based on Reddit density, not represented-survey sampling
- Some V2 features (F4, F5, F10, F15, F16) depend on user-network scale or external integrations — honest guesses, expect new failure modes
- Classplus was profiled for context only; it's institution-side and not a real Dayo competitor
- Twitter thread hook chosen for visceral readability, not real engagement testing — tweak based on metrics

## Notes on the mirror

The two repos (`dayo-product-research` and `hermes-overnight`) currently contain identical contents. If they diverge in the future:
- `dayo-product-research` = the product canonical repo
- `hermes-overnight` = the long-term research-dump catchall for any autonomous runs
