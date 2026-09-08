# Azimatul Matsniya — Business Intelligence Portfolio

A single-page portfolio website for a Business Intelligence Engineer role.
Static HTML — no build step, no dependencies.

## Contents

- `portfolio.html` — the full site (HTML + CSS + a small amount of JS, all inline)
- `Picture/` — dashboard screenshots used in the Projects section

## Features

- **Light / dark mode** — cheerful coral + teal palette in both. The toggle in the
  nav bar remembers the choice (`localStorage`) and defaults to the visitor's
  system preference.
- **Download as PDF** — the "Download PDF" / "PDF" buttons open the browser's
  print dialog with a print stylesheet, so the visitor can save a clean,
  light-themed PDF of the portfolio.
- Responsive layout with a mobile nav.

## Preview locally

Open `portfolio.html` in a browser, or serve the folder:

```bash
python -m http.server 8000
```

Then visit http://localhost:8000/portfolio.html

## Sections

- **Hero** — role summary and headline stats
- **Skills** — Visualization & BI, Database, Programming Languages
- **Experience** — professional timeline
- **Projects** — Power BI dashboards (health sector, NGO, and a consulting PoC)
- **Contact** — email, location, LinkedIn

## Deploying with GitHub Pages

1. Push this repository to GitHub.
2. **Settings → Pages → Source: Deploy from a branch**, branch `main`, folder `/ (root)`.
3. The site publishes at `https://<username>.github.io/portfolio.html`
   (rename the file to `index.html` if you want it served from the bare
   `https://<username>.github.io/` URL).

## Customize

Colors are CSS variables at the top of the `<style>` block in `portfolio.html`:
`:root { ... }` holds the light palette, `:root[data-theme="dark"] { ... }` the
dark one. Update content directly in the markup.
