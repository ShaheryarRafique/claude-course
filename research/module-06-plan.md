# Module 6 — Claude Code Pro · Slide Plan

The advanced half of Claude Code, split off from Module 5 (Claude Code Essentials). Mirrors Claude Code 101's "Customizing" module + Anthropic's "Claude Code in action" course. OPTIONAL / power-user track. Audience: those who finished Module 5 and want to customize and automate. Feature tour, small example per feature. Global examples.

Deck conventions: same as Module 5 (dark divider + dark lesson cards, objectives rule, lean lessons, tables/promptcards, no swappable-duplicate bullets).

## Module outcomes ("By the end of this module")
- Use subagents to keep your main conversation clean
- Package reusable know-how into skills
- Connect Claude Code to your tools with MCP
- Guarantee actions with hooks
- Run longer sessions with confidence (steer, configure, verify)

## Framing slides
1. **Divider (dark):** `06` · Module 6 · **Claude Code Pro** · `Optional · Customize and automate Claude Code`
2. **By the end of this module** — the outcomes.
3. **Go deeper** (refs): code.claude.com/docs (sub-agents, skills, mcp, hooks) · Claude Code in action + Intro to Agent Skills (academy.claude.com).

---

## PART A — Extend Claude Code (the four customizing features)

### Lesson 6.1 — Subagents
Objectives: (1) Explain what a subagent is · (2) Use one for a noisy side task
- **What it is:** *"specialized AI assistants that handle specific types of tasks"* — each runs in its own context and *"returns only the summary,"* so a big side task doesn't flood your main chat.
- **Use it / example:** say *"use a subagent to investigate how our login handles token refresh"* — findings come back clean. (Writing your own agent file — a `.md` in `.claude/agents/` — is the next step.)
- Recap.

### Lesson 6.2 — Skills
Objectives: (1) Explain what an Agent Skill is · (2) Tell it apart from a subagent
- **What it is:** a `SKILL.md` that *"extends Claude's knowledge"* with your project/team/domain know-how, loaded **on demand** in the current chat (auto, or `/skill-name`).
- **Skill vs subagent:** a skill = reference/procedure loaded inline; a subagent = complex work done in isolation. CLAUDE.md loads every session; a skill loads only when relevant. Skills ship inside **plugins** (`/plugin`, named `plugin:skill`). Example: an `api-conventions` skill Claude follows when relevant.
- Recap.

### Lesson 6.3 — MCP
Objectives: (1) Explain what MCP does in plain words · (2) Connect Claude Code to one of your tools
- **What it is:** *"an open standard that lets Claude connect to hundreds of external tools and data sources"* — read and act on them directly instead of pasting data in. Connects to GitHub, Google Drive, Slack, a database, an issue tracker, etc.
- **Example:** *"Add the feature described in JIRA issue ENG-4521 and create a PR on GitHub."* Setup shape: `claude mcp add …` (one line), manage with `/mcp`. Caveat: when a simple CLI tool exists (like `gh`), it's often enough.
- Recap.

### Lesson 6.4 — Hooks
Objectives: (1) Explain what a hook is · (2) Know when a hook is worth it
- **What it is:** *"user-defined commands that execute automatically at specific points"* in Claude Code's lifecycle. Unlike CLAUDE.md (advisory), hooks are **deterministic** — the action happens *every time* (e.g., run a check after each edit, or block a dangerous delete).
- **Who it's for:** mostly teams/organizations (security, validation, CI). Claude can write one for you.
- Recap.

## PART B — Work at scale ("Claude Code in action" — RESEARCH BEFORE BUILDING)

Candidate lessons from Anthropic's "Claude Code in action" course (9 lessons: steering, configuration, automation, verification). Research these from code.claude.com + the course before building:
- **6.5 — Steer longer sessions** (keep a long task on track: plan mode, `/rewind`, interrupting, re-planning)
- **6.6 — Verify and trust the output** (tests, screenshots, "show evidence," the `/verify` habit at scale)
- **6.7 — Automate the boring parts** (slash commands, CLAUDE.md rules, headless/`-p` mode, running Claude in scripts)
- **6.8 — Configure Claude Code to your workflow** (settings, permissions rules, model choice, output styles)

## Notes / flags
- Build Module 5 (Essentials) FIRST; Module 6 is the optional follow-on.
- Reconcile with the old "Connect and Automate" module — subagents/skills/MCP now live here, so Connect & Automate becomes connectors + Cowork only (or merges).
- Before building Part B, run researcher-anthropic on "Claude Code in action" (steering, configuration, automation, verification) for accurate content.
- Re-verify commands/flags with fact-verifier before recording.
