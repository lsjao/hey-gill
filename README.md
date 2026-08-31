# Hey, Gill.

Birthday invite page — Yellow Submarine / 60s psychedelic styling.

**Live:** https://lsjao.github.io/hey-gill/

## The night

**Saturday, 12 September 2026**

| | Venue | Time |
|---|---|---|
| Stop 1 | Borro Manila — Sct. Borromeo Cor. Sct. Tobias, Quezon City | 6:30 PM |
| Stop 2 | Friends Screen Simulation Golf — 4F Century Mall, Makati | 10:00 PM |

## Stack

Single static `index.html` with inline CSS. No build step, no JS of our own.

- **Google Fonts** — Shrikhand (display, arched on SVG `textPath`), Baloo 2 (body)
- **Pinterest `pinit.js`** — the four outfit reference pins. Ad blockers may block
  this; each pin degrades to a plain link.

Maps are keyless Google Maps embeds, so there's no API key to manage.

## Type scale

Sizes follow a golden-ratio scale (φ = 1.618) declared as `--s0`…`--s5` in `:root`.
Two deliberate departures, both commented in the file:

- the title is 250px, which sits between rungs (the rung was 196px)
- the hero banner and date were stepped down a further ÷1.5, so they hold φ
  against each other but not against the title

The title is SVG text on a curved path, so its rendered size is
`font-size × (max-width ÷ viewBox width)` — the two knobs are commented in the CSS.

## Deploying

GitHub Pages serves `main` from the repo root. Push and it redeploys in about a minute.

`.nojekyll` is present so Jekyll doesn't filter anything.
