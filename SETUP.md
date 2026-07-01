# Real Estate EA Kit — Setup Guide

Welcome. This guide walks you through setting up your personal AI executive assistant from scratch. Budget **45–60 minutes** the first time.

---

## What You'll Have When You're Done

A personal AI assistant that:
- Writes listing descriptions, social media posts, and WhatsApp follow-ups in your voice
- Drafts RedNote (小红书) scripts in Chinese for property content
- Tracks your sales pipeline and P&L
- Manages your calendar and daily briefings
- Gets smarter about you with every session

---

## What You Need Before Starting

| Requirement | Cost | Link |
|---|---|---|
| Claude Pro subscription | USD $20/month | [claude.ai](https://claude.ai) |
| GitHub account | Free | [github.com](https://github.com) |
| This kit (you already have it) | — | — |

---

## Step 1: Get Claude Pro

1. Go to [claude.ai](https://claude.ai) and sign up
2. Upgrade to **Claude Pro** ($20 USD/month)
3. This gives you access to Claude Code — the tool that powers your assistant

---

## Step 2: Set Up GitHub

1. Go to [github.com](https://github.com) and create a free account
2. Click **New Repository** (top right, green button)
3. Name it anything — e.g. `my-ea` or `agent-assistant`
4. Set it to **Private**
5. Click **Create Repository**

---

## Step 3: Upload the Kit to Your Repo

**Option A — GitHub Desktop (recommended, no coding needed)**
1. Download [GitHub Desktop](https://desktop.github.com)
2. Sign in with your GitHub account
3. Clone your new repo to your computer
4. Copy all the files from this kit into the cloned folder
5. Commit and push (big blue button)

**Option B — Upload via browser**
1. Open your GitHub repo
2. Click **Add file → Upload files**
3. Drag in all the kit files
4. Click **Commit changes**

---

## Step 4: Fill In Your Details

Open these files and replace every `[PLACEHOLDER]` with your real info:

### `context/me.md`
- Your name, agency, brand name, location

### `context/work.md`
- Your services, revenue target, social media handles, website

### `context/current-priorities.md`
- Your top 3–5 priorities right now

### `context/goals.md`
- Your quarterly revenue and business goals

### `CLAUDE.md`
- Replace `[YOUR_NAME]` with your name
- Replace `[ASSISTANT_NAME]` with whatever you want to call your assistant (e.g. Jay, Max, Alex)
- Replace `[YOUR_AGENCY]` with your agency name

---

## Step 5: Connect Claude Code to Your Repo

1. Open [claude.ai/code](https://claude.ai/code) or the Claude Code app
2. Click **New Project** → **Connect GitHub**
3. Select your repo
4. Claude Code will load your `CLAUDE.md` and context files automatically

---

## Step 6: Your First Session

Type: **"Hi [ASSISTANT_NAME]"**

Your assistant will greet you. Then try:

- *"Write a listing writeup for [property address]"*
- *"Draft a WhatsApp follow-up for a buyer I met yesterday"*
- *"Create an Instagram post about [topic]"*
- *"Write a RedNote script on [topic] in Chinese"*

---

## Step 7: Connect MCP Integrations (Optional but Powerful)

MCP servers let your assistant take real actions — creating calendar events, reading your Notion pipeline, generating Canva designs.

To connect them:
1. In Claude Code, go to **Settings → MCP Servers**
2. Add the integrations you use:
   - **Google Calendar** — for scheduling and daily briefings
   - **Notion** — for pipeline and notes
   - **Canva** — for marketing graphics
   - **Google Drive** — for file storage

Each integration has a one-time auth step. Once connected, your assistant can use them automatically.

---

## Skills Reference

Your assistant comes with 10 built-in skills. Invoke them naturally:

| Skill | How to Use |
|---|---|
| **listing-writeups** | "Write a listing for [address, details]" |
| **social-media-content** | "Create an Instagram post about [topic]" |
| **follow-up-templates** | "Draft a follow-up WhatsApp for [situation]" |
| **rednote-scripts** | "Write a RedNote script about [topic] in Chinese" |
| **blog-content** | "Write a blog post on [topic] for SEO" |
| **marketing-visuals** | "Create a Canva brief for [property/campaign]" |
| **calendar-management** | "What's on my calendar this week?" |
| **sales-pipeline** | "Update my pipeline — [deal details]" |
| **pnl-tracker** | "Log a deal: [amount, type, date]" |
| **research** | "Research [topic] for Singapore property market" |

---

## Tips for Getting the Most Out of It

- **Keep context files updated.** The more your assistant knows about you, the better it performs.
- **Save recurring workflows as skills.** If you do something more than 3 times, ask your assistant to build a skill for it.
- **Use the decision log.** Every meaningful business decision goes in `decisions/log.md` — your assistant references it.
- **Talk to it like a colleague.** No need for formal prompts. Just say what you need.

---

## Troubleshooting

**Assistant doesn't know my details**
→ Make sure you filled in all the `[PLACEHOLDER]` fields in the context files and re-opened the session.

**Skills aren't working**
→ Check that the skill files are in `.claude/skills/[skill-name]/SKILL.md`

**MCP integrations not connecting**
→ Re-authorise from Claude Code Settings → MCP Servers

---

## Need Help?

Contact: **[YOUR SUPPORT CONTACT]**

---

*Built on Claude Code by Anthropic. Claude Pro subscription required.*
