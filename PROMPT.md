Build a single-file HTML presentation based on the content in `script.md`.

Read the following files before you start:
- `script.md` for the slide content and talking points
- `brand/` for my colors, fonts, and design tokens
- `examples/` for reference screenshots of the style I want
- `STYLE-GUIDE.md` for the design rules and slide type patterns

Generate a single `index.html` file with:
- Arrow key navigation (left/right), spacebar to advance, touch/swipe support
- Dot indicators at bottom center, slide counter top-right
- Drawing tools top-left: pen (Q), rectangle (W), arrow (E), eraser (R), clear all (Esc)
- Eraser works by holding click and dragging across drawn elements
- Drawings auto-clear on slide change
- Arrow keys always navigate slides even when a draw tool is active
- Subtle fade + slide-up transition between slides
- Subtle grain texture overlay
- One key idea per slide — keep text minimal, I'll be talking over these

For emphasis, use underline/bold/italic sparingly:
- Bold accent color on key differentiating words in headlines (not every slide)
- Colored underline on the most important 1-2 words per slide max
- Italic (in the display font) only on bottom-text editorial takeaway lines
- Never combine all three on the same word

Use the slide type patterns from STYLE-GUIDE.md (title, feature cards, comparison, checklist, code mock, transition) and pick the right type for each section of the script.
