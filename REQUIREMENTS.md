# Hulmane The Saga — Project Requirements

> Captured: 2026-05-11 | Author: Lakshmi Hulmane | Status: ACTIVE

---

## 1. Universe Structure — Multi-Volume Series

The project is a multi-volume saga covering different continents. Each volume is a self-contained season.

| Volume | Name | Continent | Status |
|--------|------|-----------|--------|
| Volume 1 | Bharat Varsha | Indian Subcontinent | **Active — Build Now** |
| Volume 2 | Europe Hulmane Saga | Europe | Coming Soon |
| Volume 3 | Asian Hulmane Saga | Remaining Asia | Coming Soon |
| Season 4 | American Hulmane Saga | American Continent | Coming Soon |
| Season 5 | Australia Hulmane Saga | Australia Continent | Coming Soon |
| Season 6 | African Hulmane Saga | African Continent | Coming Soon |

---

## 2. Root-Level Structure

- `index.html` stays at **git root** — this is the **master index page** showing all volumes/seasons as tiles
- Non-Volume-1 entries appear as "Coming Soon" tiles
- A folder `hulmane-the-saga-volume-1/` lives at git root level
- All Volume 1 content lives inside `hulmane-the-saga-volume-1/`

```
/hulmane-the-saga/                        ← git root
├── index.html                            ← Master index (all volumes)
├── REQUIREMENTS.md                       ← This file
├── IMPLEMENTATION_PLAN.md                ← Phased build plan
├── hulmane-the-saga-volume-1/            ← Volume 1 (Bharat Varsha)
│   ├── index.html                        ← Volume 1 home page
│   ├── kingdoms.html                     ← Kingdoms of Bharatavarsha (overview)
│   ├── council.html                      ← Volume 1 Grand Council
│   ├── characters.html                   ← Heroes gallery
│   ├── css/
│   ├── js/
│   ├── data/
│   └── bharatavarsha/                    ← The world of Volume 1
│       ├── global-map.html               ← Bharat Shanshant Map
│       └── regions/
│           ├── south/kingdoms/[kingdom]/
│           ├── north/kingdoms/[kingdom]/
│           ├── east/kingdoms/[kingdom]/
│           ├── west/kingdoms/[kingdom]/
│           ├── central/kingdoms/[kingdom]/
│           └── northeast/kingdoms/[kingdom]/
├── docs/                                 ← Keep as-is
├── project_planning/                     ← Keep as-is
└── com/                                  ← OLD structure (migrate then remove)
```

---

## 3. Kingdoms — Terminology & Organization

- **No "states" anywhere.** The word "state" is replaced with "kingdom" everywhere.
- 28 kingdoms total in Volume 1 (Bharat Varsha), organized into 6 regions:

| Region | Kingdoms |
|--------|----------|
| South | Andhra Pradesh · Telangana · Tamil Nadu · Kerala · Karnataka |
| West | Maharashtra · Gujarat · Goa · Rajasthan |
| East | West Bengal · Odisha · Bihar · Jharkhand |
| North | Uttar Pradesh · Uttarakhand · Himachal Pradesh · Punjab · Haryana |
| Northeast | Assam · Arunachal Pradesh · Manipur · Meghalaya · Mizoram · Nagaland · Sikkim · Tripura |
| Central | Madhya Pradesh · Chhattisgarh |

---

## 4. Kingdoms Overview Page (`kingdoms.html`)

- Title: **"Kingdoms of Bharatavarsha"**
- This is a **high-level preview** page — not detail pages
- Shows all 28 kingdoms as cards/tiles, organized by region
- Each card links to that kingdom's dedicated folder/page
- Map of Bharat Shanshant with kingdoms distributed on it
- No "states" language

---

## 5. Per-Kingdom Folder Structure

Each kingdom gets its own dedicated folder with the following:

