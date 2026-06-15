# Dayo — Competitor Deep Dive

Scope: apps Indian engineering students actually use (or try) for timetables, attendance, and study planning. Each profile pulls from Play Store descriptions, official sites, and user reviews. India-specific apps given extra weight because they are the real competitive set.

Note on methodology: this is not lab research. Ratings and download counts are approximate from public Play/App Store listings at time of search. Some apps (Classplus, Notion) are not direct competitors — included to clarify what Dayo is *not* competing with.

---

## 1. Bunk it (bunkitapp.in) — *PRIMARY DIRECT COMPETITOR*

Indian-built, Indian-targeted, by Faisal Khan (Instagram handle @\_faisal.in). This is the app Dayo will most directly fight for users.

**Core features:**
- Per-subject and overall attendance tracking
- "Safe Skip %" — how attendance will look if you skip the maximum allowed
- Bunk calculator (subject-wise)
- "Can I Skip Today?" quick check for impact of skipping today's class
- Leave Planner — enter planned leaves, see projected attendance
- Long Weekend Finder — finds best leave combinations
- AI-generated JSON from a timetable screenshot (uses external AI like Gemini — not built-in OCR)
- Card / Table / Graph views
- QR code class sharing (import/export)
- Daily reminder notifications (default 5 PM IST)
- Backup/restore via JSON
- Community: polls + mass-bunk probability (unlocks when all active members safe above 75%)

**Play Store / App Store:** No exact download count surfaced — web app with downloadable wrapper. Says "India's #1 free attendance tracker."

**Pricing:** Free with "Premium" tier (Premium badge in UI). Some advanced features paywalled (Premium tier assumed via "👑 Premium" UI marker).

**Top 3 things users praise:**
1. AI timetable-to-JSON conversion removes the worst manual step
2. "Can I Skip Today?" is fast and matches college math
3. Offline-first, no forced sign-in

**Top 3 things users complain about (from Play Store and Reddit):**
1. AI prompt-step is awkward — you have to copy a prompt into Gemini and paste back. OCR is "95% accurate" per their own disclosure (so still needs verification) ("💡 Long Weekend Finder" — full OCR disclaimer on site)
2. Mass-bunk community only works if everyone joins the same class — empty network effect problem
3. No unified morning view / no integration with class schedule and attendance in one screen

**Checklist:**
| | |
|---|---|
| Attendance tracker | ✅ |
| Bunk calculator | ✅ |
| Timetable photo import | ⚠️ (requires external AI paste-back) |
| AI features | ⚠️ (uses external AI, not native) |
| Timetable sharing | ✅ (QR code, not 6-digit) |
| India semester / 75% | ✅ (explicitly built for this) |

**Verdict:** Bunk it is strong on attendance but weak on the schedule side. Dayo's edge is the photo-to-timetable UX (Gemini native) and the morning briefing layer that combines schedule + attendance + status into one surface.

---

## 2. My Study Life

Global cross-platform planner. Long-running, well-known, backed by a real company.

**Core features:**
- Classes, assignments, exams, tasks, revision
- Weekly and *rotating* schedules (not just weekly)
- Cross-device sync (mobile + web)
- Reminders
- Dashboard view of upcoming work
- Free for students (ToS mentions paid school plans)

**App Store:** "Trusted by over 24 million students in 197 countries."

**Pricing:** Free for individual students. School/institution licenses paid.

**Top 3 things users praise:**
1. Cross-platform sync actually works
2. Rotating schedule support (handles week A / week B timetables)
3. Clean, distraction-free UI

**Top 3 things users complain about:**
1. No attendance tracking — the biggest gap for Indian students
2. India-specific semester structure not modeled (no concept of "current semester subjects only")
3. Overkill for the "where is my next class + how many can I bunk" use case

**Checklist:**
| | |
|---|---|
| Attendance tracker | ❌ |
| Bunk calculator | ❌ |
| Timetable photo import | ❌ |
| AI features | ❌ |
| Timetable sharing | ❌ |
| India semester / 75% | ❌ |

**Use case:** International general-purpose planner. Not built for the Indian 75% problem. Dayo's wedge is "we solve the problem My Study Life ignores."

---

## 3. Structured (Structured app)

Premium daily planner, uses visual timeline + AI.

**Core features:**
- Visual time-blocked day view
- Inbox, recurring tasks, sub-tasks
- Pomodoro focus timer
- Apple Watch, widgets, Live Activities (iOS-heavy)
- Structured Pro: calendar sync, AI day planning, "Replan," custom notifications

