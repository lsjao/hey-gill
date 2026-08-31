# Hey, Gill.

Birthday invite page — Magical Birthday Tour theme, 60s psychedelic poster styling.

**Live:** https://lsjao.github.io/hey-gill/

## The night

**12 September 2026**

| | Venue | Time |
|---|---|---|
| Stop 1 | Borro Manila — Sct. Borromeo Cor. Sct. Tobias, Quezon City | 6:30 PM |
| Stop 2 | Friends Screen Simulation Golf — 4F Century Mall, Makati | 10:00 PM |

## Stack

Single static `index.html` with inline CSS and no build step. Two external dependencies:

- **Google Fonts** — Rammetto One (headlines), Baloo 2 (body), Permanent Marker (accents)
- **Pinterest `pinit.js`** — the four outfit reference pins. Ad blockers may block this; each pin degrades to a plain link.

Maps use keyless Google Maps embeds, so there's no API key to manage.

## Deploying

GitHub Pages serves `main` from the repo root. Push to `main` and it redeploys in about a minute.

```sh
git add index.html
git commit -m "..."
git push
```

`.nojekyll` is present so Jekyll doesn't filter anything.
