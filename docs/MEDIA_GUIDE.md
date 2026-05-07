# Hulmane-The-Saga — Media Organisation Guide

> Where every file goes. Read before creating or placing any media asset.

---

## The Two-Tree System

All media lives in exactly two places:

```
media/          ← PRODUCTION art (your final/generated outputs)
samples/media/  ← REFERENCE images (Gemini, ChatGPT, mood boards, research)
```

**The folder structure inside both trees is identical.**
Same region → state → story path. Just different root.

---

## Full Folder Map

```
media/
├── images/                          ← Generated SVGs / character reference art
│   └── <region>/<state>/            ← State-level art, usable across ALL stories
│       Example: images/south/karnataka/karnataka-portrait.svg
│
├── HULMANE-THE-SAGA/                     ← World-level content (not state-specific)
│   ├── grand-council/               ← The 7-member council art
│   ├── sacred-tattoo/               ← Tattoo system diagrams, progression art
│   ├── world-overview/              ← Full-world maps, establishing shots
│   ├── world-map/                   ← Interactive map assets
│   ├── intro-sequence/              ← Opening cinematic / title sequence
│   └── crossover-stories/           ← Stories with heroes from multiple states
│       each folder: images/ samples/ videos/ audio/
│
├── regions/                         ← 6 regional zones
│   └── <region>/                    ← Regional hero, regional overview
│       south/ west/ east/ north/ northeast/ central/
│       each: images/ samples/ videos/ audio/
│
└── states/
    └── <region>/<state>/
        ├── images/                  ← State hero, villain, animal (not story-specific)
        ├── samples/                 ← State-level reference images
        ├── videos/                  ← Kingdom intro video, hero reel
        ├── audio/                   ← Kingdom theme music, hero theme
        └── stories/
            └── <story-slug>/
                ├── images/          ← Generated art for THIS story only
                ├── samples/         ← AI reference images for THIS story
                ├── videos/          ← Trailers, animatics, scene videos
                └── audio/           ← Narration, BGM, sound effects
```

---

## All 28 State Story Slugs

Drop images directly into these folders:

### South India
| State | Story Folder Path |
|---|---|
| Andhra Pradesh | `media/states/south/andhra-pradesh/stories/dharmakshetra-amaravati/` |
| Telangana | `media/states/south/telangana/stories/chaya-golkonda-shadow-fortress/` |
| Tamil Nadu | `media/states/south/tamil-nadu/stories/sangam-tamilakam/` |
| Tamil Nadu | `media/states/south/tamil-nadu/stories/song-that-shatters/` |
| Kerala | `media/states/south/kerala/stories/parashurama-kshetra/` |
| Karnataka | `media/states/south/karnataka/stories/vijayanagara-reborn/` |
| Karnataka | `media/states/south/karnataka/stories/buried-temple-western-ghats/` |

### West India
| State | Story Folder Path |
|---|---|
| Maharashtra | `media/states/west/maharashtra/stories/swarajya-sahyadri/` |
| Gujarat | `media/states/west/gujarat/stories/simha-dwara/` |
| Goa | `media/states/west/goa/stories/samudra-dvipa/` |
| Rajasthan | `media/states/west/rajasthan/stories/maru-maya/` |

### East India
| State | Story Folder Path |
|---|---|
| West Bengal | `media/states/east/west-bengal/stories/sundara-vana/` |
| Odisha | `media/states/east/odisha/stories/kalinga-chakra/` |
| Bihar | `media/states/east/bihar/stories/vajra-bhumi/` |
| Jharkhand | `media/states/east/jharkhand/stories/vana-agni/` |

### North India
| State | Story Folder Path |
|---|---|
| Uttar Pradesh | `media/states/north/uttar-pradesh/stories/ganga-simhasana/` |
| Uttarakhand | `media/states/north/uttarakhand/stories/deva-bhumi/` |
| Himachal Pradesh | `media/states/north/himachal-pradesh/stories/hima-chhaya/` |
| Punjab | `media/states/north/punjab/stories/panch-nada/` |
| Haryana | `media/states/north/haryana/stories/kurukshetra-bhoomi/` |