```
bharatavarsha/regions/south/kingdoms/karnataka/
├── index.html          ← Kingdom overview / landing page
├── identity.html       ← Emblem, colors, motto, sacred animal, hero, villain
├── story.html          ← Kingdom story / narrative arc
├── rules.html          ← Tattoo evolution + Weapons (design, how it works)
└── media/
    ├── emblem/         ← Kingdom emblem images
    ├── portraits/      ← Hero / villain portraits
    ├── vehicles/       ← Kingdom vehicle art
    ├── weapons/        ← Weapon art
    └── tattoo/         ← Tattoo progression art
```

- **All media for a kingdom lives inside that kingdom's `media/` folder**
- Media filenames must be descriptive: `karnataka-hero-portrait.png`, `karnataka-royal-emblem.svg`, etc.
- Copy relevant files from old scattered locations into each kingdom's media folder

---

## 6. Kingdom Pages — Content Rules

### `index.html` (Kingdom Landing)
- Overview card: name, region, hero name, villain name, sacred animal
- Quick links to identity, story, rules pages
- Preview of emblem and hero portrait

### `identity.html` (Kingdom Identity)
- Full kingdom identity: emblem, colors, motto, sacred animal + bird
- Hero profile (name, deity, weapon, guru)
- Villain profile (dark version)
- Tattoo current level indicator

### `story.html` (Kingdom Story)
- Main narrative arc
- Sub-stories
- Links to related kingdoms

### `rules.html` (Kingdom Rules)
- **Tattoo section**: how tattoos evolve for this kingdom's hero (footprint → leg → half body → full body)
- **Weapons section**: weapon design, how it works, sacred origin
- Visual progression charts

---

## 7. The Map

- The global map within Volume 1 is called **"Bharat Shanshant"** (not "India map")
- Kingdoms are distributed inside this map
- Each region is highlighted, kingdoms clickable

---

## 8. Council Pages

- Each volume has its **own council page** with its own circle of council members
- Volume 1 council → `hulmane-the-saga-volume-1/council.html`
- A **global council page** at the master level will eventually contain all volumes' councils
- Council page is NOT per-kingdom — it is per-volume (and eventually global)

---

## 9. Media Organization Rules

- Media belongs **inside the kingdom's own folder** — not in a central media/ directory
- File naming convention: `[kingdom-slug]-[subject]-[type].[ext]`
  - Example: `karnataka-hero-portrait.png`
  - Example: `karnataka-royal-emblem.svg`
  - Example: `karnataka-tattoo-level-1.png`
  - Example: `karnataka-vehicle-war-elephant.png`
  - Example: `karnataka-weapon-trishula.png`
- When migrating, copy from old locations; do not just move (verify first)

---

## 10. Navigation Structure (Volume 1)

```
Master Root index.html
  └── hulmane-the-saga-volume-1/
        Volume 1 Nav:
          Home | Kingdoms | Heroes | Council | Bharat Shanshant Map
```

Volume 1 nav links:
- **Home** → `volume-1/index.html`
- **Kingdoms** → `volume-1/kingdoms.html` (all 28, by region)
- **Heroes** → `volume-1/characters.html`
- **Council** → `volume-1/council.html`
- **Map** → `volume-1/bharatavarsha/global-map.html`

---

## 11. What Changes from Old Structure

| Old | New |
|-----|-----|
| `com/hulmane/hulmane-the-saga/` | `hulmane-the-saga-volume-1/` at git root |
| `state-stories.html` | `kingdoms.html` (Kingdoms of Bharatavarsha) |
| `kingdom-identity.html` (single page for all) | Per-kingdom `identity.html` |
| `media/images/[region]/[state]/` | `bharatavarsha/regions/[region]/kingdoms/[kingdom]/media/` |
| "States" terminology | "Kingdoms" everywhere |
| No volume structure | Master index + per-volume folder |
| Centralized media | Kingdom-owned media |
| `regions.html` (separate page) | Regions are sections within `kingdoms.html` |

---

## 12. Out of Scope (For Later Volumes)

- Volume 2–6 content (placeholder tiles only)
- Global council (placeholder only)
- Interactive map with kingdom boundaries drawn
- Dynamic filtering/search on kingdoms page
