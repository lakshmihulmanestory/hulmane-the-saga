# MahaHulmane — Character Design System

> Every hero and villain in MahaHulmane is built from a structured set of attributes.
> This document defines the schema. The data lives in `data/heroes.csv` and `data/villains.csv`.
> Divine reference definitions live in `data/references/`.

---

## The Core Principle

**Every character is an intersection of four layers:**

```
LAYER 1 — THE LAND        (state, region, landscape, kingdom theme)
LAYER 2 — THE BOND        (sacred animal + bird — together they define the character's nature)
LAYER 3 — THE DIVINE      (deity, Mahabharata parallel, avatar, ancestor — the spiritual DNA)
LAYER 4 — THE FIGHT       (ancient weapon + modern weapon — how they express their power)
```

Hero and villain are built from the **same four layers** — identical inputs, opposite outputs.
The animal bond is the same. The divine reference is the shadow/mirror of the same deity.
They diverge only in their CHOICE, not their origin.

---

## Complete Character Schema

Every hero and villain must have ALL of these fields defined.
Use `data/heroes.csv` and `data/villains.csv` to track them.

### IDENTITY
| Field | Description | Example |
|---|---|---|
| `id` | URL-safe slug | `karnataka` |
| `state` | Full state name | `Karnataka` |
| `region` | One of 6 regions | `south` |
| `kingdom_name` | The kingdom's story title | `Vijayanagara Reborn` |
| `kingdom_theme` | One-sentence story tone | `An empire buried and rising again` |
| `era` | Temporal setting | `ancient`, `modern`, `both` |
| `landscape` | Dominant geography | `Western Ghats forest, river valleys, ancient ruins` |

### CHARACTER DESIGN
| Field | Description | Example |
|---|---|---|
| `name` | Hero/villain name | `Tungabhadra` |
| `title` | Short title | `The River Queen` |
| `gender` | Gender | `female` |
| `age` | Age at story start | `35` |
| `role` | `hero` or `villain` | `hero` |
| `costume_style` | Aesthetic tradition | `Vijayanagara bronze-era armor over battle saree` |
| `colour_primary` | Dominant colour | `#44ff88` (deep forest green) |
| `colour_secondary` | Accent colour | `#ffd700` (Vijayanagara gold) |
| `physical_signature` | One unmistakable visual trait | `Jasmine flowers braided into hair even before combat` |
| `tattoo_symbol` | The sacred beast mark | `Elephant footpad → foreleg → half body → full body` |

### SACRED BONDS
| Field | Description | Example |
|---|---|---|
| `sacred_animal` | State animal (scientific name optional) | `Indian Elephant (Elephas maximus indicus)` |
| `animal_symbolism` | What the animal represents | `Wisdom, memory, unstoppable force` |
| `animal_power` | What ability the bond grants | `Seismic battlefield sensing — feel every footstep within 1km` |
| `sacred_bird` | State bird (state bird of India) | `Indian Roller / Neelakantha (Coracias benghalensis)` |
| `bird_symbolism` | What the bird represents | `Divine messenger, transformation, sky-bound truth` |
| `bird_role` | How the bird appears in stories | `Scout / messenger / omen / spirit guide` |

### WEAPONS
| Field | Description | Example |
|---|---|---|
| `ancient_weapon_name` | Traditional weapon name | `Gajadanda` |
| `ancient_weapon_type` | Weapon category | `Mace` |
| `ancient_weapon_material` | What it's made of | `Meteorite iron, topped with bronze elephant head` |
| `ancient_weapon_ability` | Special/sacred power | `Channels elephant battle-memory when hero enters Gaja-Trance` |
| `modern_weapon_name` | Tech-upgraded version name | `Gajadanda Mk.II` |
| `modern_weapon_type` | Tech category | `Cybernetic seismic mace` |
| `modern_weapon_ability` | Tech special power | `Underground radar pulse, seismic burst on impact` |

