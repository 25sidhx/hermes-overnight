# Dayo V2 — Feature Specification

Pain point clusters referenced below are from student_pain_points.md.

Build difficulty scale:
- **Easy** = 1–2 days for one solo dev
- **Medium** = 3–5 days
- **Hard** = 1–2 weeks+

Impact score = how much this feature alone would make a student pick Dayo over a competitor (1–10).

Differentiation flag = **Y** if no competitor in the gap matrix has this (or does it poorly).

---

## PROPOSED FEATURES (17 total)

### F1 — "Class actually happened?" / proxy-cancellation marker
**Description:** After a class ends, a one-tap asks "Did this class actually happen?" If teacher was absent or class got cancelled, the student can mark it as cancelled — attendance math adjusts so no class counts as neither present nor absent.
**Solves:** Theme 8 (Class cancellation / proxy attendance / lab variance)
**Difficulty:** Easy
**Impact:** 8
**Differentiator:** Y — Bunk it and others treat attendance as student-only decision. None of them model "the class didn't run."

### F2 — Lab vs Theory separation
**Description:** Different attendance rules for labs (often 100% mandatory or averages different). Student tags a subject slot as "theory" or "lab" and threshold is set per type.
**Solves:** Theme 7 (single live source of truth — niche refinement), Theme 3 (Indian math)
**Difficulty:** Easy
**Impact:** 6
**Differentiator:** ⚠️ Partial — Bunk it can do this through JSON; not surfaced in main UI. Dayo surfaces it.

### F3 — WhatsApp share of timetable & "join batch" link
**Description:** A "Share on WhatsApp" button on the timetable auto-fills a WhatsApp message with the schedule preview and a 6-digit code. Tapping the code deep-links into Dayo.
**Solves:** Theme 6 (WhatsApp is the class ops layer)
**Difficulty:** Medium
**Impact:** 9
**Differentiator:** Y — no competitor has any WhatsApp integration

### F4 — "Today's class was actually held?" check (collaborative)
**Description:** Within minutes, if multiple students in the same batch tap "class was held," it confirms the class actually ran. If 3+ students say "didn't run," Dayo automatically marks the class as cancelled for the whole batch (opt-in).
**Solves:** Theme 8
**Difficulty:** Hard (real-time, opt-in privacy model)
**Impact:** 8
**Differentiator:** Y — closest analog is Bunk it's mass-bunk poll, but that's the opposite intent; Dayo's is the safety check.

### F5 — Per-subject "what's my rank in the batch?" (proxy signal)
**Description:** Aggregate, anonymized "your attendance is in the top decile of your batch for this subject" signal. Builds social reassurance without revealing specific peers.
**Solves:** Theme 7
**Difficulty:** Hard (privacy fence, server-side aggregates)
**Impact:** 4
**Differentiator:** Y
**Risk:** privacy backlash. Defer or test carefully.

### F6 — Widget: "Today"
**Description:** Home-screen widget (Android + iOS via PWA bridge) showing today's class at top, attendance % in danger zone if any, next-bunk-safe count.
**Solves:** Theme 5 (bunk math is uncached, repeated daily)
**Difficulty:** Hard (PWA widget support varies; iOS limited)
**Impact:** 9
**Differentiator:** Y — no Indian-student competitor has a working widget.

### F7 — Quick "Mark as attended" from the morning briefing
**Description:** When the morning briefing push lands, a single tap on the notification marks attendance for the next class. Tapping → opens "attended / bunked" for the first subject of the day.
**Solves:** Theme 5
**Difficulty:** Medium
**Impact:** 8
**Differentiator:** Y — zero-friction attendance push

### F8 — Subject difficulty rating (1-tap) → AI study hints
**Description:** Student rates each subject "hard / okay / chill." The AI uses this to rotate "what should I revise tonight" recommendations.
**Solves:** Theme 2 (manual pain — extends Dayo from "tracking" to "guidance")
**Difficulty:** Easy
**Impact:** 6
**Differentiator:** Y

### F9 — Streak / heatmap of attendance
**Description:** GitHub-style green-square heatmap on the dashboard. Visual reward for consistent attendance.
**Solves:** Theme 7 (gamifies the source of truth)
**Difficulty:** Easy
**Impact:** 7
**Differentiator:** ⚠️ Partial — visual flair is uncommon in this category

### F10 — Parents' WhatsApp summary (opt-in)
**Description:** Optional. Dayo sends a single weekly WhatsApp to parent — "Hi, X attended Y of Z classes last week, attendance is X%."
**Solves:** Theme 1 (detention fear — adds social pressure + safety net for some families)
**Difficulty:** Medium
**Impact:** 4 (only opt-in users)
**Differentiator:** Y — Indians care about this; no app does it.
**Risk:** Cultural pushback from older students.

