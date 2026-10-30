# Iridescent lab: static test site

Two self-contained pages, built from `/workspace/design-lab/iridescent/` by `node build.mjs`.

- `index.html`: Sigil, the demo landing page
- `design-system.html`: tokens, motif, motion and components
- `tokens.css` / `tokens.json`: the design tokens (the pages inline their CSS, so these files are reference copies)
- `favicon.svg`, `.nojekyll`

All links are relative, so the folder works at any sub-path (tested at `/iridescent-lab/`). There are no external requests: no fonts, CDNs, analytics, or secrets.

Theme: Auto follows the OS (Night when the OS prefers dark), and the Auto/Dune/Night switch on each page is saved in `localStorage` under `iridescent-theme`. Reduced motion is respected.

Local preview: `cd .. && python3 -m http.server` then open `/iridescent-site/`.
