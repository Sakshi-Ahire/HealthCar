# HealthCar.co — Mike Danielson | HealthCar

Static, dependency-free site. `node build.mjs` regenerates `site/` from `src/content.mjs` (all approved copy).
Deploy: upload the contents of `site/` to any static host (Hostinger/GoDaddy/Netlify/Vercel). Preview: the `healthcar` entry in `.claude/launch.json` (port 8590).

## Before launch (set in build.mjs `CFG`)
- `calendly` — Mike's Calendly URL (Contact page button)
- `contactEmail` / `formEndpoint` — contact form target (mailto fallback if no endpoint)
- `showQuoteNames` — flip to true as each quote permission arrives (names/titles are already in content.mjs)
- Optional `src/story-body.html` — the approved "What Inspired This" one-pager (The Story page body)
- Replace `site/assets/mike-hero.*` with the new headshot when ready; register mikedanielson.com and 301 to healthcar.co
- About photo tiles are hidden until real photos exist: set `showPhotos: true` in `build.mjs` `CFG`, then drop images into `.photo[data-slot]`
