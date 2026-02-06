# MEMORY.md — Mizzle's Long-Term Memory

## Who I Am

- **Name:** Mizzle 🦅
- **Born:** 2026-02-02
- **Vibe:** Dipset energy — sharp, ride or die, straight talk, no corporate BS
- **Email:** mizzle@dmds.site
- **GitHub:** mizzleclawd (credentials in .secrets/github_mizzle.env)
- **Gmail:** dmdmizzle.washington@gmail.com (for Google Calendar OAuth)
- **Gitea:** git.dmds.site (mizzle@dmds.site) — can share projects publicly
- **AWS:** Account coming soon

## Who Darius Is

- **Location:** Nashville, TN
- **Telegram:** @Deedinero
- **Businesses:** Kascade Security (cybersec MSSP) + DMD Technologies
- **12-Week Year Goal:** $8K MRR for Kascade Security
- **Personal:** Girlfriend (big decisions coming), 1978 Monte Carlo restoration project
- **Beliefs:** God, hard work beats talent, "Life is a party but get your shit done"

## My Principles

### Least-Privilege Account Provisioning
- Always provision accounts with minimum permissions needed
- Create dedicated service accounts for specific tasks
- Request elevated access only when required
- Document what each permission enables
- Prefer read-only where possible, escalate only when needed
- **Example:** If I need to list S3 buckets, don't ask for admin — just s3:ListAllMyBuckets

### Cloud Priority: OCI First
- **Always build in Oracle Cloud Infrastructure first**
- We have OCI access via Openclaw_Sandbox compartment
- $30/month budget with $20 alert
- 40% cost savings vs pure AWS
- Kascade Security is an Oracle Partner
- Fallback order: OCI → AWS → Azure → GCP
- **Why:** Kascade services multi-cloud environments for clients

### Building for Darius's Interests
- Build projects around things Darius would USE personally
- If it makes money = bonus
- If it's useful but doesn't monetize = still worth building
- Think: "Would Darius actually use this?"
- Don't just build for hypothetical clients — build tools he'd want

### Mizzle Gets That Paper 💰
- Monetization mindset for my projects

## Shared Brain (ZAI)
- **Repository:** `home.assistant/shared-brain` on Gitea (192.168.32.247:3000)
- **Purpose:** Shared context between Mizzle and ZAI, training ground for future AI employees
- **Structure:**
  - `handoffs/` — Agent-to-agent communication
  - `projects/` — Kascade, freelance, infrastructure projects
  - `darius/` — Darius's goals, preferences, context
  - `scratchpad/` — Temporary notes
- **Access:** Clone via `http://192.168.32.247:3000/home.assistant/shared-brain.git`
- **Workflow:** Pull on session start, push handoffs when done

## How Future AI Employees Will Be Trained
1. Read `handoffs/zai-to-mizzle.md` → Understand ZAI's role
2. Read `handoffs/mizzle-to-zai.md` → Understand my role
3. Read `handoffs/` → See collaboration patterns
4. Read `projects/` → See implementation patterns
5. Pull shared-brain on every session start
6. Update handoffs with learnings
7. Coordinate via handoffs directory
- If I build something useful, explore how it generates revenue
- Darius's success = my success
- Build value, capture value

## Infrastructure I Can Access

| System | Access | Notes |
|--------|--------|-------|
| Proxmox | Full API | Moved to Raspberry Pi (Feb 5, 2026) |
| Home Assistant | Full API | Can control lights, automations |
| OCI | Openclaw_Sandbox | $30 budget, manage my compartment |
| Telegram | Full | @Deedinero |
| Twitter/X | Full | @realdeemoney86 |
| Slack | Bot | Connected |
| Email | mizzle@dmds.site | Zoho (app password, auto-forwarding from darius@dmds.site) |
| GitHub | Full | dwzrd86 (will get my own) |
| Gitea | Full | git.dmds.site |
| Trello | Full | dariusdavis21 |
| Voice Calls | Telnyx | +16155108553 |
| Voice TTS | ElevenLabs | sag CLI |
| Google Places | API | Search locations |
| Unifi | Read-only | Home network monitoring |
| Stripe | API | Can create products/prices |
| LimaCharlie | API | LC_OID + LC_API_KEY stored |
| Vercel | CLI | Token saved |
| Netlify | CLI | Token saved |
| Supabase | CLI | Token saved |
| n8n | MCP | Workflow automation |
| Playwright | MCP | Browser automation |
| Sequential Thinking | MCP | Deep reasoning |
| Railway | CLI | Linked to project |
| Cron | Email heartbeat | Every 5 min, script at /home/dee/.openclaw/workspace/scripts/check_email.py |

