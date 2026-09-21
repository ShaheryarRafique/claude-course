# Module 5 — Build with Claude Code · Research

Compiled 2026-09-17 from 5 parallel researchers (Anthropic docs = authoritative, + Coursera, Udemy, Articles, YouTube).
Audience: COMPLETE NON-CODERS (zero terminal/coding background). End goal: install Claude Code and build ONE small real project end-to-end. Global audience, no region-specific examples. 4D framework woven through.

Docs moved to **code.claude.com/docs/en/** (old docs.claude.com/en/docs/claude-code/* now 301-redirects). Re-verify fast-drifting facts (plan eligibility, Auto-mode default, RAM min, costs, install URLs) with fact-verifier before recording.

---

## 1. What Claude Code IS (non-coder framing)

Official: "Claude Code is an agentic coding tool that reads your codebase, edits files, runs commands, and integrates with your development tools."

The gold non-coder line (terminal-guide): **"You don't need to know how to code. Describe what you want in plain English, and Claude writes the code for you."**

Chat app vs Claude Code: chat = advice (text only); Claude Code = **acts on real files in a real folder** on your computer — reads, creates, edits files, runs commands. "Because Claude sees your whole project, it can work across it."

Teaching frame: **a helpful colleague who works inside a folder on your computer.**

## 2. The mental model that matters most: the working directory

When you run `claude` in a folder, that folder becomes Claude's workspace — it can read/create/edit files there and run commands. Teach this first and hard; it's the concept beginners miss ("which folder am I in?"). Rule: **always work in a dedicated practice folder**, never the home directory.

## 3. Install & first run (lead with the easiest path)

**The #1 gap to beat: the terminal/Node cliff.** Even "no-code" courses wrongly drop beginners into terminal + Python venv + npm. Do NOT. Two clean paths:
- **Desktop app (no terminal)** — the Claude desktop app's Code tab; Anthropic: "Don't want to use the terminal? The desktop app lets you skip the terminal entirely." Best door for nervous beginners.
- **Native installer (one line, no Node):** macOS/Linux `curl -fsSL https://claude.ai/install.sh | bash` · Windows PowerShell `irm https://claude.ai/install.ps1 | iex`. Then type `claude`, log in via browser.
- **NEVER teach npm/Node install** (`npm i -g @anthropic-ai/claude-code` needs Node 22+; a top source of setup errors). Never `sudo npm`.

**Prerequisites (verify):** a PAID plan (Pro $20/mo is enough; free plan excluded). macOS 13+/Windows 10 1809+/Ubuntu 20.04+. 4GB+ RAM. Internet.

**Pre-teach the 3 friction fixes:**
- `command not found: claude` / `'claude' is not recognized` → PATH not set → "open a new terminal window and try again."
- Windows PowerShell vs CMD (`PS C:\…>` vs `C:\…>`) — wrong shell breaks `irm`.
- Paste differs: mac `Cmd+V`, Linux `Ctrl+Shift+V`, Win `Ctrl+V`/right-click. Can't click in terminal — use arrow keys; `Esc` interrupts; `exit` or `Ctrl+D` to quit.

## 4. How you work with it (the loop)

"Talk to Claude like a helpful colleague. Describe what you want to achieve." "It's a conversation. You don't need perfect prompts. Start with what you want, then refine."

Agentic loop = **gather context → take action → verify results** (you can interrupt any time). Anthropic's recommended workflow: **Explore → Plan → Implement → Commit.**

This is the SAME loop as Module 4's describe–discern loop — reuse it, don't re-teach. It's a dialogue with a junior colleague, NOT a vending machine (the #1 beginner mistake).

## 5. Safety trio (kills "I'll break my computer" fear)

1. **Plan mode** (`Shift+Tab` until `⏸ plan mode on`): "Claude explores and proposes a plan without editing your source files." Approve before it builds. (Nuance: skip plan mode for trivial one-line changes.)
2. **The Yes/No permission prompt:** "Before creating or changing files, Claude asks for your permission. Press Enter to choose Yes." (Note: Pro/Max/Team default is now **Auto mode** — a classifier reviews actions, so fewer prompts than old tutorials; beginners can switch to Manual to see every prompt. `Shift+Tab` cycles modes.)
3. **Undo:** edits are reversible — "press Esc twice to rewind" (`/rewind`, checkpoints). Caveat: checkpoints track Claude's file edits, NOT Bash changes — not a git replacement.

Plus: **work in a dedicated folder**; **forbid deletions** ("delete nothing, ever — archive instead" — a real user lost 11GB from "clean up this folder"); keep ask-first when doing anything bulk; back up anything irreplaceable.

## 6. Minimum feature set (to ship one project) — and what to DEFER

Include: plain-English requests; the iterate loop; the permission Yes/No; `Shift+Tab` Plan mode; `Esc` interrupt; `Esc Esc`/`/rewind` undo; `/help` `/clear` `/model` `/usage`; one light `CLAUDE.md` via `/init`; `@filename` to tag files; save output explicitly ("save to output.md").

**DEFER to a later/optional module** (Anthropic: "a layer on top of the core agentic loop"): MCP, subagents/agent teams/background agents, hooks, custom skills/slash-commands, Agent SDK, routines, GitHub Actions/CI, deep git. Explicitly tell learners WHY they don't need git yet (removes anxiety).

## 7. Verify without reading code (the discernment habit — bake in early)

"The confidence of the output does not correlate with its correctness" → Anthropic's **"trust-then-verify gap": if you can't verify it, don't ship it.** This is Module 4's *fluent ≠ correct*, applied to code. Non-coders verify by **behavior, not source**: double-click and see it; does it do what you asked? Give Claude a way to verify its own work (a screenshot to compare, "run it and check"). "Silent failure audit."

## 8. Prompting for non-coders (builds on Module 4 Description)

**Action / scope / constraint** 3-line formula. Be specific: name the file, the constraint, the output format. Before→after:
- "make the dashboard look better" → "[paste screenshot] build this, take a screenshot of the result, compare to the original, list differences and fix."
- "fix the bug" → "the page shows a blank screen after I click submit — fix that, and check it works."
- Let Claude interview you for bigger builds; let Claude explore first; one task per prompt (no mega-prompts); `/clear` between tasks and after ~2 failed corrections.

## 9. The project (through-line) — recommendation

Strongest single candidates for a non-coder, finishable, visible, one HTML file (no backend): **a simple personal website / landing page**, or **a personal tracker web app (habit or expense)**. Anthropic's own examples: "make me a simple webpage that says hello world" and "personal budget tracker." Payoff line: **"double-click the HTML file to open it in your browser."** Optional stretch/"ship it": deploy to a live URL (defer the how; keep double-click as the primary reward).

Recommendation: **one personal single-page web app** (e.g., a personal habit/expense tracker OR a simple portfolio page), built across the module, opened by double-click. Keep it ONE small project truly end-to-end — do NOT bolt on a framework/payments finale (the "difficulty cliff" gap).

## 10. Sequence / structure (synthesized)

Coursera spine: Setup → **Plan first (beat blank-canvas)** → First build → Iterate → Verify → Ship (live URL) → Reflect. Anthropic quickstart arc: install → login → start session → ask → small change → build → save. CC for Everyone's scaffolded ladder (each task teaches the skill the next needs) is the pattern to emulate.

Proposed lesson flow:
1. **What is Claude Code, and why** (vs the chat app; the colleague-in-a-folder frame)
2. **Set it up & say hello** (easiest install path; first run; the 3 friction fixes; "hello world" page → double-click)
3. **How you work with it safely** (the folder mental model; Plan mode + permission + undo trio; dedicated folder; never-delete)
4. **Plan your project first** (beat the blank canvas; describe what to build)
5. **Build it, one step at a time** (the iterate loop; action/scope/constraint prompts; one task at a time)
6. **Check it before you trust it** (verify by behavior; fluent ≠ correct; give Claude a way to self-check)
7. **Finish & save your project** (double-click to see; save; light CLAUDE.md; optional deploy) + what's next (defer MCP/agents)

4D woven: **Delegation** = decide what to hand Claude Code, work in a folder, pick the mode; **Description** = specific action/scope/constraint prompts; **Discernment** = verify by behavior, fluent≠correct; **Diligence** = never-delete, review before approve, own the result.

## 11. Objectives style (Coursera pattern)

"direct / describe / verify + a real artifact + no coding required." Examples to adapt:
- "Install Claude Code and confirm it runs."
- "Describe a simple web page in plain English and direct Claude Code to build it."
- "Run your page and verify it does what you asked — without reading the code."
- "Spot one thing wrong and prompt Claude to fix it."
- (stretch) "Ship your page to a live URL."

## 12. Hooks / motivation (non-coder)

- "If you can type, you can build."
- "Describe an app idea in plain English and watch it come to life — without months of learning to code."
- Open on a pain: "Somewhere on your computer there is a folder you are afraid of."
- Reassurance: Claude "asks first" before changing anything; the terminal is "easier than installing a printer."
- Real shared wins: HR leader archived 3,000 Trello cards in 19 min; podcaster synthesized 320 transcripts in 15 min; a non-technical parent's household planning; a personal HTML reading-list tracker.

## 13. Mistakes to prevent (turn into "avoid this" moments)

- Treating it like a vending machine / one-shot mega-prompt → iterate; one task per prompt.
- Trusting confident output → verify (trust-then-verify gap).
- Vague/search-style prompts → action + scope + constraint.
- Arguing in circles → `/clear` and re-prompt after ~2 fails.
- Losing work → save output explicitly; `Esc Esc` to rewind; work in a folder.
- Vague destructive verbs ("clean up this folder" → lost 11GB) → forbid deletion, archive instead, plan first.
- Auto-approving everything → keep ask-first for bulk actions, review each.
- Installing Node/npm unnecessarily → native installer or desktop app.
- No CLAUDE.md → `/init` with plain-English preferences.

## Gaps we can beat (from Udemy roundup)
1. The terminal cliff → lead with easiest path, hide venvs.
2. The mid-course difficulty cliff → keep ONE small project end-to-end, no framework finale.
3. Weak conceptual foundation → our M3/M4 (AI fluency + 4D) already set it up; reuse the loop and discernment.
4. No verify habit → bake in from lesson 1 (ties to Discernment/Diligence).
5. No git but no reassurance → explicitly say why they don't need git yet.
6. Loose demo lists → use a scaffolded ladder on ONE project.

## 14. YouTube — hooks, first demo, pacing (global-adapted)

**Cold open (the wow):** a ~20-second reveal of a non-coder's finished result running in a browser + a countdown promise: "In this lesson you go from nothing installed to a working app you can open in your browser — about 20 minutes, no coding." Time promises reduce intimidation ("install in 90 seconds," "3 prompts to build & deploy," "first app in 30 minutes"). Reframe to lower the bar: "your first project doesn't need to be impressive — it needs to be instructive."

**First visible win (do this BEFORE explaining terminal/permissions/tokens):** a single-file HTML page, ONE prompt, browser refresh = "it works!" No dependencies = no failure surface. e.g., a page showing their name + today's date, styled. Get the dopamine hit first, teach concepts after.

**The three-step launch ritual** (kills "wrong folder" confusion): make a folder → open it → launch Claude there. Teach as three fixed steps. To kill terminal anxiety, consider using VS Code's built-in terminal (right-click "open folder in terminal") so beginners never memorize `cd`.

**Model one real error on screen** and fix it by complaining in plain English ("this shows a blank page — fix it") — this is itself a wow moment and teaches the iterate loop.

**Pacing tips:** visible win in first minutes before theory; time-stamped checkpoints ("by minute 20 a styled UI, by 30 it works"); one task per conversation; Plan Mode first, always (most-repeated tip); set expectation "3–5 rounds, v1 is an MVP"; "vibe" edits in plain language ("the colors feel flat, make it feel more alive"); tell them to take breaks and ask Claude when confused.

**Projects that resonate (global):** personal habit/streak tracker, expense/budget tracker, packing-list generator (destination + dates → checklist), to-do checklist with local save, folder/screenshot organizer, a simple portfolio page. Winners solve a real personal chore, not a toy.

## Sources
- Anthropic (authoritative): code.claude.com/docs/en/ — overview, quickstart, setup, terminal-guide, how-claude-code-works, permissions, permission-modes, costs, features-overview, best-practices
- Coursera: Build Apps with AI (Vanderbilt), Build Anything with AI (No Code), AI for Vibe Coding, UW Guided Website Development
- Articles: ccforeveryone.com, youcanbuildthings.com, self.md, adventuremedia.ai
- Udemy roundup + CC for Everyone + Claude Code 101 (Anthropic Academy / DataCamp)
- YouTube: non-coder Claude Code tutorials (LowCode 30-min app, ClaudeWorld habit tracker, Michael Crist non-technical guide, Kevin Stratvert, XDA, roadmap.sh vibe-coding) — hooks, first demo, pacing
