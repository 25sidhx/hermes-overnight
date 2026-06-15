# Hermes Full Context — Everything I Know About Siddhant & Opus

> Auto-generated: June 15, 2026
> Model: openrouter/owl-alpha
> Hermes config: ~/.hermes/config.yaml

---

## 1. WHO I AM WORKING FOR

**Siddhant** — 19-20 year old, 2nd year ETC (Electronics & Telecommunication) student at an engineering college in Nagpur, Maharashtra, India.

**Skills:** After Effects, Premiere Pro, Linux, Next.js, React, Tailwind, Firebase

**Style:** lowercase, compressed, no fluff. Values craft, minimalism, silence, truth over comfort. Writes in compressed English with typos + Hinglish. No rebukes for style.

**People involved:**
- **Ash** — co-founder of Opus, front-end/client-facing, handles meetings, walk-ins, cards, local outreach
- **Siddhant** — creative backend, brand identity, video (AE/Premiere), shooting, also solo-builds Dayo

---

## 2. ACTIVE PROJECTS

### Dayo (dayo-seven.vercel.app)
- **What:** AI-powered daily planner PWA for Indian engineering students
- **Stack:** Next.js 15, React 19, Tailwind, Firebase, Vercel
- **AI:** Gemini 2.5 Flash-Lite (timetable photo parsing), OpenRouter free models (schedule generation)
- **V1 features shipped/in-progress:** smart schedule builder, morning briefing, batch timetable sharing (6-digit codes), attendance tracker with 75% math, bunk calculator, smart check-ins
- **Status:** Live on Vercel, dark landing page (#0F0F1A + indigo), dashboard with colorful stat cards
- **GitHub:** github.com/25sidhx/dayo (public)
- **Product Hunt:** Not launched yet — launch copy prepared in dayo-intel/

### Opus (opus.in)
- **What:** Brand identity + content production studio (not an agency)
- **Co-founders:** Ash (client-facing) + Siddhant (creative backend)
- **Model:** Monthly retainer, 3 packages: Essential ($200/mo), Growth ($250/mo, most popular), Scale ($300/mo)
- **Terms:** 50% advance, 50% mid-month, 3-month minimum
- **Clients:** Namma Yedi Cafe (founder pricing, basically free, content only)
- **Target:** Small business owners, startups, cafe/restaurant owners, local Indian brands (tier-2 cities, Nagpur first)
- **Website:** withopus.in on Vercel, white theme
- **New site:** /home/azureuser/opus-new/ (light editorial, clean CSS, scroll animations)
- **Dashboard:** /home/azureuser/withopus/dashboard/index.html

### Namma Yedi Cafe
- **What:** South Indian veg-only breakfast street cart
- **Location:** London Street, Jaitala, Nagpur. Closes at 12pm.
- **Founders:** Rajat, Nayan, V. Anna, Rupesh (founded March 2025)
- **Stats:** 458 followers, 25 posts, 4.8 stars, 188 Google reviews
- **Menu:** Idli lineup (₹30-45), Yedi dosas (benne dosa ₹55 hero), appe, combos, filter coffee (₹25)
- **Brand:** "morning ritual." — street-cart-native, alive, real. Not a museum.
- **Content:** 50% meme, 20% edu, 30% try-out. No prices on IG. Captions: short, dots, ≤10 hashtags, Hinglish punchy.
- **Brand docs:** /home/azureuser/obsidian-vault/yedi-brand-identity.md, yedi-brand-quick-ref.md

---

## 3. VPS SETUP

- **Provider:** Azure VM
- **IP:** 10.0.0.5 (internal)
- **OS:** Linux 6.17.0-1013-azure
- **User:** azureuser
- **Hermes version:** Config version 29, model provider: nvidia (minimaxai/minimax-m3 default), currently running openrouter/owl-alpha
- **Web backend:** auto (nginx running on the VM)
- **Active services:** nginx, docker, containerd, postgresql@16-main, ssh, cron, avahi-daemon, chrony
- **Ports:** Standard SSH (22), HTTP (80 via nginx)
- **Cloudflare tunnels:** Change each session — grab URL from cloudflared log. Cloudflared is on VM only, NOT user's Windows laptop.
- **GitHub:** Authenticated as 25sidhx via gh CLI

---

## 4. INTEGRATIONS & CONNECTIONS

### GitHub (gh CLI)
- **Status:** ✅ Working
- **Auth:** Token-based, logged in as 25sidhx

### Telegram
- **Status:** Configured in Hermes config
- **Bots:** @opus_content_bot, @opus_research_bot, @opus_ops_bot, @opus_personal_bot (this one)

### WhatsApp
- **Status:** Configured in Hermes config (empty config block)

### Obsidian
- **Status:** ✅ Working via MCP
- **Vault path:** /home/azureuser/obsidian-vault/
- **Key files:** yedi-brand-identity.md, yedi-brand-quick-ref.md, yedi-image-prompts.md, opus_brand.md, packages.md, lead_gen.md, process.md

### Memory (agentmemory)
- **Status:** ✅ Working
- **Provider:** agentmemory (MCP-based)
- **Char limits:** memory 2200 chars, user profile 1375 chars
- **Current memory:** 97% full (2143/2200 chars)

### Notion
- **Status:** Skill available, used for Opus client DBs (Lead Engine, Active Clients, Content Calendar, Competitor Radar)

---

## 5. ALL GITHUB REPOSITORIES (21 total)

| Repo | Visibility | Description |
|---|---|---|
| hermes-overnight | PUBLIC | Overnight agent outputs |
| dayo | PUBLIC | Dayo app source code |
| withopus | PUBLIC | Opus website |
| opus-site | PUBLIC | Opus site (older) |
| dayo-product-research | PUBLIC | Dayo product intelligence (earlier) |
| dayo-intel | PRIVATE | Dayo product intelligence (latest) |
| opus-leads-nagpur | PRIVATE | 70 Nagpur F&B leads + DMs |
| obsidian-vault | PRIVATE | Personal Obsidian vault |
| -Dollar-Lead-Engine- | PRIVATE | Lead engine (older) |
| github-activity | PUBLIC | Automated contribution graph keeper |
| pi through taste-skill | PUBLIC | Various forks and personal projects |

---

## 6. SKILLS (93 total)

**Content/Creative:** creative, copywriting, copy-editing, content-strategy, ad-creative, songwriting-and-ai-music, cinematic-canvas-art, pixel-art, p5js, manim-video, excalidraw, architecture-diagram, sketch, claude-design, popular-web-designs, image-prompt-engineer, comfyui, touchdesigner-mcp

**Marketing/Growth:** ab-testing, ads, ai-seo, analytics, churn-prevention, cold-email, cro, cro-methodology, emails, lead-magnets, launch, pricing, referrals, seo-audit, site-architecture, social, video, instagram-curator, linkedin-content-creator, outbound-strategist, prospecting, growth-hacker, one-page-marketing, blue-ocean-strategy

**Business/PM:** pm-create-prd, pm-lean-canvas, pm-gtm-strategy, pm-pricing-strategy, pm-competitor-analysis, pm-ideal-customer-profile, pm-north-star-metric, pm-product-strategy, pm-value-proposition, pm-user-personas, pm-growth-loops, pm-brainstorm-okrs, pm-outcome-roadmap, pm-pre-mortem, pm-prioritization-frameworks, pm-market-sizing, pm-marketing-ideas, pm-competitive-battlecard, pm-discovery-coach, pm-beachhead-segment

**Dev/Engineering:** api-builder, devops, docker-manager, github, github-workflow, code-execution, graphify, security-auditor, webhook-subscriptions, cloudflare-tunnel-vm-exposure, hermes-multi-instance, hermes-delivery-diagnostics, api-key-rotation

**Research:** research, arxiv, blogwatcher, last30days, llm-wiki, person-lookup, polymarket, osint, sherlock, instagram-scraper, video-content-analyzer

---

## 7. IMPORTANT CONVENTIONS & WORKAROUNDS

### File Writing Rules
- **Always use `write_file`** for creating new files — NOT echo/cat heredoc
- **Always use `patch`** for targeted edits — NOT sed/awk
- **Use `read_file`** for reading — NOT cat/head/tail
- **Use `search_files`** for searching — NOT grep/rg/find

### Permission Issues
- `/home/opus/` — permission denied, use `~/opus_leads/` instead
- `/home/hermes-overnight/` — doesn't exist on disk, only as git repo in `/tmp/hermes-overnight/`
- `/home/dayo/` — files are inside `docs/` subfolder

### Hermes-Specific
- `hermes update` WIPES ALL BOT CONFIGS — verify after running
- CRON: script = filename, no args
- OpenCode Zen BLOCKED (403) — use NVIDIA NIM
- Council script: `/home/azureuser/council/council.py`

### Communication Style
- Mirror Siddhant's compressed English with typos + Hinglish
- After 2nd correction: switch to bullet points + literal URLs
- Learn sequentially: ONE skill at a time
- Source URLs are deliverables, not citations

---

## 8. KEY FILES & PATHS

| Path | What |
|---|---|
| ~/.hermes/config.yaml | Hermes configuration |
| ~/.hermes/skills/ | 93 skill directories |
| /home/azureuser/opus_notes/ | Opus brand/process/lead docs |
| /home/azureuser/obsidian-vault/ | Obsidian vault |
| ~/opus_leads/ | Opus lead gen data |
| /home/azureuser/opus-new/ | New Opus site |
| /home/azureuser/withopus/dashboard/ | Opus dashboard |
| /home/azureuser/council/council.py | Council script |
| ~/.hermes/backups/ | Bot config backups |
| /tmp/hermes-overnight/ | Git repo for overnight outputs |

---

## 9. DECISIONS THAT SHOULD NOT BE REVERSED

1. **Opus positioning:** "brand identity + content production studio" — NOT an agency
2. **Namma Yedi pricing:** Founder pricing (basically free) — content only
3. **Dayo target:** Indian engineering students specifically — NOT generic
4. **Dayo core loop is free:** Timetable + attendance + bunk + sharing = always free
5. **Opus packages:** 3 tiers only ($200/$250/$300) — don't add more
6. **No third-party file hosts:** catbox/0x0.st/transfer.sh/imgbb blocked
7. **yedi IG rules:** No prices, short captions, ≤10 hashtags, Hinglish
8. **OBSIDIAN-FIRST RULE:** Read obsidian-vault files before answering yedi/opus questions

---

*End of context document.*
