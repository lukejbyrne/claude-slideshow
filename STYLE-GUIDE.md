# Slideshow Style Guide

## Format
- Single self-contained HTML file (no build tools, no frameworks)
- Arrow key navigation (left/right), spacebar also advances
- Touch/swipe support for mobile preview
- Dot indicators at bottom center (current slide highlighted)
- Slide counter top-right (e.g. "3 / 12") in DM Mono
- Keyboard hint bottom-right ("← →") in very faint text
- Drawing tools top-left: pen (Q), rectangle (W), arrow (E), eraser (R), clear all (Esc)
- Drawings auto-clear on slide change
- Arrow keys always navigate slides even when a draw tool is active

## Brand Kit
- Background: `#0c0c0b`
- Text: `#fef8ea` (cream)
- Primary accent: `#e85d4a` (coral)
- Secondary accent: `#f4a261` (warm orange)
- Card background: `#161615`
- Card border: `rgba(254, 248, 234, 0.06)`
- Muted text: `rgba(254, 248, 234, 0.45)`
- Drawing color: `#e85d4a` (coral)

## Typography
- **Headlines**: Instrument Serif, weight 400, `clamp(36px, 4.5vw, 64px)`
- **Body/cards**: Manrope, weights 400–600
- **Labels/tags/mono**: DM Mono, weight 400–500
- All via Google Fonts, no local files needed

## Emphasis Rules (the balance)
- **Bold coral** (`<strong>`) on key differentiating words in headlines — not every slide, just the ones that carry the main point
- **Coral underline** (`.ul-coral`) sparingly on the most important words — the ones you'd circle on a whiteboard. Max 1-2 per slide
- **Orange underline** (`.ul-orange`) when emphasising something specific to the "secondary" tool/concept in a comparison
- **Italic** only on bottom-text takeaway lines — uses Instrument Serif italic via `<em>` inside `.bottom-text`. These are the editorial one-liners the presenter says as they transition
- **Never** combine underline + italic + bold on the same word. Pick one treatment
- **Never** underline or bold subtitle text — subtitles stay muted and plain

## Layout Principles
- One key idea per slide — if you need two ideas, make two slides
- Centered content, generous whitespace
- Headlines centered, cards below, takeaway text at bottom
- Card grids: `.cards-3` for three items, `.cards-2` for comparisons
- Side-by-side comparisons use `.card-big` with `.tag` labels (antigravity/orange vs claude/coral pattern — adapt tag names to the comparison topic)

## Card Styles
- Dark background `#161615` with very subtle border
- Rounded corners: 14px for small cards, 16px for big cards
- Emoji icons at top of small cards (28px)
- Card titles in Manrope 600, descriptions in muted text
- Tags are uppercase DM Mono with colored background tint + border

## Slide Types (reusable patterns)
1. **Title slide** — headline + subtitle, nothing else
2. **Feature cards** — headline + 3 cards (emoji, title, description) + bottom text
3. **Comparison** — headline + 2 big cards with tags + optional bottom text
4. **Checklist comparison** — headline + 2 cards with ✓ lists
5. **Code/file mock** — headline + subtitle + code block card
6. **Transition** — small uppercase label + big headline + subtitle

## Subtle Details
- Grain overlay via inline SVG filter (very subtle, opacity 0.5)
- Slide transitions: fade + 12px translateY, 0.5s cubic-bezier
- Active dot scales 1.3x and turns coral
- No animations beyond slide transitions — keep it calm

## What NOT to Do
- No gradients on backgrounds
- No drop shadows on cards
- No hover effects on slide content (it's a presentation, not a web app)
- No walls of text — if you're writing a paragraph, it belongs in your script, not on screen
- No images unless absolutely necessary — the presenter IS the visual
- Don't use Inter, Roboto, or system fonts
- Don't use purple/blue accent colors — stick to coral/orange warmth
