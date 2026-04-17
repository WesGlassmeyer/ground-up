# GroundUp Web — Project Context
Last updated: April 17, 2026

## What This Is
A web services business targeting BJJ schools and martial arts gyms in tourist cities that have weak or nonexistent digital presence. We build clean English-language websites and fix Google Business listings so traveling practitioners can find these gyms.

## The Business Model
- **Website build:** $400–600 flat fee (50% deposit upfront, 50% on delivery)
- **Google Business Profile cleanup:** $150–250
- **Monthly maintenance:** $75–150/month (update photos, posts, monitor reviews)
- **Hosting management (optional upsell):** $40–50/month per client

## Brand
- **Business name:** GroundUp Web
- **Domain:** groundupweb.com
- **Portfolio site:** Live at groundupweb.com
- **Email:** hello@groundupweb.com and wes@groundupweb.com (both forward to personal inbox via ImprovMX)

## Tech Setup
- **GitHub repo:** ground-up
- **Repo structure:** portfolio/index.html is the main site, portfolio/examples/ contains all demo sites
- **Netlify:** Connected to GitHub repo, auto-deploys on push, publish directory is portfolio/
- **Domain:** groundupweb.com pointed to Netlify nameservers
- **Email forwarding:** ImprovMX (hello@ and wes@ both forward to personal inbox)
- **Namecheap:** Domain registrar

## Demo Sites (live at groundupweb.com/examples/)
| File | Location | Region | Status |
|---|---|---|---|
| bjj-saranda.html | Sarandë, Albania | Mediterranean / Adriatic | Demo (prospect, not a client) |
| bjj-canggu.html | Canggu, Bali | Southeast Asia | Demo (fictional) |
| bjj-medellin.html | Medellín, Colombia | Latin America | Demo (fictional) |
| bjj-lisbon.html | Lisbon, Portugal | Europe | Demo (fictional) |

## Regional Demo Links (for pitch agent)
- Mediterranean / Adriatic: https://groundupweb.com/examples/bjj-saranda.html
- Southeast Asia: https://groundupweb.com/examples/bjj-canggu.html
- Latin America: https://groundupweb.com/examples/bjj-medellin.html
- Europe: https://groundupweb.com/examples/bjj-lisbon.html

## The Niche
BJJ schools and martial arts gyms in tourist-heavy cities — specifically targeting:
- Coastal towns in the Adriatic, Mediterranean, Southeast Asia, Latin America
- English-language sites targeting traveling practitioners who Google "BJJ [city]" before trips
- Sites built primarily in English, with key info (address, schedule, phone) in native language too

## Pitching Process
1. Agent researches a city and finds specific businesses with weak/missing digital presence
2. Agent writes a specific cold pitch email referencing exactly what's broken about their presence
3. You send it — email, Instagram DM, Facebook message, or WhatsApp depending on what's available
4. Follow up once after one week if no reply
5. Take 50% deposit before building anything

## Pitch Structure
- Lead with the specific problem ("When a traveler searches 'BJJ [city]' your gym doesn't come up")
- One sentence on why it matters to them (travelers decide before they land)
- One sentence: GroundUp Web + link to relevant regional demo
- Low-friction close: offer to show what we'd build, no price, no pressure
- Sign off: "Wes" only
- 4–5 sentences for email, shorter for DM
- No price mentioned — get the reply first

## Agent Pipeline
A Claude-powered React app (groundup-agent.jsx) handles the full prospect pipeline:

**Step 1 — City Queue:** Generates 40 target cities fitting the niche, saves to internal storage. Run once, adds more when the queue runs low.

**Step 2 — Research:** Pulls next unworked city, web-searches for BJJ/martial arts gyms, scores digital presence, logs qualifying prospects with contact info.

**Step 3 — Pitch Writer:** Writes personalized 4–5 sentence cold pitches per prospect, links correct regional demo automatically.

**Step 4 — Follow-up Tracker:** Checks for prospects contacted 7+ days ago, writes follow-up messages, sends via Telegram if configured.

**Export:** After each session, copy the prospect list from the app and paste into this file to keep Claude in sync.

## Prospect Status Tracking
Statuses: not_contacted → contacted → replied → won / lost

## Prospects
*(Paste updated prospect list from agent app here after each session)*

## Current Clients
None yet. Zero clients as of April 2026.

## What's Done
- [x] Business name and brand decided (GroundUp Web)
- [x] Domain purchased (groundupweb.com)
- [x] Email forwarding set up (hello@ and wes@)
- [x] Portfolio site built and live (portfolio/index.html)
- [x] 4 regional demo sites built and live (portfolio/examples/)
- [x] GitHub repo created and linked to Netlify
- [x] Auto-deploy pipeline working
- [x] Netlify form live — audit requests go to inbox
- [x] Agent pipeline built (groundup-agent.jsx)

## What's In Progress
- [ ] Set up new Telegram bot and channel for GroundUp follow-up alerts
- [ ] Add Telegram credentials to agent app settings
- [ ] Run first city queue generation and prospect research

## What Needs To Get Done
- [ ] Set up Stripe account to accept payments
- [ ] Write a simple one-page client service agreement
- [ ] Register LLC (after first paying client)
- [ ] Build pitch conversation script for when someone says yes
- [ ] Find affiliate links: DSCR lenders, Vivian Health, AMN Healthcare (for calculator sites crossover)

## How Claude Helps
- Runs the agent pipeline (city research, prospect finding, pitch writing, follow-up tracking)
- Builds the websites (HTML/CSS)
- Writes all copy
- Handles Google listing optimization copy
- Writes follow-up emails and client communication
- You find/approve, hit send, handle the money

## To Start A New Chat
Paste this file or say: "I'm working on GroundUp Web, a service building websites for BJJ gyms in tourist cities. Here's my context: [paste]"
