# Cherry's Labs

A collaborative project between cherry and el showcasing their projects, programs, and 3D printed creations.

Live at **[cherryslabs.elphiene.com](http://cherryslabs.elphiene.com)** (Cloudflare Pages).

## Quick start

```bash
# Preview locally — no build step
open index.html

# Deploy
npx wrangler pages deploy .
```

## Repo structure

```
.
├── *.html               ← pages (index, hardware, software, store, wiki, design-system)
├── style.css            ← shared stylesheet
├── images/              ← all site assets
├── wiki/                ← individual wiki article pages
├── mockup/              ← design iteration scratch
├── brand/               ← brand brief docs (tone, tokens)
├── linux-pc-package/    ← separate side project: a KDE Plasma desktop theme sharing the site's brand tokens
├── wrangler.toml        ← Cloudflare Pages config
├── .assetsignore        ← controls what actually deploys (separate from .gitignore)
├── package.json         ← only for platform auto-detection (Coolify/Vercel/etc.), see below
└── CONTENT_TEMPLATE.md  ← Cherry fills this in for content
```

## Cloudflare situation

The site is built and deployed to Cloudflare Pages (project name `cherryslabs`, set in `wrangler.toml`). It's now served from `cherryslabs.elphiene.com` instead of `cherryslabs.com`, because `cherryslabs.com`'s DNS lives in Cherry's Cloudflare account (currently pointed at a home IP, not the Pages project) and El can't edit it there. `cherryslabs.elphiene.com` is a subdomain of `elphiene.com`, which El's own Cloudflare account controls, so it can be pointed at the Pages project directly.

Deploying with `npx wrangler pages deploy .` still updates the Pages project as before; the only change is which hostname is wired up to serve it.

## Tech

Pure HTML5/CSS3/JavaScript. No frameworks, no build tools, no dependencies.

`package.json` exists solely so Node-based hosts (Coolify, Vercel, etc.) auto-detect the project and know how to run it — it declares no dependencies. `npm run build` is a no-op (there's nothing to build), and `npm start` serves the repo root as-is via `npx serve` on `$PORT`.

## Contributors

- **cherry** — Projects, content, 3D prints
- **el (elphiene)** — Webmaster, code, maintenance
