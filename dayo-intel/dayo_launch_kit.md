# Dayo — Go-to-Market Strategy

Built by: solo dev (Siddhant, ECE 2nd year, Nagpur). Budget: zero. Audience: Indian engineering students.

---

## TARGET COLLEGES — Where to seed first

### Why tier-2 engineering colleges (the real beachhead)

Three reasons that overlap:

1. **They enforce 75% strictly.** Tier-1 (IIT/BITS/VIT) either removed the rule (IIT Roorkee, 2024) or have lenient defaults (BITS pilani flexibility, VIT usually let-offs). Tier-2 *enforces 75% and detains.* Detention fear = highest urgency = highest daily-active use.
2. **They use ugly ERPs.** Tier-1 has decent internal apps. Tier-2 uses outsourced DigiCampus / Academia / local custom. Dayo slots in as the *student's personal* layer over whatever the college runs.
3. **Higher peer-referral density.** Tier-2 batches are 60–120 strong and form stable WhatsApp groups. One student sharing the 6-digit code propagates to 80 friends in <24 hours.

### Autonomous vs affiliated

- **Autonomous colleges** (e.g. autonomous state colleges, deemed universities) — preferential. They have local control over rules → 75% is usually more rigid. Their timetables are messier printed PDFs. Perfect photo-timetable use case.
- **Affiliated colleges** (under state universities) — also good but rules vary per affiliated university. Slightly weaker signal.

### Maharashtra-specific or national first?

**Maharashtra first.** Three reasons on top:
1. Dev is in Nagpur. Personal first-degree network at VNIT/IIMs N/other Nagpur colleges. Reachable for in-person testing.
2. Maharashtra has a large density of tier-2 colleges (Pune, Nagpur, Mumbai, Amravati, Aurangabad) with high attendance strictness.
3. After Maharashtra, expand to: Karnataka (lots of tier-2 colleges, similar culture), then UP/MP/TN.

### Top 5 college types / regions to seed first

1. **VNIT Nagpur + colleges immediately around it (Nagpur cluster):**
   Dev's home base. Personal reputation = triggers installs. Demo class with a friend in ECE/ME/CSE. Aim: 70%+ of one branch using Dayo within 4 weeks.
2. **Other Maharashtra top-tier state colleges — Pune and Mumbai COEP/VJTI/SPIT/BITS-Pilani-Goa-tier secondaries:**
   Students here are digitally active, post on Instagram, decent budget autonomy. Pune alone = 50+ tier-2 colleges. Easy expansion once VNIT validates.
3. **Karnataka tier-2 colleges (Bangalore and Hubli-Dharwad):**
   Best in terms of both volume and digital savviness. RVCE, BMS, BMSIT, KLE — strong, well-networked classes. After Maharashtra stable.
4. **South Indian state-engineering colleges (AP/Telangana/TN):**
   JNTU, Anna University, SRM feeder colleges. Cultural habit of class WhatsApp groups = viral loop snaps in cleanly. Larger class sizes (60–90) = more installs per code.
5. **Rest of Hindi belt (UP MP, Rajasthan):**
   Highest attendance-fear density. Slowest UI literacy. Worse network. Only worth it AFTER Maharashtra is stable — these users need the widget + push notifications to compensate for the network. Save for Month 3+.

---

## VIRAL LOOP — How one student becomes a batch

### The exact sequence

1. **Install + setup.** Student installs Dayo, adds their timetable via photo (30 seconds). They share their 6-digit code with their two closest friends in class → "bhai try kar" in WhatsApp.
2. **First 5 users in a batch.** Once 5+ classmates have joined via the code, the *real* value unlocks: the morning briefing and the "safe to bunk today" widget. The widget + briefing is what becomes part of the daily ritual.
3. **The "is class held today?" check (V2 feature F4).** When a teacher is missing, one of them taps "class didn't run." If 15 students in the batch independently tap, the system cancels for the whole batch. *This is the moment* Dayo becomes infrastructure, not an app. Until V2 ship F4, the equivalent is the morning briefing habit.
4. **The "I might get detained" pull.** Once a student's attendance drops near 80%, the push notification ("Data Structures is at 78%") interrupts them just enough to attend the next class. Once that student tells a friend "bro this app saved me," it spreads.
5. **The next-semester carry-over + new batch onboarding.** Old students add their juniors to the WhatsApp class group. They re-install Dayo each year. Annual re-seed.

