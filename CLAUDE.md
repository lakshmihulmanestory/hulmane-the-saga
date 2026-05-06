# MahaHulmane — AI Agent Context

> Read this first. Everything you need to orient yourself in this project.

## What is MahaHulmane?

**MahaHulmane** ("The Great Assembly of Warriors") is an original Indian fantasy IP
inspired by the Mahabharata and Hindu mythology. It is being built as a **multi-format
transmedia franchise** — not just a single story, but a full universe designed to scale
across film, animation, games, books, and more.

The world has **28 kingdoms** (one per Indian state), each with:
- A **hero** bonded to a **sacred animal** (the state animal), inspired by a Hindu deity
- A **villain** who shares the same animal but channels its dark spirit
- Multiple **stories** per kingdom (main arc + sub-stories)
- A **tattoo system** that tracks each hero's journey visually

---

## Target Formats — Read Before Writing Any Content

This IP is being developed for **multiple audiences and formats simultaneously**.
Every piece of content (images, story text, audio, video) must be tagged to its format.
See `docs/STORY_FORMATS.md` for the full breakdown.

| Format | Audience | Tone | Length |
|---|---|---|---|
| Feature Film | 13+ / General | Epic, cinematic | 2–2.5 hr per story arc |
| Animation Series | 8–16 / Family | Action-adventure | 22 min episodes |
| Animation Movie | 6–12 / Kids+Family | Heroic, colourful | 90 min |
| Comics (Monthly) | 8–14 | Bold, kinetic, cliff-hanger | 24–32 pages per issue |
| Graphic Novel | 10+ | Literary, Amar Chitra Katha | 200–250 pages collected |
| 5-Min Kids Stories | 3–7 | Simple, warm, moral lesson | 500–800 words |
| State Story Book | 8–14 | Cultural pride, adventure | 80–120 pages per book |
| Big RPG Game | 16+ | Deep lore, dark fantasy | Open world |
| Mobile Game | 10+ | Action, strategy | Session-based |
| Stickers | All ages | Bold silhouette, 5cm–8cm | PNG transparent 300 DPI |
| Collector Cards | All ages | Portrait + stats, trading card | 63×88mm, foil variants |
| T-shirts & Apparel | Kids + Adults | Kingdom badge, silhouette, tattoo art | Vector print-ready |
| Art Prints | All ages | Fine art scenes, state maps | 300 DPI, A4–A1 sizes |
| Toys & Figures | 3–14+ | Action figures, plush animals, vinyl | Turnaround sheets needed |

---

## Character Data — CSV Files

All 28 heroes and villains are fully tagged in machine-readable CSV:

| File | Contents |
|---|---|
| `data/heroes.csv` | All 28 heroes — identity, sacred animal + bird, ancient + modern weapons, guru, ancestors, deity, Vishnu avatar, Shiva form, Ganesha attribute, Mahabharata parallels, tags |
| `data/villains.csv` | All 28 villains — same structure but dark versions — dark deity, dark animal power, villain motivation, hero mirror point |
| `data/references/deities.csv` | All Hindu deity references used — domain, quality, symbol, which heroes, story use |
| `data/references/vishnu-avatars.csv` | All 10 Dashavatara — quality, story role, character archetype |
| `data/references/shiva-forms.csv` | 12 Shiva forms — domain, quality, story role |
| `data/references/ganesha-attributes.csv` | 10 Ganesha attributes — domain, story role |
| `data/references/mahabharata-characters.csv` | 17 Mahabharata characters (heroes + villains) — how to use, what to avoid |
| `data/references/state-birds.csv` | All 28 state birds — symbolism, conservation status, story role per hero |

See `docs/CHARACTER_SYSTEM.md` for the full schema and rules for using these references in writing.

---

## Project File Structure

```
MahaHulmane/
├── CLAUDE.md              ← YOU ARE HERE (AI agent context)
├── docs/                  ← Full documentation for team + AI agents
│   ├── PROJECT_VISION.md  ← IP vision, world rules, lore bible overview
│   ├── STORY_FORMATS.md   ← All target formats, audience specs, content rules
│   ├── MEDIA_GUIDE.md     ← How to name and place every media file
│   └── CHARACTERS.md      ← Character design rules and deity mapping
├── media/                 ← Production media (generated art, SVG, video, audio)
│   ├── images/            ← Generated SVGs by region/state (character reference art)
│   ├── MAHAHULMANE/       ← Grand Council, Sacred Tattoo, world-level content
│   ├── regions/           ← 6 regional hero content
│   └── states/            ← 28 kingdoms → stories → images/samples/videos/audio
├── samples/               ← AI-generated reference images (Gemini, ChatGPT, etc.)
│   └── media/             ← Mirrors media/ structure exactly
├── stories/               ← Story HTML pages (asia/india/region/state/)
├── js/                    ← Characters data, app logic
├── css/                   ← Styles
└── [HTML pages]           ← Website: index, characters, gallery, etc.
```

---

## Key Rules for Any AI Agent Working Here

1. **Every story exists in multiple formats** — when writing or generating content,
   always ask: which format is this for? Kids story? Game? Film? Each has different rules.

2. **Hero and villain share the same animal** — one is the good spirit, one the dark.
   They are mirrors, not opposites. This is the core narrative engine.

3. **Hindu deity inspiration is mandatory** — every hero maps to a specific deity or
   Mahabharata character. See `docs/CHARACTERS.md` for the full mapping.

4. **Media goes in `media/states/<region>/<state>/stories/<story-slug>/`**
   Samples (AI reference) go in `samples/media/states/<region>/<state>/stories/<story-slug>/`

5. **Story slugs are fixed** — do not rename existing story folders.
   See `docs/MEDIA_GUIDE.md` for the complete slug list.

6. **The tattoo system is the visual progress tracker** — footprint → leg → half body →
   full body. Never depict a hero above their earned tattoo level.

---

## The 28 Kingdoms at a Glance

| Region | States |
|---|---|
| South | Andhra Pradesh · Telangana · Tamil Nadu · Kerala · Karnataka |
| West | Maharashtra · Gujarat · Goa · Rajasthan |
| East | West Bengal · Odisha · Bihar · Jharkhand |
| North | Uttar Pradesh · Uttarakhand · Himachal Pradesh · Punjab · Haryana |
| Northeast | Assam · Arunachal Pradesh · Manipur · Meghalaya · Mizoram · Nagaland · Sikkim · Tripura |
| Central | Madhya Pradesh · Chhattisgarh |
