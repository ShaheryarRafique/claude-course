# Module 2, Lesson 2.1 — Recording Script (read aloud)

Covers slides `#/25`–`#/35`: the Module 2 title card and objectives, then all of Lesson 2.1, "Make Claude more powerful." Read this straight through while recording. Copy every PROMPT block below into Claude on screen. Re-verify prices, model names, effort levels, and free-vs-paid access on claude.com/pricing the same day you record — these are the fastest-drifting facts in the whole deck (see the slide notes for the 2026-08-31 fact-check).

Note to presenter: this lesson is dense — six new concepts (model, token, effort, tools, connectors, skills/plugins) plus one live demo plus a four-option exercise, inside a title card that claims 18 minutes. Do not rush the demo to protect the clock. If you are consistently running past 20 minutes, cut the exercise walkthrough short on screen and let students do it at their own pace instead of narrating all four options.

---

## Module 2 title card — Claude's Toolkit

Hook: You met Claude and had your first conversation in Module 1. Now let's open up the rest of the app.

Talking points:
- This module is the tour of everything you can turn on: the right model, the right tool, then Projects, Artifacts, and Memory.
- Five short lessons, each with a demo and a hands-on exercise.
- We are not teaching the 4D framework yet, that mindset is all of Module 3. This module is pure app skills.

Close: Let's start with what's actually thinking underneath Claude.

---

## Module 2 objectives — By the end of this module

Hook: Here is exactly what you'll be able to do by the end of this module.

Talking points:
- You'll feed it files, choose the right model, and turn on the right tool for the job.
- You'll build a lasting Project with instructions and a knowledge base.
- You'll build an Artifact, and set up Memory and a Style.

Close: Let's get into it, starting with the model itself.

---

## Lesson 2.1 slide 1 — Make Claude more powerful (title card)

Hook: Claude is not just the chat box. In the next twenty minutes you'll see everything you can turn on to make it far more capable.

Talking points:
- You'll pick the right model, and set the effort.
- You'll turn on web search and research.
- You'll connect your apps, and use skills.
- The hands-on setup for connectors and skills comes later, this is the tour.

Close: Let's demystify one word first: model.

---

## Lesson 2.1 slide 2 — What is a model, or an LLM?

Hook: Before you pick a model, you need to know what it actually is.

Talking points:
- A model is the engine behind Claude, it's what writes the reply.
- LLM means large language model, trained on huge amounts of text.
- It predicts language one piece at a time, it does not look answers up like a search engine.
- Claude is the app you use. The model is the engine running underneath it.

Close: Now that you know what a model is, let's pick one.

---

## Lesson 2.1 slide 3 — Pick the right model

Hook: You don't need to memorise version numbers, think in tiers.

Talking points:
- Haiku: speed, for a quick, simple task.
- Sonnet: the everyday default, for most work.
- Opus: deep reasoning, for a hard problem.
- Fable: a large, long, multi-step project, the one built to run for a long time on its own.
- Free access is lighter across every model, not locked to just Haiku and Sonnet. Paid plans raise your usage limits and give priority access to Opus and Fable, worth it for something like a multi-week research project (verify current pricing before recording, this claim drifts fastest).

Close: Once you've picked a model, the next lever is how hard it thinks. But first, one more word: token.

---

## Lesson 2.1 slide 4 — What is a token?

Hook: You'll hear "token" a lot, here's the one-breath definition.

Talking points:
- A token is a small chunk of text, roughly three quarters of a word.
- Claude reads and writes in tokens, not whole words.
- Show the example on screen: "Claude is helpful" splits into four tokens, Claude / is / help / ful. The aha moment is that "helpful" itself splits in two.

Close: Hold that thought, because effort is what controls how many tokens Claude spends thinking.

---

## Lesson 2.1 slide 5 — Set the effort

Hook: Effort is how hard the model thinks before it answers, and it's a dial, not an on/off switch.

Talking points:
- Low or Medium: quick, simple tasks, like "fix this typo."
- High, the default: most everyday work, like "draft a reply to this email."
- Extra high or Max: hard reasoning, slower but deeper, like "debug why this script fails."
- More effort means more tokens spent thinking before you get a reply, so raise it only when a problem genuinely needs the depth.
- One correction to make out loud if a student asks: Haiku doesn't support effort levels at all, effort is a Sonnet, Opus, and Fable setting (verify before recording).

Close: Effort controls how hard Claude thinks. Now let's give it something to think with.

---

## Lesson 2.1 slide 6 — Turn on the right tool

Hook: A tool lets Claude step outside the chat to get what it doesn't already know.

Talking points:
- Web search: current facts, with links you can check yourself.
- Research: a deep, cited report pulled from many sources. It needs web search turned on, and is on paid plans.
- If you need hard thinking with no web involved, that's not a tool question, just raise the effort instead.

[DEMO] Turn on web search live and run:
[PROMPT]
Search the web for the latest news on [topic] this week, and give me three points with a link for each.
- Click one of the citation links on screen so students see it's a real, checkable source, not a guess.

[DEMO] (Optional, takes a few minutes) Turn on Research and run:
[PROMPT]
Research [a question you care about] and give me a short, cited report with the key findings.

Close: Now let's connect Claude to the apps you already use.

---

## Lesson 2.1 slide 7 — Connect your apps

Hook: Connectors let Claude use the tools you already work in, instead of you copying things back and forth.

Talking points:
- Google Calendar: "what is on my calendar next week?"
- Gmail: "draft a reply to the latest email from my client."
- Notion or Drive: "find our pricing doc and summarise it."
- Custom: wire up your own tool with a custom connector.
- Say this clearly, it's the question every nervous beginner has: you approve access when you connect an app, Claude only ever sees what you can see, and it checks with you before doing anything that changes something.

Close: Connectors give Claude your apps. Skills give it expertise.

---

## Lesson 2.1 slide 8 — Skills and plugins

Hook: A skill is expertise Claude loads automatically the moment it's relevant.

Talking points:
- Ask for "a slide deck from this outline" and the built-in Slides skill fires on its own. Same idea for Excel, Word, and PDFs.
- You can build your own skill for a workflow you repeat often.
- Plugins bundle skills and connectors together for a kind of work, like sales outreach or finance reporting.

Close: You now know the full toolkit. Let's put it to work.

---

## Lesson 2.1 slide 9 — Try it yourself

Hook: Your turn. Pick one tool from this lesson and actually use it.

[EXERCISE] [PAUSE] Turn on web search and ask Claude something that changed this week, then click a link to check it yourself. That's the one to lead with on screen.

Other options if you want to go further (name these but don't demo all of them live):
- Connect your calendar and ask what's coming up.
- Run Research for a short cited report.
- Ask for an Excel sheet or a slide deck.
- Raise the effort on one genuinely hard question.

Reflection to pose aloud: which of these tools will you actually reach for this week?

Close: You've made Claude more powerful. Next, let's give it a permanent home: Projects.
