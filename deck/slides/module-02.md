<!-- .slide: data-background-color="#17181a" class="dark" -->

<div class="mod-num">02</div>

### Module 2

## Claude's Toolkit

<span class="tag core">Core</span> For everyone · about 1 hour 20 min

Note: This module follows Anthropic's own Claude 101. You met Claude and had your first conversation in Module 1. Now the rest of the app: the tools you can turn on, then Projects, Artifacts, and Memory. Five lessons, each a recorded video with a title card, an exercise, and every prompt ready in the copy-paste doc (resources/module-01-copypaste.md). We do not teach the 4D framework here, that is all of Module 3.

---

<div class="lesson-no">Module 2 · What you will be able to do</div>

# By the end of this module

- Feed it files, choose the right model, and turn on the right tool
- Build a lasting Project with instructions and a knowledge base
- Build an Artifact, and set up Memory and a Style

Note: Module objectives, Anthropic style. Every claim here is an app skill, not a mindset. The mindset is Module 3.

---

<!-- .slide: data-background-color="#17181a" class="dark" -->

<div class="lesson-no">Lesson 2.1 · 18 min</div>

## Make Claude more powerful

By the end of this lesson you will be able to:

- Pick the right model, and set the effort
- Turn on web search and research
- Connect your apps, and use skills

Note: Lesson title card. Claude is not just the chat box. This is the tour of what you can turn on to make it far more capable. The hands-on setup for connectors, skills, and cowork comes in Module 4.

---

<div class="lesson-no">Lesson 2.1 · The basics</div>

# What is a model, or an LLM?

- A **model** is the engine behind Claude, it writes the reply
- **LLM** means large language model, trained on huge amounts of text
- It predicts language, it does not look answers up

Claude is the app. The model is what is thinking underneath it.

Note: One term to demystify before picking a model. Keep it plain and quick: engine, not search index. Sets up the next slide, where model becomes something to choose.

---

<div class="lesson-no">Lesson 2.1 · Your model</div>

# Pick the right model

| When you need | Pick |
| --- | --- |
| Speed on a quick, simple task | Haiku |
| The everyday default, for most work | Sonnet |
| Deep reasoning on a hard problem | Opus |
| A large, long, multi-step project | Fable |

Free gives you Haiku and Sonnet. Opus and Fable are on the paid plans. Start on the everyday model, and move up only when the task needs it.

Note: Verified 2026-08-17, current lineup Opus 5, Sonnet 5, Haiku 4.5, Fable 5. Capability ladder is Haiku, Sonnet, Opus, Fable, with Fable built for long, autonomous work. Re-verify version numbers before recording.

---

<div class="lesson-no">Lesson 2.1 · Tokens</div>

# What is a token?

A **token** is a small chunk of text, roughly three quarters of a word. Claude reads and writes in tokens.

"Claude is helpful" splits into 4 tokens: `Claude` `is` `help` `ful`.

More effort means more tokens spent thinking before you get a reply.

Note: Quick definition, not a deep dive. The split example makes it concrete, "helpful" breaking into "help" and "ful" is the aha moment, words are not always one token. Just enough so "effort" and "tokens" on the next slide make sense: higher effort burns more tokens per reply. Keep it to one breath.

---

<div class="lesson-no">Lesson 2.1 · Effort</div>

# Set the effort

Effort is how hard the model thinks before it answers.

| Effort | Good for | Example |
| --- | --- | --- |
| Low, Medium | Quick, simple tasks | "Fix this typo" |
| High (default) | Most everyday work | "Draft a reply to this email" |
| Extra high, Max | Hard reasoning, slower but deeper | "Debug why this script fails" |

High is already on by default, turn it up only for genuinely hard problems. The top levels are not on every model.

Note: Verified 2026-08-17. Five levels: Low, Medium, High, Extra high (xhigh), Max. Default is High. Extra high and Max are not on Haiku. Effort and thinking are separate settings, this replaced the old "extended thinking" toggle.

---

<div class="lesson-no">Lesson 2.1 · The toolbox</div>

# Turn on the right tool

A **tool** lets Claude step outside the chat to get what it does not already know.

| Tool | Gives you |
| --- | --- |
| Web search | Current facts, with links you can check |
| Research | A deep, cited report from many sources |

Research needs web search on, and is on the paid plans. For hard thinking with no web, just raise the effort.

<span class="demo">Demo</span>

Note: Web search for a quick current fact, research for a deep cited report. Hard reasoning is now the effort control, not a separate tool. UI placement of these toggles shifts, so verify before recording.

---

<div class="lesson-no">Lesson 2.1 · Connectors</div>

# Connect your apps

Connectors let Claude use the tools you already work in.

- **Google Calendar** "what is on my calendar next week?"
- **Gmail** "draft a reply to the latest email from my client"
- **Notion or Drive** "find our pricing doc and summarise it"
- **Custom** wire up your own tool with a custom connector

Claude reads your data, and with your permission, takes actions for you.

