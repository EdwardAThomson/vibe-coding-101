 
# Tooling & Setup for Vibe Coding

This page is a practical overview of common Vibe Coding tools and how to pick a setup that fits your budget and workflow.

The goal: **get from idea → running code → iteration** with as little friction as possible.


## YouTube videos: 
If you prefer to learn by watching videos, here are my videos to help:

* (5 minute overview)[https://youtu.be/Q3Moo9CHlQ8]
* (30 minute deep dive)[https://youtu.be/l5t13qk11R8]


## The 3 common setups

### Setup A — Chatbot-only

**Best for:** learning the workflow, quick prototypes, brainstorming  
**What you use:** ChatGPT (or similar) + a basic editor

**Pros**

- Fastest to start
- Works anywhere
- Great for drafting `spec.md` and `plan.md`

**Cons**

- Copy/paste overhead
- Harder to apply small diffs cleanly
- Less helpful for navigating larger codebases

**Minimal stack**

- Chatbot (ChatGPT / Claude / Gemini / etc.)
- Any editor (VS Code, Notepad++, Vim, etc.)
    - VS Code is a full IDE that is free to download and use.
- Git (optional but recommended)

---

### Setup B — IDE assistant (recommended for most people)

**Best for:** building real projects, iterating quickly, keeping changes controlled  
**What you use:** an IDE with an AI assistant that can edit files directly

**Pros**

- The AI can edit your code in-place (less copy/paste)
- Easier to apply patch-style changes
- Faster debug loop (run → fix → run)
- Can edit multiple files at once

**Cons**

- Most tools are paid (all have free trials, although Google's AG has a completely free tier)
- You still need to review changes

**Typical stack**
- IDE: Cursor, Windsurf, Antigravity, VS Code with Roocode plugin, JetBrains, etc.
- Terminal + Git

**Recommended habits**
- Keep milestones short
- Run tests / run the app after each change

---

### Setup C — Agentic CLI (power-user mode)

**Best for:** larger refactors, repo-wide changes, automation, repetitive tasks  
**What you use:** a CLI “agent” that can read the repo and apply changes across files

**Pros**

- Great for multi-file edits
- Useful for “make this consistent everywhere” tasks

**Cons**

- Easier to cause large unintended changes
- Needs stronger guardrails (diff-only, tight scope, review)
- Often costs more (depending on model usage)
- Harder to review changes, often requires opening IDE anyway

**Typical stack**

- CLI agent + terminal
- IDE for review
- Git for safety (commit early, commit often)



## Costs (how to think about it)

Tool pricing changes constantly, but the categories are stable:

- **Chat-only:** often has a free tier, paid tiers for better models/limits
    - Starting at $20 / month
    - OpenAI Max plan is $200 / month
    - Anthropic offers $100 and $200 / month pro and max tiers.
    - For Gemini, usage is bundled into the Google One subscription. Prices are ~$20 and $120 / month.
- **IDE assistants:** commonly a monthly subscription
    - Google offers a free tier for Antigravity.
    - Most other IDE assistants start at $20 / month.
    - Windsurf allows for purchasing top-up credits.
- **Agentic CLI:** can be subscription-based or usage-based (tokens)
    - Usage costs are bundled into the cost of the chatbot tiers.



## Recommended “starter stack” (minimal friction)

- Start cheap: Chat + a normal editor
- Upgrade when copy/paste slows you down
- If you’re doing large edits, Git + diff review becomes non-negotiable


## Safety rails (highly recommended)

### 1) Use Git as a time machine

- Create a GitHub account
- Commit when you reach a working checkpoint
- If the AI breaks things, you can roll back
- Ask AI for help with Git commands

### 2) Prefer diffs over rewrites

Ask for:

- “Only change the smallest amount needed”
- “Do not refactor unrelated code”

### 3) Keep scope tight

Good:

- “Implement Milestone 1 only”
- “Only edit `App.jsx` and `styles.css`”

Bad:

- “Improve the whole project”

### 4) Run constantly

- Run after every meaningful change
- If it doesn’t run, you’re not iterating — you’re guessing



