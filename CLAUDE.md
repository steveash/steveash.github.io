# CLAUDE.md

Personal presence site for Steve Ash, served at **manycupsofcoffee.com** (see `public/CNAME`) from GitHub Pages (`steveash.github.io`).

## Stack

**Astro** (static output), no UI framework, plain CSS in `src/styles/global.css`. The site is a single landing page (`src/pages/index.astro`): bio, links (LinkedIn, GitHub, Google Scholar, email), and a "Selected work" list. `src/layouts/Base.astro` holds the `<head>`, meta/OG tags, and GA4. The avatar (`src/assets/me-2018.jpg`) is optimized at build time via `astro:assets` (downscaled, WebP, Exif stripped). `@astrojs/sitemap` generates `sitemap-index.xml`; `public/robots.txt` points at it. A styled `src/pages/404.astro` is served as `404.html`.

Analytics is GA4 — `GA_ID` in `src/layouts/Base.astro` (currently `G-VRLC5PYCRF`); while it's the `G-XXXXXXXXXX` placeholder the snippet is omitted.

## Local development

```
npm install
npm run dev      # http://localhost:4321
npm run build    # outputs to dist/
```

## Deploy

GitHub Actions (`.github/workflows/deploy.yml`) builds on push to `master` and publishes `dist/`. **One-time setup:** in repo Settings → Pages, set Source to "GitHub Actions" (it previously used the native Jekyll build).

## The /posts archive

The old 2009–2016 Jekyll blog is frozen as static HTML under `public/` (`public/posts/`, the per-post slug dirs, `public/talks/`, `public/about/`, `public/assets/`, `public/reveal.js`). These are pre-rendered pages served verbatim, linked from the landing-page footer. They are **not** rebuilt from any Jekyll source (which has been removed) — to change a post, edit the HTML in `public/` directly. The park-photo background was replaced with a solid `#f7e3d3` across all archived pages.
