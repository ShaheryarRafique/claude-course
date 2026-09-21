<!-- .slide: data-background-color="#17181a" class="dark" -->

<div class="mod-num">05</div>

### Module 5

## Claude Code

<span class="tag core">Core</span> Most people use it like a chat box. Now we drive it.

Note: The reframe. This module takes you from installing Claude Code to driving it like a pro: what it is, how it works, its real building blocks, and the habits that separate most people from the rest. Built on Anthropic's official Claude Code docs. One idea per slide, taught lesson by lesson, like Module 4.

---

<div class="lesson-no">Module 5 · What you will be able to do</div>

# By the end of this module

- Install Claude Code and run it in your own project
- Drive a change through explore, plan, implement, and commit
- Use the building blocks: skills, agents, memory, hooks, MCP, plugins
- Ship like a pro: reach for the right tool and check every result

Note: Module outcomes, one capability each, in the order we teach them. First get it running and understand how it works, then each building block, then the pro habits that tie it all together.

---

<!-- .slide: data-background-color="#17181a" class="dark" -->

<div class="lesson-no">Lesson 5.1</div>

## Meet Claude Code

By the end of this lesson you will be able to:

- Explain what Claude Code is and why it beats the chat app
- Name where it can run and what it can do

Note: Start from zero. Before any feature, learners need to know what this tool actually is and why it is different from the Claude app. Source: code.claude.com/docs/en/overview.

---

<div class="lesson-no">Lesson 5.1 · What it is</div>

# What Claude Code is

An agentic coding tool that reads your codebase, edits files, runs commands, and integrates with your development tools.

- It understands your whole project, not one snippet
- It works across many files and tools to get things done
- It acts in your codebase, no copy and paste

Note: The definition, close to the doc's wording. The chat app talks about your code; Claude Code changes it. That is the leap this module is built on.

---

<div class="lesson-no">Lesson 5.1 · Where it runs</div>

# It runs where you work

- **Terminal** the full command-line tool
- **VS Code and JetBrains** inside your editor, with inline diffs
- **Desktop app** visual diffs and parallel sessions
- **Web** cloud sessions from the browser

<p class="thread">Same engine everywhere. Your CLAUDE.md and settings follow you.</p>

Note: One tool, several surfaces, all sharing the same engine. Teams also run it in CI and Slack, but the terminal and IDE are where most people start.

---

<div class="lesson-no">Lesson 5.1 · What you can do</div>

# What you can do with it

- **Build and fix** describe a feature or paste an error, it plans and implements
- **Automate the tedious** tests, lint fixes, dependency bumps, release notes
- **Commit and PR** it writes the message, branches, and opens the pull request
- **Connect your tools** reach Jira, Slack, or your database through MCP
- **Script it** pipe logs in, run it in CI, chain it with other tools

Note: Straight from the doc's "What you can do" list. This is the motivation slide: the range is much wider than "write a function for me."

---

<div class="lesson-no">Lesson 5.1 · Recap</div>

# Quick recap

- Claude Code is an agentic coding tool that edits files, runs commands, and uses git
- It runs in the terminal, your IDE, the desktop app, or the web
- It builds, fixes, automates, commits, and connects to your tools

<div class="refs">
<a href="https://code.claude.com/docs/en/overview" target="_blank" rel="noopener"><span class="ref-src">Read more ·</span> Claude Code overview</a>
</div>

Note: Ten second reminder. Next, let us get it installed and running on your machine.

---

<!-- .slide: data-background-color="#17181a" class="dark" -->

<div class="lesson-no">Lesson 5.2</div>

## Install and first run

By the end of this lesson you will be able to:

- Install Claude Code on Mac or Windows
- Sign in and open it in your project

Note: The setup lesson. This is the step that stops most people, so we make it exact for both operating systems. Source: code.claude.com/docs/en/overview and /setup.

---

<div class="lesson-no">Lesson 5.2 · Install it</div>

# Install it in one line

One command installs it. No Node, no extra setup. A paid plan is required: Pro, Max, Team, or API credits.

- **Mac or Linux** &nbsp; `curl -fsSL https://claude.ai/install.sh | bash`
- **Windows (PowerShell)** &nbsp; `irm https://claude.ai/install.ps1 | iex`

Prefer an app? Download the desktop app or run it in the browser.

<div class="refs">
<a href="https://code.claude.com" target="_blank" rel="noopener"><span class="ref-src">Download ·</span> code.claude.com</a>
<a href="https://claude.ai/code" target="_blank" rel="noopener"><span class="ref-src">Web ·</span> claude.ai/code</a>
</div>

Note: The native installer does not need Node or npm. Package-manager options exist too: brew install --cask claude-code on Mac, winget install Anthropic.ClaudeCode on Windows. The desktop app bundles the CLI. The free claude.ai plan does not include Claude Code.

---

<div class="lesson-no">Lesson 5.2 · First run</div>

# Your first run

- Open your project folder in the terminal
- Type `claude` and sign in through the browser
- Confirm it with `claude --version`
- Now ask it to make a change, in plain English

<p class="thread">You are now driving Claude inside your own code.</p>

Note: The first-run flow. The sign-in is a one-time browser step. Once claude --version prints a number, you are ready to give it real instructions.

---

<div class="lesson-no">Lesson 5.2 · Recap</div>

# Quick recap

- Install with one line on Mac, Linux, or Windows, no Node needed
- A paid plan (Pro, Max, Team, or API credits) is required
- Run `claude` in your project, sign in, then start giving instructions

<div class="refs">
<a href="https://code.claude.com/docs/en/setup" target="_blank" rel="noopener"><span class="ref-src">Read more ·</span> Setup and install options</a>
</div>

Note: Ten second reminder. Next, the workflow that keeps Claude from jumping straight to code.

---

<!-- .slide: data-background-color="#17181a" class="dark" -->

<div class="lesson-no">Lesson 5.3</div>

## The workflow

By the end of this lesson you will be able to:

- Move a change through explore, plan, implement, and commit
- Use plan mode to review before any edit

Note: The single most important habit in the module. Left alone, Claude jumps straight to code. This workflow slows it down at the right moment. Source: code.claude.com/docs/en/best-practices.

---

<div class="lesson-no">Lesson 5.3 · The four phases</div>

# Explore, plan, implement, commit

Left alone, Claude jumps straight to code, and often solves the wrong problem. So we move a change through four phases.

