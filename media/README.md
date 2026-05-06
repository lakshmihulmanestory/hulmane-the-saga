# MahaHulmane — Media Folder

All project media lives here. Every folder has four subfolders: `images/` `samples/` `videos/` `audio/`

## Structure

```
media/
│
├── MAHAHULMANE/              World-level content (Grand Council, Sacred Tattoo, crossovers)
│   ├── grand-council/        The 7-member Council art & media
│   ├── sacred-tattoo/        Tattoo system diagrams, animations
│   ├── world-overview/       Full-world establishing shots
│   ├── world-map/            Interactive map assets
│   ├── intro-sequence/       Opening cinematic assets
│   └── crossover-stories/    Stories where heroes from multiple states appear together
│
├── regions/                  6 Regional hero content (one folder per region)
│   ├── south/
│   ├── west/
│   ├── east/
│   ├── north/
│   ├── northeast/
│   └── central/
│
└── states/                   28 State kingdoms
    ├── south/
    │   ├── andhra-pradesh/
    │   │   ├── images/       Generated SVG/art for this state's hero, villain, animal
    │   │   ├── samples/      Reference/generated images (Gemini, ChatGPT, etc.)
    │   │   ├── videos/       Story videos, character intros
    │   │   ├── audio/        Story narration, character voice, music
    │   │   └── stories/
    │   │       └── dharmakshetra-amaravati/
    │   │           ├── images/   Art specific to this story arc
    │   │           ├── samples/  ← sample images already here
    │   │           ├── videos/
    │   │           └── audio/
    │   ├── karnataka/
    │   │   └── stories/
    │   │       ├── vijayanagara-reborn/    ← 10 samples + 2 SVGs here
    │   │       └── buried-temple-western-ghats/
    │   ├── kerala/
    │   │   └── stories/
    │   │       └── parashurama-kshetra/   ← 4 samples here
    │   ├── tamil-nadu/
    │   │   └── stories/
    │   │       └── song-that-shatters/
    │   └── telangana/
    │       └── stories/
    │           └── chaya-golkonda-shadow-fortress/   ← 2 samples here
    ├── west/    goa/ gujarat/ maharashtra/ rajasthan/
    ├── east/    bihar/ jharkhand/ odisha/ west-bengal/
    ├── north/   haryana/ himachal-pradesh/ punjab/ uttar-pradesh/ uttarakhand/
    ├── northeast/
    │   ├── assam/
    │   │   └── stories/
    │   │       ├── ganda-kshetra-rhinoceros-realm/   ← 8 samples here
    │   │       └── rhino-knight/
    │   └── arunachal-pradesh/ manipur/ meghalaya/ mizoram/ nagaland/ sikkim/ tripura/
    └── central/ chhattisgarh/ madhya-pradesh/
```

## Rules

| Folder | What goes here |
|--------|---------------|
| `images/` | Generated SVG illustrations, character portraits, scene art (built by code) |
| `samples/` | Reference images from Gemini / ChatGPT / other AI tools used as visual reference |
| `videos/` | Story videos, character intro clips, scene animations |
| `audio/` | Narration tracks, character voice lines, background music, sound effects |

## Adding a new story

1. Create `media/states/<region>/<state>/stories/<story-slug>/`
2. Add all four subfolders: `images/ samples/ videos/ audio/`
3. Drop sample images in `samples/`, generated art in `images/`

## Adding a crossover story (multiple states)

Put it in `media/MAHAHULMANE/crossover-stories/` and name the subfolder clearly:
e.g. `crossover-stories/karnataka-assam-elephant-alliance/`
