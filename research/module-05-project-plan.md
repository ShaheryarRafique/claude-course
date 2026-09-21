# Module 5 Project — "Ship a Lead Tracker with Claude Code"

The capstone for Module 5. The learner drives Claude Code, from an empty folder to a running,
shipped app, deliberately using the workflow and every building block the module taught. Global,
beginner-friendly, with a coding-track stretch path.

## Outcome (one line)
By the end you have driven Claude Code to build, verify, and ship a real web app, plus the setup
(CLAUDE.md, a skill, a subagent review, a hook) that proves you drove it like a pro, not chatted at it.

## Why this app
A Lead Tracker is something any freelancer, shop, or agency actually needs: capture a lead, see the
list, update its status, mark it won or lost. Small enough to finish in one sitting, real enough to
keep using. Swap it for a task tracker, expense log, or booking sheet if you prefer — the steps are
identical, only the spec changes.

## What it does (spec v1)
- Add a lead: name, contact, source, status (New / Contacted / Won / Lost)
- See all leads in a list, newest first
- Change a lead's status; delete a lead
- Data persists in the browser (localStorage), no backend
- One clean page, works on phone and desktop

## Tech, kept beginner-friendly
- A single-folder web app: `index.html` + a little JS + CSS, data in localStorage
- Runs by opening the file in a browser — no server, no database
- Git for version control (Claude writes the commits)

## The build path (maps 1:1 to the module)

### Phase 0 — Set the stage · Memory
- Make an empty folder, open Claude Code in it
- Run `/init`, then edit CLAUDE.md: the app's purpose, "vanilla JS, no frameworks", "keep it one file", your naming style
- 4D: Delegation — you set the ground rules, Claude builds within them

### Phase 1 — Explore & Plan · Workflow + Description
- Turn on plan mode (`Shift+Tab`)
- Prompt: "I want to build a Lead Tracker [features]. Interview me about the edge cases and tradeoffs, then write SPEC.md with acceptance criteria." (the "let Claude interview you" habit)
- Review and edit SPEC.md — its acceptance criteria become your verification checklist
- 4D: Description — a precise spec beats a vague ask

### Phase 2 — Implement · Workflow
- Approve the plan, let Claude build feature by feature: add-a-lead → the list → status changes → delete → persistence
- After each feature, open it in the browser and check it against the spec
- Habit: small verifiable steps, not one giant prompt

### Phase 3 — Give it a check · Diligence
- Ask Claude to add a check it can run itself — a small test, or an "open it and confirm each acceptance criterion" pass
- Prompt: "run the check, fix anything that fails, and show me the evidence"
- 4D: Diligence — evidence, not claims

### Phase 4 — The pro layer (pick 2, do all 4 for the full badge)
- **Skill** — write `.claude/skills/add-field/SKILL.md` that captures how you add a new field end to end, then use it to add a "notes" field
- **Subagent** — "use a subagent to review the code for bugs and edge cases", then fix what it finds
- **Hook** — a PostToolUse hook that formats after every edit, or a PreToolUse hook that blocks deleting your data file
- **Loop** — `/loop until the check passes, fix what fails each round` while you make tea

### Phase 5 — Ship it · Commands + git
- "commit my changes with clear messages" as you go; end with a clean history and a working app
- Optional (coding track): connect the GitHub MCP or use `gh` to open a PR

## Deliverables (what to show)
1. The running app — a short screen recording or screenshots (add → list → mark won)
2. `SPEC.md` with acceptance criteria
3. `CLAUDE.md`
4. Proof of at least two building blocks actually used: the skill file, the hook in settings.json, or the subagent's review output
5. The git log

## What good looks like (rubric)
- The app meets every acceptance criterion in the spec
- You explored and planned before building — SPEC.md exists and shaped the code
- There is a real check Claude ran, with evidence it passed
- At least two building blocks are set up and actually used, not just named
- Clean, readable commits

## Stretch goals (optional coding track)
- Search / filter by status; export to CSV; a "follow-up date" that sorts to the top
- Swap localStorage for a tiny backend (Node + a JSON file) — now you use the prereqs
- Build a second app with the SAME setup by packaging your skill + hook as a plugin

## Time
- Core: ~60–90 minutes guided · With stretch goals: 2–3 hours

## How it threads the module
Every phase reuses a lesson — `/init` & CLAUDE.md (Memory), plan mode (Workflow), the spec
(Description), the check (Diligence), skill/subagent/hook (building blocks), commits (Commands),
`/loop` (Loops) — and the 4Ds run straight through: Delegation, Description, Discernment, Diligence.

## Slides to build next (Module 4 style)
1. Dark divider — "Your project: Ship a Lead Tracker"
2. "What you'll build" — the spec, one clean list
3. "The build path" — the five phases (a flow diagram, reusing the `.diagram` style)
4. "Prove you drove it" — deliverables + rubric
5. Stretch goals (optional coding track)
Plus, optionally: a downloadable one-page brief and a starter-prompts pack (the exact prompts per phase).

## Notes / flags
- Keep the core app static (localStorage) so the everyone-track can finish; stretch goals serve the coding track.
- All commands used are already fact-verified in the module (`/init`, plan mode `Shift+Tab`, `/agents`, hooks in `.claude/settings.json`, `/loop`, `claude mcp add`).
- The app is swappable — if the user prefers a task tracker / expense log / booking sheet, only the spec changes.
