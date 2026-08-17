# Claude 101 — full current content (authoritative), captured 2026-08-17

The real, current Claude 101 course, pasted by the user from the live Claude tab. This is the primary blueprint. Rewrite in our own words for our course; never copy verbatim. Their structure:
- **Meet Claude:** What is Claude / Your first conversation / Getting better results / How you'll work on your desktop
- **Organizing your work:** Projects / Artifacts / Skills
- **Expanding Claude's reach:** Connectors / Enterprise Search / Research
- **Putting it all together:** Use-cases by role / Other ways to work with Claude
- **Conclusion & certificate**

Maps to OUR 6 modules: M1 Claude Essentials = Meet Claude + Projects + Artifacts + Memory + other-ways; M2 Prompt Engineering = getting-better-results deep; M3 Introduction to Cowork = Skills + Connectors + Research + desktop three-shapes; M4 Claude Code; M5 The Claude API; M6 Capstone.

---

## Lesson 1 — What is Claude? (signature assets)
- **Constitutional AI:** Claude is guided by principles to avoid toxic/discriminatory output and illegal/unethical help, and to be helpful, honest, harmless. Trained to align with human values and operate transparently.
- **More than a chatbot:** a reliable, predictable thinking partner for summarization, search, writing, Q&A, coding, and more.
- **Steerable and collaborative:** takes direction on personality, tone, behavior; less likely to produce harmful output; easier to steer.
- **Access on all plans** (Free/Pro/Max/Team/Enterprise); chats, projects, memory, preferences sync across web, desktop, mobile.
- **Capabilities:** writing/content; research/analysis (context window 200K+ tokens ~500 pages, up to 1M on paid supported models); coding (a top strength); problem-solving/reasoning with **Thinking** (answer instantly or reason step by step first); **Learning mode** (guides your reasoning instead of giving answers).
- **SIGNATURE INTERACTIVE — "Which of these needs a thinking partner?"** Six real requests, decide search box vs thinking partner:
  1. "What's the exchange rate from US dollars to euros today?" → **Search box** (nothing of yours in it).
  2. "Rewrite my update below so the delay reads as a decision, not an apology." (+ draft) → **Thinking partner**.
  3. "best structure for a quarterly business review presentation" → **Thinking partner**, but typed like a search you get ten generic templates; the real version: "Here's last quarter's review and the two slides leadership pushed back on. Restructure the story for this quarter."
  4. "I've pasted a customer's complaint thread below. Help me work out what they're actually asking for before I reply." → **Thinking partner** (no page to look up; reasoning + your correction).
  5. "What's the difference between a purchase order and an invoice?" → **Search box** as typed; becomes thinking-partner the moment your situation enters ("A vendor sent us an invoice with no PO...").
  6. "How many working days are there between March 3 and March 24?" → **Search box** (a calendar answers it; not every request needs a partner).
  Lesson: it is about whether YOUR context and judgement are in the request.
- **Ways to access:** Claude.ai (web/desktop/mobile, the course focus); Claude Code (agentic coding, file manipulation); @Claude in Slack; Claude Design (idea/sketch → interactive prototype); Claude for Microsoft 365 (Excel/PowerPoint/Word/Outlook sidebar).
- Reflection: which of your tasks would benefit from a thinking partner (ask Claude to scan your calendar).

## Lesson 2 — Your first conversation (signature assets)
- Talk to Claude **like a coworker**: naturally, concisely, conversationally.
- **PROMPT FRAMEWORK (rooted in Description, 4D):**
  1. **Set the stage** — your role, objectives, context.
  2. **Define the task** — the action you want (write, analyze, build...).
  3. **Specify rules** — style, tone, format, examples.
  - Worked example: "I'm the marketing lead at an indie streaming startup preparing a Series A pitch deck. Research the independent film streaming market — trends, competitor positioning, growth opportunities. Use current web research with citations, structured as a professional report up to 5 pages with an executive summary, market analysis, competitive landscape, and growth opportunities." (stage / task / rules labelled).
  - Framework is the 4D Framework for AI Fluency (Dakan, Ringling College; Feller, University College Cork): Delegation, Description, Discernment, Diligence.
