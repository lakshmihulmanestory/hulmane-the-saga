---
name: Character Gallery System
description: SVG portrait gallery added for all 28 kingdoms — hero, villain, animal, weapons, Hindu god inspiration
type: project
---

Added on 2026-05-04: A full character portrait gallery system.

**Files created:**
- `js/portrait-renderer.js` (648 lines) — Contains:
  - `window.VILLAIN_DATA` — All 28 villain names, titles, weapons, dark deity
  - `window.MODERN_WEAPONS` — Modern weapon upgrades for all 28 heroes
  - `window.DEITY_DATA` — Hindu god/Mahabharata inspiration for all 28 heroes
  - `drawAnimal()` — SVG animal silhouettes for all 20+ animal types
  - `drawFigure()` — Hero/villain figure with deity-specific crown
  - `drawEnvironment()` — Regional background (mountains/water/desert/forest)
  - `drawWeaponIcon()` — Weapon silhouettes
  - `drawMandalaBorder()` — Hindu mandala decorative ring
  - `renderKingdomPortrait()` — Generates 820x500 SVG portrait card
  - `initPortraitGallery()` — Renders full gallery to a container

- `character-gallery.html` (420 lines) — Gallery page with:
  - Filter buttons by region (all 6 regions)
  - Portrait grid (each card = hero+villain side by side, animal, weapons, deity)
  - Fullscreen modal with detailed hero/villain info + link to story page
  - Weapons strip showing traditional + villain + modern upgrade

**Why:** User requested images showing the animal, hero, villain, and modern weapons for each kingdom, inspired by Hindu gods and Mahabharata characters.