**Pricing:** Pro is $2.99/mo, $9.99/yr, $29.99 lifetime. Free tier exists (limited).

**Top 3 things users praise:**
1. AI day planning ("draft your schedule in seconds")
2. Visual timeline is satisfying for ADHD users
3. Polished iOS-native experience

**Top 3 things users complain about:**
1. iOS-only effective experience (Android tier is weaker)
2. Pro paywall hits core features — AI replanning locked
3. No attendance tracking, no India context, expensive for what it offers an Indian student

**Checklist:**
| | |
|---|---|
| Attendance tracker | ❌ |
| Bunk calculator | ❌ |
| Timetable photo import | ⚠️ (scan-feature mentioned but for calendars/not timetables) |
| AI features | ⚠️ (Pro only) |
| Timetable sharing | ❌ |
| India semester / 75% | ❌ |

**Use case:** Premium iOS productivity. Not Dayo's target market.

---

## 4. iStudiez Pro

Veteran student planner (since iOS early days). Strong for college course tracking.

**Core features:**
- Course/term/semester management
- Assignments + grade tracking + GPA calc
- Schedule view, calendar, planner
- Available iOS, Mac, Windows (no Android historically)

**Pricing:** Paid one-time (historically $1.99 to higher tiers in later years).

**Top 3 things users praise:**
1. Purpose-built for student course structure
2. Grade tracking + GPA built in
3. Senior, stable app — well-known

**Top 3 things users complain about:**
1. No Android version — Indian engineering students are predominantly Android
2. No attendance tracker
3. Outdated UX compared to modern apps

**Checklist:**
| | |
|---|---|
| Attendance tracker | ❌ |
| Bunk calculator | ❌ |
| Timetable photo import | ❌ |
| AI features | ❌ |
| Timetable sharing | ❌ |
| India semester / 75% | ⚠️ (term concept exists, but no 75% rule) |

**Use case:** iOS-only audience, US-style term system. Irrelevant to most Indian students.

---

## 5. Engross: ADHD Focus Timer

Pomodoro + to-do + calendar + "app blocker."

**Core features:**
- Pomodoro / Stopwatch timer (configurable)
- Progressive To-Do list
- Focus session tracking
- Calendar / routine view
- "App blocker" for phone addiction

**Pricing:** Free with in-app purchases.

**Top 3 things users praise:**
1. Pomodoro + to-do + calendar combo
2. Customizable timer ranges
3. Genuinely useful for ADHD focus

**Top 3 things users complain about:**
1. No timetable or attendance tracking
2. Productivity-focused, not academic-focused
3. Notifications and routine management is shallow

**Checklist:**
| | |
|---|---|
| Attendance tracker | ❌ |
| Bunk calculator | ❌ |
| Timetable photo import | ❌ |
| AI features | ❌ |
| Timetable sharing | ❌ |
| India semester / 75% | ❌ |

**Use case:** Focus / ADHD product. Could be a *complementary* app to Dayo, not a competitor. Possibly mention as integration partner.

---

## 6. Notion (student use case)

Not a mobile app, but heavily used by Indian students for planning.

**Core features:**
- Databases, pages, templates, calendar views
- Student templates available in marketplace
- Self-managed — user builds their own system

**Pricing:** Free for individuals. Notion Plus for power users.

**Top 3 things users praise:**
1. Total flexibility — build whatever system you want
2. Free
3. Powerful template ecosystem

**Top 3 things users complain about:**
1. Setup overhead is brutal — takes hours to build a working student system
2. Mobile experience is slow and clunky for daily use
3. No attendance math, no automatic 75% calculation, no notifications for class

**Checklist:**
| | |
|---|---|
| Attendance tracker | ⚠️ (only via templates, manually calculated) |
| Bunk calculator | ❌ |
| Timetable photo import | ❌ |
| AI features | ✅ (Notion AI, separate paywall) |
| Timetable sharing | ✅ (shared pages, not designed for class schedules) |
| India semester / 75% | ❌ |

**Use case:** Power-user alternative. Dayo wins on "ready in 2 minutes vs 2 hours." Use as a positioning foil: "Notion for the 99% of students who don't want to build a system."

---

## 7. Classplus (co.andrea.mjzyt / Classplus app)