### SPIRITUAL NETWORK
| Field | Description | Example |
|---|---|---|
| `guru_name` | Mentor name (or `None`) | `Sage Vidyaranya` |
| `guru_type` | `living`, `spirit`, `ancestor`, `divine`, `none` | `spirit` |
| `guru_relationship` | How guru connects to hero | `Spirit of Vijayanagara's founder — appears in visions at ruins` |
| `guru_teaches` | What skill or wisdom they give | `How the Shila-Rakshasa was first sealed; patience over power` |
| `ancestor_1` | First ancestor guide name | `Hampi Builders — the engineers of Vijayanagara` |
| `ancestor_1_type` | `bloodline`, `clan`, `kingdom`, `divine_lineage` | `kingdom` |
| `ancestor_1_gift` | What they give hero | `Architectural knowledge — reading stone like a map` |
| `ancestor_2` | Second ancestor (or blank) | (blank) |
| `ancestor_council` | Named council of ancestors? | `The Builders' Council — 7 ancestral architects` |

### DIVINE REFERENCES
| Field | Description | Allowed Values |
|---|---|---|
| `primary_deity` | Main Hindu god inspiration | Any deity name — see `data/references/deities.csv` |
| `deity_aspect` | Which form/avatar of that deity | e.g. `Indrani (Queen of Svarga)` |
| `deity_quality` | What quality of that deity this hero embodies | e.g. `Nurture through strength, commands elephant armies` |
| `vishnu_avatar` | Which Dashavatara if applicable | See `data/references/vishnu-avatars.csv` — or `None` |
| `vishnu_quality` | What avatar quality this hero mirrors | |
| `shiva_form` | Which Shiva aspect if applicable | See `data/references/shiva-forms.csv` — or `None` |
| `shiva_quality` | What Shiva quality this hero mirrors | |
| `ganesha_attribute` | Which Ganesha quality if applicable | See `data/references/ganesha-attributes.csv` — or `None` |
| `ganesha_quality` | How this attribute manifests in the hero | |
| `other_deity` | Any other divine reference | Free text |

### MAHABHARATA REFERENCES
| Field | Description | Allowed Values |
|---|---|---|
| `mb_primary` | Primary Mahabharata parallel | See `data/references/mahabharata-characters.csv` |
| `mb_primary_quality` | What quality they share | e.g. `Bhima's unstoppable rage channelled through dharma` |
| `mb_secondary` | Second Mahabharata parallel | Another character, or blank |
| `mb_story_echo` | Which Mahabharata episode this story echoes | e.g. `Burning of the Khandava forest — protecting what must be preserved` |
| `mb_inversion` | How this story INVERTS the Mahabharata version | e.g. `Unlike Drona, the guru here teaches to protect, not to exclude` |

---

## How to Use References When Writing

### Rule 1 — Show, Don't Name
When writing any format, **never write** "like Bhima, she was unstoppable."
Instead: show the quality — the unstoppable charge, the refusal to fall, the rage that protects.
A reader who knows the Mahabharata will feel it. One who doesn't will simply see a great hero.

