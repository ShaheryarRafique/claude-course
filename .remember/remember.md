# Handoff

## State
Refining "Claude Zero to Master" course LESSON BY LESSON in `deck/` (reveal.js, cache b=86). GLOBAL audience (no rupee/region examples). Module 1 (Claude Essentials, follows Claude 101) + Module 2 (The 4D Framework) built; index.html loads title+module-01+module-02. Per lesson: clean slides + script `scripts/module-01.md` + prompt pack `resources/module-01-copypaste.md`. Polished with user through LESSON 1.4 (done). Opening script `scripts/00-opening.md` rewritten to the real 6 modules.

## Next
1. Continue Module 1 review with user at LESSON 1.5 (Projects) — they go lesson by lesson, wait for their cue/screenshots.
2. After M1 slides locked: re-sync `scripts/module-01.md` (lags recent 1.2/1.3/1.4 edits) + make a clean student-facing prompt sheet.
3. Module 2 is parked; do NOT touch until user signs off Module 1.

## Context
- RULES: exercise slides heading = "# Try it yourself", task-only, NO demo chip, 3-4 concrete relatable options + "do your own". Demo chips say only "Demo". Prompt method = "technique" (NOT "recipe"). Favor before/after examples + small tables over abstract bullets. `.promptcard` shows a real prompt on a slide; `.qa`/`.rule` for verdict/takeaway (dark slides only).
- After editing deck/slides/*.md bump `?b=NN` in deck/index.html AND index-pdf.html.
- Do NOT jump ahead of the user's current lesson (got scolded for rebuilding Module 2 unprompted).
- Verified 2026-08-17 (in memory): models Haiku 4.5 / Sonnet 5 / Opus 5 / Fable 5 (Fable = largest/autonomous); effort levels Low/Medium/High(default)/Extra high/Max.
