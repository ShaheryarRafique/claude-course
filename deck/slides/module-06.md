<!-- .slide: data-background-color="#17181a" class="dark" -->

<div class="mod-num">06</div>

### Module 6

## Claude Design

<span class="tag core">Core</span> You are the designer, start to finish.

Note: The reframe. Most people think design needs Figma, Canva, or a designer on call. Here you describe the visual, Claude builds a first version, and you shape it until it is yours. Built on Anthropic's own material: the Claude Design help guides, Claude 101's artifacts lesson, and the Academy tutorial on decks. Two lessons: make a design, then make it on brand and ship it.

---

<div class="lesson-no">Module 6 · What you will be able to do</div>

# By the end of this module

- Describe a design and get a strong first draft
- Refine it with chat, comments, and direct edits
- Keep every design on brand with a design system
- Turn it into a deck or code, then share and export it

Note: Module outcomes. The first two are Lesson 6.1, the last two are Lesson 6.2. On screen we keep the gym from Module 4, so students see one project grow.

---

<!-- .slide: data-background-color="#17181a" class="dark" -->

<div class="lesson-no">Lesson 6.1</div>

## Your first design

By the end of this lesson you will be able to:

- Write a design prompt that gets a strong first draft
- Refine it like a designer

Note: The make-something lesson. Callback to Module 2's Artifacts lesson: that was a plain artifact, a tool. Claude Design is a template for a deliverable, with a canvas you can edit. Source: support.claude.com, Get started with Claude Design.

---

<div class="lesson-no">Lesson 6.1 · What it is</div>

# A conversation, plus a canvas

<svg class="diagram" viewBox="0 0 760 170" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="You describe in the chat, Claude builds on the canvas, you refine">
<defs><marker id="dah" markerWidth="9" markerHeight="9" refX="6.5" refY="3" orient="auto"><path d="M0,0 L7,3 L0,6 Z" fill="#7c2d3a"/></marker></defs>
<rect x="40" y="22" width="230" height="126" rx="14" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="155" y="54" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="19" fill="#17181a">Conversation</text>
<rect x="66" y="72" width="150" height="20" rx="10" fill="#efe9df"/>
<rect x="104" y="102" width="140" height="20" rx="10" fill="#7c2d3a" opacity="0.85"/>
<rect x="490" y="22" width="230" height="126" rx="14" fill="#17181a"/>
<text x="605" y="54" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="700" font-size="19" fill="#f7f5f0">Canvas</text>
<rect x="516" y="70" width="178" height="24" rx="5" fill="#b8848d"/>
<rect x="516" y="102" width="84" height="30" rx="5" fill="#3a3c40"/>
<rect x="610" y="102" width="84" height="30" rx="5" fill="#3a3c40"/>
<path d="M270,62 C350,40 410,40 486,62" fill="none" stroke="#7c2d3a" stroke-width="2.5" marker-end="url(#dah)"/>
<text x="380" y="34" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="14" fill="#6b6659">you describe, it builds</text>
<path d="M490,112 C410,136 350,136 274,112" fill="none" stroke="#7c2d3a" stroke-width="2.5" stroke-dasharray="6 5" marker-end="url(#dah)"/>
<text x="380" y="160" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-style="italic" font-size="14" fill="#7c2d3a">you refine, it updates</text>
</svg>

Note: The mental model, straight from the help guide: Claude Design pairs a conversation with a canvas. You describe what you want, Claude builds it on the canvas beside the chat, and every change shows up live. It makes landing pages, one-pagers, clickable prototypes, decks, and campaign visuals. No design skills needed. It is an Anthropic Labs product, launched April 2026, now built into Claude.

---

<div class="lesson-no">Lesson 6.1 · Where to find it</div>

# Where to open it

| Where | How |
| --- | --- |
| Any chat | just ask, or pick **Output → Design** |
| Artifacts tab | start from a **Design** template |
| Claude Code | type `/design` |
| claude.ai/design | the standalone app |

Note: Since the September 2026 update, Design is one of three artifact templates, next to Slides for talks and Docs for writing. Beta on Pro, Max, and Team, on by default. On Enterprise an owner turns it on. The Free plan gets plain artifacts, not the templates. On a phone you can ask and view, but editing needs web or desktop.

---

<div class="lesson-no">Lesson 6.1 · The technique</div>

# Four things every design prompt needs

- **Goal** what you are building
- **Layout** how it is arranged
- **Content** what it shows
- **Audience** who will use it

<div class="promptcard"><span class="lbl">Prompt</span>

