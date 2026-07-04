# Cherry's Labs

A collaborative project between cherry and el showcasing their projects, programs, and 3D printed creations.

Live at **[cherryslabs.com](http://cherryslabs.com)** (Cloudflare Pages).

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

The site is built and deployed to Cloudflare Pages (project name `cherryslabs-modern`, set in `wrangler.toml`), but `cherryslabs.com`'s DNS currently points at a home IP instead of the Pages project. In practice that means:

- The domain resolves and serves over **plain HTTP**, not HTTPS — there's no TLS cert being served for it right now.
- What actually answers requests is a local `openresty` reverse proxy on the home network, not Cloudflare Pages.
- Deploying with `npx wrangler pages deploy .` still works and updates the Pages project, but that build isn't what's reachable at `cherryslabs.com` until DNS is repointed at Pages.

Fixing this means updating the domain's DNS to point at the Cloudflare Pages project (or Cloudflare proxying to it) instead of the home IP.

## Tech

Pure HTML5/CSS3/JavaScript. No frameworks, no build tools, no dependencies.

`package.json` exists solely so Node-based hosts (Coolify, Vercel, etc.) auto-detect the project and know how to run it — it declares no dependencies. `npm run build` is a no-op (there's nothing to build), and `npm start` serves the repo root as-is via `npx serve` on `$PORT`.

## Contributors

- **cherry** — Projects, content, 3D prints
- **el (elphiene)** — Webmaster, code, maintenance
