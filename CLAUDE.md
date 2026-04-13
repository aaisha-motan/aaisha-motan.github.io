# CLAUDE.md - Portfolio Project Memory

## Project Overview

Personal portfolio website for **Aaisha Motan** (AI Developer).

- **Live**: https://aaisha-motan.github.io
- **Repo**: aaisha-motan/aaisha-motan.github.io
- **Deploy**: Push to main → GitHub Pages auto-deploys (~60s)

---

## CRITICAL RULES

- This is a **PERSONAL** project — NOT BlissDrive
- NEVER log portfolio changes in Aaisha Dashboard activity or Knowledgebase pipeline
- NEVER commit .env files or API keys
- NEVER add a contact form (was removed intentionally)

---

## Tech Stack

- Pure static HTML/CSS/JS — single file (index.html ~120KB)
- No build step, no package.json, no dependencies
- Google Fonts (Inter, JetBrains Mono)
- All CSS inline in style tag, all JS inline in script tag
- Dark theme with purple accent (#a78bfa)

---

## Structure

- `index.html` — entire site
- `Aaisha.jpg` — profile photo
- `Aaisha_Motan_Resume.pdf` — resume download
- `favicon.svg` — site icon

---

## Page Sections

1. **Nav** — links + Resume/Let's Talk buttons (wrapped in flex container)
2. **Hero** — title, CTAs, 4-stat bar
3. **About** — photo + bio
4. **Services** — 6 cards (AI Bots, Automation, RAG, Reporting, API, Process)
5. **Projects** — TABBED (4 tabs: Knowledgebase, AI Visibility Tracker, Work Intelligence, ROI Calculator)
6. **Tech Stack** — Auto-scrolling MARQUEE (26 tech items, duplicated for seamless loop, hover to pause)
7. **AI-First** — why AI matters
8. **Why Me** — 6 value props
9. **2026 Focus** — skills grid + TABBED tools (7 categories: LLMs, Agents, Automation, RAG, Multimodal, Brand, Observability)
10. **CTA** — contact links (email, phone, LinkedIn, GitHub)
11. **Footer**

---

## Interactive Features

- Project tabs: `switchProject(idx)` — shows one project at a time
- Tools tabs: `switchTools(key)` — shows tools by category
- Tech marquee: CSS `@keyframes` infinite scroll, pauses on hover
- Scroll progress bar at top
- Smooth scroll navigation
- No scroll-triggered opacity animations (removed — caused invisible content)

---

## Known Issues Fixed

- Scroll animations caused invisible content (opacity:0 never triggered) — removed all
- Footer had large empty space below — reduced CTA/footer padding
- Nav buttons Resume/Let's Talk had gap — wrapped in flex container

---

## Current Project Stats (update when projects change)

- **Knowledgebase**: 1,900+ meetings, 23 team members, 10 cron jobs, 4 Fathom accounts
- **AI Tracker**: 4 engines, 43 clients, 200+ prompts, 6 prompt categories
- **Work Intelligence**: 6 pages, 4 repo sources, daily auto-sync
- **ROI Calculator**: 3-tab UI, 2 govt API integrations, 5-year projections

---

*Last Updated: April 9, 2026*
