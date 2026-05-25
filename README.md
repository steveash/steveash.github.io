# manycupsofcoffee.com

Personal website for Steve Ash, live at **https://www.manycupsofcoffee.com**.

It's a single-page professional presence site — a short bio, profile links
(LinkedIn, GitHub, Google Scholar, email), and a "Selected work" list — plus a
frozen archive of the old 2009–2016 blog kept reachable for posterity.

## Stack

- **[Astro](https://astro.build/)** (static output), no UI framework — plain CSS.
- Build-time image optimization via `astro:assets` (`sharp`).
- `@astrojs/sitemap` for `sitemap-index.xml`.
- Hosted on **GitHub Pages**, deployed by **GitHub Actions**.
- Custom domain `www.manycupsofcoffee.com` (`public/CNAME`).

## Project layout

```
src/
  pages/
    index.astro      # the landing page (bio, links, selected work)
    404.astro        # styled not-found page
  layouts/
    Base.astro       # <head>, meta/OG tags, GA4 analytics
  styles/global.css  # all styling (light/dark, accent, motion)
  assets/me-2018.jpg # avatar (optimized at build time)
public/              # served verbatim, no processing:
  CNAME, robots.txt, favicon.*
  posts/ talks/ about/ assets/ reveal.js/ + per-post slug dirs
                     # ^ the frozen Jekyll-era blog archive
astro.config.mjs     # site URL + integrations
.github/workflows/deploy.yml  # CI build + deploy
```

## Local setup

Requires **Node 20+** (CI uses Node 22).

```bash
npm install
```

## Local dev / test

```bash
npm run dev       # http://localhost:4321 — live reload while editing
npm run build     # production build into dist/
npm run preview   # serve the built dist/ at http://localhost:4321
```

There is no test suite; `npm run build` is the check — it must complete without
errors before deploying.

> **Tip:** the archive's directory-style URLs (e.g. `/posts/`) 404 under
> `npm run dev` (a quirk of how the dev server serves `public/`), but work under
> `npm run preview` and in production. Use `preview` to verify archive links.

### Editing common things

- **Bio, links, selected work:** `src/pages/index.astro` (plain data arrays).
- **Look & feel:** `src/styles/global.css` (colors/motion are CSS variables at top).
- **Analytics:** `GA_ID` in `src/layouts/Base.astro` (GA4).
- **An old blog post:** edit the static HTML directly under `public/` — the
  archive is pre-rendered and is **not** rebuilt from any Jekyll source.

## Dev cycle

1. `npm run dev` and edit.
2. `npm run build` to confirm a clean production build (`npm run preview` to
   spot-check, especially archive links).
3. Commit and push to `master`.

## Deployment

Fully automated. **Pushing to `master` deploys** — the
`.github/workflows/deploy.yml` workflow runs `npm ci && npm run build` and
publishes `dist/` to GitHub Pages (~30s). No manual steps.

GitHub Pages is configured with **Source = "GitHub Actions"** (not the legacy
branch build). The custom domain lives in both the Pages settings and
`public/CNAME` (single primary domain, `www.manycupsofcoffee.com`); the apex
`manycupsofcoffee.com` redirects to it via DNS.
