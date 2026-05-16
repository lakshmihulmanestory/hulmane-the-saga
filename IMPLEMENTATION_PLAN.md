# Hulmane The Saga — Implementation Plan

> Created: 2026-05-11 | Refer to REQUIREMENTS.md for full requirements
> Use this file to track progress across sessions. Mark [x] when done.

---

## How to Resume After a Break

1. Open this file — check which Phase you are on
2. Find the first unchecked `[ ]` item
3. Read REQUIREMENTS.md Section that corresponds to the phase
4. Continue from there

---

## Phase 0 — Documentation ✅ COMPLETE

- [x] Write REQUIREMENTS.md
- [x] Write IMPLEMENTATION_PLAN.md (this file)

---

## Phase 1 — Root Master Index

**Goal:** Create a master `index.html` at git root (`/hulmane-the-saga/index.html`) that shows all volumes as tiles. Volume 1 is active; others are "Coming Soon."

**File:** `/hulmane-the-saga/index.html`

- [ ] Create `/hulmane-the-saga/index.html`
  - Title: "Hulmane The Saga — The Eternal Assembly"
  - Show 6 volume/season tiles in a grid
  - Volume 1 tile: active, links to `hulmane-the-saga-volume-1/index.html`
  - Volumes 2–6: coming soon (greyed out, no link)
  - Include the motto image and project branding
  - Standalone CSS (inline or minimal) — no dependency on old style.css

---

## Phase 2 — Create Volume 1 Folder & Move Shared Assets

**Goal:** Create `hulmane-the-saga-volume-1/` at git root. Move CSS, JS, data, shared HTML pages into it.

**Files to create/move:**

- [ ] Create directory: `hulmane-the-saga-volume-1/`
- [ ] Copy `com/hulmane/hulmane-the-saga/css/style.css` → `hulmane-the-saga-volume-1/css/style.css`
- [ ] Copy all JS files → `hulmane-the-saga-volume-1/js/`
- [ ] Copy all data files → `hulmane-the-saga-volume-1/data/`
- [ ] Create `hulmane-the-saga-volume-1/index.html` (Volume 1 home — adapt from old index.html)
  - Nav: Home | Kingdoms | Heroes | Council | Map
  - Links updated to new paths
- [ ] Copy `characters.html` → `hulmane-the-saga-volume-1/characters.html` (update nav + links)
- [ ] Copy `character-gallery.html` → `hulmane-the-saga-volume-1/character-gallery.html`
- [ ] Copy `mahabharata_family_tree.html` → `hulmane-the-saga-volume-1/mahabharata-family-tree.html`
- [ ] Copy `galactic-threat.html` → `hulmane-the-saga-volume-1/galactic-threat.html`
- [ ] Copy `media/images/hulmane-the-saga-motto.png` → `hulmane-the-saga-volume-1/media/shared/hulmane-the-saga-motto.png`
- [ ] Copy `media/backup/` → `hulmane-the-saga-volume-1/media/shared/tattoo-reference/`

---

## Phase 3 — Create Kingdom Folder Structure (28 Kingdoms)

**Goal:** Create all kingdom folders under `bharatavarsha/regions/[region]/kingdoms/[kingdom]/` with empty placeholder pages and `media/` subdirectories.

- [ ] Create base: `hulmane-the-saga-volume-1/bharatavarsha/`
- [ ] Create: `hulmane-the-saga-volume-1/bharatavarsha/regions/`

**South Region (5 kingdoms):**
- [ ] `regions/south/kingdoms/karnataka/` with index.html, identity.html, story.html, rules.html, media/{emblem,portraits,vehicles,weapons,tattoo}/
- [ ] `regions/south/kingdoms/kerala/` (same structure)
- [ ] `regions/south/kingdoms/tamil-nadu/` (same structure)
- [ ] `regions/south/kingdoms/andhra-pradesh/` (same structure)
- [ ] `regions/south/kingdoms/telangana/` (same structure)

**West Region (4 kingdoms):**
- [ ] `regions/west/kingdoms/maharashtra/`
- [ ] `regions/west/kingdoms/gujarat/`
- [ ] `regions/west/kingdoms/goa/`
- [ ] `regions/west/kingdoms/rajasthan/`

**East Region (4 kingdoms):**
- [ ] `regions/east/kingdoms/west-bengal/`
- [ ] `regions/east/kingdoms/odisha/`
- [ ] `regions/east/kingdoms/bihar/`
- [ ] `regions/east/kingdoms/jharkhand/`