<svg class="diagram" viewBox="0 0 760 130" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Explore, plan, implement, commit">
<defs><marker id="fah" markerWidth="9" markerHeight="9" refX="6.5" refY="3" orient="auto"><path d="M0,0 L7,3 L0,6 Z" fill="#7c2d3a"/></marker></defs>
<g>
<rect x="6" y="34" width="160" height="66" rx="12" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="86" y="64" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="19" fill="#17181a">Explore</text>
<text x="86" y="85" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="13" fill="#6b6659">understand</text>
</g>
<g>
<line x1="166" y1="67" x2="200" y2="67" stroke="#7c2d3a" stroke-width="2.5" marker-end="url(#fah)"/>
<rect x="200" y="34" width="160" height="66" rx="12" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="280" y="64" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="19" fill="#17181a">Plan</text>
<text x="280" y="85" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="13" fill="#6b6659">decide the steps</text>
</g>
<g>
<line x1="360" y1="67" x2="394" y2="67" stroke="#7c2d3a" stroke-width="2.5" marker-end="url(#fah)"/>
<rect x="394" y="34" width="160" height="66" rx="12" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="474" y="64" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="19" fill="#17181a">Implement</text>
<text x="474" y="85" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="13" fill="#6b6659">build &amp; test</text>
</g>
<g>
<line x1="554" y1="67" x2="588" y2="67" stroke="#7c2d3a" stroke-width="2.5" marker-end="url(#fah)"/>
<rect x="588" y="34" width="166" height="66" rx="12" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="671" y="64" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="19" fill="#17181a">Commit</text>
<text x="671" y="85" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="13" fill="#6b6659">ship it</text>
</g>
</svg>

<p class="thread">Explore and plan decide the result. Implement and commit just carry it out.</p>

Note: Four phases. The mistake beginners make is skipping the first two. Explore and plan are where a good result is decided. The diagram carries the idea so the slide is not a wall of text.

---

<div class="lesson-no">Lesson 5.3 · One task, four prompts</div>

# The same task, four prompts

Adding "Log in with Google", one prompt per phase:

| Phase | What you type |
| --- | --- |
| Explore | read `src/auth`, see how login and sessions work, no edits |
| Plan | I want Google login. Which files change? Make a plan. |
| Implement | build it from your plan, write tests for the callback, run them |
| Commit | commit with a clear message and open a PR |

Note: The concrete example, straight from the docs. The point to land: explore and plan happen before a single line is written, so Claude builds the right thing. Source: code.claude.com/docs/en/best-practices.

---

<div class="lesson-no">Lesson 5.3 · Plan mode</div>

# Plan mode, and when to skip it

Press `Shift+Tab` to turn on plan mode. Claude explores and plans, but cannot edit a file until you approve.

- **Plan** when a change touches several files, or code you do not know
- **Skip it** for a typo, a log line, or a rename, just ask directly
- On Pro and Max, auto mode handles routine approvals for you

<p class="thread">If you can describe the change in one sentence, skip the plan.</p>

Note: From the doc's callback: planning adds overhead. Use it when the approach is uncertain or the change is broad; skip it for tiny, obvious fixes. Plan mode is a keyboard toggle, not a slash command.

---

<div class="lesson-no">Lesson 5.3 · Recap</div>

# Quick recap

- Work in four phases: explore, plan, implement, commit
- Turn on plan mode with `Shift+Tab` to approve the plan before any edit
- Planning first beats letting Claude jump straight to code

<div class="refs">
<a href="https://code.claude.com/docs/en/best-practices" target="_blank" rel="noopener"><span class="ref-src">Read more ·</span> Best practices</a>
</div>

Note: Ten second reminder. Next, a look under the hood: how Claude Code actually works.

---

<!-- .slide: data-background-color="#17181a" class="dark" -->

<div class="lesson-no">Lesson 5.4</div>

## How Claude Code works

By the end of this lesson you will be able to:

- Describe the loop Claude runs on every task
- Name what it can reach, and how you extend it

Note: The mental model. Understanding the loop makes every later feature click into place. Source: code.claude.com/docs/en/how-claude-code-works.

---

<div class="lesson-no">Lesson 5.4 · The loop</div>

# The loop it runs

Give Claude a task and it works in three phases, over and over, until the job is done.

<svg class="diagram" viewBox="0 0 760 250" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="The agentic loop: gather context, take action, verify, repeat">
<defs><marker id="lah" markerWidth="9" markerHeight="9" refX="6.5" refY="3" orient="auto"><path d="M0,0 L7,3 L0,6 Z" fill="#7c2d3a"/></marker></defs>
<g>
<rect x="18" y="34" width="212" height="76" rx="14" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="124" y="68" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="21" fill="#17181a">Gather context</text>
<text x="124" y="93" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="14" fill="#6b6659">search and read files</text>
</g>
<g>
<line x1="230" y1="72" x2="270" y2="72" stroke="#7c2d3a" stroke-width="2.5" marker-end="url(#lah)"/>
<rect x="274" y="34" width="212" height="76" rx="14" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="380" y="68" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="21" fill="#17181a">Take action</text>
<text x="380" y="93" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="14" fill="#6b6659">edit code, run commands</text>
</g>
<g>
<line x1="486" y1="72" x2="526" y2="72" stroke="#7c2d3a" stroke-width="2.5" marker-end="url(#lah)"/>
<rect x="530" y="34" width="212" height="76" rx="14" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="636" y="68" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="21" fill="#17181a">Verify</text>
<text x="636" y="93" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="14" fill="#6b6659">run tests or checks</text>
</g>
<g>
<path d="M636,110 L636,178 Q636,198 616,198 L144,198 Q124,198 124,178 L124,110" fill="none" stroke="#7c2d3a" stroke-width="2.5" stroke-dasharray="6 5" marker-end="url(#lah)"/>
<text x="380" y="226" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-style="italic" font-size="16" fill="#7c2d3a">repeat until the task is done</text>
</g>
</svg>

<p class="thread">You can interrupt at any point to steer it.</p>

Note: The agentic loop, verbatim from the doc: gather context, take action, verify results, repeating. Claude Code is the harness around the model, the tools and context that turn it into an agent. The diagram replaces the bullet list to cut the text.

---

<div class="lesson-no">Lesson 5.4 · What it can access</div>

# What it can reach

When you run `claude` in a folder, it can reach:

<svg class="diagram" viewBox="0 0 760 300" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="What Claude Code can access: project, terminal, git, memory, extensions">
<line x1="380" y1="150" x2="130" y2="50" stroke="#7c2d3a" stroke-width="1.5"/>
<line x1="380" y1="150" x2="630" y2="50" stroke="#7c2d3a" stroke-width="1.5"/>
<line x1="380" y1="150" x2="93" y2="150" stroke="#7c2d3a" stroke-width="1.5"/>
<line x1="380" y1="150" x2="667" y2="150" stroke="#7c2d3a" stroke-width="1.5"/>
<line x1="380" y1="150" x2="380" y2="254" stroke="#7c2d3a" stroke-width="1.5"/>
<g>
<rect x="44" y="24" width="172" height="52" rx="12" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="130" y="47" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="16" fill="#17181a">Your project</text>
<text x="130" y="65" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="12" fill="#6b6659">files &amp; folders</text>
</g>
<g>
<rect x="544" y="24" width="172" height="52" rx="12" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="630" y="47" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="16" fill="#17181a">Your terminal</text>
<text x="630" y="65" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="12" fill="#6b6659">any command</text>
</g>
<g>
<rect x="16" y="124" width="154" height="52" rx="12" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="93" y="147" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="16" fill="#17181a">Git</text>
<text x="93" y="165" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="12" fill="#6b6659">branch, history</text>
</g>
<g>
<rect x="590" y="124" width="154" height="52" rx="12" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="667" y="147" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="16" fill="#17181a">Memory</text>
<text x="667" y="165" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="12" fill="#6b6659">CLAUDE.md + auto</text>
</g>
<g>
<rect x="278" y="228" width="204" height="52" rx="12" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="380" y="251" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="16" fill="#17181a">Extensions</text>
<text x="380" y="269" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="12" fill="#6b6659">skills · MCP · subagents</text>
</g>
<rect x="308" y="120" width="144" height="60" rx="14" fill="#17181a"/>
<text x="380" y="156" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="18" fill="#f7f5f0">Claude Code</text>
</svg>

