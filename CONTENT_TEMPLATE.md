# Content Template

Fill this file in with your content. Claude will use it to populate the site pages.
Leave a field blank or write `TBD` if you don't have it yet.

---

## Homepage (`index.html`)

### Site intro
> Short tagline or description shown at the top of the page.

```
[FILL IN: 1–2 sentence description of Cherry's Labs]
```

### Cherry's card
```
Name: Cherry
Pronouns: [FILL IN]
Role/tagline: [FILL IN — e.g. "founder, hardware tinkerer"]
Bio: [FILL IN — 2–4 sentences]
Links:
  - GitHub: [FILL IN]
  - [other]: [FILL IN]
Photo: [filename in modern/images/photos/ — or TBD]
```

### El's card
```
Name: El
Pronouns: they/them
Role/tagline: [FILL IN — e.g. "developer, software side"]
Bio: [FILL IN — 2–4 sentences]
Links:
  - GitHub: https://github.com/elphiene
  - [other]: [FILL IN]
Photo: [filename in modern/images/photos/ — or TBD]
```

---

## Projects page (`projects.html`)

> One block per project. Copy and repeat the block for each project.

```
--- PROJECT ---
Name: [FILL IN]
Status: [WIP / Complete / On Hold]
Description: [FILL IN — 1–3 sentences]
Tags: [e.g. Hardware, Python, SteamOS]
GitHub: [URL or TBD]
Live URL: [URL or N/A]
Image: [filename in modern/images/projects/ — or TBD]
---------------
```

Existing (already on site):
- Tidal-Collaborative — WIP — needs image

---

## Programs page (`programs.html`)

> One block per program. Existing entries are listed below — add new ones.

```
--- PROGRAM ---
Name: [FILL IN]
Status: [WIP / Complete]
Platform: [e.g. SteamOS/Linux, Web, Windows]
Description: [FILL IN — 1–3 sentences]
Tags: [e.g. Rust, HTML, Python]
GitHub: [URL or TBD]
Screenshot: [filename in modern/images/programs/ — or TBD]
---------------
```

Existing (already on site):
- Tidal-Collaborative — WIP — SteamOS/Linux
- Deckcraft — WIP — SteamOS/Linux — **GitHub link missing**
- Non-Steam-Grid-Generator — Complete — Web (HTML)
- DockSwitch — Complete — SteamOS/Linux

---

## Store page (`store.html`)

> One block per product. Copy and repeat.

```
--- PRODUCT ---
Name: [FILL IN]
Price: [FILL IN — e.g. $12.00 AUD]
Description: [FILL IN — 1–2 sentences]
Category: [e.g. 3D Print, Gadget, Tech]
Stock: [In Stock / Made to Order / Coming Soon]
Photo: [filename in modern/images/products/ — or TBD]
---------------
```

---

## Wiki pages (`modern/wiki/`)

> Fill in the development notes for each project's wiki article.

### deckcraft
```
Tech stack:
  Language: [FILL IN]
  Framework: [FILL IN]
  Key dependencies: [FILL IN]

Development notes:
  [FILL IN — design decisions, known issues, roadmap, anything useful]

GitHub: [URL — TBD]
```

### dockswitch
```
Tech stack:
  Language: Rust
  Target: SteamOS / Linux
  Key crates/libraries: [FILL IN — e.g. udev for dock events]
  Systemd integration: [FILL IN]

Development notes:
  [FILL IN — design decisions, how dock events are detected, known issues, roadmap]

GitHub: https://github.com/CherryGaySoda/DockSwitch
```

### non-steam-grid-generator
```
Tech stack:
  Language: HTML/CSS/JavaScript (no frameworks, browser-only)
  Key browser APIs: [FILL IN — e.g. Canvas API, File API]
  Image processing: [FILL IN]

Development notes:
  [FILL IN — design decisions, known issues, roadmap]

GitHub: https://github.com/CherryGaySoda/Non-Steam-Grid-Generator
```

### tidal-collaborative
```
Tech stack:
  Backend: Node.js (Express + WebSocket)
  Database: SQLite
  Deployment: Docker (node:20-alpine, amd64 + arm64)
  Key dependencies: [FILL IN]
  Architecture: [FILL IN — e.g. how the real-time sync works]
  Database schema notes: [FILL IN]

Development notes:
  [FILL IN — design decisions, known issues, roadmap]

GitHub: https://github.com/elphiene/tidal-collaborative
```
