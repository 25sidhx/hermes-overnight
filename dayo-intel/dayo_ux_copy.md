# Dayo — In-App UX Copy (V1)

Tone: a smart college senior in your batch — calm, honest, mildly funny, never corporate. Not a startup, not a "coach," not a "growth-hacker."

Style rules used throughout:
- lowercase for body where natural
- no exclamations used as filler
- contractions allowed
- Indian English — words like "bunk," "class," "lab," "midsem," "endsem" are used freely
- when something is solved, say what it does; when something is missing, admit it
- avoid: "Welcome aboard," "We're excited," "Let's go," "You got this," "✨"

---

## ONBOARDING

### Splash screen
- **Tagline:** *don't get detained.*

### Welcome screen
- **Headline:** *Hey. Dayo here.*
- **Subtext:** *I'll keep track of your classes, your attendance, and how many you can still bunk. Takes about 60 seconds to set up — no email needed.*

### Step 1 — Name
- **Label:** *what should I call you?*
- **Placeholder:** *name or nickname*
- **Helper text:** *Just so the morning briefing doesn't say "good morning student." Anything works.*

### Step 2 — College / branch
- **Label:** *college and branch*
- **Placeholder:** *e.g. VNIT Nagpur, ECE*
- **Helper text:** *Doesn't have to be exact — it shows up on your schedule so your cramming friends can recognize it.*

### Step 3 — Semester
- **Label:** *which semester are you in?*
- **Helper text:** *This affects how your timetable is structured. You can change it later when midsem is over and you've totally forgotten everything from this one.*

### Step 4 — Timetable setup
- **Headline:** *let's get your timetable in*
- **Photo upload option:**
  - **CTA:** *snap a photo of my timetable*
  - **Helper text:** *Take a clear, well-lit pic of your printed timetable. I'll convert it in a few seconds — no typing.*
- **Manual entry option:**
  - **CTA:** *enter it myself*
  - **Helper text:** *Tap to add subjects and their time slots. Good if your timetable is messy or you haven't got it yet.*

### Notification permission ask (after first subject added)
- **Title:** *can I ping you in the morning?*
- **Body:** *7 AM every day with today's classes, your safe-bunk count for each subject, and a warning if anything's getting close to 75%.*
- **Allow button:** *yeah, do it*
- **Not now button:** *not now*

---

## SCHEDULE BUILDER

- **Page title:** *your timetable*

### Subject input
- **Label:** *subject name*
- **Placeholder:** *e.g. Data Structures, ECE-201*

### Time slot input
- **Label:** *time slot*
- **Placeholder:** *e.g. 10:00 – 11:00*

### Day selector
- **Label:** *which days?*
- **Helper text:** *Tap all the days this class runs. Most labs are 1–2 days.*

### Empty state (no subjects added yet)
- **Headline:** *no classes yet*
- **Subtext:** *Add at least one to unlock attendance tracking and the morning briefing.*
- **CTA:** *+ add first class*

### Success state (after adding first subject)
- **Toast / inline message:** *Got it — [subject name] locked in. Add the rest when you have a minute.*

---

## MORNING BRIEFING

- **Card headline (before 9 AM):** *good morning. here's your day*
- **Card headline (after 9 AM):** *today, in case you're already overwhelmed*

- **Today's schedule label:** *today's classes*
- **Attendance summary label:** *your attendance right now*

- **Safe-bunk message (when attendance > 80%):**
  *„You can safely skip [X] more [subject name] classes before [75%/your target] becomes a problem."*

- **Danger-zone message (any subject 75–80%):**
  *„Heads up — [subject name] is at [X]%. One more miss and you're on thin ice."*

- **CTA:** *open full schedule*

---

## ATTENDANCE TRACKER

- **Page title:** *attendance*

### Subject attendance card
- **Present count label:** *present*
- **Absent count label:** *missed*
- **Percentage label:** *current %*

### Status badge text
- **Safe (above 80%):** *safe*
- **Warning (75–80%):** *careful*
- **Danger (below 75%):** *danger*

### "Mark today" CTA
- **CTA label:** *mark today*

### Bunk calculator section
- **Input label:** *how many more classes can I skip?*
- **Result label (safe):** *You can miss [X] more classes and still stay at [target %].*
- **Result label (cannot bunk):** *You can't bunk this anymore without falling below [target %]. Time to actually show up.*
- **Result label (recovery needed):** *You need to attend [X] more classes in a row to get back to [target %]. One at a time.*

### Empty state (no attendance data yet)
- **Headline:** *nothing to track yet*
- **Subtext:** *Once you mark a few classes, your attendance % shows up here.*

---

## TIMETABLE SHARING

### "Share my timetable" CTA
- **CTA label:** *share my timetable*

### 6-digit code display screen
- **Headline:** *your batch code*
- **Subtext:** *Anyone in your batch can paste this in Dayo to get your full schedule. The code is tied to your batch — they're not getting your personal attendance.*
- **Copy code button:** *copy code*

### Enter code screen
- **Headline:** *got a code from a friend?*
- **Input placeholder:** *6-digit code*
- **Join button:** *join*

### Success state (after joining)
- **Headline:** *you're in*
- **Subtext:** *Their timetable has been added to your account. Verify the time slots look right before saving.*

### Error state (invalid code)
- **Headline:** *that code didn't work*
- **Subtext:** *Double-check with the friend who sent it. Codes are 6 digits and case doesn't matter.*

---

## ERROR & EDGE STATES

### Timetable photo parse failed
- **Message:** *Couldn't read this one — the photo might be blurry or cropped. Try another angle or just type it in.*
- **Retry CTA:** *try again*

### No internet connection
- **Message:** *You're offline, but everything's still here. Anything you change will sync when you're back online.*

### Sync error (generic, no "Firebase" mention)
- **Message:** *Couldn't save that just now. We kept a copy — pull-to-refresh to try again.*

### Empty schedule for today
- **Message:** *No class today. Enjoy it. Tomorrow's schedule appears at 7 AM.*

---

## PUSH NOTIFICATIONS

### Morning briefing (sent at 7 AM)
- **Title:** *good morning, [name]*
- **Body:** *[N] classes today. [X] subject[s] on the edge — open Dayo to see.*

### Class starting in 15 minutes
- **Title:** *[subject name] in 15*
- **Body:** *Room time. Or don't — you're at [X]%.*

### Low attendance warning (subject drops below 80%)
- **Title:** *[subject name] is at [X]%*
- **Body:** *You've got [N] more miss[es] before [75%/target]. Don't let good attendance die.*

### Below 75% alert (urgent)
- **Title:** *[subject name] is below 75%*
- **Body:** *You might not be eligible for exams. Attend [N] classes in a row to recover.*

---

## BEST-LINE FAN-OUTS (use in marketing, in-app empty states, anywhere that fits)

- *"Don't get detained."*
- *"I keep your attendance. You keep doing you."*
- *"75% rule? Solved."*
- *"Your timetable, on your lock screen."*
- *"Snap. Done. Back to doomscrolling."*