### F11 — "Pre-bunk" / week-ahead planner
**Description:** Calendar view of next 2 weeks. Tap a future date → "if you skip these classes today, your attendance drops to X%." Lets student plan a real skip decision.
**Solves:** Theme 5
**Difficulty:** Medium
**Impact:** 8
**Differentiator:** Y (closest analog is Bunk it's Long Weekend Finder — Dayo can do it faster in UX)

### F12 — Multi-batch timetable (only valid subjects for current semester)
**Description:** User can flip between "this semester's subjects" and "previous semester's," or "this elective / that elective." Each profile has independent attendance.
**Solves:** Theme 7 (long-term users)
**Difficulty:** Easy
**Impact:** 5
**Differentiator:** ⚠️ Partial — My Study Life has it. Dayo differentiates by tying it to attendance profiles.

### F13 — Voice / quick text "add next class"
**Description:** "Hey Dayo, tomorrow I have DSA at 10" — adds a one-off class via OpenRouter with natural language parse.
**Solves:** Theme 2
**Difficulty:** Medium (LLM call latency + parsing)
**Impact:** 6
**Differentiator:** Y

### F14 — "Confirmed safe to bunk today" one-tap answer widget
**Description:** Tile-size widget that shows up before each class: green = safe to skip / yellow = borderline / red = don't you dare. Built around the morning-class decision.
**Solves:** Theme 5, Theme 1
**Difficulty:** Medium
**Impact:** 9
**Differentiator:** Y

### F15 — College ERP paste-link integration (read-only)
**Description:** User pastes their Academia ERP / DigiCampus URL. Dayo auto-imports attendance numbers (where public portals allow). If blocked, Dayo just shows a "your ERP doesn't expose this — keep marking here" message.
**Solves:** Theme 4 (ERP portals are bad)
**Difficulty:** Hard (every college is different; many block scraping)
**Impact:** 5
**Differentiator:** Y
**Risk:** Build cost vs payoff. Build only if 1–2 colleges offer a clean endpoint.

### F16 — "Compare with batch" heatmap (aggregated)
**Description:** Each subject card shows "your attendance vs batch average" with a small bar chart. Aggregated, anonymized, opt-in via batch code.
**Solves:** Theme 7
**Difficulty:** Hard (privacy, opt-in flow)
**Impact:** 5
**Differentiator:** Y
**Risk:** Dead on arrival if join rate is too low.

### F17 — In-app "what happens if I drop this subject this semester?" simulator
**Description:** Toggle a subject "I'm thinking of dropping" → see impact on attendance for the *other* subjects.
**Solves:** Theme 5 (decision support)
**Difficulty:** Easy
**Impact:** 5
**Differentiator:** Y

---

## GROUPED RELEASE PLAN

### MUST SHIP in V2 (high impact, doable this semester)

| Rank | Feature | Impact | Difficulty |
|---|---|---|---|
| 1 | **F3 — WhatsApp share** | 9 | Medium |
| 2 | **F14 — "Safe to bunk today" widget** | 9 | Medium |
| 3 | **F6 — Widget: Today** | 9 | Hard |
| 4 | **F11 — Pre-bunk week planner** | 8 | Medium |
| 5 | **F7 — Mark attended from notification** | 8 | Medium |
| 6 | **F1 — Class actually happened marker** | 8 | Easy |
| 7 | **F9 — Attendance streak heatmap** | 7 | Easy |
| 8 | **F8 — Subject difficulty rating** | 6 | Easy |

**Why this group:** every F1 here has impact 6+ and a doable build. The 8 features combine to make Dayo feel like the obvious answer to "I'm an engineering student who doesn't want to get detained and doesn't want to type." Punch-line in the launch deck: "share the code, share the schedule, mark attendance from a notification, see your streak."

### NICE TO HAVE in V2 (high value but harder — worth the sprint if time permits)

| Rank | Feature | Impact | Difficulty |
|---|---|---|---|
| 1 | **F4 — Collaborative "did class run?" check** | 8 | Hard |
| 2 | **F13 — Voice / NL "add next class"** | 6 | Medium |

These are the "after the 8 must-haves" picks. F4 has the highest social-virality payoff if it works; build only if the no-network-fallback UX is clean. F13 is a delight feature that won't drive installs.

### SAVE FOR V3 (lower impact or very hard without clear payoff)

| Rank | Feature | Impact | Difficulty |
|---|---|---|---|
| 1 | **F5 — Per-subject batch rank (privacy-sensitive)** | 4 | Hard |
| 2 | **F10 — Parents' WhatsApp summary** | 4 | Medium |
| 3 | **F15 — ERP integration** | 5 | Hard |
| 4 | **F16 — Compare-with-batch heatmap** | 5 | Hard |
| 5 | **F17 — Drop-subject simulator** | 5 | Easy |
| 6 | **F2 — Lab vs Theory separation** | 6 | Easy |
| 7 | **F12 — Multi-batch timetable** | 5 | Easy |

Move F2, F12, F17 up to V2 *if* engineering effort is <2 days each after the must-haves. They're each small but valuable. The rest needs an architectural decision (privacy / ERP integration) before the build is justified.

---

## NON-OBVIOUS RECOMMENDATIONS

1. **The viral loop is the timetable code, not the attendance %.** Always-on marketing surface = "share your schedule." Once a whole batch installs, the attendance math locks them in.
2. **Notifications > dashboard.** Indian engineering students check WhatsApp 60+ times/day. Pushing *correctly* into that surface is worth more than a beautiful dashboard.
3. **"Safe to bunk today" widget is a brand-defining feature.** If only one thing ships in V2, make it this. It answers the one question every Indian engineering student asks themselves at 8:55 AM.
4. **Don't fight Bunk it on mass-bunk.** They have it. Trying to win on "negative" features — encouraging bunks — is bad for brand and risky for college enforcement. Differentiate on the *defensive* "safe to skip today" answer instead.