**North Region (5 kingdoms):**
- [ ] `regions/north/kingdoms/uttar-pradesh/`
- [ ] `regions/north/kingdoms/uttarakhand/`
- [ ] `regions/north/kingdoms/himachal-pradesh/`
- [ ] `regions/north/kingdoms/punjab/`
- [ ] `regions/north/kingdoms/haryana/`

**Northeast Region (8 kingdoms):**
- [ ] `regions/northeast/kingdoms/assam/`
- [ ] `regions/northeast/kingdoms/arunachal-pradesh/`
- [ ] `regions/northeast/kingdoms/manipur/`
- [ ] `regions/northeast/kingdoms/meghalaya/`
- [ ] `regions/northeast/kingdoms/mizoram/`
- [ ] `regions/northeast/kingdoms/nagaland/`
- [ ] `regions/northeast/kingdoms/sikkim/`
- [ ] `regions/northeast/kingdoms/tripura/`

**Central Region (2 kingdoms):**
- [ ] `regions/central/kingdoms/madhya-pradesh/`
- [ ] `regions/central/kingdoms/chhattisgarh/`

---

## Phase 4 — Kingdoms Overview Page

**Goal:** Create `hulmane-the-saga-volume-1/kingdoms.html` — "Kingdoms of Bharatavarsha"

- [ ] Create `hulmane-the-saga-volume-1/kingdoms.html`
  - Title: "Kingdoms of Bharatavarsha"
  - Sections by region: South | West | East | North | Northeast | Central
  - Each kingdom shown as a card: name, hero name, sacred animal, region
  - Cards link to `bharatavarsha/regions/[region]/kingdoms/[kingdom]/index.html`
  - Pull data from `js/kingdom-identity-data.js`
  - No "state" word anywhere on page

---

## Phase 5 — Karnataka Kingdom Pages (First Full Example)

**Goal:** Build Karnataka as the first complete kingdom — all 4 pages + media.

Karnataka folder: `bharatavarsha/regions/south/kingdoms/karnataka/`

- [ ] `index.html` — Kingdom overview (hero summary, quick links, emblem preview)
- [ ] `identity.html` — Full identity (migrate + enhance from old `kingdom-identity.html` Karnataka section)
- [ ] `story.html` — Kingdom story (migrate from old `karnataka-story.html`)
- [ ] `rules.html` — Tattoo evolution + Weapons
- [ ] Copy media:
  - [ ] `media/images/south/karnataka/karnataka-portrait.svg` → `karnataka/media/portraits/karnataka-hero-portrait.svg`
  - [ ] Relevant emblems from `media/emblems/` → `karnataka/media/emblem/karnataka-royal-emblem.png`
  - [ ] Relevant vehicle art → `karnataka/media/vehicles/`
  - [ ] Relevant weapon art → `karnataka/media/weapons/`
  - [ ] Tattoo art from backup → `karnataka/media/tattoo/`

---

## Phase 6 — Remaining South Kingdom Pages

**Goal:** Build Kerala, Tamil Nadu, Andhra Pradesh, Telangana (same structure as Karnataka).

- [ ] Kerala — 4 pages + media folder structure
- [ ] Tamil Nadu — 4 pages + media folder structure
- [ ] Andhra Pradesh — 4 pages + media folder structure
- [ ] Telangana — 4 pages + media folder structure

---

## Phase 7 — West, East, North, Northeast, Central Kingdom Pages

**Goal:** Build all remaining 23 kingdoms. Use the same 4-page structure. Content can be "Coming Soon" placeholder with correct branding, or filled from CSV data.

- [ ] West: Maharashtra, Gujarat, Goa, Rajasthan (4 kingdoms)
- [ ] East: West Bengal, Odisha, Bihar, Jharkhand (4 kingdoms)
- [ ] North: Uttar Pradesh, Uttarakhand, Himachal Pradesh, Punjab, Haryana (5 kingdoms)
- [ ] Northeast: Assam, Arunachal Pradesh, Manipur, Meghalaya, Mizoram, Nagaland, Sikkim, Tripura (8 kingdoms)
- [ ] Central: Madhya Pradesh, Chhattisgarh (2 kingdoms)

---

## Phase 8 — Council Pages

**Goal:** Create Volume 1 Grand Council page.

- [ ] `hulmane-the-saga-volume-1/council.html`
  - Volume 1 Bharat Varsha Grand Council
  - Shows council circle for Volume 1 kingdoms
  - Migrate / adapt from old `council.html`