A landing page for a small gym: hero with a "Book a free class" button, timetable, trainer cards, prices. For busy beginners, friendly not intimidating. Mobile first.

</div>

Note: The help guide's formula: goal, layout, content, audience. This is Description from Module 4 applied to visuals, call it back, do not re-teach it. Contrast it aloud with "make a gym website", every blank you leave, Claude fills with a guess. Tip from the guide: attach a screenshot of a site you like and say "match this", a picture carries style better than adjectives.

---

<div class="lesson-no">Lesson 6.1 · Refine it</div>

# Chat, comment, or edit it yourself

| Use | When | Example |
| --- | --- | --- |
| **Chat** | big changes | "move the prices above the trainers" |
| **Comment** | one element | click the button: "make this larger" |
| **Edit directly** | quick fixes | drag, resize, retype text |

Note: The decision table from the help guide. The first draft is a starting point, the value is in refining. Be specific: "tighten the gap between fields to 8px" beats "this does not look right". Claude can also build sliders to tune spacing and colour live. Beta glitch: if a comment is not picked up, paste it into the chat.

---

<div class="lesson-no">Lesson 6.1 · Two prompts worth knowing</div>

# Ask for options, then a critique

<div class="promptcard"><span class="lbl">Explore</span>

Show me 3 different layouts: one minimal, one bold, one photo-led.

</div>

<div class="promptcard"><span class="lbl">Critique</span>

Review this for contrast, hierarchy, and mobile. List the top 5 problems, then fix them.

</div>

Note: Anthropic's tips: ask for two or three variations when unsure, comparing is faster than guessing. And treat Claude as a design collaborator, not just a generator, the critique prompt is Discernment from Module 4. There is no version history yet, so before trying a new direction say "save what we have, then try a completely different approach".

---

<div class="lesson-no">Lesson 6.1 · Your turn</div>

# Try it yourself

<p class="try"><b>Your turn</b> Design one thing for your project with all four parts, then change it once by chat, once by comment, and once by direct edit.</p>

<div class="uc-grid">
<div class="uc">A landing page for a gym or café</div>
<div class="uc">A 4-screen app onboarding flow</div>
<div class="uc">A flyer for an event</div>
<div class="uc">A portfolio page</div>
</div>

Or design something your own project needs.

Note: Keep this design open, Lesson 6.2 puts it on brand and ships it. Reflection to pose aloud: which of the four prompt parts changed the result the most?

---

<div class="lesson-no">Lesson 6.1 · Recap</div>

# Quick recap

- Claude Design is a conversation plus a live canvas
- Every prompt needs a goal, layout, content, and audience
- Chat for big changes, comment for one element, edit for quick fixes

<div class="refs">
<a href="https://support.claude.com/en/articles/14604416-get-started-with-claude-design" target="_blank" rel="noopener"><span class="ref-src">Read more ·</span> Get started with Claude Design</a>
</div>

Note: Ten second reminder. Next, make it look like your brand, and get it out the door.

---

<!-- .slide: data-background-color="#17181a" class="dark" -->

<div class="lesson-no">Lesson 6.2</div>

## On brand, and out the door

By the end of this lesson you will be able to:

- Set up a design system so every design matches your brand
- Turn a design into a deck or code, then share and export it

Note: The second half: consistency, then shipping. Sources: Set up your design system in Claude Design; Academy tutorial on decks; Get started, Export and share.

---

<div class="lesson-no">Lesson 6.2 · Design systems</div>

# One design system, every design