Note: From the doc's "What Claude can access." Because it sees the whole project, it can search, read many files, edit across them, and verify, not just autocomplete one line.

---

<div class="lesson-no">Lesson 5.4 · Extend it</div>

# Extend Claude Code

The built-in tools are the foundation. You add a layer on top:

- **Skills** package know-how it reuses
- **Subagents** offload work into their own space
- **Hooks** automate and enforce your rules
- **MCP** connect the tools outside it

<p class="thread">The rest of this module is that layer, one block at a time.</p>

Note: From the doc's "Extending the base capabilities." This is the bridge: the building blocks that follow are exactly these extensions.

---

<div class="lesson-no">Lesson 5.4 · Recap</div>

# Quick recap

- Claude works in a loop: gather context, take action, verify
- It can reach your project, terminal, git, memory, and any extensions
- Skills, subagents, hooks, and MCP extend what it can do

<div class="refs">
<a href="https://code.claude.com/docs/en/how-claude-code-works" target="_blank" rel="noopener"><span class="ref-src">Read more ·</span> How Claude Code works</a>
</div>

Note: Ten second reminder. Now the building blocks, starting with skills.

---

<!-- .slide: data-background-color="#17181a" class="dark" -->

<div class="lesson-no">Lesson 5.5</div>

## Skills

By the end of this lesson you will be able to:

- Explain what a skill is
- Write and load your own

Note: First building block. A skill is packaged know-how Claude reuses. Source: code.claude.com/docs/en/skills.

---

<div class="lesson-no">Lesson 5.5 · What it is</div>

# What a skill is

A skill is a reusable instruction file that Claude pulls in when a task needs it.

- It is a small markdown file, `SKILL.md`
- It holds a routine you would otherwise repeat
- Claude adds it to its toolkit, ready when it fits

Note: The plain definition. A skill is a saved routine, a review checklist, a house style, a debugging method, that Claude reuses instead of you re-typing it.

---

<div class="lesson-no">Lesson 5.5 · How it loads</div>

# How a skill loads

- **Automatic** Claude reads each skill's description and loads it when your task matches
- **Manual** or call it yourself by name, type `/name`
- **Cheap** only the description is loaded until the skill is actually used

<svg class="diagram" viewBox="0 0 760 92" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Your task matches a description, so the skill loads">
<defs><marker id="skah" markerWidth="9" markerHeight="9" refX="6.5" refY="3" orient="auto"><path d="M0,0 L7,3 L0,6 Z" fill="#7c2d3a"/></marker></defs>
<rect x="18" y="26" width="180" height="46" rx="10" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="108" y="54" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="16" fill="#17181a">your task</text>
<rect x="290" y="26" width="214" height="46" rx="10" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="397" y="54" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="16" fill="#17181a">a description</text>
<rect x="588" y="26" width="154" height="46" rx="10" fill="#17181a"/>
<text x="665" y="54" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="16" fill="#f7f5f0">it loads</text>
<line x1="198" y1="49" x2="286" y2="49" stroke="#7c2d3a" stroke-width="2.5" marker-end="url(#skah)"/>
<text x="242" y="40" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="11" fill="#6b6659">matches</text>
<line x1="504" y1="49" x2="586" y2="49" stroke="#7c2d3a" stroke-width="2.5" marker-end="url(#skah)"/>
<text x="545" y="40" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="11" fill="#6b6659">so</text>
</svg>

Note: The key idea: the description is the trigger. Claude matches your task to it and loads the skill on its own, no command needed. Descriptions are cheap; the full skill loads only when it fires.

---

<div class="lesson-no">Lesson 5.5 · In the wild</div>

# Skills people install

| Skill | What it does |
| --- | --- |
| superpowers | brainstorm, plan, test, debug |
| code-review | review the diff for bugs |
| code-simplifier | tighten and refactor code |
| pdf, docx, xlsx | read and create documents |
| frontend-design | build non-generic UI |

<p class="star">superpowers, github.com/obra/superpowers, is the pack most people install first</p>

Note: Real, popular skills, so it is concrete. superpowers and the dev skills are community favourites; pdf, docx, and xlsx are Anthropic's official document skills.

---

<div class="lesson-no">Lesson 5.5 · Write your own</div>

# Write your own skill

A skill is a folder with a `SKILL.md` inside. Save it in `.claude/skills/` for the project, or `~/.claude/skills/` for yourself.

<div class="filecard"><span class="fname">.claude/skills/review-pr/SKILL.md</span>
<span class="fbody"><span class="k">description:</span> Use when reviewing a pull request &nbsp;<span class="c"># the trigger</span><br><span class="k">allowed-tools:</span> Read, Bash &nbsp;<span class="c"># optional</span><br><br>Then your review steps, in plain markdown.</span>
</div>

- The `SKILL.md` file is all you need, `description` is what makes Claude auto-load it
- Everything else is optional: `allowed-tools`, `model`, `paths`
- Keep the `description` tight, it is capped at **1,536 characters**

Note: Skills are creatable, not magic. The details worth knowing: the description is truncated at 1,536 characters in the listing, so front-load the key use case. There is no cap on how many skills you can have. The folder name becomes the /command. A personal skill in ~/.claude overrides a project skill of the same name (enterprise beats personal beats project). The opening --- must be the file's first line, or the whole file is treated as content. Reference files and scripts can sit in the same folder.

---

<div class="lesson-no">Lesson 5.5 · Recap</div>

# Quick recap

- A skill is packaged know-how in a `SKILL.md` file
- Claude loads it automatically when the description matches, or you call it with `/name`
- Write your own by dropping a folder in `.claude/skills/`

<div class="refs">
<a href="https://code.claude.com/docs/en/skills" target="_blank" rel="noopener"><span class="ref-src">Read more ·</span> Agent Skills documentation</a>
</div>

Note: Ten second reminder. Next, when a job is bigger than a skill, you hand it to an agent.

---

<!-- .slide: data-background-color="#17181a" class="dark" -->

<div class="lesson-no">Lesson 5.6</div>

## Agents and subagents

By the end of this lesson you will be able to:

- Explain what a subagent is
- Know when to use one, a team, or a workflow