- [ ] Add placeholder for Global Council (link from master index.html)

---

## Phase 9 — Bharat Shanshant Map Page

**Goal:** Create the global map page for Volume 1.

- [ ] `hulmane-the-saga-volume-1/bharatavarsha/global-map.html`
  - Title: "Bharat Shanshant"
  - Interactive map with 6 regions highlighted
  - Click region → scrolls/links to that region's kingdoms
  - Adapt from old `js/india-map.js`

---

## Phase 10 — Media Migration (Full)

**Goal:** Copy all existing media from old `com/` structure into kingdom-specific folders with clean naming.

**Source locations:**
- `com/hulmane/hulmane-the-saga/media/images/[region]/[kingdom]/`
- `com/hulmane/hulmane-the-saga/media/emblems/`
- `com/hulmane/hulmane-the-saga/media/ancient-vehicles/`
- `com/hulmane/hulmane-the-saga/media/ancient-weapons/`

**Target:** `bharatavarsha/regions/[region]/kingdoms/[kingdom]/media/[type]/[kingdom]-[subject].[ext]`

- [ ] Map old emblem files to specific kingdoms (emblems are named by grid position — need to identify which is which)
- [ ] Map old vehicle files to kingdoms
- [ ] Map old weapon files to kingdoms
- [ ] Rename all files to descriptive names
- [ ] Update all HTML `src=` paths after migration

---

## Phase 11 — Cleanup

**Goal:** Remove old `com/` directory once everything is verified in new structure.

- [ ] Verify all pages in new structure open correctly
- [ ] Verify all links work (no broken hrefs)
- [ ] Verify all images load (no broken src paths)
- [ ] Archive old `com/` directory (or delete after git commit backup)
- [ ] Update `docs/CLAUDE.md` or `com/hulmane/hulmane-the-saga/CLAUDE.md` → move to root `CLAUDE.md`

---

## Progress Tracker

| Phase | Description | Status |
|-------|-------------|--------|
| 0 | Documentation | ✅ Done |
| 1 | Root master index.html | ✅ Done |
| 2 | Volume 1 folder + shared assets | ✅ Done |
| 3 | 28 kingdom folder structure | ✅ Done |
| 4 | Kingdoms overview page | ✅ Done |
| 5 | Karnataka full pages (4 pages + media) | ✅ Done |
| 6 | All 27 remaining kingdoms (placeholder 4-page sets) | ✅ Done |
| 7 | West/East/North/Northeast/Central kingdoms | ✅ Done (placeholders) |
| 8 | Council page (volume-1/council.html) | ✅ Done |
| 9 | Bharat Shanshant map page | ✅ Done |
| 10 | Media migration (Karnataka complete, others TBD) | 🔄 Partial — Karnataka done |
| 11 | Cleanup old com/ structure | ⬜ Not started — verify first |

---

## Session Log

| Date | Session | Completed |
|------|---------|-----------|
| 2026-05-11 | Session 1 | Phase 0 — Requirements + Plan written |
| 2026-05-11 | Session 1 (cont.) | Phases 1–9 complete. New structure fully built. Karnataka is the first complete kingdom. All 27 others have 4 placeholder pages each. |

---

## Next Session — Where to Resume

**Start here next time:**
- Phase 10: Media migration for remaining kingdoms
  - South: Copy existing state media for Andhra Pradesh, Kerala, Tamil Nadu, Telangana into their kingdom folders
  - Check `com/hulmane/hulmane-the-saga/media/states/` for which kingdoms have existing media
  - Assign emblem images from `media/emblems/` (grid-named files) to specific kingdoms
  - Assign vehicle images from `media/ancient-vehicles/` to specific kingdoms
  - Phase 11: After full verification, archive or remove old `com/` directory

---

## Notes / Decisions

- Karnataka is chosen as the "first full kingdom" because it has the most existing content (portrait.svg, story.html, karnataka-portrait.html)
- Emblem files are currently named by grid position (emblems_r1_c1.png etc) — mapping to kingdoms is a manual task needed in Phase 10
- The old `com/hulmane/hulmane-the-saga/js/kingdom-identity-data.js` contains all 28 kingdom identity records — reuse this data, do not rewrite
- Media files for vehicles/weapons in old structure are not per-kingdom yet — they are generic ancient-vehicles/ancient-weapons — assignment to kingdoms will be done during Phase 10
