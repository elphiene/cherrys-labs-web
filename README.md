# Cherry's Labs

A collaborative project between cherry and el showcasing their projects, programs, and 3D printed creations.

Live at **[cherryslabs.com](https://cherryslabs.com)** (Cloudflare Pages).

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
├── *.html              ← pages (index, hardware, software, store, wiki)
├── style.css           ← shared stylesheet
├── images/             ← all site assets
├── wiki/               ← individual wiki article pages
├── mockup/             ← design iteration scratch
├── wrangler.toml       ← Cloudflare Pages config
└── CONTENT_TEMPLATE.md ← Cherry fills this in for content
```

## Tech

Pure HTML5/CSS3/JavaScript. No frameworks, no build tools, no dependencies.

## Contributors

- **cherry** — Projects, content, 3D prints
- **el (elphiene)** — Webmaster, code, maintenance