Note: Second building block. Where a skill is instructions, an agent is another Claude that does the job. Source: code.claude.com/docs/en/sub-agents.

---

<div class="lesson-no">Lesson 5.6 · What it is</div>

# What a subagent is

A subagent is another Claude that takes a job, works in its own space, and hands back just the result.

- It works on its own, you do not watch it
- It reports the answer, not the 40 files it read
- You choose its tools and its model

Note: The plain definition. A skill is instructions Claude follows. A subagent is another Claude that actually goes and does the work, in its own context window.

---

<div class="lesson-no">Lesson 5.6 · When to reach for one</div>

# When to reach for one

Use a subagent when a task would flood your main chat with work you do not need to watch.

- **Investigate** "how does our billing work?", it reads many files, returns a summary
- **Review** a fresh Claude checks your diff, with no bias from the build-up
- **Search** "which three files matter for checkout?", it digs, you get the shortlist

<p class="thread">The noisy work happens in its own context. Yours stays clean.</p>

Note: Three sharp cases, each distinct: investigate to learn, review to check, search to narrow down. The common thread is isolation: the side task never clutters your main conversation.

---

<div class="lesson-no">Lesson 5.6 · How they run</div>

# One, a team, or a workflow

<svg class="diagram" viewBox="0 0 760 216" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="One agent, a team, or a workflow">
<defs><marker id="wah" markerWidth="8" markerHeight="8" refX="6" refY="2.75" orient="auto"><path d="M0,0 L6.5,2.75 L0,5.5 Z" fill="#7c2d3a"/></marker></defs>
<line x1="253" y1="24" x2="253" y2="152" stroke="#e0dacb" stroke-width="1.5"/>
<line x1="507" y1="24" x2="507" y2="152" stroke="#e0dacb" stroke-width="1.5"/>
<circle cx="127" cy="84" r="34" fill="#7c2d3a"/>
<text x="127" y="90" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="15" fill="#f7f5f0">agent</text>
<text x="127" y="176" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="18" fill="#17181a">One agent</text>
<text x="127" y="199" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="13" fill="#6b6659">delegate one job</text>
<line x1="380" y1="52" x2="348" y2="112" stroke="#7c2d3a" stroke-width="1.6"/>
<line x1="380" y1="52" x2="412" y2="112" stroke="#7c2d3a" stroke-width="1.6"/>
<line x1="348" y1="112" x2="412" y2="112" stroke="#7c2d3a" stroke-width="1.6"/>
<circle cx="380" cy="52" r="23" fill="#7c2d3a"/>
<text x="380" y="56" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="10" fill="#f7f5f0">lead</text>
<circle cx="348" cy="112" r="21" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<circle cx="412" cy="112" r="21" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="380" y="176" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="18" fill="#17181a">A team</text>
<text x="380" y="199" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="13" fill="#6b6659">they talk &amp; share tasks</text>
<circle cx="588" cy="96" r="14" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<circle cx="633" cy="96" r="14" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<circle cx="678" cy="96" r="14" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<circle cx="633" cy="42" r="17" fill="#7c2d3a"/>
<circle cx="633" cy="134" r="16" fill="#7c2d3a"/>
<line x1="622.1" y1="55.1" x2="596.9" y2="85.2" stroke="#7c2d3a" stroke-width="1.8" marker-end="url(#wah)"/>
<line x1="633" y1="59" x2="633" y2="82" stroke="#7c2d3a" stroke-width="1.8" marker-end="url(#wah)"/>
<line x1="643.9" y1="55.1" x2="669.1" y2="85.2" stroke="#7c2d3a" stroke-width="1.8" marker-end="url(#wah)"/>
<line x1="598.7" y1="105" x2="620.8" y2="123.7" stroke="#7c2d3a" stroke-width="1.8" marker-end="url(#wah)"/>
<line x1="633" y1="110" x2="633" y2="117" stroke="#7c2d3a" stroke-width="1.8" marker-end="url(#wah)"/>
<line x1="667.3" y1="105" x2="645.2" y2="123.7" stroke="#7c2d3a" stroke-width="1.8" marker-end="url(#wah)"/>
<text x="633" y="45.5" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="9" fill="#f7f5f0">1 job</text>
<text x="633" y="137.5" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="9" fill="#f7f5f0">merge</text>
<text x="633" y="176" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="18" fill="#17181a">A workflow</text>
<text x="633" y="199" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="13" fill="#6b6659">fan out, then merge</text>
</svg>

<p class="thread">One to delegate. A team to collaborate. A workflow to fan out.</p>

Note: Three shapes with a concrete example each. One agent for a bounded side task, like a single code review. A team when work is open-ended and needs coordination, like building a feature together. A workflow when a known job splits across many helpers, like reviewing all 50 changed files at once, each helper takes one file and a checker merges.

---

<div class="lesson-no">Lesson 5.6 · Write your own</div>

# Write your own agent

An agent is a single `.md` file. Save it in `.claude/agents/` for the project, or `~/.claude/agents/` for yourself.

<div class="filecard"><span class="fname">.claude/agents/code-reviewer.md</span>
<span class="fbody"><span class="k">name:</span> code-reviewer &nbsp;<span class="c"># required</span><br><span class="k">description:</span> when Claude should use it &nbsp;<span class="c"># required</span><br><span class="k">tools:</span> Read, Grep &nbsp;<span class="o">·</span>&nbsp; <span class="k">model:</span> sonnet &nbsp;<span class="c"># optional</span><br><br>Body: the system prompt for this agent.</span>
</div>

- `name` and `description` are required, `tools` and `model` are optional
- Common ones: code-reviewer, test-writer, debugger, or run `/agents`

<p class="star">code-reviewer is the classic first agent, a fresh Claude that reviews your diff</p>

Note: Show agents are creatable. The body becomes the agent's system prompt, and it starts with fresh context. Only name and description are required; tools and model just narrow what it can touch.

---

<div class="lesson-no">Lesson 5.6 · Recap</div>

# Quick recap

- A subagent is another Claude that works in its own space and returns the result
- Use it to investigate, review, or search, keeping your main chat clean
- One to delegate, a team to collaborate, a workflow to fan out

<div class="refs">
<a href="https://code.claude.com/docs/en/sub-agents" target="_blank" rel="noopener"><span class="ref-src">Read more ·</span> Subagents documentation</a>
</div>

Note: Ten second reminder. Next, memory, how Claude remembers your project.

---

<!-- .slide: data-background-color="#17181a" class="dark" -->

<div class="lesson-no">Lesson 5.7</div>

## Memory

By the end of this lesson you will be able to:

- Name the two kinds of memory Claude uses
- Set up CLAUDE.md for your project

Note: Third building block. Two kinds: the memory you write, and the memory Claude keeps on its own. Source: code.claude.com/docs/en/memory.

---

<div class="lesson-no">Lesson 5.7 · Two kinds</div>

# Two kinds of memory