Note: Famous connectors: Google Calendar, Gmail, Notion, Google Drive, Slack, and many more, plus custom connectors built on the open MCP standard. Claude only sees what you can see. Deep setup and workflows are Module 4.

---

<div class="lesson-no">Lesson 2.1 · Skills and plugins</div>

# Skills and plugins

- **Skills** reusable expertise Claude loads for a task. Built-in skills make Excel sheets, slide decks, Word docs, and PDFs. You can build your own for a workflow you repeat
- **Plugins** ready-made bundles of skills and connectors for a kind of work, like sales or finance

Note: Skills are how-to packages Claude loads when relevant, the Office file creation is a skill. Custom skills codify your own workflow. Plugins bundle skills and connectors for a role. Deep dive in Module 4.

---

<div class="lesson-no">Lesson 2.1 · Your turn</div>

# Try it yourself

<p class="try"><b>Your turn</b> Turn on web search and ask Claude something that changed this week, then click a link to check it.</p>

<div class="uc-grid">
<div class="uc">Connect your calendar and ask what is coming up</div>
<div class="uc">Run Research for a short cited report</div>
<div class="uc">Ask for an Excel sheet or a slide deck</div>
<div class="uc">Raise the effort on one hard question</div>
</div>

Or try any tool on a task from your own week.

Note: Get them to turn a tool on and see the difference. In the script, run web search live and click a citation. Reflection to pose aloud: which tool will you use most? Prompts in the copy-paste doc.

---

<!-- .slide: data-background-color="#17181a" class="dark" -->

<div class="lesson-no">Lesson 2.2 · 18 min</div>

## Projects

By the end of this lesson you will be able to:

- Explain what a Project is and when to use one
- Set instructions and a knowledge base
- Build a reusable workspace

Note: Lesson title card with its objectives. Mirrors Claude 101 "introduction to projects". From here we build one thing all module: an exam prep workspace. Professionals build the same for a client or a job hunt.

---

<div class="lesson-no">Lesson 2.2 · Your workspace</div>

# A reusable workspace

- **What** one place for your instructions and files, for one thing you do again and again
- **Why** Claude keeps your context, so you never re-explain yourself
- **When** a course, a client, a job hunt, a research topic
- The rule people miss: chats in a Project do not share context, only the knowledge base does

Note: Faithful to Claude 101: Projects are self-contained workspaces with their own chats, knowledge base, and instructions. Foreground the "context is not shared unless it is in the knowledge base" rule, it is the most missed idea.

---

<div class="lesson-no">Lesson 2.2 · Set it up</div>

# Instructions and knowledge base

- **Instructions** tell Claude how to behave everywhere in the Project: tone, role, format
- **Knowledge base** holds the files Claude should always use
- Name your files clearly, Claude uses the names to find the right one
- As your files grow, Claude searches them for you automatically

<span class="demo">Demo</span>

Note: Claude 101's setup steps. Build it live: create the Project, paste a tutor instruction, upload the syllabus, then show the before and after. Descriptive file names matter. Full script in the copy-paste doc.

---

<div class="lesson-no">Lesson 2.2 · Your turn</div>

# Try it yourself

<p class="try"><b>Your turn</b> Create your own Project, write its instructions, and upload one real file.</p>

<div class="uc-grid">
<div class="uc">Exam prep, one Project per subject</div>
<div class="uc">A freelance client workspace</div>
<div class="uc">Your job hunt: CV, roles, and prep</div>
<div class="uc">A thesis or research workspace</div>
</div>

Note: They build their own Project now. The grid gives ideas for students and professionals. Prompts and instructions text in the copy-paste doc.

---

<!-- .slide: data-background-color="#17181a" class="dark" -->

<div class="lesson-no">Lesson 2.3 · 18 min</div>

## Artifacts

By the end of this lesson you will be able to:

- Explain what an Artifact is and when Claude makes one
- Build a usable tool with no code
- Share or publish what you make

Note: Lesson title card with its objectives. Mirrors Claude 101 "creating with artifacts". This Artifact goes into their exam prep Project.

---

<div class="lesson-no">Lesson 2.3 · What it is</div>

# Build it, do not just chat about it

- An Artifact is a standalone, usable output in a window beside the chat
- Claude makes one when the content is big, self contained, and something you will reuse
- Documents, web pages, charts, diagrams, and interactive tools
- Word, Excel, and PowerPoint come back as files you can download

Note: Faithful to Claude 101: Claude creates an artifact when content is significant and self contained, typically over fifteen lines, and something you will edit or reuse. Office files are file creation, not artifacts.

---

<div class="lesson-no">Lesson 2.3 · Build and share</div>

# From idea to shareable tool

- Just describe what you want, or say "put this in an artifact"
- Be specific, and say who it is for
- Change one thing at a time: "make the bar green", "save my data"
- **Publish** gives a link anyone can use, no account needed

<span class="demo">Demo</span>

Note: Claude 101's create-iterate-publish flow. Live build: ask for a study tracker, refine one step at a time, then publish. Only that version becomes public and it is not indexed by search engines. Full script in the copy-paste doc.

---

<div class="lesson-no">Lesson 2.3 · Your turn</div>