<svg class="diagram" viewBox="0 0 760 190" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Your brand sources become a design system, used by every design">
<defs><marker id="dsh" markerWidth="9" markerHeight="9" refX="6.5" refY="3" orient="auto"><path d="M0,0 L7,3 L0,6 Z" fill="#7c2d3a"/></marker></defs>
<g font-family="Plus Jakarta Sans, sans-serif" text-anchor="middle">
<rect x="14" y="18" width="160" height="40" rx="10" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="94" y="43" font-weight="700" font-size="15" fill="#17181a">logo &amp; colours</text>
<rect x="14" y="74" width="160" height="40" rx="10" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="94" y="99" font-weight="700" font-size="15" fill="#17181a">a good deck or PDF</text>
<rect x="14" y="130" width="160" height="40" rx="10" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="94" y="155" font-weight="700" font-size="15" fill="#17181a">your code</text>
<line x1="174" y1="38" x2="276" y2="84" stroke="#7c2d3a" stroke-width="2" marker-end="url(#dsh)"/>
<line x1="174" y1="94" x2="276" y2="94" stroke="#7c2d3a" stroke-width="2" marker-end="url(#dsh)"/>
<line x1="174" y1="150" x2="276" y2="104" stroke="#7c2d3a" stroke-width="2" marker-end="url(#dsh)"/>
<rect x="280" y="44" width="200" height="100" rx="14" fill="#17181a"/>
<text x="380" y="80" font-weight="700" font-size="18" fill="#f7f5f0">Design system</text>
<text x="380" y="104" font-size="12" fill="#b8848d">colours · type</text>
<text x="380" y="122" font-size="12" fill="#b8848d">components · layout</text>
<line x1="480" y1="84" x2="584" y2="38" stroke="#7c2d3a" stroke-width="2" marker-end="url(#dsh)"/>
<line x1="480" y1="94" x2="584" y2="94" stroke="#7c2d3a" stroke-width="2" marker-end="url(#dsh)"/>
<line x1="480" y1="104" x2="584" y2="150" stroke="#7c2d3a" stroke-width="2" marker-end="url(#dsh)"/>
<rect x="588" y="18" width="156" height="40" rx="10" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="666" y="43" font-weight="700" font-size="15" fill="#17181a">landing page</text>
<rect x="588" y="74" width="156" height="40" rx="10" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="666" y="99" font-weight="700" font-size="15" fill="#17181a">deck</text>
<rect x="588" y="130" width="156" height="40" rx="10" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="666" y="155" font-weight="700" font-size="15" fill="#17181a">one-pager</text>
</g>
</svg>

Note: A design system captures your colours, typography, components, and layout, and Claude applies it to every new design. The key line from the product page: Claude checks its output against your system and corrects it before you see it. Two ways to make one: in a chat, upload a logo, brand PDF, or a deck you like, best for a brand; or from Claude Code run /design-sync, best for a product already built in React. Test it with a landing page and a one-pager, then turn on Published so your team uses it. Tip: real examples beat specs, a finished page shows the feel, a palette alone does not.

---

<div class="lesson-no">Lesson 6.2 · Decks</div>

# A deck in one prompt

<div class="promptcard"><span class="lbl">Prompt</span>

Create a 6-slide deck pitching our gym to a local company for staff memberships: the problem, our classes, results, group pricing, next steps.

</div>

- Edit by number: "On slide 3, change the headline to…"
- Or convert: "make a one-pager from this deck"

Note: From the Academy tutorial, one of the most popular uses inside Anthropic. Say the slide count, the audience, and the sections. Charts appear from data you describe, and because it is HTML it can animate. The templates convert into each other: doc to deck, deck to one-pager.

---

<div class="lesson-no">Lesson 6.2 · Make it real</div>

# Hand it to Claude Code

<svg class="diagram" viewBox="0 0 760 110" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Claude Design to handoff bundle to Claude Code to live site">
<defs><marker id="dhh" markerWidth="9" markerHeight="9" refX="6.5" refY="3" orient="auto"><path d="M0,0 L7,3 L0,6 Z" fill="#7c2d3a"/></marker></defs>
<g font-family="Plus Jakarta Sans, sans-serif" text-anchor="middle">
<rect x="10" y="26" width="160" height="58" rx="12" fill="#fffdf9" stroke="#7c2d3a" stroke-width="2"/>
<text x="90" y="61" font-weight="700" font-size="17" fill="#17181a">Claude Design</text>
<rect x="210" y="26" width="160" height="58" rx="12" fill="#f0ece2" stroke="#7c2d3a" stroke-width="2" stroke-dasharray="6 4"/>
<text x="290" y="53" font-weight="700" font-size="16" fill="#17181a">handoff bundle</text>
<text x="290" y="72" font-size="12" fill="#6b6659">design + intent</text>
<rect x="410" y="26" width="160" height="58" rx="12" fill="#17181a"/>
<text x="490" y="61" font-weight="700" font-size="17" fill="#f7f5f0">Claude Code</text>
<rect x="610" y="26" width="140" height="58" rx="29" fill="#7c2d3a"/>
<text x="680" y="61" font-weight="700" font-size="17" fill="#f7f5f0">live site</text>
<line x1="170" y1="55" x2="206" y2="55" stroke="#7c2d3a" stroke-width="2.5" marker-end="url(#dhh)"/>
<line x1="370" y1="55" x2="406" y2="55" stroke="#7c2d3a" stroke-width="2.5" marker-end="url(#dhh)"/>
<line x1="570" y1="55" x2="606" y2="55" stroke="#7c2d3a" stroke-width="2.5" marker-end="url(#dhh)"/>
</g>
</svg>