Misunderstood — Classplus the SaaS company is a teacher/coaching management platform. There is also a "Class Plus" generic student app. Including both here for clarity.

**Real Classplus (classplusapp.com):**
- For coaching institutes and tutors
- Attendance, fees, live classes, payments
- Sold to institutes, not students
- *Not a Dayo competitor* — different buyer

**Top 3 things users (students) complain about (Classplus institutional software on review sites):**
1. "Fraud company with 0 customer service. They sell you subscriptions promising false claims." (MouthShut)
2. "Very High Commissions, Poor Performing System Slow Loading" (Quora)
3. "Limited customization options… not for traditional schools" (Techjockey)

**Class Plus generic student app (Google Play, co.andrea.mjzyt):**
- Attendance, lesson planning, assignments
- Generic, not India-engineering specific
- Low traction

**Takeaway:** Classplus is NOT a Dayo competitor. Useful only as a reference for what *not* to build (institution-side software). Skip from the dayo's marketing radar.

---

## 8. India-specific attendance apps (long tail, quick survey)

Saturated subcategory. Most are 10K–100K downloads, basic design, single-purpose.

### Attendance Manager (Ajack) — com.codekaaru.attendancejack
- 75% rule focus, multi-subject
- Simple UI, calibrated for Indian semester
- In-app purchases, ads

### BunkWise — com.eshinmakeapps.bunkwise
- Bunk planner, attendance calculator
- Problems: clunky manual entry, no daily schedule view

### Bunk Manager — com.bunk.manager
- Old, basic, no photo input, ads-heavy
- One of the OG bunk-calculator apps

### College Attendance Tracker — com.sirmaur.attendance_tracker
- 4.6 rating, 10K+ downloads, 72 reviews
- Attendance %, bunk calc, notes/to-dos, dark mode, mini-games
- Strength: "designed for Indian students"
- Weakness: To-do + attendance + timetable UI gets crowded fast ("attendance interface is a bit lacking compared to another tracker app" — user review)

### Self Attendance — saurabhrao.selfattendance
- Multi-purpose but barebones

### Pattern across the long tail:**
- All do attendance and bunk math correctly
- All require manual entry of timetable (text)
- None offer seamless photo-to-timetable
- None deliver a unified "what's today like" morning briefing
- None do timetable sharing via code — usually share via JSON file or QR

**This is the lane Dayo occupies.**

---

## 9. Quick comparator summary

| App | Attendance | Bunk math | Photo timetable | Share | India 75% | Free core |
|---|---|---|---|---|---|---|
| **Bunk it** | ✅ | ✅ | ⚠️ AI paste | QR | ✅ | ⚠️ Premium tier |
| **My Study Life** | ❌ | ❌ | ❌ | ❌ | ❌ | ✅ |
| **Structured** | ❌ | ❌ | ⚠️ | ❌ | ❌ | ❌ Pro paywall |
| **iStudiez Pro** | ❌ | ❌ | ❌ | ❌ | ⚠️ | ❌ paid |
| **Engross** | ❌ | ❌ | ❌ | ❌ | ❌ | ✅ |
| **Notion (student)** | ⚠️ manual | ❌ | ❌ | page-level | ❌ | ✅ |
| **BunkWise / Bunk Manager / Ajack** | ✅ | ✅ | ❌ | ❌ | ✅ | ⚠️ ads/IAP |
| College Attendance Tracker (Sirmaur) | ✅ | ✅ | ⚠️ image upload limited | ❌ | ❌ | ✅ | ⚠️ ads/IAP |
| **Dayo V1** | ✅ | ✅ | ✅ native Gemini | ✅ 6-digit | ✅ | ✅ |

Dayo's specific advantage stack:
1. Native photo-to-timetable (Gemini native, not paste-prompt)
2. 6-digit sharing code (zero friction vs QR / JSON file)
3. Morning briefing layer (no competitor consolidates schedule + attendance in one daily view)
4. 100% free core (no Premium tier blocking 75% math)
5. PWA — installs on any phone, no Play Store friction

---

# PHASE 3 — FEATURE GAP MATRIX

Legend: ✅ has it · ❌ missing · ⚠️ partial/limited