<svg class="diagram" viewBox="0 0 760 200" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Two kinds of memory: CLAUDE.md you write, auto-memory Claude writes">
<defs><marker id="sah" markerWidth="9" markerHeight="9" refX="6.5" refY="3" orient="auto"><path d="M0,0 L7,3 L0,6 Z" fill="#7c2d3a"/></marker></defs>
<line x1="380" y1="20" x2="380" y2="168" stroke="#e0dacb" stroke-width="1.5"/>
<rect x="150" y="26" width="100" height="36" rx="18" fill="#7c2d3a"/>
<text x="200" y="50" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="15" fill="#f7f5f0">You</text>
<line x1="200" y1="62" x2="200" y2="96" stroke="#7c2d3a" stroke-width="2.5" marker-end="url(#sah)"/>
<rect x="108" y="100" width="184" height="50" rx="10" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="200" y="123" text-anchor="middle" font-family="ui-monospace, Menlo, monospace" font-weight="700" font-size="15" fill="#17181a">CLAUDE.md</text>
<text x="200" y="141" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="11" fill="#6b6659">rules &amp; conventions</text>
<text x="200" y="182" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="12" fill="#6b6659">read every session</text>
<rect x="510" y="26" width="100" height="36" rx="18" fill="#7c2d3a"/>
<text x="560" y="50" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="15" fill="#f7f5f0">Claude</text>
<line x1="560" y1="62" x2="560" y2="96" stroke="#7c2d3a" stroke-width="2.5" marker-end="url(#sah)"/>
<rect x="468" y="100" width="184" height="50" rx="10" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="560" y="123" text-anchor="middle" font-family="ui-monospace, Menlo, monospace" font-weight="700" font-size="15" fill="#17181a">MEMORY.md</text>
<text x="560" y="141" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="11" fill="#6b6659">what it learns</text>
<text x="560" y="182" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="12" fill="#6b6659">saved for next time</text>
</svg>

<p class="thread">You write the rules. Claude writes what it learns.</p>

Note: The overview before the detail. Left, the memory you author. Right, the memory Claude keeps on its own. The next two slides take each in turn.

---

<div class="lesson-no">Lesson 5.7 · The memory you write</div>

# CLAUDE.md, the memory you write

CLAUDE.md is a file Claude reads every session. Put in it what you would tell a new teammate.

<div class="filecard"><span class="fname">CLAUDE.md</span>
<span class="fbody">Run the tests with <span class="k">npm test</span>.<br>Never touch files in <span class="k">/dist</span>, they are generated.<br>Use our logger, not <span class="k">console.log</span>.</span>
</div>

- `./CLAUDE.md` is shared with your team, `~/.claude/CLAUDE.md` is just yours
- Run `/init` and Claude drafts a first one from your code

<p class="star">the best CLAUDE.md is short, only what Claude cannot guess from the code</p>

Note: The memory under your control. The example makes it concrete: commands, no-go areas, house style. The project file is shared in git; the user file follows you everywhere.

---

<div class="lesson-no">Lesson 5.7 · The memory it keeps</div>

# The memory it keeps on its own

Claude also saves what it learns and reads it back next session, so you stop repeating yourself.

- It notes small facts, like "tests live in `/spec`" or "this repo uses pnpm"
- Each note is a file, gathered in a `MEMORY.md` index you can read
- Type `/memory` to see or edit everything it has saved

<p class="thread">Correct it once. It remembers next time.</p>

Note: Auto-memory. The difference from CLAUDE.md: you write CLAUDE.md, Claude writes this. Fix something today, and it saves that lesson for tomorrow instead of asking again. The detail: it loads the first 200 lines or 25 KB of MEMORY.md at the start of each session.

---

<div class="lesson-no">Lesson 5.7 · Recap</div>

# Quick recap

- CLAUDE.md is the memory you write, auto-memory is what Claude saves itself
- Write CLAUDE.md like notes for a new teammate, `/init` drafts a first one
- `/memory` opens everything, move a note into CLAUDE.md to share it

<div class="refs">
<a href="https://code.claude.com/docs/en/memory" target="_blank" rel="noopener"><span class="ref-src">Read more ·</span> Memory and CLAUDE.md</a>
</div>

Note: Ten second reminder. Next, hooks, making a rule something Claude cannot skip.

---

<!-- .slide: data-background-color="#17181a" class="dark" -->

<div class="lesson-no">Lesson 5.8</div>

## Hooks

By the end of this lesson you will be able to:

- Explain what a hook is
- Know when a hook beats a note in CLAUDE.md

Note: Fourth building block. A hook is automation that fires at fixed points in Claude's work. Source: code.claude.com/docs/en/hooks-guide.

---

<div class="lesson-no">Lesson 5.8 · What it is</div>

# What a hook is

A hook is a command Claude Code runs automatically at a set moment, like a git pre-commit hook, but for Claude's actions.

- Configured in `.claude/settings.json`
- Pick a moment, run any command
- It can even block an action before it happens

<div class="filecard"><span class="fname">.claude/settings.json</span>
<span class="fbody"><span class="k">PreToolUse</span> on <span class="k">Bash</span> &nbsp;<span class="o">&rarr;</span>&nbsp; run a check<br><span class="c"># exit non-zero, and the command is blocked</span></span>
</div>

Note: The mechanism. Where CLAUDE.md asks nicely, a hook runs code. A PreToolUse hook can inspect an action and stop it, for example blocking a dangerous delete.

---

<div class="lesson-no">Lesson 5.8 · When it fires</div>

# Moments you can hook

<svg class="diagram" viewBox="0 0 760 175" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Hook events across one turn: SessionStart, UserPromptSubmit, PreToolUse, PostToolUse, Stop">
<defs><marker id="tah" markerWidth="9" markerHeight="9" refX="6.5" refY="3" orient="auto"><path d="M0,0 L7,3 L0,6 Z" fill="#c9c2b4"/></marker></defs>
<line x1="40" y1="95" x2="716" y2="95" stroke="#c9c2b4" stroke-width="2" marker-end="url(#tah)"/>
<rect x="413" y="81" width="104" height="28" rx="6" fill="#fffdf9" stroke="#7c2d3a" stroke-width="1.5"/>
<text x="465" y="99" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="12" fill="#17181a">a tool runs</text>
<circle cx="95" cy="95" r="6" fill="#7c2d3a"/>
<circle cx="245" cy="95" r="6" fill="#7c2d3a"/>
<circle cx="388" cy="95" r="6" fill="#7c2d3a"/>
<circle cx="548" cy="95" r="6" fill="#7c2d3a"/>
<circle cx="690" cy="95" r="6" fill="#7c2d3a"/>
<text x="95" y="66" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="12" fill="#17181a">SessionStart</text>
<text x="245" y="66" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="12" fill="#17181a">UserPromptSubmit</text>
<text x="388" y="66" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="12" fill="#7c2d3a">PreToolUse</text>
<text x="548" y="66" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="12" fill="#7c2d3a">PostToolUse</text>
<text x="690" y="66" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="12" fill="#17181a">Stop</text>
<text x="95" y="128" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="11" fill="#6b6659">session opens</text>
<text x="245" y="128" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="11" fill="#6b6659">your prompt</text>
<text x="388" y="128" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="11" fill="#6b6659">before the tool</text>
<text x="548" y="128" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="11" fill="#6b6659">after the tool</text>
<text x="690" y="128" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="11" fill="#6b6659">turn ends</text>
</svg>

