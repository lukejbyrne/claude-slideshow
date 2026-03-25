# Claude Slideshow

Build slick, presentation-ready slideshows with Claude Code — one prompt, one HTML file, full drawing tools.

## What you get

A single self-contained HTML file with:
- Arrow key navigation
- Drawing tools built in (pen, rectangle, arrow, eraser)
- Your brand colors and fonts
- Dark, minimal aesthetic designed for screen recording

## Setup

### 1. Fill in your content

**`script.md`** — Paste your talking points, script, or bullet points. Organize by section. This is what Claude reads to generate your slides.

**`brand/`** — Drop your brand files here. This can be:
- A CSS file with your color variables and font imports
- A design tokens file (JSON, TS, etc.)
- A simple text file listing your colors and fonts
- Screenshots of your existing site/product for color matching

**`examples/`** — Drop screenshots of presentation styles you like. Claude will use these as visual reference for the layout and feel.

### 2. Run the prompt

Open Claude Code in this directory and paste the contents of `PROMPT.md`.

That's it. One prompt. Claude reads your script, brand, and examples, then builds the presentation.

### 3. Iterate

The first output won't be perfect — that's the point. Talk to Claude like a designer:
- "too much underline, dial it back"
- "make the subtitle italic"
- "add a slide between 3 and 4"
- "the cards feel cramped"

### 4. Present

Open the generated `index.html` in your browser. Full screen it. Use the drawing tools while you talk.

## Drawing tools

| Key | Tool |
|---|---|
| Q | Pen (freehand) |
| W | Rectangle |
| E | Arrow |
| R | Eraser (hold + drag) |
| Esc | Clear all drawings |
| ← → | Navigate slides |

## File structure

```
├── README.md          ← You're here
├── PROMPT.md          ← The one prompt to paste into Claude Code
├── STYLE-GUIDE.md     ← Design rules Claude follows
├── template.html      ← Working reference with example slides
├── script.md          ← Your talking points go here
├── brand/             ← Your brand files go here
└── examples/          ← Reference screenshots go here
```

## Example

See `template.html` for a working 3-slide example with all slide types (title, feature cards, comparison).