### Northeast India
| State | Story Folder Path |
|---|---|
| Assam | `media/states/northeast/assam/stories/ganda-kshetra-rhinoceros-realm/` |
| Assam | `media/states/northeast/assam/stories/rhino-knight/` |
| Arunachal Pradesh | `media/states/northeast/arunachal-pradesh/stories/arunodaya-kshetra/` |
| Manipur | `media/states/northeast/manipur/stories/sangai-nata/` |
| Meghalaya | `media/states/northeast/meghalaya/stories/megha-maata/` |
| Mizoram | `media/states/northeast/mizoram/stories/tlawmngaihna-desh/` |
| Nagaland | `media/states/northeast/nagaland/stories/dzukou-rashtra/` |
| Sikkim | `media/states/northeast/sikkim/stories/beyul-kshetra/` |
| Tripura | `media/states/northeast/tripura/stories/tri-pura/` |

### Central India
| State | Story Folder Path |
|---|---|
| Madhya Pradesh | `media/states/central/madhya-pradesh/stories/hridaya-sthana/` |
| Chhattisgarh | `media/states/central/chhattisgarh/stories/dandakaranya/` |

---

## File Naming Convention

### Pattern
```
<state>-<story-or-subject>-<format-code>-<type>-<number>.<ext>
```

### Format Codes
| Code | Format |
|---|---|
| `FILM` | Feature Film |
| `ANIM-S` | Animation Series |
| `ANIM-M` | Animation Movie |
| `COMIC` | Comics |
| `GN` | Graphic Novel |
| `KIDS` | 5-Min Kids Story |
| `BOOK` | State Story Book |
| `RPG` | RPG Game |
| `MOBILE` | Mobile Game |
| `REF` | General reference (any format) |

### Type Codes
| Code | What it is |
|---|---|
| `concept` | Concept art / mood board |
| `portrait` | Character portrait / profile |
| `scene` | Scene illustration |
| `model` | Character model sheet / turnaround |
| `bg` | Background / environment art |
| `icon` | Small icon / symbol |
| `cover` | Cover art |
| `map` | Map / layout |
| `storyboard` | Storyboard panel |
| `ref` | Reference image |

### Examples
```
karnataka-tungabhadra-FILM-portrait-01.jpg
karnataka-vijayanagara-ANIM-S-scene-temple-01.png
assam-kamalavarna-KIDS-portrait-01.png
gujarat-simhavikrama-RPG-model-front-01.png
karnataka-elephant-REF-01.jpg              ← no format tag = general use
andhra-krishnaveni-BOOK-cover-01.jpg
```

---

## What Goes Where — Quick Decision

| I have... | Put it in... |
|---|---|
| Generated SVG character portrait (usable in any format) | `media/images/<region>/<state>/` |
| Gemini / ChatGPT reference image for a story | `samples/media/states/<region>/<state>/stories/<slug>/` |
| Final scene illustration for Vijayanagara Reborn film | `media/states/south/karnataka/stories/vijayanagara-reborn/images/` |
| Story trailer video for Buried Temple | `media/states/south/karnataka/stories/buried-temple-western-ghats/videos/` |
| Karnataka kingdom theme music (used in all stories) | `media/states/south/karnataka/audio/` |
| Grand Council overview image | `media/HULMANE-THE-SAGA/grand-council/images/` |
| Sacred Tattoo system diagram | `media/HULMANE-THE-SAGA/sacred-tattoo/images/` |
| A story where Karnataka + Assam heroes team up | `media/HULMANE-THE-SAGA/crossover-stories/images/` |
| South India regional hero group shot | `media/regions/south/images/` |

---

## Adding a New Story

1. Create the folder in both trees:
   ```bash
   mkdir -p media/states/<region>/<state>/stories/<new-story-slug>/{images,samples,videos,audio}
   mkdir -p samples/media/states/<region>/<state>/stories/<new-story-slug>/{images,samples,videos,audio}
   ```
2. Add the story slug to `docs/MEDIA_GUIDE.md` table above
3. Add story details to `docs/PROJECT_VISION.md` and `docs/STORY_FORMATS.md`
4. Update `CLAUDE.md` if it changes the key rules

---

## Adding a New State Story Book

Each of the 28 state books gets its own manuscript folder:
```
docs/manuscripts/
  south/
    karnataka/
      vijayanagara-reborn-STATE-BOOK.md
      buried-temple-STATE-BOOK.md
    andhra-pradesh/
      dharmakshetra-amaravati-STATE-BOOK.md
  ...
```
*(manuscripts/ folder not yet created — create when writing begins)*