<p class="thread">CLAUDE.md is advice. A hook is a guarantee.</p>

Note: One turn, left to right, with the points a hook can fire. PreToolUse runs before a tool and can block it; PostToolUse runs after, for a formatter or tests. UserPromptSubmit fires on every prompt; SessionStart on open. The line to remember: advice can be ignored, a hook happens every time.

---

<div class="lesson-no">Lesson 5.8 · In practice</div>

# Hooks people set up

- **Auto-format** run Prettier after every file Claude writes
- **Block danger** stop a `rm -rf`, or a write to `/migrations`
- **Run tests** kick off the suite after each edit
- **Load context** pull in the latest notes at session start

<p class="star">auto-format after every edit is the hook almost everyone adds first</p>

Note: Concrete hooks people actually configure, one per common event, defined in `.claude/settings.json`. The detail: a command hook that exits with code 2 blocks the action outright. "Block writes to the migrations folder" is a common one straight from the docs.

---

<div class="lesson-no">Lesson 5.8 · Recap</div>

# Quick recap

- A hook runs a command automatically at a set point in Claude's work
- It can check, fix, or block, every single time, with no asking
- Reach for it when a rule you must never skip needs enforcing, not just advising

<div class="refs">
<a href="https://code.claude.com/docs/en/hooks-guide" target="_blank" rel="noopener"><span class="ref-src">Read more ·</span> Hooks guide</a>
</div>

Note: Ten second reminder. Next, MCP, how Claude reaches your real tools.

---

<!-- .slide: data-background-color="#17181a" class="dark" -->

<div class="lesson-no">Lesson 5.9</div>

## MCP

By the end of this lesson you will be able to:

- Explain what MCP does in plain words
- Tell an MCP server apart from a skill

Note: Fifth building block. MCP is the bridge from Claude to the tools outside it. Source: code.claude.com/docs/en/mcp.

---

<div class="lesson-no">Lesson 5.9 · What it is</div>

# How Claude reaches your tools

MCP is the bridge from Claude to the tools outside it, one server per tool, all listed in one `.mcp.json`.

<svg class="diagram" viewBox="0 0 760 166" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="MCP bridges Claude Code to GitHub, Postgres, and the browser">
<defs><marker id="mah" markerWidth="9" markerHeight="9" refX="6.5" refY="3" orient="auto"><path d="M0,0 L7,3 L0,6 Z" fill="#7c2d3a"/></marker></defs>
<rect x="20" y="62" width="160" height="50" rx="12" fill="#17181a"/>
<text x="100" y="92" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="16" fill="#f7f5f0">Claude Code</text>
<rect x="250" y="68" width="86" height="38" rx="19" fill="#7c2d3a"/>
<text x="293" y="92" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="15" fill="#f7f5f0">MCP</text>
<rect x="430" y="20" width="150" height="38" rx="10" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="505" y="44" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="15" fill="#17181a">GitHub</text>
<rect x="430" y="69" width="150" height="38" rx="10" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="505" y="93" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="15" fill="#17181a">Postgres</text>
<rect x="430" y="118" width="150" height="38" rx="10" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="505" y="142" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="15" fill="#17181a">Browser</text>
<line x1="180" y1="88" x2="246" y2="88" stroke="#7c2d3a" stroke-width="2.5" marker-end="url(#mah)"/>
<line x1="336" y1="86" x2="426" y2="42" stroke="#7c2d3a" stroke-width="2" marker-end="url(#mah)"/>
<line x1="336" y1="88" x2="426" y2="88" stroke="#7c2d3a" stroke-width="2" marker-end="url(#mah)"/>
<line x1="336" y1="90" x2="426" y2="134" stroke="#7c2d3a" stroke-width="2" marker-end="url(#mah)"/>
</svg>

<div class="promptcard"><span class="lbl">Add a server</span>

`claude mcp add`, then manage it in a session with `/mcp`

</div>

Note: The mechanism. Instead of pasting data in, Claude reads and acts on the real thing. Add a server once, share the .mcp.json with your team. The payoff, straight from the docs: "add the feature described in JIRA issue ENG-4521 and open a PR on GitHub."

---

<div class="lesson-no">Lesson 5.9 · The distinction</div>

# Skill vs MCP

- **A skill** is instructions Claude follows
- **An MCP server** is a tool Claude can actually use

<p class="thread">Instructions versus tools. That is the whole difference.</p>

Note: The one distinction to hold onto. A skill teaches Claude how; an MCP gives Claude something new to act on.

---

<div class="lesson-no">Lesson 5.9 · Servers people connect</div>

# Servers people connect

| Server | What it unlocks |
| --- | --- |
| GitHub | read PRs, open issues, search repos |
| Postgres | query your database directly |
| Playwright | drive a real browser, take screenshots |
| Sentry | pull live errors and releases |
| Figma | read designs and component specs |

<p class="star">GitHub is the server most teams connect first</p>

Note: Real servers so it is concrete. Each gives Claude a new set of actions. Browse the full list at the Anthropic directory, claude.ai/directory.

---

<div class="lesson-no">Lesson 5.9 · Recap</div>

# Quick recap

- MCP connects Claude to your real tools and data
- Add one with `claude mcp add`, manage with `/mcp`, share it in `.mcp.json`
- A skill is instructions to follow, an MCP is a tool to use

<div class="refs">
<a href="https://code.claude.com/docs/en/mcp" target="_blank" rel="noopener"><span class="ref-src">Read more ·</span> MCP documentation</a>
</div>

Note: Ten second reminder. Next, plugins, packaging your whole setup as one install.

---

<!-- .slide: data-background-color="#17181a" class="dark" -->

<div class="lesson-no">Lesson 5.10</div>

## Plugins

By the end of this lesson you will be able to:

- Explain what a plugin bundles
- Install one from a marketplace

Note: Sixth building block. A plugin is every block above, packaged as one install. Source: code.claude.com/docs/en/plugins.

---

<div class="lesson-no">Lesson 5.10 · What it is</div>

# One install, your whole setup

A plugin packages a setup you trust and installs it into any repo in one step.

