# Azimatul Matsniya — Business Intelligence Portfolio

A single-page portfolio website for a Business Intelligence Engineer role.
Built as a static HTML page — no build step, no dependencies.

## Contents

- `index.html` — the full site (HTML + CSS + a small amount of JS, all inline)

## Preview locally

Just open `index.html` in a browser, or serve the folder:

```bash
python -m http.server 8000
```

Then visit http://localhost:8000

## Sections

- **Hero** — role summary and headline stats
- **Skills** — Visualization & BI, Database, Programming Languages
- **Experience** — professional timeline
- **Projects** — three BI case studies (Power BI, Apache Superset, Python)
- **Contact** — email, location, LinkedIn

## Deploying with GitHub Pages

1. Push this repository to GitHub.
2. In the repo, go to **Settings → Pages**.
3. Set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`.
4. The site publishes at `https://<username>.github.io/<repo>/`
   (or `https://<username>.github.io/` if the repo is named `<username>.github.io`).

## Customize

Colors and fonts are defined as CSS variables at the top of the `<style>` block
in `index.html` (`--bg`, `--amber`, `--serif`, etc.). Update content directly in
the markup.
