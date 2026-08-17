# Module 2 source — Anthropic "AI Fluency: the 4D Framework" (authoritative), captured 2026-08-17

Full current content of Anthropic's "AI Fluency for small business owners" course, pasted by the user from the live Claude tab. PRIMARY blueprint for OUR Module 2. It is framed for small-business owners; broaden our version to students + all professionals (keep the business examples as one of several role lenses). Rewrite in our own words; never copy verbatim.

**AI Fluency = using AI in ways that are efficient, effective, ethical, and safe.** The 4D Framework (Delegation, Description, Discernment, Diligence) is its foundation. Attribution: developed by Prof. Rick Dakan (Ringling College) and Prof. Joseph Feller (University College Cork).

## The two loops (core mental model)
- **Inner loop — Description ↔ Discernment:** you describe what you want, the model responds, you judge what is useful, you describe again, sharper. Drives higher-quality output through back-and-forth.
- **Outer loop — Delegation ↔ Diligence:** upfront you decide what/tool/data to hand off; afterward you verify, attribute, and own the result. Frames every interaction.
- Delegation sets the stage; Description and Discernment do the work in between; Diligence closes it.

## The four D's
- **Delegation** — decide what AI handles and what stays with you (the right task, right tool, right data). Ask "should AI do this?" not just "can it?"
- **Description** — communicate clearly what you need and how AI should approach it. (This is where prompting craft lives.)
- **Discernment** — critically evaluate what AI gives back: quality, accuracy, relevance, bias — and evaluate the collaboration itself so the next prompt is sharper.
- **Diligence** — use AI responsibly: verify, attribute, be transparent, own the final result.

## Lesson-by-lesson assets

### L1 — Intro / define your values (build a reusable context document)
- **Exercise: your "AI briefing sheet."** Self-reflect: business/role mission, vision, values, situation, constraints; finish "If AI could help me ___, I would spend more time ___." Then have Claude interview you and synthesize a structured, reusable context document you paste into future chats. (OUR version: a student/professional context sheet — role, goals, subjects/clients, constraints, standards.)
- Every efficiency gain should translate to better outcomes and more time for high-value work.

### L2 — The 4D Framework
- Two loops (above). **Exercise: tag your context document** — mark each goal/task with the D it needs; whichever D dominates is where you'll gain fastest. Then take one real task one round with AI; note which D felt natural, which caught you off guard.

### L3 — AI capabilities and limitations
- Generative AI CREATES new content (vs analyzing). Three enablers: transformer architecture, vast training data, massive compute. Two training stages: pre-training (patterns from billions of examples) + fine-tuning (follow instructions helpfully).
- **Strengths:** versatility across tasks, conversational flow, connecting to external tools.
- **Limits:** knowledge cutoffs, hallucinations, context-window size, complex multi-step reasoning. Best apps pair human judgment/creativity/oversight with AI speed/scale.
- **Exercise: test the edges** — pick a domain you know cold; run a versatility test (explain 3 ways for 3 audiences), a hallucination test (ask for real resources, then verify one exists), and a knowledge-cutoff/reasoning test (ask something time-sensitive/local; does it caveat? then have it address a misconception you wrote down).
- **Interactive: "Text Your Friend Markov"** — a next-token generator built from a tiny transition matrix (frequency table → normalize → probability distribution → sampling). Markov (1906) → n-gram phone keyboards (~2010, SwiftKey/QuickType) → RNNs then transformers (2017). Great plain-English explainer of how LLMs pick the next word.

### L4 — Refining with AI (the Description ↔ Discernment loop)
- Effective Description provides context (what your work is, what you're accomplishing, what you need). Discernment isn't optional — flag specific claims (regulations, pricing, deadlines) to verify against primary sources. Loop is iterative; AI accelerates research but you remain the decision-maker.
- **Exercises:** (1) policy/legislation tracking — research a regulation, then flag ≥2 claims to verify, note missing perspectives, flag outdated/conflated info. (2) market/competitive research — check that competitors/data are real and current (AI fabricates names/stats), verify numbers to source, judge relevance to your size. (OUR version: research a topic/exam board/industry with the same verify-the-claims discipline.)

### L5 — Data & privacy (the Delegation ↔ Diligence loop)
- Some tools train on your inputs. Match tool to task by sensitivity. **Strip what isn't needed** (replace names with "Customer A", remove figures/contact info) before sharing. If something goes wrong, delete the conversation and request data deletion. Build validated approaches, not blind trust.
- **Exercise sequence (one full Delegation–Diligence loop):** (1) Decide what to share — pick a real doc, mark sensitive bits, sanitize, write your brief (goal + 2-3 things you already noticed + what a good output looks like). (2) Validate with AI — did it catch your patterns, surface new ones, miss/misstate anything? (3) Own the result — check accuracy, usefulness, accountability ("would I put my name on this?").

### L6 — Putting it all together (automate a workflow with all 4 D's)
- Start with **Problem Awareness** (what repeats?). **Delegation:** FAQs = good AI candidates; complaints/judgment calls stay human (three buckets: AI can handle / AI assists-human decides / human only).
- **Rich Description in three parts:** **Product** (end result, inputs, outputs), **Process** (step-by-step logic like instructions for a literal new employee, decision points, when to escalate, what docs it needs), **Performance** (tone, how to handle uncertainty — "if unsure, say so and flag; never guess", what it must never do).
- Test iteratively with 3-5 real examples (Discernment); expect 2-3 refinement rounds.
- **Diligence in three parts:** **Creation** (why appropriate, ≥3 failure modes + safeguards, real-world impact), **Deployment** (review every output vs sample; when to reduce oversight; monitoring; kill-switch triggers), **Transparency** (who needs to know AI is involved, the actual disclosure language, path to a human, any legal disclosure rules).
- Deliverable: a short **"Automation Readiness Statement"** (3-5 sentences: what, why appropriate, safeguards, transparency).

### L7 — Keeping the human in the loop (AI use policy)
- Being "the human in the loop" = you decide what problems AI should solve, not just oversight. Avoid dependency through understanding, not avoidance ("can you explain what the AI is doing?"). AI should free you for MORE human work (the handwritten card, the personal outreach). Set cultural norms about the time AI saves.
- **Exercise: draft a one-page AI use policy** with three sections: **What we use AI for** (approved tasks/tools), **What stays human** (non-negotiable judgment/relationships/accountability), **How we stay accountable** (oversight, transparency, what happens when something goes wrong). Build it with AI from your context document, then edit to sound like you. Stress-test: if a customer asked "do you use AI?", does it give a clear honest answer?

## How OUR Module 2 should use this (blend with Claude 101 "Getting better results")
- Spine = the 4D Framework with the two loops, made concrete for students + professionals + business owners (multi-role lenses, not only small business).
- Description lesson absorbs the Claude 101 prompt craft: set-stage/define-task/specify-rules recipe, the common-challenges troubleshooting table, the iteration mindset, show-an-example.
- Discernment lesson: evaluating outputs, capabilities vs limits, hallucination testing, **evals** (5-10 examples → test prompts → compare → refine).
- Diligence lesson: verification habits, data hygiene/privacy, transparency, the AI use policy.
- Delegation lesson: what to hand off vs keep; the three buckets.
- Running deliverables students keep: their **context document / AI briefing sheet** (built in L1) and a personal **AI use policy** (L7). Capstone-style: automate one repetitive task end to end (Product/Process/Performance + Diligence).
- Keep the "Text Your Friend Markov" next-token explainer as the plain-English "how does it work" beat.
