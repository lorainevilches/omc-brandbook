# OhMyCodes — Brandbook

Static brandbook for OhMyCodes, a digital studio focused on the automotive sector. Documents the visual identity: logo versions, color palette, typography, brand pillars, and tone of voice.

## Stack

- HTML5
- Plain CSS3 (no framework)
- Vanilla JS — Intersection Observer for scroll-triggered entry animations
- Google Fonts: Inter + JetBrains Mono

## Structure

```
/
├── index.html
├── css/
│   ├── base.css        # reset, CSS variables, global utilities
│   ├── layout.css      # nav, cover, sections, grids, footer
│   ├── components.css  # cards, color swatches, logo cards, typography examples, voice card
│   └── animations.css  # .anim-hidden / .anim-visible
└── assets/
    └── images/
        ├── OMC_ID_-_DARK_BG.jpg
        └── OMC_ID_-_LIGHT_BG.jpg
```

## Running locally

Any static file server works. Quickest options:

```bash
# VS Code Live Server extension — open index.html, click "Go Live"

# Python
python3 -m http.server 8080

# Node (npx, no install needed)
npx serve .
```

No build step. No dependencies to install.

## Notes

- Fully responsive
- Dark mode by default
- Logo images must be in `assets/images/` — the HTML references that path directly
- Scroll animations run once per element via Intersection Observer, no external library