<svg class="diagram" viewBox="0 0 760 178" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="One plugin bundles skills, agents, hooks, and MCP">
<rect x="208" y="20" width="344" height="126" rx="16" fill="#fbfaf6" stroke="#7c2d3a" stroke-width="2" stroke-dasharray="7 5"/>
<text x="380" y="44" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="14" fill="#7c2d3a">one plugin</text>
<rect x="240" y="58" width="130" height="34" rx="8" fill="#fffdf9" stroke="#7c2d3a" stroke-width="1.6"/>
<text x="305" y="80" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="15" fill="#17181a">skills</text>
<rect x="390" y="58" width="130" height="34" rx="8" fill="#fffdf9" stroke="#7c2d3a" stroke-width="1.6"/>
<text x="455" y="80" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="15" fill="#17181a">agents</text>
<rect x="240" y="100" width="130" height="34" rx="8" fill="#fffdf9" stroke="#7c2d3a" stroke-width="1.6"/>
<text x="305" y="122" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="15" fill="#17181a">hooks</text>
<rect x="390" y="100" width="130" height="34" rx="8" fill="#fffdf9" stroke="#7c2d3a" stroke-width="1.6"/>
<text x="455" y="122" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="15" fill="#17181a">MCP</text>
<text x="380" y="168" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="13" fill="#6b6659">install it once, your whole team gets all of it</text>
</svg>

<p class="thread">Your best setup, shipped to everyone.</p>

Note: The value. Everything you just learned, skills through MCP, can travel together as one unit instead of being rebuilt in every repo.

---

<div class="lesson-no">Lesson 5.10 · How to install</div>

# Install one in two steps

- Add a marketplace: `/plugin marketplace add <repo>`
- Install from it: `/plugin install <name>`
- Manage everything with `/plugin`

<p class="star">popular installs: the superpowers pack, and pr-review-toolkit for reviews</p>

Note: The workflow. A marketplace is just a repo of plugins. Add it once, then install what you need by name.

---

<div class="lesson-no">Lesson 5.10 · Recap</div>

# Quick recap

- A plugin bundles skills, agents, hooks, and MCP as one installable unit
- Add a marketplace, then `/plugin install` what you need
- Use it to give a whole team the same setup in one command

<div class="refs">
<a href="https://code.claude.com/docs/en/plugins" target="_blank" rel="noopener"><span class="ref-src">Read more ·</span> Plugins documentation</a>
</div>

Note: Ten second reminder. Next, loops, letting Claude run a task until it is done.

---

<!-- .slide: data-background-color="#17181a" class="dark" -->

<div class="lesson-no">Lesson 5.11</div>

## Loops

By the end of this lesson you will be able to:

- Use `/loop` to repeat a task until it is done
- Explain the Ralph loop and when it fits

Note: The pattern that runs Claude while you step away. One official, one from the community. Sources: code.claude.com/docs/en/scheduled-tasks and ghuntley.com/ralph.

---

<div class="lesson-no">Lesson 5.11 · The built-in loop</div>

# Let it run on a loop

`/loop` repeats a task on its own until a check passes.

<svg class="diagram" viewBox="0 0 780 200" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="The loop repeats until a check passes">
<defs><marker id="loah" markerWidth="9" markerHeight="9" refX="6.5" refY="3" orient="auto"><path d="M0,0 L7,3 L0,6 Z" fill="#7c2d3a"/></marker></defs>
<rect x="70" y="34" width="210" height="64" rx="14" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="175" y="72" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="19" fill="#17181a">Run the task</text>
<rect x="360" y="34" width="210" height="64" rx="14" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="465" y="72" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="19" fill="#17181a">Check it</text>
<rect x="628" y="42" width="104" height="48" rx="24" fill="#17181a"/>
<text x="680" y="72" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="17" fill="#f7f5f0">done</text>
<line x1="280" y1="66" x2="356" y2="66" stroke="#7c2d3a" stroke-width="2.5" marker-end="url(#loah)"/>
<line x1="570" y1="66" x2="624" y2="66" stroke="#7c2d3a" stroke-width="2.5" marker-end="url(#loah)"/>
<text x="597" y="52" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="12" fill="#6b6659">passes</text>
<path d="M465,98 L465,150 Q465,165 450,165 L190,165 Q175,165 175,150 L175,98" fill="none" stroke="#7c2d3a" stroke-width="2.5" stroke-dasharray="6 5" marker-end="url(#loah)"/>
<text x="320" y="188" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-style="italic" font-size="14" fill="#7c2d3a">fails, so it fixes and repeats</text>
</svg>

<div class="promptcard"><span class="lbl">In practice</span>

`/loop until the tests pass, fix what fails each round`

</div>

Note: The official, session-scoped loop. It keeps one conversation going and re-runs your instruction until the check passes, so you can walk away from a repetitive grind. Claude can pick its own interval, from a minute to an hour.

---

<div class="lesson-no">Lesson 5.11 · The Ralph loop</div>

# The Ralph loop

Geoffrey Huntley's community trick: run the same prompt in a fresh session, over and over, until a whole app is built, a CMS, a lead tracker, a booking system.

<svg class="diagram" viewBox="0 0 800 210" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="The Ralph loop: the same prompt runs in a fresh session each round until the app is built">
<defs><marker id="rah" markerWidth="9" markerHeight="9" refX="6.5" refY="3" orient="auto"><path d="M0,0 L7,3 L0,6 Z" fill="#7c2d3a"/></marker></defs>
<rect x="16" y="46" width="122" height="54" rx="10" fill="#fbfaf6" stroke="#7c2d3a" stroke-width="2"/>
<text x="77" y="70" text-anchor="middle" font-family="ui-monospace, Menlo, monospace" font-weight="700" font-size="14" fill="#17181a">PROMPT.md</text>
<text x="77" y="88" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="11" fill="#6b6659">same prompt</text>
<circle cx="255" cy="73" r="32" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="255" y="81" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="22" fill="#7c2d3a">1</text>
<circle cx="410" cy="73" r="32" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="410" y="81" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="22" fill="#7c2d3a">2</text>
<circle cx="565" cy="73" r="32" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="565" y="81" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="22" fill="#7c2d3a">3</text>
<rect x="688" y="50" width="98" height="46" rx="23" fill="#17181a"/>
<text x="737" y="78" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="14" fill="#f7f5f0">app built</text>
<line x1="138" y1="73" x2="219" y2="73" stroke="#7c2d3a" stroke-width="2.5" marker-end="url(#rah)"/>
<line x1="289" y1="73" x2="374" y2="73" stroke="#7c2d3a" stroke-width="2.5" stroke-dasharray="6 5" marker-end="url(#rah)"/>
<line x1="444" y1="73" x2="529" y2="73" stroke="#7c2d3a" stroke-width="2.5" stroke-dasharray="6 5" marker-end="url(#rah)"/>
<line x1="599" y1="73" x2="684" y2="73" stroke="#7c2d3a" stroke-width="2.5" marker-end="url(#rah)"/>
<text x="410" y="128" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-style="italic" font-size="13" fill="#6b6659">a fresh Claude each round</text>
<rect x="150" y="150" width="500" height="44" rx="10" fill="#f0ece2" stroke="#7c2d3a" stroke-width="1.5"/>
<text x="400" y="177" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="13" fill="#17181a">your files carry the state, each round reads and writes them</text>
</svg>

<p class="thread">`/loop` keeps one session going. Ralph starts fresh each round.</p>

