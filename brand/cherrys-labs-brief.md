# Cherry's Labs — Design Brief

Reference for El + Claude. Source of truth for the Cherry's Labs visual identity. Tokens below mirror `style.css` `:root` — if they drift, the stylesheet wins.

## Essence

A two-person tech collective (cherry + el) showcasing software, hardware/3D prints, and a wiki. Personality: **dark cyber / retro-futurist, neon-glitch, glassy.** Confident and technical but playful — Y2K-web lineage filtered through a modern glassmorphic UI.

One-liner: *neon-lit lab notebook for two builders.*

## Voice

Lowercase, terse, a little irreverent. Labels are short (`home`, `software`, `wiki`). No corporate gloss. Confident maker energy.

## Colour palette

| Role | Hex | CSS var | Usage |
|---|---|---|---|
| Background | `#000000` | `--color-bg` | Page base, pure black |
| Text | `#ffffff` | `--color-text` | Body copy |
| Primary accent | `#ec4899` | `--color-pink` | Headings, links, glows, hover borders |
| Secondary accent | `#9354d3` | `--color-purple` | Gradients, ambient glow, depth |
| Surface | `#1a1a1a` | `--color-grey` | Card/header base (used translucent) |
| Surface hi | `#2a2a2a` | `--color-grey-light` | Hover surface |

Ambient depth: two faint radial glows on the black bg — **purple top-right, pink bottom-left** (~5% opacity). Pink leads, purple supports. Most accents are pink; purple mostly lives inside gradients and glows.

## Typography

| Role | Font | Notes |
|---|---|---|
| Headings / nav | **Audiowide** | Wide retro-futurist display. All headings, nav, logo lockups |
| Body | **Quantico** | Squared-off techy sans, 16px base, 1.6 line-height |
| Glitch accent | **Rubik Glitch** | Sparingly — special/easter-egg moments only |
| Mono | Courier New | Code, terminal-flavoured bits |

## Visual language

- **Glassmorphism** is the core motif: dark translucent surfaces (`rgba(18–26,…,0.8)`), strong backdrop blur (20px), 1px translucent-white borders.
- **Pink neon glow**: drop-shadows and box-shadows in `rgba(236,72,153,…)`. Logo carries a pink drop-shadow. Headings get a soft white text-glow.
- **Gradient washes**: subtle 135° pink→transparent→purple diagonal across cards and the fixed header.
- **Fixed glass header** with pink-tinted gradient, pink glow shadow, pink bottom border.
- **Motion**: cards fade in staggered (~0.1s each); hovers lift (-2 to -3px) with cubic-bezier easing and layered pink glows; scrolling animated `<title>` in the browser tab.
- **Status tags**: `wip` / `complete` / `abandoned` / `on-hold` as small pills.
- Radius 10px. Spacing scale 8/16/24/40/60.

## Logo

Current asset: `images/logos/cherrys-labs.png` (wordmark, ~250px in header, pink glow). Also `cherrys-labs-200R.png`.

Direction for the redesign:
- **Wordmark in Audiowide** (or a close custom cut), lowercase `cherry's labs`.
- Must read on pure black with a pink neon glow.
- Produce a **vector SVG master**, then export PNG @1x/2x + favicon/app-icon sizes.
- Optional mark: a small glyph (cherry, flask/lab motif, or pixel glitch) usable standalone as favicon/avatar.

## Asset checklist (to-do)

- **Logo** — SVG master + PNG exports + favicon set. Dark-bg, pink glow.
- **Wallpaper** — black base, purple/pink ambient glows, glass + glitch accents. Desktop 1920×1080 & 2560×1440, plus mobile.
- **Screensaver** — pick format (animated/video vs. image slideshow) + target OS. Lean into the neon-glitch + scrolling-text motif.
- **Business cards** — 90×55mm (AU), 3mm bleed, CMYK, 300dpi, front/back. Black card, pink foil/neon wordmark feel. Needs a **vector, CMYK** logo — note that screen pink `#ec4899` shifts in CMYK; proof it.

## Do / Don't

- **Do**: pure black, pink-led with purple support, glass surfaces, soft neon glow, lowercase, Audiowide headings.
- **Don't**: light backgrounds, flat material-style cards, heavy Rubik Glitch everywhere, drop the glow (it's the signature), title-case nav.