- **Adding context:** uploads (PDF, DOCX, CSV, TXT, PNG, JPEG), connectors, custom preferences (Settings > General > personal preferences).
- **Iterating:** ask follow-ups; give feedback ("too formal, make it conversational"); redirect or restart; pencil icon to edit and resubmit a message.
- **Personalizing:** **Memory** (auto-saves role, preferences, decisions, working style; review/edit/delete in Settings; syncs) and **Styles** (concise/formal/explanatory or a custom style; applies across all chats).

## Lesson 3 — Getting better results (signature assets)
- **COMMON CHALLENGES TABLE (challenge → what's happening → try this):**
  - Too generic → not enough context → add audience/role/constraints (vague "Write an email about the project delay" vs the full enterprise-client version).
  - Too long/short → Claude guessing length → be explicit ("two-paragraph summary", "under 100 words").
  - Wrong format → understood what, not how → show an example or describe structure ("bullet points with bold headers").
  - Confident but wrong → plausible but incorrect on niche facts → verify high-stakes facts, ask for sources/confidence, enable web search.
  - Wrong tone → defaults to professional → describe tone plainly, give an example.
- **Iteration mindset:** first draft = starting point; give specific feedback ("cut the first two paragraphs, make the conclusion action-oriented"); know when to start fresh.
- **AI Fluency + full 4D definitions** (Delegation/Description/Discernment/Diligence).
- **EVALS (lightweight):** gather 5-10 real examples of a task → write test prompts with natural context → compare Claude's output to yours (captures key info? tone right? what's missing?) → refine prompts/add examples/flag where human review is essential. Rooted in Discernment.