### Rule 2 — The Deity Reference Is Atmosphere, Not Identity
The hero is **inspired by** Indrani — they are NOT Indrani.
The deity provides: visual symbolism (Airavata's white elephant), a power archetype (divine command),
and a moral framework (justice through nurture). The hero is their own person.

### Rule 3 — The Bird Has a Story Role
The state bird is not decoration. In every story:
- **Omen**: The bird appears before something important happens
- **Messenger**: Carries a signal between characters  
- **Spirit guide**: In the hero's darkest moment, the bird appears and shows the way
- **Bond proof**: The villain's version of the bird is always absent, caged, or corrupted

### Rule 4 — Ancestor Support Is Earned
The ancestral support does not appear in chapter 1.
- Level 1 tattoo: Hero is alone — no ancestor guidance
- Level 2 tattoo: A single ancestor makes contact (dream, vision, inscription)
- Level 3 tattoo: The ancestor council speaks (together, in a sacred space)
- Level 4 tattoo: The hero BECOMES an ancestor — they are now part of the lineage

### Rule 5 — Ancient + Modern Weapons Have Different Contexts
- **Ancient weapon**: Used in moments of deep emotional truth — final battles, protection of sacred things
- **Modern weapon**: Used in tactical, strategic situations — the mind weapon
- They should NEVER be equally powerful — the ancient weapon always has the decisive moment

### Rule 6 — Villain Parallels Are Sympathetic, Not Evil
The villain's Mahabharata parallel must make them understandable:
- Karna parallel = someone doing the right things for the wrong alliance
- Duryodhana parallel = someone convinced of their own righteousness
- Ashwatthama parallel = someone whose grief broke their moral compass
- Shakuni parallel = someone weaponising intelligence born from real injustice

---

## Tagging System for Stories and Media Files

When creating any content (writing, art, audio, video), add tags from this list:

### Deity Tags
`@deity-indrani` `@deity-ganesha` `@deity-vishnu` `@deity-shiva`
`@deity-durga` `@deity-kartikeya` `@deity-saraswati` `@deity-kali`
`@deity-surya` `@deity-varuna` `@deity-parvati` `@deity-lakshmi`
`@avatar-narasimha` `@avatar-parashurama` `@avatar-krishna` `@avatar-rama`
`@avatar-varaha` `@avatar-vamana` `@avatar-kurma` `@avatar-matsya`
`@avatar-balarama` `@avatar-kalki`

### Mahabharata Tags
`@mb-arjuna` `@mb-bhima` `@mb-yudhishthira` `@mb-karna`
`@mb-draupadi` `@mb-abhimanyu` `@mb-bheeshma` `@mb-drona`
`@mb-duryodhana` `@mb-shakuni` `@mb-ashwatthama` `@mb-vidura`
`@mb-krishna` `@mb-gandhari` `@mb-kunti`

### Story Element Tags
`@bond-animal` `@bond-bird` `@bond-broken` `@bond-restored`
`@weapon-ancient` `@weapon-modern` `@weapon-combined`
`@guru-living` `@guru-spirit` `@guru-ancestor` `@guru-none`
`@ancestor-single` `@ancestor-council` `@ancestor-bloodline`
`@tattoo-1` `@tattoo-2` `@tattoo-3` `@tattoo-4`

### Format Tags (from STORY_FORMATS.md)
`@format-film` `@format-anim-series` `@format-anim-movie`
`@format-comic` `@format-gn` `@format-kids` `@format-book`
`@format-rpg` `@format-mobile`
`@format-sticker` `@format-card` `@format-apparel` `@format-print` `@format-toy`

### Usage Example
A piece of script tagged:
```
@state-karnataka @deity-indrani @avatar-none @mb-bhima @mb-draupadi
@bond-animal @bond-bird @weapon-ancient @guru-spirit @ancestor-council
@tattoo-3 @format-film @format-book
```
Tells any AI agent or team member exactly what references to draw on when working with it.

---

## How to Add New References

**Adding a new deity, avatar, or Mahabharata reference:**
1. Add a row to the relevant CSV in `data/references/`
2. Add the tag `@deity-[name]` or `@mb-[name]` to `docs/CHARACTER_SYSTEM.md` tag list above
3. Update `CLAUDE.md` if it's a frequently used reference

**Adding a new story attribute (e.g. a new weapon type or guru type):**
1. Add the field to the schema table above
2. Add a column to `data/heroes.csv` and `data/villains.csv`
3. Fill in the value for every existing character (or `TBD` if unknown)

**Adding a new hero/state:**
1. Add a row to `data/heroes.csv`
2. Add a row to `data/villains.csv`
3. Create story folders: `media/states/<region>/<state>/stories/<slug>/`
