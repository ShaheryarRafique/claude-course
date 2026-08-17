# Module 2 — Exercises, Live Demos, and Quiz

Running example: build your "Final Exam Prep" workspace. Everything below is exact: type the prompts as written, click the buttons named, and you get the described result. Written in English; students can ask Claude to reply in their own language if they prefer.

Model note: names drift, so this uses tiers (fast model, everyday model, deep model). Verify current names on a live account before recording.

---

## Live demo 1 — Build an Artifact on camera (target under 3 minutes)

Goal: turn an empty chat into a working, colourful "Exam Countdown and Study Tracker" that runs live, with a progress bar, in three prompts. No code typed by you. Start a fresh chat on the everyday model (fast enough to render live).

**Prompt 1 — build it (paste exactly):**
> Build a React artifact: an "Exam Countdown and Study Tracker" for a student in Lahore preparing for five final exams. Top section: a countdown showing days left until my first exam on 15 December 2026. Below it: a list of five subjects, Physics, Chemistry, Maths, English, Pakistan Studies, each with a checkbox for "revised" and a number input for "hours studied". Use a clean card layout, a green accent, and simple icons. Keep it to a single file. Make it fully interactive so I can tick subjects and type hours right now.

Narrate on camera: saying "React artifact" and "single file" is what makes Claude render a live app instead of a code block. The panel opens on the right. Tick two boxes, type a few hours, it reacts instantly.

**Prompt 2 — the crowd pleaser:**
> Add a progress bar at the top that fills based on how many of the five subjects I have ticked as revised. Show it as a percentage too, for example "2 of 5 revised, 40%". Animate the bar so it slides when I tick a box.

Tick a box on camera, the bar slides. This is the wow moment: it proves it is real software, not a picture.

**Prompt 3 — make it stick:**
> Add a total hours counter that sums the hours across all five subjects, shown in a card next to the progress bar. Also save my ticks and hours to localStorage so my data survives a page refresh.

Refresh the panel on camera, the data is still there.

**Publish (about 20 seconds):** click Publish at the top right of the panel, then Copy link. Anyone can open it in a browser with no Claude login. Paste the link in the video description.

Done state: ticking a box moves the bar and updates "X of 5, Y%"; typing hours updates the total; refresh keeps the data; the published link opens for a logged out person.

---

## Live demo 2 — Build a Project on camera

Goal: show that a Project beats a plain chat because instructions and your real notes persist across every chat.

**Create:** Sidebar, Projects, New project. Name it "Final Exam Prep". Describe it as preparing for five final exams in December.

**Custom instructions (paste):**
> You are my exam prep tutor. I am a student in Lahore preparing for finals on 15 December 2026. Rules: 1) Only teach from the syllabus and past papers in this Project's files; if something is outside them, say so first. 2) Explain simply, with everyday local examples. 3) Default format: a three line summary first, then details, then one practice question. 4) When I say "quiz me", ask five questions one at a time and wait for my answer before revealing the correct one. 5) Never invent a formula or date; if a past paper is unclear, tell me which file and page.

**Upload to the knowledge base (keep each 1 to 3 pages):** your syllabus, one past paper, and a short text file "my weak topics" you type in a minute (for example: Weak, rotational motion and thermodynamics numericals. Strong, optics.).

**Before and after (show side by side):**
- Before, in a plain chat: "Give me five likely questions for my physics final." Result: generic textbook questions.
- After, inside the Project, the same prompt: questions in your past paper's pattern, weighted to your weak topics, ending with a practice question, because the instructions and files are in scope.
- Proof: ask "Which file did you use for question 3?" Inside the Project it names your file; the plain chat cannot.

---

## Your turn — one exercise per feature

Do these, or the quiz is unpassable.

1. **Conversations.** New chat: "Explain Newton's second law in three lines, then give me one numerical to solve." Rename the chat to "Physics, Newton". Edit your first message to add "and include units", resend. Done when: renamed, and the answer shows units.
2. **Files.** Upload one past paper. Ask: "List every question in this paper about thermodynamics, with its page number." Done when: it returns question numbers with page references from your file.
3. **Web search.** Ask: "Search the web for my university's exam date sheet for December 2026, and give me the source link." Done when: the answer has a real, clickable source URL.
4. **Model choice.** Ask "Explain entropy simply" once on the fast model and once on the deep model. Done when: you can say in one sentence which you would pick for quick revision versus deep understanding, and why.
5. **Artifacts.** Build: "Build a React artifact: a flashcard app with ten chemistry flashcards, term on front, definition on back, a flip animation, a shuffle button, and a known or unknown counter." Then: "Add a progress bar showing how many I have marked as known." Done when: cards flip, shuffle works, the bar moves.
6. **Projects.** Create a Project "Chemistry Prep", paste three rules (include "quiz me one question at a time"), upload one syllabus file. Inside it, type "quiz me". Done when: it asks one question and waits.
7. **Memory.** In a normal chat: "Remember that my finals are on 15 December 2026 and I like a three line summary first." Start a new chat later and ask "how many days till my finals?" Done when: the new chat already knows. Then open Settings, Memory, and confirm the entry is listed, and that you can delete it.

---

## Quiz (five questions, answers below)

1. You built the tracker, ticked three subjects, refreshed, and the ticks vanished. Which build step did you skip, and what one word fixes it?
2. In your Project the same prompt gave better, personalised questions than a plain chat. Name the two Project ingredients that caused the difference.
3. You need a fast quiz session of forty recall questions, and separately you are stuck on a hard multi step derivation. Which model for each, and why?
4. You ask for your university's date sheet and it must not guess. Which feature must be on, and what proves the answer is trustworthy?
5. You told Claude to remember your exam date. A friend on their own account asks the same question. Will Claude know your date for them, and where do you view or delete what it remembered?

**Answers.** 1) You skipped saving to storage; the fix word is localStorage. 2) The custom instructions and the files knowledge base. 3) Fast model for the forty quick questions (fast and cheap); deep model for the hard derivation (built for hard multi step reasoning). 4) Web search must be on; it is trustworthy only if it includes a real source link you can open. 5) No, memory is tied to your own account; view or delete it in Settings, Memory.
