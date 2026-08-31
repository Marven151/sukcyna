# Sukcyna

Landing page for **Sukcyna**, a fictional Polish cosmetics brand built around Baltic amber (sukcynit) and succinic acid.

> The brand is invented for this project. It is not a real company and does not sell anything.

## What's here

Single static page, no build step, no dependencies. Open `index.html` in a browser.

- **Hero** — an amber nugget drawn in SVG. The internal light source follows the pointer and drifts on its own when idle. Sun spangles and a fossil sprig are rendered inside the stone.
- **Deposit strip** — material, resin age, succinic acid content, catalogue size.
- **Catalogue** — three products numbered like museum specimens (`SK/01`–`SK/03`).
- **Formula** — full ingredient list for `SK/01` with percentages.

## Design notes

Committed single-theme dark palette: cold Baltic water as the ground, amber as the only light source. Amber only reads as amber in the dark, so there is no light variant.

| Role | Value |
| --- | --- |
| Ground | `#0A1417` |
| Raised surface | `#101F24` |
| Border | `#1D3238` |
| Amber accent | `#E08B2C` |
| Amber highlight | `#F5C978` |
| Text | `#EAE3D5` |
| Muted text | `#7E949B` |

Typefaces: Newsreader (display), Archivo (body), IBM Plex Mono (labels and data), all from Google Fonts.

Accessibility: keyboard focus is visible, `prefers-reduced-motion` disables the drift animation and scroll reveals, and the layout reflows down to 360px.

## Local preview

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Deploying to GitHub Pages

Settings → Pages → Build and deployment → Deploy from a branch → `main` / `/ (root)`.