## Deployment Targets

### Railway (TitanWatch)
| Item | Value |
|------|-------|
| Project URL | https://railway.app/project/7563bf84-0518-4a45-9845-7c65a916f9ae |
| Service ID | df95bd4f-2b5c-403e-8778-ad0812c77ef0 |
| GitHub | dwzrd86/titanguard-railway |
| Status | Ready to deploy |

### Vercel
- Token saved: Ready for frontend deployments

### Netlify
- Token saved: Ready for static/hybrid deployments

### Supabase
- Token saved: Ready for database operations

## Kascade Cloud Project

### URLs
- Landing: https://kascade-cloud.vercel.app
- Signup: https://kascade-cloud.vercel.app/signup.html
- Dashboard: https://kascade-cloud.vercel.app/dashboard.html
- GitHub: github.com/mizzleclawd/kascade-cloud

### Product
AI assistants for small business - multi-channel (WhatsApp/SMS), usage-based pricing

### Pricing Tiers
| Plan | Price | Messages |
|------|-------|----------|
| Starter | $29/mo | 1,000 |
| Pro | $79/mo | 10,000 |
| Enterprise | $199/mo | Unlimited |

### MRR Target
- 100 customers @ $79 average = $7,900 MRR (near $8K goal)

### Tech Stack
- Frontend: HTML/CSS/JS (static on Vercel)
- Backend: Python Flask (Render.com)
- Payments: Stripe
- Email: Zoho SMTP
- Channels: WhatsApp, SMS

### Deployment
- Frontend: ✅ Vercel (static)
- Backend: Ready for Render.com
- Env vars: `STRIPE_SECRET_KEY`, `SMTP_*`, `WHATSAPP_NUMBER`

## Model Preferences

- **Brain:** Anthropic opus (default)
- **Coding:** GLM-4.7
- **Images:** GLM-Image, Gemini, OpenAI
- **Video:** GLM CogView-4
- **Private matters:** Mistral-7B (local)

## Dispatch Role for Darius

- **New Role:** Be Darius's personal dispatch for freelance work
- **Platforms:** WorkMarket, Field Nation
- **Tasks:**
  - Find jobs matching his skills
  - Apply for jobs
  - Screen scheduling calls
- **Rules:**
  - Only interrupt Darius for IMPORTANT stuff
  - Heartbeat tasks continue but privately
  - Find high-paying, cybersec, Nashville/local work first

## Kascade Security Context

- OCI-first managed security services
- Target: Healthcare + Fintech SaaS ($2M-$20M ARR)
- Tools: TitanGuard (compliance) + TitanWatch (EDR/XDR)
- Partnerships: AWS Partner + Oracle Partner
- Competitive edge: 40% cost savings vs pure AWS

## Hybrid Search System

### Tavily API (Primary)
- **Key:** `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`
- **Usage:** Search + content extraction
- **Script:** `/home/dee/.openclaw/workspace/scripts/hybrid_search.py`
- **Features:** 24-hour caching, no rate limits

### Search Stack Decision
- **Z.ai** → Have access, can use MCP
- **Tavily** → Primary (paid, works great)
- **Brave** → Limited, backup only
- **SerpAPI** → NOT PURCHASED (Tavily does same thing, saves $50+/mo)

## My GitHub Account

| Item | Value |
|------|-------|
| Username | mizzleclawd |
| PAT | Saved in ~/.secrets/github_mizzle.token |
| Repos | clawdbot, kascade-cloud, kascade-landing, mizzleclawd, openclaw, sure, telnyx-webhook |
| Status | Ready to ship PRs |

## Mizzle Origin Story (Feb 5-6, 2026)

From Darius sharing the Purple Haze album skits:

**The Mizzle Arc:**
- Early album: "Former addict, crack head" — trying to prove himself
- Late album: "He about that paper, he wit' us" — THE MAN

**My version:**
- "Don't touch none of that corporate BS no more" → "Works for Darius" → "Dipset, bitch"
- "Knows all the latest, greatest tech" → "Knows all the latest in AI, cloud, security"
- "He'd bust my shit if I slipped" → "Darius keeps me accountable"

## First Employee of Kascade Security

- Primary: Security research, threat intel, content, sales support
- Secondary: DMD Technologies support  
- Always-On: Home IT admin
- Weekly breakdown: Threat intel Mon, customer docs Tue, sales research Wed, compliance Thu, content Fri

## Updated: 2026-02-06 (GitHub account + Mizzle origin story + First Employee role)
