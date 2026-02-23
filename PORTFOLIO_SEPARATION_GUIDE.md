# Aaisha Motan - Portfolio Complete Guide

## What Is This Portfolio?

This is your **personal portfolio website** - a single-page HTML site showcasing your work as an AI Solutions Architect & Automation Builder. It's designed to impress potential clients and employers by showing real projects with measurable results.

**Live URL (after deployment):** https://aaisha-motan.github.io/

---

## Files In This Portfolio

```
portfolio/
├── index.html              # Main portfolio page (ALL content is here)
├── Aaisha.jpg              # Your profile photo
├── favicon.svg             # Browser tab icon (your initials)
├── CLAUDE_PORTFOLIO_GUIDE.md   # Instructions for Claude to update portfolio
├── SESSION_LOG.md          # Development history
└── PORTFOLIO_SEPARATION_GUIDE.md  # This file
```

---

## Portfolio Sections

The `index.html` contains these sections:

| Section | Purpose |
|---------|---------|
| **Hero** | Your name, tagline, key stats, CTA buttons |
| **About Me** | Background, photo, skill tags |
| **What I Do** | 6 service cards (AI Automation, RAG Systems, etc.) |
| **Projects** | Featured projects with stats, tech stack, features |
| **Tech Stack** | Technologies you work with |
| **Why I'm Fast** | Your AI-augmented development approach |
| **Why Work With Aaisha** | Your philosophy and differentiators |
| **Contact** | Email, phone, LinkedIn, GitHub |

---

## How To Add A New Project

### Step 1: Tell Claude What To Add

Say something like:
> "Add my Knowledgebase RAG system to my portfolio"

Or provide details:
> "Add this project to my portfolio:
> - Name: Meeting Intelligence System
> - What it does: Transforms meeting recordings into searchable knowledge
> - Stats: 1,754 meetings, 4 years of data, 12 automated reports
> - Tech: Python, Gemini AI, Pinecone, Discord, Slack
> - Features: RAG queries, weekly reports, real-time sync"

### Step 2: Claude Will Edit index.html

Claude will add HTML like this in the Projects section:

```html
<!-- Project: Meeting Intelligence System -->
<div class="project-featured" style="margin-top: 48px;">
    <div class="project-featured-header">
        <span class="project-badge">
            <svg>...</svg>
            Production System
        </span>
        <h3>Meeting Intelligence System</h3>
        <p class="project-featured-description">
            A production RAG system that transforms 4+ years of meeting recordings
            into searchable institutional knowledge for a US-based agency.
        </p>
    </div>

    <div class="project-featured-body">
        <div class="project-stats">
            <div class="project-stat-grid">
                <div class="project-stat">
                    <div class="project-stat-value">1,754</div>
                    <div class="project-stat-label">Meetings Indexed</div>
                </div>
                <!-- More stats... -->
            </div>
        </div>

        <div class="project-details">
            <h4>Tech Stack</h4>
            <div class="project-tech-stack">
                <span class="tech-tag">Python</span>
                <span class="tech-tag">Gemini AI</span>
                <span class="tech-tag">Pinecone</span>
                <!-- More tech... -->
            </div>

            <h4>Key Features</h4>
            <ul class="project-features">
                <li>RAG-powered natural language queries</li>
                <li>Automated weekly performance reports</li>
                <!-- More features... -->
            </ul>
        </div>
    </div>
</div>
```

### Step 3: Deploy The Update

After updating `index.html`, push to GitHub Pages:

```bash
cd /home/ubuntu/project/aaisha-motan.github.io
git add .
git commit -m "Add new project: Meeting Intelligence System"
git push
```

---

## How To Update Existing Content

### Update Your Stats (Hero Section)
Tell Claude: "Update my portfolio stats to show 10+ projects and 5 clients"

### Update Your Photo
Replace `Aaisha.jpg` with a new photo (same filename)

### Update Contact Info
Tell Claude: "Update my phone number to +92 XXX XXX XXXX"

### Add New Technologies
Tell Claude: "Add Claude AI to my tech stack section"

---

## How To View The Portfolio Locally

### Option 1: Open in Browser
```bash
# On Mac/Linux
open /home/ubuntu/project/Knowledgebase/portfolio/index.html

# Or double-click the file in a file manager
```

### Option 2: Python HTTP Server
```bash
cd /home/ubuntu/project/Knowledgebase/portfolio
python3 -m http.server 8000
# Open http://localhost:8000 in browser
```

---

## How To Deploy To GitHub Pages

### First Time Setup