# Try it yourself

<p class="try"><b>Your turn</b> Build one small tool for yourself, then publish it and send the link to a friend.</p>

<div class="uc-grid">
<div class="uc">A flashcard app for revision</div>
<div class="uc">A budget or tip calculator</div>
<div class="uc">A one page resume</div>
<div class="uc">A quiz to test yourself</div>
</div>

Note: They build and publish their own Artifact. All no code, all in minutes. Example prompts in the copy-paste doc.

---

<!-- .slide: data-background-color="#17181a" class="dark" -->

<div class="lesson-no">Lesson 2.4 · 12 min</div>

## Memory and Styles

By the end of this lesson you will be able to:

- Understand how Claude's Memory works
- Save context so you never repeat yourself
- Set a Style for Claude's voice

Note: Lesson title card with its objectives. From Claude 101's personalizing content: Memory and Styles.

---

<div class="lesson-no">Lesson 2.4 · It remembers you</div>

# Memory, in three layers

- Claude saves key context: your role, preferences, and decisions
- Standalone chats share one memory
- Each Project has its own separate memory
- Incognito remembers nothing

<p class="try"><b>Your task</b> Say "Add to memory: I am preparing for finals, target 85 percent", then open Settings, Memory, and see it saved.</p>

Note: Faithful to Claude 101: Memory auto-saves context so you stop repeating yourself, and you can review or delete it in Settings. It is a set of structured entries, not a full transcript. Verify the round trip live before recording.

---

<div class="lesson-no">Lesson 2.4 · Its voice</div>

# Set a Style

- Pick a preset: concise, formal, or explanatory
- Or describe your own voice once
- Claude keeps that style across every chat

Reflect: what voice do you want Claude to use for your work?

Note: Styles is Memory's twin: Memory is what Claude knows about you, Styles is how it writes. Set it once, it applies everywhere.

---

<!-- .slide: data-background-color="#17181a" class="dark" -->

<div class="lesson-no">Lesson 2.5 · 12 min</div>

## Other ways to work with Claude

By the end of this lesson you will be able to:

- Use Claude in the browser and on a schedule
- Pick the right tool with a quick guide
- Answer the questions beginners ask

Note: Lesson title card with its objectives. Mirrors Claude 101's "other ways to work". Light touch, the deep automation is Module 4.

---

<div class="lesson-no">Lesson 2.5 · Beyond the chat box</div>

# Claude where you already work

- **Claude in Chrome** a side panel on any page: summarise, fill forms, take actions
- **Scheduled tasks** run a job on a schedule, in the cloud, even with your laptop closed
- Also in **Slack**, **Excel**, **Word**, and **PowerPoint**

<p class="try"><b>Try this</b> On a long article, open the Chrome side panel: "Summarise this page in five points I can revise from."</p>

Note: Claude in Chrome and scheduled tasks are paid and still in beta, use them on trusted sites and low-risk tasks. Deeper automation is Module 4, Cowork. Keep this a quick tour.

---

<div class="lesson-no">Lesson 2.5 · Work like a pro</div>

# Your quick decision guide

When a new task arrives:

- Something you do often? Make it a **Project**
- Need a usable tool or document? Ask for an **Artifact**
- On a web page? Use **Claude in Chrome**
- Quick and simple? Just ask

Note: A one glance cheat sheet for everything in this module. Have them run it on a real task from their week.

---

<div class="lesson-no">Lesson 2.5 · You might be wondering</div>

# Common questions

- **Is this free?** Most of it. The free plan has some limits, heavier use needs Pro
- **What about my data?** You control it in settings, and never paste secrets. More on this in Module 3
- **Is using it for my work honest?** Use it to draft and learn, then make it yours and be open about it
- **What if I lose a chat?** Your edits live under the version arrows, and Projects keep your work

Note: Answer the real questions in a beginner's head. Data safety is covered in depth in Module 3, keep it to one line here.

---

<div class="lesson-no">Module 2 · Recap</div>

# What you learned

- Your model and effort, and the tools you can turn on
- Projects, Artifacts, and Memory, the core of the app
- You set up a reusable workspace and built your own Artifact

Note: Recap of the whole toolkit before the project. Read it as a checklist of wins. Every item is an app skill, which is exactly what this module promised.

---

<!-- .slide: data-background-color="#17181a" class="dark" -->

### Module 2 project

## Finish your exam prep workspace

A Project with tutor instructions, your syllabus and past papers, Memory of your target, and the study tracker Artifact you built.

Note: The capstone pulls Modules 1 and 2 together. Professionals build the same for a client or a job hunt. Full brief in the exercises file.

---

<!-- .slide: data-background-color="#17181a" class="dark" -->

<div class="lesson-no">What is next</div>

## Coming up in Module 3

You can use Claude and the app. Next, the 4D Framework: how to work with AI so the results are reliable enough to depend on.

Note: Clean hand-off. Modules 1 and 2 taught the tool. Module 3 teaches the method, delegating, describing, judging, and verifying. Notice we did not teach the four habits here, so they land fresh next module.