Note: Callback to Module 5, do not re-teach Claude Code. First, everyone can make a design clickable: "the Join button opens a sign-up form", and test it with real people before any code. When it is ready to become software, Export, Handoff to Claude Code packs a bundle with your design intent, so Claude Code builds from the design, not from a screenshot. From Claude Code, /design imports a design or exports code as a live prototype.

---

<div class="lesson-no">Lesson 6.2 · Share and export</div>

# Pick the right way out

| You want to | Do this |
| --- | --- |
| Get feedback | share with **comment** access |
| Send it to a client | export **PDF** |
| Edit in PowerPoint | export **PPTX** |
| Keep designing | send to **Canva** or **Adobe** |
| Put it live | send to **Vercel** or **Wix** |

Note: Designs start private. Share for view, comment, or edit, and editors can chat with Claude together. Full export list: zip, PDF, PPTX, standalone HTML for animation, and send-to for Adobe, Canva, Gamma, Miro, Netlify, Lovable, Replit, Vercel, Wix and more, re-check it the week you record. Before you ship, Diligence from Module 4: are the prices and dates right, is the contrast readable, does it work on a phone, are the images yours to use? Known beta limits: no version history yet, basic co-editing, and it uses your plan's normal limits.

---

<div class="lesson-no">Lesson 6.2 · Your turn</div>

# Try it yourself

<p class="try"><b>Your turn</b> Put your Lesson 6.1 design on brand, make one more piece from it, then share one and export one.</p>

<div class="uc-grid">
<div class="uc">Build a design system from your logo</div>
<div class="uc">Make a 5-slide pitch deck</div>
<div class="uc">Turn the deck into a one-pager</div>
<div class="uc">Export a PDF for a client</div>
</div>

Note: No brand yet? Ask Claude to propose a palette, two fonts, and a tone first, then build the system from that. Re-run the Lesson 6.1 prompt and compare before and after. Module 5 graduates can stretch: hand the page to Claude Code and get it running.

---

<div class="lesson-no">Lesson 6.2 · Recap</div>

# Quick recap

- A design system keeps every design on brand, automatically
- One prompt makes a deck, and it converts into a one-pager
- Hand it to Claude Code, or share and export it

<div class="refs">
<a href="https://support.claude.com/en/articles/14604397-set-up-your-design-system-in-claude-design" target="_blank" rel="noopener"><span class="ref-src">Read more ·</span> Set up your design system</a>
</div>

Note: Ten second reminder. To close, the habits that separate most people from the pros.

---

<div class="lesson-no">Module 6 · Pro habits</div>

# Most people vs the pros

| Most people | The pros |
| --- | --- |
| A one-line prompt | Goal, layout, content, and audience |
| Accept the first draft | Ask for three options, then pick |
| "Make it better" | One specific, measurable change |
| Restyle every design by hand | Set up a design system once |
| Ship it as it is | Ask for a critique, then check it yourself |

Note: Same tool, the whole gap is in the habits. Every row maps to a slide in this module.

---

<div class="lesson-no">Module 6 · Where to go next</div>

# Take it further

<div class="refs">
<a href="https://support.claude.com/en/articles/14604416-get-started-with-claude-design" target="_blank" rel="noopener"><span class="ref-src">Official ·</span> Get started with Claude Design</a>
<a href="https://academy.claude.com/courses/claude-101/creating-with-artifacts" target="_blank" rel="noopener"><span class="ref-src">Anthropic ·</span> Claude 101, Creating with artifacts</a>
<a href="https://academy.claude.com/tutorials/using-claude-design-for-presentations-and-slide-decks" target="_blank" rel="noopener"><span class="ref-src">Anthropic ·</span> Claude Design for presentations</a>
<a href="https://academy.claude.com/use-cases/create-brand-assets" target="_blank" rel="noopener"><span class="ref-src">Use case ·</span> Create brand assets</a>
</div>

Note: One references slide to close. The help guide first, then Anthropic's Academy lessons and the brand assets use case. Links open in a new tab.

---

<!-- .slide: data-background-color="#17181a" class="dark" -->

<div class="lesson-no">What is next</div>

## Coming up

You can now design, build, and automate with Claude. Next, we bring it all together.

Note: Bridge to the next module. Wording to be finalised once the roadmap order after Module 6 is confirmed.