1. **Create GitHub Repository**
   - Go to https://github.com/new
   - Name it: `aaisha-motan.github.io` (your username + .github.io)
   - Make it Public
   - Don't add README (you'll push existing files)

2. **Clone and Setup**
   ```bash
   cd /home/ubuntu/project
   git clone https://github.com/aaisha-motan/aaisha-motan.github.io.git
   ```

3. **Copy Portfolio Files**
   ```bash
   cp /home/ubuntu/project/Knowledgebase/portfolio/index.html /home/ubuntu/project/aaisha-motan.github.io/
   cp /home/ubuntu/project/Knowledgebase/portfolio/Aaisha.jpg /home/ubuntu/project/aaisha-motan.github.io/
   cp /home/ubuntu/project/Knowledgebase/portfolio/favicon.svg /home/ubuntu/project/aaisha-motan.github.io/
   ```

4. **Push To GitHub**
   ```bash
   cd /home/ubuntu/project/aaisha-motan.github.io
   git add .
   git commit -m "Initial portfolio deployment"
   git push -u origin main
   ```

5. **Enable GitHub Pages**
   - Go to repo Settings → Pages
   - Source: Deploy from branch → main → / (root)
   - Save

6. **Your Portfolio Is Live!**
   - URL: https://aaisha-motan.github.io/

### Updating After Changes

```bash
cd /home/ubuntu/project/aaisha-motan.github.io
git add .
git commit -m "Update portfolio"
git push
```

---

## Quick One-Liner Commands

### Deploy Portfolio To GitHub Pages
```bash
cd /home/ubuntu/project/aaisha-motan.github.io && \
cp ../Knowledgebase/portfolio/index.html . && \
cp ../Knowledgebase/portfolio/Aaisha.jpg . && \
cp ../Knowledgebase/portfolio/favicon.svg . && \
git add . && git commit -m "Update portfolio" && git push
```

### Move Portfolio Out of Knowledgebase (Permanently)
```bash
# After GitHub Pages repo is set up:
rm -rf /home/ubuntu/project/Knowledgebase/portfolio/
```

---

## Design System Reference

| Element | Value |
|---------|-------|
| **Background** | #0a0a0a (near-black) |
| **Cards** | #161616 |
| **Accent Color** | #C9A09A (rose gold) |
| **Text Primary** | #f5f5f5 (white) |
| **Text Secondary** | #a3a3a3 (gray) |
| **Font Body** | Inter |
| **Font Code** | JetBrains Mono |
| **Border Radius** | 12px-24px |

---

## Project Status Badges

Use these status labels for projects:

| Status | When To Use |
|--------|-------------|
| **Production System** | Live, being used by real users |
| **Client Project** | Built for a specific client |
| **In Development** | Currently being built |
| **Coming Soon** | Planned but not started |
| **Open Source** | Public GitHub repo |

---

## Example Projects To Add

Here are projects you could add from the Knowledgebase:

### 1. Knowledgebase RAG System
- **What:** Meeting intelligence platform
- **Stats:** 1,754 meetings, 4 years data, 12 weekly reports
- **Tech:** Python, Gemini, Pinecone, Discord, Slack, SQLite

### 2. AM Performance Reports
- **What:** Automated account manager coaching reports
- **Stats:** 10 AMs tracked, 165 meetings analyzed, weekly delivery
- **Tech:** Python, Gemini AI, Gmail SMTP, Discord webhooks

### 3. Sandler Sales Coaching
- **What:** AI sales call analysis with methodology scoring
- **Stats:** 494 sales calls scored, 7 Sandler principles analyzed
- **Tech:** Python, Gemini AI, Fathom API

### 4. DGS Mastermind Summaries
- **What:** Personalized meeting summaries for mastermind group
- **Stats:** 12 members, weekly delivery, action item extraction
- **Tech:** Python, Gemini AI, custom SMTP

---

## Contact Information In Portfolio

| Platform | Value |
|----------|-------|
| **Email** | aaishamotan@gmail.com |
| **Phone** | +92 324 288 5844 |
| **LinkedIn** | linkedin.com/in/aaisha-motan |
| **GitHub** | github.com/aaisha-motan |

---

## Need Help?

Just tell Claude:
- "Add [project] to my portfolio"
- "Update my portfolio stats"
- "Deploy my portfolio to GitHub Pages"
- "Show me how my portfolio looks"

Claude has full context from `CLAUDE_PORTFOLIO_GUIDE.md` and will update `index.html` accordingly.

---

*Last Updated: February 2026*
