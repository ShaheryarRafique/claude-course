# Module 5 — Build with Claude Code · Plan (v5, workshop-structured)

Rebuilt after studying the SoftAims "Claude Code — Dev Workshop" artifact (30 slides). Keep OUR theme (maroon/cream reveal.js). Adopt the artifact's STRUCTURE and CONTENT DEPTH, not its dark/orange visuals. This makes Module 5 a serious, well-structured Claude Code module: the build basics for everyone, then the power layer and the patterns that make someone actually good.

## The reusable slide format (adopt for every "feature" lesson)
kicker `Lesson 5.X · Feature` → big title → **one-line definition with an analogy** → left column **"How it works"** (3 bolded lead-ins) → right column **"Where it wins" / the concrete list** (uses, events, servers) → a **real config/prompt snippet** (promptcard or code block) → a **one-line callout takeaway** (`.rule`-style). Short on screen, detail in Note.

## Module outcome ("By the end of this module")
- Install Claude Code and open it in your own folder
- Direct it, in plain English, to plan, build, and verify a change
- Steer long runs, and let it manage your code with git
- Use the power layer: skills, subagents, rules, hooks, memory, MCP, plugins
- Ship the way strong teams do: spec-driven, with a real check on every result

## PART 1 — Use it (the build basics, for everyone)
Keep the action-first essentials we already wrote, tightened.
- **5.1 Meet Claude Code & get in** — advise → act (it works in your folder); set up your tools (VS Code, Node, Git, Python); install; first real file. Reframe hook, straight from the artifact: *"Most people use Claude like a chat box. Now we drive it."*
- **5.2 Build it together** — plan mode (scope) · permissions (it asks) · the build · rewind (undo). One real thing, controls learned in the flow.
- **5.3 Steer it & ship it** — `/compact` to keep a long run on track · Claude manages your code with git.

## PART 2 — The power layer (each = the rich format above)
- **5.4 Skills** — *a reusable instruction file (SKILL.md) Claude pulls in when the task needs it.* How it works (a file it adds to its toolkit / triggers automatically or by name / packages a routine). Where it wins (a review checklist, a deploy step, a house style). Snippet: a tiny SKILL.md. Callout: a skill is know-how Claude reuses.
- **5.5 Subagents & agent teams** — *one big job, split across helper Claudes working at once, then double-checked.* How it works (you give one big job → it splits into helpers, one slice each → a fresh checker merges into one summary). Team vs Workflow (a lead + teammates who talk, vs a script running silent helpers). Where it wins (review all changed files, a big migration, audit every endpoint, deep research, fix-until-green). Callout: a subagent keeps your main chat clean.
- **5.6 Rules** — *instructions that load only for the files you're editing.* How it works (tied to a file path / loads on match / keeps context small). Where it wins (per-area rules: jobs, migrations, models, tests). Snippet: `.claude/rules/*.md` with a `paths:` header. Callout: right rule, right file, small context.
- **5.7 Hooks** — *a command that runs automatically at a set moment, like a git pre-commit hook, but for Claude's actions.* How it works (pick a moment / run any command / it can even block an action). The event list (PreToolUse, PostToolUse, UserPromptSubmit, Stop, SessionStart/End, etc.). Snippet: `.claude/settings.json` PreToolUse blocking `rm -rf`. Callout: CLAUDE.md is advice, a hook is a guarantee.
- **5.8 Memory & CLAUDE.md** — *Claude writes down what it learns and reads it back next session.* How it works (one lesson per file / `/init` for CLAUDE.md / `/memory` to view/edit / auto-memory is local, move a lesson into CLAUDE.md to share with the team). Snippet: a memory file with frontmatter. Callout: fix it once, never again.
- **5.9 MCP** — *how Claude reaches outside itself: GitHub, your database, the browser, Figma.* How it works (one server per tool / it adds real actions, not just reading / listed in one `.mcp.json`). Servers people plug in (GitHub, Postgres, Playwright/Chrome, Context7, Sentry). Callout (verbatim-worthy): *a skill is instructions Claude follows; an MCP is a tool Claude can actually use.*
- **5.10 Plugins** — *package a setup you trust — skills, hooks, subagents, MCP — as one installable unit your whole team gets.* How it works (bundle your setup / share it / install with `/plugin`). Where it wins (a team's standard toolkit in one command). Callout: your best setup, shipped to everyone.

## PART 3 — Patterns that make you good
- **5.11 Give Claude a way to check its work** (the #1 lever) — *the difference between a session you babysit and one you walk away from.* Claude stops when it "looks done" → give it a pass/fail signal (a test, a build, a screenshot) → the loop closes itself. Vague vs verifiable prompt (before/after). Callout: ask for evidence, not claims. (Callback to Module 4 Discernment, applied to code.)
- **5.12 Spec-driven development** — *before a line is written, Claude works out the delta and the plan with you.* The delta-first flow (extract the delta → review and brainstorm, it asks you the questions first → write the spec with test cases as the acceptance criteria → then build). One feature, one spec folder. Callout: agree the spec, then building is just following it.
- **5.13 Claude Code is a harness** (the mental model to close on) — *the model reasons; the harness is everything around it — tools, context, the loop, tests, memory — that turns a raw model into an agent you can trust.* Guides (rules, skills, docs) prevent mistakes; sensors (tests, a judge agent) catch them. Callout: the wins are in the harness, not just the model.

## Module recap
Everything you learned about directing AI (the 4Ds) now runs on your real project, wrapped in a harness you control. One line: **you do not use Claude Code, you drive it.**

## Notes
- Size: ~13 lessons, ~40+ slides. This is a full workshop, matching the artifact's ambition and the user's "one module, everything" call. If too big, Part 3 (or Plugins) can move to a follow-on.
- Audience shift: this is builder/developer-leaning ("the team that wants to get good"). Part 1 keeps a gentle on-ramp; Parts 2–3 assume they are building for real.
- 4D as callbacks only (5.11 verification = Discernment/Diligence). Never re-teach.
- Verify config snippets and commands (`/memory`, `.claude/rules`, hook events, `.mcp.json`, `/plugin`) against code.claude.com with fact-verifier before recording.
- Overlap guard vs the Cowork module: this is strictly building code in a project; Cowork stays office/knowledge work.