| Feature | Bunk it | My Study Life | Structured | iStudiez Pro | Engross | Notion (student) | BunkWise/Bunk Manager | Dayo V1 |
|---|---|---|---|---|---|---|---|---|
| AI schedule generation (text → plan) | ❌ | ❌ | ⚠️ Pro only | ❌ | ❌ | ❌ | ❌ | ✅ OpenRouter |
| Timetable photo parsing (native) | ⚠️ paste-prompt | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ✅ Gemini Flash-Lite |
| 75% attendance math (Indian rule) | ✅ | ❌ | ❌ | ❌ | ❌ | ⚠️ template manual | ✅ | ✅ |
| Bunk count calculator | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ✅ | ✅ |
| Timetable sharing via short code | ⚠️ QR | ❌ | ❌ | ❌ | ❌ | ⚠️ page share | ❌ | ✅ 6-digit |
| Morning briefing / daily summary | ❌ | ⚠️ dashboard | ⚠️ timeline | ⚠️ planner view | ⚠️ calendar | ❌ | ❌ | ✅ |
| Offline support | ✅ | ⚠️ partial | ❌ | ❌ | ⚠️ | ⚠️ slow | ✅ | ✅ PWA |
| India semester structure support | ✅ | ❌ | ❌ | ⚠️ term only | ❌ | ❌ | ✅ | ✅ |
| Free tier with no paywalled core features | ⚠️ Premium exists | ✅ | ❌ | ❌ paid | ✅ IAP only | ⚠️ AI paywall | ⚠️ ads/IAP | ✅ |
| Push notifications for class reminders | ⚠️ attendance-only | ✅ | ⚠️ Pro | ⚠️ | ❌ | ❌ | ⚠️ | ✅ |
| Low attendance alerts (below 80%) | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ✅ |
| Multiple timetable profiles (parallel semesters) | ❌ | ✅ | ⚠️ | ✅ | ❌ | ⚠️ | ❌ | ❌ (V2 candidate) |
| Widget support (home screen) | ❌ | ⚠️ limited | ✅ iOS only | ⚠️ | ⚠️ | ❌ | ❌ | ❌ (V2 candidate) |
| WhatsApp / notification integration | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ (V2 candidate) |
| Dark mode | ⚠️ | ✅ | ✅ | ✅ | ✅ | ✅ | ⚠️ | ✅ |
| App blocker / focus (anti-distraction) | ❌ | ❌ | ⚠️ via reminders | ❌ | ✅ | ❌ | ❌ | ❌ |
| Assignments / homework tracking | ❌ | ✅ | ✅ | ✅ | ✅ todo | ✅ | ❌ | ❌ (V2 candidate) |
| Grade / GPA tracking | ❌ | ✅ | ❌ | ✅ | ❌ | ⚠️ template | ❌ | ❌ (V3) |
| Rotating schedule (Week A / Week B) | ❌ | ✅ | ❌ | ✅ | ❌ | ⚠️ manual | ❌ | ❌ |
| Mass-bunk community (multi-user) | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ (V3) |

## Dayo's Moat — features nobody else does (or does well)

These are Dayo's strongest marketing angles. Lead with them in any pitch material.

1. **Native photo-to-timetable.** Gemini 2.5 Flash-Lite converts a paper/PDF timetable image to structured data in one tap. No paste-prompt into another AI. No manual typing of 6 subjects × 5 days × time slots.
2. **6-digit timetable-sharing code.** Your entire batch joins your timetable in 10 seconds by typing 6 digits. QR apps need camera line-up, JSON apps need file transfer. Dayo treats timetable distribution like WiFi-password sharing. This is the *viral lever*.
3. **Unified morning briefing.** One card, every morning, surfaces: today's classes, attendance %, safe-bunk count for each subject, and a danger warning if anything is below 80%. No one else does schedule + attendance in one push surface.
4. **Built for the Indian 75% rule as first-class math.** Not a template; not a formula the student writes. Default threshold is 75%, changeable per college.
5. **PWA — installs in 10 seconds, no Play Store.** Works offline by default. Crucial for Indian network reality.
6. **Solo dev = no premium tier, no ads, no upsell.** Built by a student who gets it. Free core, forever. This is positioning vs Bunk it (which already has a Premium tier).
7. **Daily low-attendance push.** Push notifications fire when any subject slides under 80% — not after the fact, not buried in an in-app badge. The "you got detained wasn't expecting it" failure mode is the worst pain in Theme 1 of student_pain_points.md; this kills it.
8. **AI schedule generation for what to do *next*.** Once attendance is safe, the AI plans "what should you actually study right now" — moves Dayo from "policing tool" to "study partner" (higher emotional loyalty).

