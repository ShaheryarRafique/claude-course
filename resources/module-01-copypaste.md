# Module 1 — Copy-paste pack

Paste this whole file into a Google Doc. While recording, copy each **PROMPT** block straight into Claude. Everything a student needs is a real, ready task. Running example: a student's exam prep. The professional or business owner does the same with a client or their own work.

How to read this: each lesson has the demo prompts you run on screen, the student task, and the follow-up prompts to refine.

---

## Access links (share with students)

- Web: https://claude.ai/login
- Desktop (Mac and Windows): https://claude.com/download
- Android: https://play.google.com/store/apps/details?id=com.anthropic.claude&hl=en
- iPhone and iPad: https://apps.apple.com/us/app/claude-by-anthropic/id6473753684

---

## Lesson 1.1 — What is Claude?

**Search box vs assistant (the reframe):** a search box answers one query and forgets; an assistant works through a whole task with you, remembers your context and files, and takes direction.

**Interactive (three examples, say the why on each):**
1. "Capital of Japan?" = search box. A plain fact, nothing of yours is in it.
2. "Rewrite my update so the delay reads as a decision, not an apology" = assistant job. It needs your draft and your judgement.
3. "Best structure for a quarterly review deck?" = looks like a search, but an assistant job the moment your own slides and goals go in. (This is the teaching moment.)

**Student task — find your first tasks. PROMPT:**
> Act as my assistant, not a search box. Here is what my week looks like: [paste your to-do list, or your class and assignment schedule]. Suggest three tasks where working with you would save me real time, and for each one say in a line why it needs an assistant and not just a quick search.

---

## Lesson 1.2 — Your first conversation

**Setup:** claude.ai, Sign up with Google, Apple, or email. No card. Install the desktop and mobile app, sign in, show the sync.

**Talk like a coworker, two examples to type live:**
> How do I hang a picture frame on a concrete wall?

> Plan my exam revision for the next seven days.

**The technique (set the stage, task, rules). PROMPT:**
> I am a final year student preparing for my finals. Turn my syllabus into a seven day revision plan. Keep it to one page, one topic per day, in plain language, with a short daily goal.

One running example: a thoughtful birthday gift, made personal by attaching your notes.

**Beat 1 — write a good prompt (build it live from the three parts). PROMPT:**
> I need a birthday gift for my sister who loves painting. Suggest five options I can buy locally, around fifty dollars, with a reason for each.

**Beat 2 — run it.** Send the prompt and read the five ideas together.

**Beat 3 — give it a file.** Drag in a short note of things she has mentioned (a text or Word file), then:
> Here are my notes about her. Use these hints to make the ideas more personal, and drop anything that does not fit.

**Beat 4 — follow up, to show iteration. PROMPT:**
> Which of these can I buy today, and where should I look?

(Alternative document demos for the later data lessons: `resources/sample-data/store-sales-2024.csv`, or a financial report PDF.)

