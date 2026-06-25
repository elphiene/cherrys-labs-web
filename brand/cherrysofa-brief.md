# Cherrysofa — Design Brief

Reference for El + Claude. Cherrysofa is the **self-hosted media streaming/archiving platform** (Jellyfin-based) by cherry. It's a sibling of [Cherry's Labs](./cherrys-labs-brief.md) — **same palette and vibe, warmer personality.**

## Essence

cherry + sofa: a **cozy, late-night couch media player.** Where Cherry's Labs is the neon lab, Cherrysofa is the dim living room at 1am — same dark glassy neon DNA, but softer, comfier, screen-glow warm. Think: the glow of a TV on a dark wall, a comfy couch, a bowl of cherries.

One-liner: *your late-night couch, always streaming.*

## Voice

Same lowercase, warm, unpretentious tone as Cherry's Labs — but cozier and more inviting. "settle in" over "boot up."

## Relationship to Cherry's Labs

Shared (keep cohesion): black backgrounds, glassmorphism, pink `#ec4899` + purple `#9354d3`, soft neon glow, Audiowide/Quantico type.

Diverged (its own personality):
- **Warmer & softer** — lean pink a touch warmer/cherry-red; let purple play a bigger, ambient "ambient room light" role.
- **Cozier shapes** — slightly rounder corners, softer glows, less hard-edged glitch than the Labs brand.
- **Screen-glow motif** — the feeling of a screen lighting a dark room (vignette + central warm glow) rather than the Labs' lab-bench neon.
- Motifs: **cherry** + **sofa/couch** silhouette, play triangle, late-night/moon hints.

## Colour palette

Inherits Cherry's Labs tokens. Adjustments:

| Role | Hex | Notes |
|---|---|---|
| Background | `#000000` / near-black | Page + Jellyfin dark UI |
| Primary accent | `#ec4899` (→ optionally warmer, e.g. `#f0517d`) | Cherry pink/red |
| Secondary accent | `#9354d3` | Ambient room glow — used more generously here |
| Warm highlight | optional amber/cherry-red | Cozy "lamp" warmth, sparingly |

Ambient: a soft central screen-glow (warm pink) fading to black at the edges (vignette), purple haze around it.

## Typography

Match Cherry's Labs for family cohesion: **Audiowide** display, **Quantico** body. Cherrysofa may use a slightly softer/rounder display for the logo if Audiowide reads too rigid for "cozy" — keep Quantico for UI text either way.

## Logo

Greenfield. Direction:
- Wordmark `cherrysofa` (one word, lowercase).
- Combine **cherry + sofa**: e.g. a couch silhouette with a cherry, or a cherry whose stem/leaf doubles as a play button, or a sofa under a warm screen-glow.
- **Must work on a dark UI** — Jellyfin's interface is dark. Pink/warm glow on black.
- Deliver **SVG master** → PNG @1x/2x, favicon, plus a square app-icon/avatar version for the Jellyfin server.

## Asset checklist (to-do)

- **Logo** — SVG master + exports + favicon + square server icon. Dark-bg, warm glow.
- **Wallpaper** — cozy late-night scene: screen-glow vignette, couch/cherry motif, purple ambient haze. Sizes: Jellyfin login/backdrop, desktop 1920×1080 & 2560×1440, mobile.
- **Metadata** — *(separate workstream, not a design asset)* — the Jellyfin library cleanup pass covered in the execution plan.

## Do / Don't

- **Do**: dark + glass + neon (shared with Labs), but warmer, softer, cozier; screen-glow vignette; cherry + couch motifs; readable on Jellyfin's dark UI.
- **Don't**: drift so far it stops feeling related to Cherry's Labs; go bright/daytime; hard glitchy edges; light logo that disappears on a dark player.
