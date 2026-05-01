# rpentomino

Static site for [rpentomino.com](https://rpentomino.com). Single full-bleed redwood photograph with a Conway's Game of Life canvas overlay. Click anywhere to seed an R-pentomino; click and drag to scatter cells.

## Files

- `index.html` — the entire site. Markup, styles, and the embedded Game of Life script are all here.
- `photos/redwood.jpg` — the redwood background.
- `vercel.json` — long-cache headers for static assets.

## Editing the simulation

The Life script is the inline `<script>` in `index.html`. Tunable constants are at the top of the IIFE: `CELL`, `STEP_MS`, `PEAK_ALPHA`, `LIFETIME_FADE`, `RIPPLE_AMP`, etc.

## Deploying

Pushed to `main` → Vercel auto-deploys. No build step.

## Local preview

Open `index.html` directly in a browser, or run any static server in this directory (e.g. `npx serve`).