Note: Flag it clearly as a community technique, not an official feature. The insight worth teaching: fresh context every round avoids a bloated conversation, and the files carry the state. You write a spec once, point Ralph at it, and it grinds through, session after session, overnight.

---

<div class="lesson-no">Lesson 5.11 · Recap</div>

# Quick recap

- `/loop` repeats a task within one session until a check passes
- The Ralph loop restarts fresh each round, using files as memory
- Reach for a loop when a job needs many patient rounds

<div class="refs">
<a href="https://code.claude.com/docs/en/scheduled-tasks" target="_blank" rel="noopener"><span class="ref-src">Read more ·</span> Scheduled tasks and /loop</a>
</div>

Note: Ten second reminder. Last building block, the commands you will actually use.

---

<!-- .slide: data-background-color="#17181a" class="dark" -->

<div class="lesson-no">Lesson 5.12</div>

## Commands

By the end of this lesson you will be able to:

- Use the commands that keep a session healthy
- Know the commands that set up your project

Note: A short, practical tour. Not every command, the handful you reach for daily. Source: code.claude.com/docs/en/sessions.

---

<div class="lesson-no">Lesson 5.12 · Keep it healthy</div>

# Commands for a healthy session

- `/clear` start fresh when the topic changes
- `/compact` shrink a long history, keep the thread
- `/context` see what is filling the window
- `/rewind` or Esc Esc, roll files back to a checkpoint

<svg class="diagram" viewBox="0 0 760 120" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="What fills the 200K context window">
<text x="380" y="18" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="12" fill="#6b6659">the 200K context window fills as you work</text>
<rect x="40" y="34" width="64" height="34" fill="#7c2d3a"/>
<rect x="104" y="34" width="86" height="34" fill="#9e4b57"/>
<rect x="190" y="34" width="176" height="34" fill="#b96f79"/>
<rect x="366" y="34" width="150" height="34" fill="#d29aa1"/>
<rect x="516" y="34" width="204" height="34" fill="#efe9df"/>
<rect x="40" y="34" width="680" height="34" rx="6" fill="none" stroke="#7c2d3a" stroke-width="2"/>
<text x="72" y="88" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="10" fill="#6b6659">system</text>
<text x="147" y="88" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="10" fill="#6b6659">memory</text>
<text x="278" y="88" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="10" fill="#6b6659">files read</text>
<text x="441" y="88" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="10" fill="#6b6659">tool output</text>
<text x="618" y="88" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="10" fill="#6b6659">free</text>
<text x="380" y="110" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-style="italic" font-size="13" fill="#7c2d3a">/clear empties it · /compact shrinks it</text>
</svg>

Note: The maintenance commands. The bar shows why a long chat drifts: system prompt, memory, every file read, and every tool output all fill the 200K window, and performance degrades as it fills. /clear empties it; /compact summarises it.

---

<div class="lesson-no">Lesson 5.12 · Set up and steer</div>

# Commands to set up and steer

- `/init` write a first CLAUDE.md from your code
- `/agents` `/mcp` `/plugin` manage your setup
- `/model` `/usage` pick a model, watch your limits
- `Shift+Tab` turn on plan mode before a big change

Note: The setup and steering commands. Note plan mode is a keyboard toggle, Shift+Tab, not a slash command. Together these are most of what you type.

---

<div class="lesson-no">Lesson 5.12 · Recap</div>

# Quick recap

- `/clear`, `/compact`, `/context`, `/rewind` keep a session clean
- `/init`, `/agents`, `/mcp`, `/plugin` set up your project
- Plan mode is `Shift+Tab`, not a command

<div class="refs">
<a href="https://code.claude.com/docs/en/sessions" target="_blank" rel="noopener"><span class="ref-src">Read more ·</span> Sessions and commands</a>
</div>

Note: Ten second reminder. That is every building block. Next, the habits that tie them together.

---

<!-- .slide: data-background-color="#17181a" class="dark" -->

<div class="lesson-no">Module 5 · Pro habits</div>

## Same tool, different results

By the end of this section you will be able to:

- Match each pain you feel to the right tool
- Adopt the habits that separate most people from the pros

Note: Section divider. The building blocks are only half of it. The other half is knowing when to reach for each one, and the working habits that make the difference.

---

<div class="lesson-no">Pro habits · The decision guide</div>

# When to reach for what

| You feel this | Reach for |
| --- | --- |
| Claude gets a convention wrong twice | add it to `CLAUDE.md` |
| You keep re-typing the same playbook | make a skill |
| You keep pasting in data Claude cannot reach | connect an MCP server |
| A side task floods your chat | run it in a subagent |
| You want it to happen every time | write a hook |
| Another repo needs the same setup | package a plugin |

Note: The single most useful slide in the module. Every feature fixes one specific pain. The signal you feel tells you which one to grab. Read a row, feel the pain, name the tool.

---

<div class="lesson-no">Pro habits · How people actually use it</div>

# Most people vs the pros

| Most people | The pros |
| --- | --- |
| Accept whatever it outputs | Read the diff, you own the code |
| Say "just build it" and hope | Let Claude interview you first |
| Take the first answer | Ask for options and the trade-offs |
| Ship without testing | Make it write tests and run them |
| Only the happy path | Name the edge cases up front |
| A vague one-line prompt | Give it the product context |

Note: Same tool, the whole gap is in the habits. This ties back to everything from Modules 3 and 4, applied to real code. Not new features, better working habits.

---

<div class="lesson-no">Module 5 · Where to go next</div>

# Take it further

<div class="refs">
<a href="https://code.claude.com/docs/en/overview" target="_blank" rel="noopener"><span class="ref-src">Official ·</span> Claude Code documentation</a>
<a href="https://code.claude.com/docs/en/best-practices" target="_blank" rel="noopener"><span class="ref-src">Official ·</span> Claude Code best practices</a>
<a href="https://academy.claude.com/courses/claude-code-101" target="_blank" rel="noopener"><span class="ref-src">Anthropic ·</span> Claude Code 101 (free course)</a>
<a href="https://github.com/anthropics/skills" target="_blank" rel="noopener"><span class="ref-src">Skills ·</span> Anthropic's official skills</a>
<a href="https://github.com/obra/superpowers" target="_blank" rel="noopener"><span class="ref-src">Skills ·</span> superpowers, a popular skill pack</a>
<a href="https://www.anthropic.com/engineering" target="_blank" rel="noopener"><span class="ref-src">Read ·</span> Anthropic engineering blog</a>
</div>

Note: One references slide to close. Official docs and the free course first, then the community skill packs and the engineering blog for how the team itself works. Links open in a new tab.

---

<div class="lesson-no">Module 5 · Recap</div>

# What you can do now

- Install Claude Code and drive it in your own project
- Move a change through explore, plan, implement, and commit
- Reach for the right building block for each job
- Give Claude a way to check its work on every run

<p class="thread">You do not use Claude Code. You drive it.</p>

Note: Module close. The through-line: the 4Ds you learned now run on your real project, wrapped in a setup you control. One line to remember, you drive it.