## Lesson 4 — How you'll work with Claude on your desktop (signature framing)
- **THREE SHAPES OF WORK** (the whole skill = knowing which you're in):
  1. **Turn by turn (Chat)** — you and Claude go back and forth; value is in the exchange. Reach for it when the answer changes what you ask next, you want to stay in it, or it's quick.
  2. **Handing work off (Cowork)** — describe an outcome; Claude plans, does it, returns the finished deliverable; you review the plan and output. Reach for it for multi-step tasks, real deliverables (doc/sheet/deck/PDF), work spanning your tools, or scheduled/background work.
  3. **Building software (Claude Code)** — Claude works in your codebase; developer workspace.
- In the product today: Chat (quick entry double-tap Option, screenshots, dictation, desktop connectors); Cowork (local folder access, scheduled tasks, subagents, projects, browser use, computer use, plugins — Pro/Max/Team/Enterprise); Code tab (Local or Cloud, approval modes).
- Decision table: ask/brainstorm/draft → Chat; multi-step ending in a deliverable / spans tools / scheduled → Cowork; write-test-ship code → Code tab.

## Organizing — Projects (matches our 1.6)
- Self-contained workspaces with own memory, chat histories, knowledge bases, custom instructions.
- Knowledge base = upload docs Claude references across all chats (no re-uploading).
- Instructions guide behavior (tone, expertise, style, format) for every chat; can automate ("when I upload a transcript, summarize with this template").
- Scales via **RAG** (searches files when knowledge nears context limit, up to 10x capacity).
- Team/Enterprise sharing: permission levels **Can view / Can edit / Owner**.
- Best practices: start focused; keep knowledge current; write clear instructions; name files descriptively ("Q4-2025-Sales-Report.pdf"); reference documents by name.
- Example projects: Q4 launch, research support, client hub, event planning, job-description generator.

## Organizing — Artifacts (matches our 1.7)
- Standalone, interactive outputs in a dedicated window. Auto-created when content is significant/self-contained (typically over 15 lines), likely to edit/reuse, stands on its own, or you'll reference later.
- Types: documents (markdown/text), code snippets, HTML pages, SVG images, Mermaid diagrams, React components. Word/Excel/PPT/PDF come via **file creation**, not artifacts (returned as downloadable files).
- Create by describing it; ask "create this as an artifact" if it doesn't. Toggle preview/code, copy, download.
- Sharing: copy/download; share within org (Team/Enterprise); **publish publicly** (Free/Pro/Max) — only the selected version is public, chat stays private, no Claude account needed to view, not indexed by search engines, unpublish anytime.
- Tips: be specific; describe the end user; iterate one change at a time; request an artifact when needed.

## Organizing — Skills (our M3)
- Folders of instructions, scripts, resources Claude loads dynamically = expertise packages. Powers Excel/PPT/Word/PDF creation. Anthropic Skills (auto, all paid) vs Custom Skills (yours).
- Enable: Settings > Capabilities > Code execution and file creation on > toggle Skills. Preview on Pro/Max/Team/Enterprise.
- Create a custom Skill by conversation: tell Claude what to create → answer its interview → upload reference materials → save; appears under Customize. Security: only install custom skills from trusted sources.
- **Skills vs Projects:** projects STORE knowledge (the what), skills PERFORM tasks (the how). A skill can reference a project's knowledge.

## Expanding — Connectors (our M3)
- Give Claude access to your everyday tools/data; read info and perform actions (search files, retrieve docs, update records) with the permissions you grant.
- **MCP = "USB-C for AI"** — one universal standard so any tool can connect. Two types: web connectors (Google Drive, Notion, Slack, Asana, Linear, Stripe...) and desktop extensions (local files, browser control, Figma).
- Setup web connector: claude.ai/directory or + > Connectors → Connect → authenticate → grant permissions → test. Security: scoped access; Claude sees only what you see; revocable anytime; only trusted sources.
- **TRY-IT interactive:** a one-sentence request ("Draft a short status update on the budget project for my manager") grows as you turn on Cloud storage / Email / Team chat — each connection lets you ask for something outside your message.

## Expanding — Research (our M3)
- Agentic multi-source investigation: plans (with Thinking) → many searches that build on each other (hundreds of sources) → synthesizes → cites. Takes minutes.
- Use for comprehensive reports, comparative analysis, deep investigations with verifiable citations. Web search must be enabled.
- vs web search (quick fact, 1-2 sources), vs Thinking (reasoning, no external info), vs enterprise search (your org's internal knowledge).
- **ROUTING interactive:** "Research / Quick web search / Thinking / Enterprise search — where would you send it?"
- Prompt tips: be specific about goals; specify sections/structure; include constraints; ask Claude to refine your research prompt. Pairs with Google Workspace integrations.

## Putting it together — Use-cases by role (our M1 other-ways / M6)
- General: project status reports, analyze feedback patterns, package brand guidelines as a skill.
- By role: Sales (battle cards, deal prep, sales reports); Marketing (campaign analysis, cross-platform content); Finance (models, investment memos, inherited spreadsheets); HR (onboarding guides); Legal (discovery timelines); Research (literature review, verify statistics). Source: claude.com Use Case Gallery.

## Putting it together — Other ways to work with Claude (our M1 1.9)
- **Claude Code** (agentic coding in terminal/IDE/browser/Slack), **@Claude** (Slack), **Claude Design** (idea/sketch → prototype), **Claude for Microsoft 365** (Excel/PowerPoint/Word/Outlook sidebars, Outlook in beta), **Claude in Chrome** (browser sidebar, observes and acts; public beta, low-risk trusted sites, asks before high-risk actions, blocks financial/adult sites).
- Summary table: Claude.ai (general), Claude Code (dev), Claude Cowork (multi-step tasks), @Claude (Slack), Claude Design (UI), Claude for M365 (edit in place), Claude in Chrome (browser).

## Devices we should adopt across OUR course
- The "search box vs thinking partner" interactive (M1 opener).
- The set-stage / define-task / specify-rules prompt framework (M1 taste, M2 core).
- The common-challenges troubleshooting table (M2).
- The three-shapes-of-work framing Chat/Cowork/Code (M1 map + M3/M4 openers).
- Evals as a Discernment habit (M2).
- Skills-vs-Projects "store knowledge vs perform tasks" line (M3).
- MCP = USB-C for AI (M3).
- Research vs web-search vs Thinking vs enterprise-search routing (M3).
- Per-lesson: estimated time, learning objectives ("by the end you'll be able to..."), key takeaways, reflection, what's next.
