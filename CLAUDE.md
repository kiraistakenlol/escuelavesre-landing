# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Landing page for **Escuela Vesre**, a Spanish school in Buenos Aires. This is a static single-page site hosted on GitHub Pages.

- **Live URL**: https://kiraistakenlol.github.io/escuelavesre-landing/
- `index.html` — the live landing page (served by GitHub Pages)
- `landing.html` — same file, kept as a named copy
- `preferences.md` — design preferences document

## Hosting

GitHub Pages serves from the `master` branch root. Any push to `master` triggers a deploy.

## Design Direction

- Retro 70s warm style with blue color palette (migrated from original warm oranges)
- Fonts: **Bodoni Moda** (hero headings), **Righteous** (display), **Outfit** (body)
- Large hero typography using `clamp()` for responsive sizing
- Floating pill-shaped info cards with bobbing animations
- Circular photo frame with decorative orbit rings
- See `preferences.md` for detailed design preferences

## Working With the Code

Everything is in a single self-contained HTML file (inline CSS + JS, no build step). To preview locally:

```
python3 -m http.server 8765
open http://localhost:8765/index.html
```

Keep `index.html` and `landing.html` in sync — they should be identical copies.