### Role of the 6-digit code (specifically)

- The code is *not* a friend invite — it's a *batch invite*. Sharing it with one friend in your batch means they can pull your schedule. Sharing it with the class WhatsApp group = whole batch onboarding in a single message.
- Code rotation per semester prevents stale data.
- Code expiry after 30 days prevents leakage / accidental mass-installs of year-old data.
- Code format: 6 digits, all numeric, designed to type in 4 seconds and remember for 20 minutes (liminal memory).

### What makes a student share unprompted

Three documented drivers (from Bunk it's QR feature success + Reddit data):

1. **Emotion avoidance.** "I don't want my friend to get detained." Students relay Dayo *to friends they care about* before they relay to strangers. Engineer the empty-state onboarding to mention "share with 2 study buddies to get X" once a basic usage threshold is hit.
2. **Social proof of cleverness.** "Look, I just photo'd my timetable and it's all set up." Showing the photo-to-timetable moment is a low-effort flex in a study group.
3. **Co-use.** "We both need to skip that 8 AM class and I want to know if it's safe." The bunk-safety answer is a *shared* answer — if one friend has Dayo and the other doesn't, the one with Dayo tells the other ("you're at 79%, skip the elective but attend DSA"). Direct value transfer every morning.

---

## DISTRIBUTION CHANNELS — Ranked by ROI for a solo dev with zero budget

### #1 — College WhatsApp groups (HIGHEST ROI)

- **What to post:** a single install link with a one-line student-voice recommendation + a screenshot of the morning briefing.
- **Format:** Plain message. No design. No image carousel. No emojis. Just the link and the sentence.
- **Frequency:** Once per group, on first day of week, between 7 PM and 9 PM IST (peak group activity).
- **Realistic outcome:** 5–15 installs per group, depending on how active it is. Optimized: post in the first 5 group chats the dev is in (his own batch's groups). 30–100 installs/week possible.
- **Lean:** This is ground-zero. Optimize for this. Don't waste time on graphics.

### #2 — r/Btechtards + r/Indian_Academia (HIGH ROI for niche.)

- **What to post:** "Built a free PWA that solves 75% attendance + takes your timetable photo. Looking for feedback from 2nd / 3rd year ENTC / ECE / ME / CSE batches. Here is what it does, here is the link."
- **Format:** Self-post, link in body, ask for feedback in title. **Don't marketing-speak.** Reddit will downvote self-promotion if it sounds promotional.
- **Frequency:** 1 post + comments follow-up. Repeat in 5–7 days if first one dies.
- **Realistic outcome:** ~30–100 installs per good post, but more importantly, *feedback* you can use to refine copy and fix bugs.
- **Lean:** Combine engagement hooks: "I'll DM the user with the most-detailed bug a free month of [future premium feature]."

### #3 — Instagram Reels (MEDIUM-HIGH ROI over 2–4 weeks)

- **What to post:** Screen-recording reels showing three specific transformations:
  1. The photo-to-timetable moment (1 photo → full schedule)
  2. The morning briefing + safe-bunk count
  3. The "you might not be eligible for exams" notification
- **Format:** 15–20 sec reels, hook in first 1.5 seconds ("75% attendance is killing me — fixed"). On-screen text only — no voiceover needed for English/Hinglish mix. Caption: Hinglish, relatable.
- **Frequency:** 3 reels/week.
- **Realistic outcome:** 1 reel goes semi-viral = 500–5000 installs. Outliers: 10 reels/week × 4 weeks compound roughly to 200–1500 installs.
- **Lean:** Don't overproduce. Screen-record + iMovie/After Effects thumbnail text = 15 minutes per reel.

### #4 — Telegram college groups (MEDIUM ROI, regional fit)

- **What to post:** Same as WhatsApp but tuned for Telegram's larger-group culture. "Drop your timetable photo in this chat and I'll generate your code."
- **Format:** Plain text + install link. Probably fewer emojis than WhatsApp.
- **Frequency:** Once per active group.
- **Realistic outcome:** Highly variable — depends on whether the college's primary channel is Telegram or WhatsApp. Useful in Tamil Nadu, Karnataka, AP, Maharashtra, Delhi-NCR. Less in rural UP/Bihar where WhatsApp dominates.
- **Lean:** Don't bother unless the college you're trying to seed uses Telegram as primary.

### #5 — LinkedIn (LOW–MEDIUM ROI, *but* useful for the dev-angle narrative)

- **What to post:** A first-person dev story: "I'm 19. I built an app to stop engineering students from getting detained. Here's what I learned shipping it in 60 days." End with the install link.
- **Format:** Long-form personal essay. Open with a vulnerability moment. Tag at least one friend/peer at the bottom.
- **Frequency:** 1 post at launch; 1 update at month 3 with metrics.
- **Realistic outcome:** 50–300 installs *from* LinkedIn, but a higher-value audience (potential product supporters, future employees if raised, beta testers who'll give feedback). Drives *credibility*, not installs.
- **Lean:** Important for the creator angle, not for virality. LinkedIn screenshots of the LinkedIn post can be reused on Instagram.

### #6 — YouTube Shorts (LOW ROI short-term, high optionality long-term)

- **What to post:** 30-sec dev-story shorts. Same as reels but posted on YouTube for evergreen discovery.
- **Format:** Same as Instagram reel, but with a slightly higher hook in first 2 seconds (algorithm is harsher).
- **Frequency:** 2–3/week either same content as Instagram or shorter.
- **Realistic outcome:** Lower daily installs than Instagram Shorts driven by YT; *but* YT search = long-tail discovery. Average 50–200 direct installs/month if you stay consistent.

---

## 30-DAY LAUNCH CALENDAR

### Week 1 — Pre-launch (build + internal polish)

Day 1–3: Bug-bash based on the saved Opus-Notes feature list. Photo-to-timetable must work on edge cases. Notification permission ask must be timed correctly.
Day 4:    Pick the 5–8 friends in your batch who'll be your *seed users*. Reach out: "Can I add you as a beta tester? I need honest feedback."
Day 5:    Onboard them. Have them each set up their timetable and try sharing codes.
Day 6:    Get feedback. Kill "almost-works" flows. Patch the things they flagged.
Day 7:    Polish UX copy from dayo_ux_copy.md. Add analytics. Set up Firebase error logging hooks.

**Deliverable end of Week 1:** A version 1.5 stable enough that you'd trust your awkward cousin to use without calling you.

### Week 2 — Soft launch (seed in 1–2 branches)

Day 8:    Pick ONE branch (probably your own: ECE 2nd year at VNIT). Identify the WhatsApp group.

Day 9:    Draft the WhatsApp-Class-Group post (template in launch copy below). Tone check.

Day 10:   Post. Frame it as "we built this, give it 60 seconds, tell me what breaks."

Day 11:   Monitor installs + crash reports. Reply to every DM in <2 hours (early users expect fast feedback).

Day 12:   A/B test the morning briefing copy. Which phrasing drives more opens of the notification?

Day 13:   Aim for 25%+ of one branch with Dayo installed by end of week.

Day 14:   Quick fix-up sprint. Kill any flow that confused users.

### Week 3 — Expand (feedback loop + bug fixes)

Day 15:   Post in r/Btechtards. Frame as "built this for Indian engineering students, want feedback." Don't pitch. Use Reddit SEO: title must include "attendance" or "75%" — whatever's searched.

Day 16:   Post a "behind the build" LinkedIn article. Tag a few college friends — virality on LinkedIn depends on tags.

Day 17–19: Pull bug list from Reddit comments + Play Store reviews if you shipped to Play Store by then.

Day 20:   Add the most-requested feature from the feedback (likely: WhatsApp share button, F3 from V2 spec).

Day 21:   Aim for 100+ installs across 2–3 colleges by end of week.

### Week 4 — Push (all channels live)

Day 22:   Publish 3 Instagram reels from the launch copy below.

Day 23:   Cross-post to Facebook college groups (different demographic — students with parents who are on Facebook).

Day 24:   Submit to Product Hunt (use the launch copy below). Have 5–10 friends ready to upvote in the first 2 hours (PH ranks based on velocity).

Day 25:   Respond to every Product Hunt comment personally. Don't automate.

Day 26:   Re-post on Reddit with a "v0.4 update" angle — "Here's what I learned from 100 students in week 1."

Day 27:   Publish one more LinkedIn post — this time linking the Product Hunt launch.

Day 28:   Run a small "refer 3 friends to get a future premium feature free" — opt-in only, no icky incentives on V1.

Day 29:   Compile metrics: installs, daily active users, attendance entries recorded, codes shared.

Day 30:   Plan month 2 focus. If the V2 must-haves from the spec doc are partly built, fold them in.

---

## PHASE 7 — LAUNCH COPY

---

## PRODUCT HUNT

### Tagline (under 60 chars)
> Don't get detained. Your attendance, sorted.

### Description (196 words)

Dayo is the daily planner made for Indian engineering students who are tired of getting caught at 74% on the detention list.

Here's the problem: most Indian engineering colleges enforce a strict 75% attendance rule. You re-type the same timetable every semester, check your attendance by mental math you don't trust, and pray every month that the teacher wasn't absent on the days you skipped. You carry your entire attendance life in your head — until it slips.

Dayo fixes the trickiest parts in seconds:

— Snap a photo of your printed or PDF timetable. We convert it to a real schedule automatically — no typing.
— Track attendance per subject. Know exactly how many classes you can still bunk, right down to the decimal.
— Get a single morning briefing at 7 AM with today's classes, current attendance %, and a warning if anything's below 80%.
— Share your timetable with your batch using a 6-digit code. Whole class joins in 10 seconds.
— Free, ad-free, no premium tier blocking the math you need.
— Works offline. Installs as a PWA, no Play Store friction.

Built by a 2nd-year ECE student in Nagpur who got detained once and decided not to let it happen again.

### 5 Features

- AI timetable parser — one photo, full schedule
- 75% rule + safe-bunk math, built in
- 6-digit code to share with your batch
- Morning briefing with today's classes and attendance status
- Free forever. No ads. No premium tier blocking core math.

### Hunter comment (100 words)

I'm a 2nd-year ECE student in Nagpur. Last semester, I almost got detained because I lost track of one elective's attendance — even though I'd been present most of the time. The college ERP was unclear, the calculator apps all assumed I'd typed out my schedule by hand, and the only thing checking my math was my own memory.

I built Dayo over a weekend as a personal fix. My batch used it. I realized other batches needed the same thing. Now I've spent months turning a personal fix into a real product. No VC money, no team, no premium tier. Just a tool I wish I'd had two semesters ago.

### What makes Dayo different

1. **Real photo-to-timetable.** Other apps make you copy an AI prompt into a different chatbot and paste back JSON. Dayo does it natively in the app.
2. **75% rule is first-class math** — not a formula the student has to wire up themselves.
3. **The 6-digit code.** No QR camera alignment, no file exports. Type 6 digits, you're in.
4. **One-screen daily summary.** No digging through tabs to know "what's happening today."

---

## TWITTER/X LAUNCH THREAD

### [Tweet 1]
> 2 months ago I almost got detained.

> Not because I was skipping class.

> Because I had to compute my attendance % in my head, every day, across 7 subjects — and I'd lost track of one elective.

> I built a fix. It's free. It's called Dayo.

> dayo-seven.vercel.app

*(275 chars)*

### [Tweet 2]
> The thing that killed me wasn't the 75% rule.

> It was typing my timetable into an app. Time slots. Days. The whole 6×5 grid.

> Every. Single. Semester.

> Dayo fixes that: snap a photo of your printed timetable, it's a real schedule in 10 seconds.

*(255 chars)*

### [Tweet 3]
> What Dayo does:
• snap a photo of your timetable → real schedule
• track attendance per subject
• know exactly how many classes you can bunk
• 6-digit code so your whole batch joins in 10 sec
• 7 AM briefing with today + attendance status

> No premium. No ads. No gating.

*(245 chars)*

### [Tweet 4]
> Built for the average engineering student, not the exceptional one.

> Not the "I use Notion + Google Calendar + Todoist" student.

> The one running between classes and forgot the password to the college ERP they were supposed to log into yesterday.

*(240 chars)*

### [Tweet 5]
> The 6-digit code is what I'm proudest of.

> One student in a batch sets up Dayo. They text the code in their class WhatsApp group. 60+ classmates paste it. Suddenly the whole batch is on Dayo.

> No login. No QR alignment. No file transfer.

*(248 chars)*

### [Tweet 6]
> Tech stack because I know someone's gonna ask:
• Next.js 15 (PWA, runs offline)
• Firebase (auth + DB, no Play Store required to install)
• Gemini 2.5 Flash-Lite (timetable photo parsing)
• OpenRouter free models (schedule + daily summary text)

> all free-tier. all solo.

*(245 chars)*

### [Tweet 7]
> Honest admission:
- No investor. No team. No ad budget.
- I am 19. In ECE 2nd year.
- I built this between classes.
- If you find a bug, DM me on Twitter — I will reply.
- If you love it, share your 6-digit code with two friends in your class.

*(227 chars)*

### [Tweet 8]
> Dayo is live.

> dayo-seven.vercel.app

> snap · share · don't get detained

> If you're an engineering student setting up your semester timetable this week, give it 60 seconds.

> If you know one, send this thread.

*(202 chars)*

---

## INSTAGRAM CAPTION (under 150 words, for a screen-recording reel)

> i got detained last semester — not because i was skipping class, but because i couldn't track attendance across 7 subjects in my head 💀
>
> so i built dayo.
>
> it does the math for the 75% rule. snap a photo of your timetable, it's done. share the code with your batch — they'll be on the same schedule in 10 seconds.
>
> morning 7am pe briefing aata hai — "aaj ka schedule + safe bunk count." no more mental math. no more detention fear.
>
> free forever. no premium tier blocking the math.
>
> made by a 2nd year ECE student in nagpur. between classes. for you.
>
> 🔗 dayo-seven.vercel.app
>
> #engineeringstudent #india #attendance #exams #collegelife #students #engineeringindia #timetable #bunkmanager

*(146 words)*

---

## THREE ONE-LINER PITCHES (different angles)

### 1. The AI angle
> A planner that converts your timetable photo into a real schedule in 10 seconds, then tells you what to skip and when.

### 2. The attendance / bunk angle
> Your 75% rule, your bunk math, your morning "is class safe to skip" answer — all on one screen, every day.

### 3. The student-built-for-students angle
> Built between classes by a 2nd-year ECE student in Nagpur who got detained once and never wanted it to happen again.

---

## COLLEGE WHATSAPP GROUP MESSAGE (under 80 words)

> bhai ek app banaya hai (free hai, no sign up, no premium wala scam). timetable ka photo click karo — 10 sec mein schedule ready. attendance % aur safe bunk count khud cal kar deta hai. 75% rule ka tension khatam.
>
> aur sabse best — 6 digit code share karo group mein, sab ke schedule ek baar mein sync ho jaate hain.
>
> try karo: dayo-seven.vercel.app
>
> (1 min setup hai. genuinely useful hai. koi premium nahi lagega baad mein, promise.)

*(70 words)*