**First-conversation tasks (pick one, single chat, quick win, from Anthropic's use-case gallery). PROMPTS:**
> Write a short, polite leave email to my manager for two days off next week.

> Write a cover letter for this job in simple, confident English: [paste the job ad]

> Explain how loans and interest actually work, simply, with one everyday example.

> Plan a one day trip to [city] on a small budget, with times, cheap food, and total cost.

> Suggest a thoughtful gift for someone who loves art, within my budget, available near me.

> Summarise these notes into five points I can revise from: [paste notes]

> Act as an interviewer for a data analyst role. Ask me one question at a time, and give feedback after each.

> Plan a birthday party for 15 people on a small budget: theme, food, and a simple timeline.

With a file attached (practise the upload):
> Summarise this document in five points I can act on. [attach a PDF or Word file]

> I have attached a report. Give me the three things I should know, and one thing to check. [attach a file]

> Here is a meeting transcript. Turn it into clear action items with an owner for each. [attach or paste the transcript]

**Files:** drag in a PDF, then:
> Read this and give me the five most important points.

---

## Lesson 1.3 — Getting better results

**The five fixes (quick reference):**
1. Too generic = add audience, role, constraints.
2. Too long or short = state the length.
3. Wrong format = show an example or describe the structure.
4. Confident but wrong = ask for sources, verify what matters.
5. Wrong tone = name the tone or paste a sample.

**"Instead of this, try this" — run the weak one, then the better one, for one or two of these:**

1. Instead of: "Write about the delay"
   Try: "Email our client that the launch slips two weeks, apologetic, under 120 words, with a new date"
2. Instead of: "Summarise this report"
   Try: "Summarise this report in five bullets, a bold header for each section"
3. Instead of: "Give me some ideas"
   Try: "As a marketer, give me five campaign ideas for students, each in one line"
4. Instead of: "Make it sound better"
   Try: "Rewrite this warm and confident, matching this sample: [paste a sample]"

**Student task. PROMPT pattern:**
> Here is a reply from you I was not happy with: [paste]. Improve it using this one change: [make it shorter / change the tone to friendly / put it in bullet points]. Do not start over.

---

## Lesson 1.4 — Make Claude more powerful

**Models (verified 2026-08-17, re-verify before recording):** Haiku (fast, simple), Sonnet (everyday default), Opus (deep reasoning), Fable (large, long, autonomous projects). Free = Haiku + Sonnet; Opus + Fable need a paid plan. **Effort levels:** Low, Medium, High (default), Extra high, Max. **Tools:** Web search (current facts + links), Research (deep cited report, paid plans, needs web search on). **Power-ups:** Connectors (Google Calendar, Gmail, Notion, Drive, Slack, + custom), Skills (Office file creation + custom workflows), Plugins (role bundles). Deep dive in Module 3.

**Web search demo. PROMPT (turn on web search first):**
> Search the web for the latest news on [topic] this week, and give me three points with a link for each.

**Research demo (optional, takes a few minutes). PROMPT (turn on Research):**
> Research [a question you care about] and give me a short, cited report with the key findings.

---

## Lesson 1.5 — Projects

**Create the Project:** New Project, name it "Final Exam Prep", short description.

**Project instructions (paste into the Instructions box):**
> You are my exam tutor for my final year. Always explain in simple language with short examples. When I ask about a topic, base your answer on the files in this project first. If something will likely be on the exam, say so. Keep answers concise and give me one practice question at the end.

**Knowledge base:** upload the syllabus and any past papers. Name files clearly, for example "Syllabus-2026.pdf" and "Past-Paper-2024.pdf".

**First prompt inside the Project. PROMPT:**
> From my syllabus, list the ten topics most likely to appear on the exam, and quote the line from the syllabus that supports each one.

**Student task. PROMPT:**
> Here is my [subject]. Create project instructions for a tutor that explains simply and always uses my uploaded notes. Then I will paste them into the Instructions box.

---

## Lesson 1.6 — Artifacts

**Study tracker build. PROMPT (the trick is to ask for a React artifact in a single file):**
> Build me a study tracker as a React artifact in a single file. I can add subjects, mark topics as done, and see how many are left. Keep the design clean and simple.

**Refine, one change at a time. PROMPTS:**
> Add a progress bar at the top that fills as I complete topics.

> Save my data so it is still there when I reopen it.

> Make the finished topics show in green.

**Publish:** click Publish or Share, copy the link, send it to a student.

**Student task options. PROMPTS:**
> Build a flashcard app as a React artifact in a single file, where I type a question and answer and can flip through them.

> Build a simple budget calculator as a single-file artifact where I enter income and expenses and see what is left.

> Build a one page resume from these details: [paste].

---

## Lesson 1.7 — Memory and Styles

**Add to memory. PROMPT:**
> Add to memory: I am preparing for my finals and my target is 85 percent.

Then open Settings, Memory, and show it saved.

**Verify in a new chat. PROMPT (open a fresh chat):**
> What am I working towards right now?

**Set a Style:** Settings, choose Concise or Explanatory, or:
> From now on, write in a friendly, simple style with short sentences and no jargon.

---

## Lesson 1.8 — Other ways to work with Claude

**Claude in Chrome. PROMPT (on a long article, side panel):**
> Summarise this page in five points I can revise from.

**Scheduled task. PROMPT:**
> Every morning at 8am, give me a five point brief on [my subject] and one thing to revise today.

**Decision guide (say aloud):** do it often = Project. Need a tool or document = Artifact. On a web page = Claude in Chrome. Quick and simple = just ask.
