# The Slide Deck

This is the single source for the course slides. All content lives in the markdown files in the `slides` folder. Edit those files and the deck updates. You do not need to touch the HTML.

## How to view it

The deck loads its slides from separate files, so it needs a small local web server rather than opening the file directly. This is one command.

1. Open a terminal in this `deck` folder.
2. Run one of these:
   - `python3 -m http.server 8000`
   - or, if you have Node, `npx serve`
3. Open `http://localhost:8000` in your browser.

Press `S` for speaker view, which shows your notes and a timer. Press `F` for full screen. Press `Esc` for a grid overview.

## How to edit content

- Each module is one file, for example `slides/module-01.md`.
- A line with three dashes starts a new slide.
- A line starting with `Note:` starts the speaker notes for that slide. Notes are only visible in speaker view, not on the slide.
- Keep on screen text short. Put your talking points and demo cues in the notes.

Track labels use small chips, for example `<span class="tag core">Core</span>`. The colours are Core blue, Builder orange, Developer purple.

## How to restyle everything

Open `theme.css`. The colours and font are set at the top under `:root`. Change them once and the whole deck restyles.

## Adding the rest of the modules

Module 1 is populated as the working sample. When you are happy with the look, the other modules are added by creating `slides/module-02.md` through `slides/module-08.md` in the same format, and uncommenting their lines in `index.html`.

## Optional security hardening

The deck loads reveal.js from a public CDN, pinned to version 5. For a local presentation this is low risk. If you ever publish the deck on the public web, add Subresource Integrity hashes (`integrity="sha384-..."` and `crossorigin="anonymous"`) to the script and stylesheet tags, or download reveal.js and serve it locally so nothing is fetched from a third party.

## Exporting to PDF

Add `?print-pdf` to the URL, for example `http://localhost:8000/?print-pdf`, then use the browser print dialog and save as PDF.
