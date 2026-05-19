# Resumable Task Checklist — Volume I, Chapters 2 → 4

> Single source of truth for what to do next. Each item below is one *atomic, completable* unit of work.
> Pick the first unchecked item. Do it. Check it. Commit. Move on.
> If a task requires a user decision (marked **[DECIDE]**), pause and ask.

> **⚠ READ BEFORE STARTING (2026-05-18):** The cast was restructured to male-led from Chapter 2 onward. Read `07-cast-male-led-restructure.md` first. Where Stage 2/3/4 task descriptions reference female heroes, treat them as superseded by `07-cast-male-led-restructure.md` §4 (Female Cast Fate) and §5 (New Male Heroes).

---

## Stage 0 — Decisions

**LOCKED:**
- [x] **D1.** 30 kingdoms (28 + Sharada-Pitha + Sagara-Ratna).
- [x] **D2.** 6 Regional Dominants (all male): Karnataka/Krishnadevaraya-Bhrata (S), UP/Gangaputra (N), Odisha/Jagannath-Bandhu (E), **Gujarat**/Simhavikrama (W), MP/Dvadashashringa (Central), **Manipur**/Moirangthem (NE). See `07-cast-male-led-restructure.md` §1.
- [x] **D3.** Maha-Adhipati = **Krishnadevaraya-Bhrata** (Karnataka). Revised from Tungabhadra. See `07` §3.
- [x] **D5.** Original 3 hero deaths confirmed. **EXPANDED** via male-led restructure to ~9 total — see D11 to confirm.

**LOCKED (continued, 2026-05-18):**
- [x] **D4.** Void Maw = "absence with intent." Cosmic forgetting. Defeated by memory, not violence. Final climax: Krishnadevaraya-Bhrata enters the Maw and shapes its face by naming forgotten ancestors.
- [x] **D6.** Heralds rule = "remember, do not kill." Killing a Herald grows the Maw; naming one converts them.
- [x] **D7.** Next continent (Volume II hook) = **Yavana-Khanda** (the Greek-coded Mediterranean / West-Asia lands). Named in Ch 4 epilogue; Sagara-Ratna (Andaman) is the launch point.
- [x] **D8.** Vyasa-of-the-Margins appears in Ch 2 only twice — Karnataka pilot + Tripura — then disappears until Ch 3.
- [x] **D9.** Double-bond mechanic = Simhavikrama (Gujarat) carries Asiatic Lion + Goan Gaur post-Ch 3.
- [x] **D10.** Fourth Herald (revealed end of Ch 3) = **Krodha** (Sikkim's Ch 1 villain).
- [x] **D11.** 9 hero deaths confirmed: Ch 2 (Tungabhadra, Himavati, Meghanadi, Tlangvala, Sagaradeva), Ch 3 (Jagannathi, Sundarvani, Krishnaveni, Shivagati).
- [x] **D12.** Krishnadevaraya-Bhrata = Bhoomi-Takshaka's twin brother (Restorationist-redemption arc, deeper bloodline conflict).
- [x] **D13.** Two new kingdoms = Sharada-Pitha (Kashmir, North) + Sagara-Ratna (Andaman, East).
- [x] **D14.** Maharashtra absorbed under Gujarat. West Dominant = Simhavikrama. Tanaji-the-Second holds Maharashtra as Gujarat's vassal.
- [x] **D15.** Assam → Manipur as NE Dominant. Moirangthem is NE Regional Dominant. Kamalavarna = Kamakhya High Priestess (cosmic, non-political).
- [x] **D16.** Back-fill first: complete Sharada-Pitha + Sagara-Ratna in Chapter 1 before any Ch 2 prose begins (Stage 0.5 below).

**All Stage 0 decisions are LOCKED. Proceed to Stage 0.5 (Chapter-1 back-fill).**

---

## Stage 0.5 — Chapter-1 Back-Fill (NEW KINGDOMS)

These add Sharada-Pitha (Kashmir) and Sagara-Ratna (Andaman & Nicobar) to Chapter 1 so the cast is complete before Chapter 2 begins. Use the existing Karnataka files as a structural template. See `07-cast-male-led-restructure.md` §2 for character spec.

- [x] **BF.1** Create `chapter-1-rise-of-legends/bharatavarsha/regions/north/sharada-pitha/{index.html,identity.html,story.html,rules.html}` + media folder. ✓ 2026-05-19
- [x] **BF.2** Write Sharad-Pandit (hero) + Avantivarman-Bhrasta (villain) into `chapter-1-rise-of-legends/data/heroes.csv` and `villains.csv` as new rows. ✓ 2026-05-19
- [x] **BF.3** Write the Kashmir Chapter-1 story (Sharad-Pandit's rise) — full kingdom-arc per the Chapter 1 voice. Lives in `js/state-stories-data.js` (the `kashmir` entry) and `js/kingdom-identity-data.js`. Title: *The Snow Library — A Film in Two Halves*. ✓ 2026-05-19
- [ ] **BF.4** (DEFERRED) Add Sharada-Pitha to the actual SVG of `chapter-1-rise-of-legends/bharatavarsha/global-map.html` and to `media/maps/bharatavarsha.png`. Text count updated; the map image itself still needs Kashmir placement on the visual artifact. *Skipped by user request in 2026-05-18 session.*
- [x] **BF.5** Create `chapter-1-rise-of-legends/bharatavarsha/regions/east/sagara-ratna/` (4 HTML files + media subfolders). ✓ 2026-05-19
- [x] **BF.6** Write Onge-Nakshatra (hero) + Kalapani-Asura (villain) into `data/heroes.csv` and `data/villains.csv`. ✓ 2026-05-19
- [x] **BF.7** Write the Andaman Chapter-1 story (Onge-Nakshatra's rise) — full saga prose in `state-stories-data.js` entry `andaman`. Title: *The Unlocking — A Film in Two Halves*. ✓ 2026-05-19
- [ ] **BF.8** (DEFERRED — same as BF.4) Add Sagara-Ratna to the SVG/image of the global map. Text count is 30; map artifact still needs Andaman dot placement.
- [x] **BF.9** Updated count `29 → 30` across `kingdoms.html`, `index.html`, `characters.html`, `systems.html`, `council.html`, `character-gallery.html`, `global-map.html`, `js/state-stories-data.js` header, `js/kingdom-identity-data.js` header, and the two in-saga "30 heroes" descriptions. ✓ 2026-05-19
- [ ] **BF.10** REVIEW with user — Chapter 1 back-fill complete (apart from the two deferred SVG/PNG map artifacts BF.4 + BF.8); sign-off before continuing to Stage 1

---

## Stage 1 — Foundation Infrastructure (one-off setup)

These are repository-level prep tasks; they don't require Chapter 2 decisions.

- [ ] **F1.** Add the Chapter 2 stub directory structure mirroring Chapter 1: `chapter-2-civil-war/bharatavarsha/regions/<region>/<kingdom>/{index.html,identity.html,story.html,rules.html}` — empty templates only. (30 kingdoms × 4 files = 120 stub files.)
- [ ] **F2.** Same for Chapter 3 (`chapter-3-rise-of-beasts/...`). Stubs only.
- [ ] **F3.** Same for Chapter 4 (`chapter-4-the-great-epic/...`). Different structure — see `05-chapter-4-the-great-epic.md` §8.
- [ ] **F4.** Create CSV delta-files:
   - `chapter-2-civil-war/data/heroes-ch2-delta.csv` (header only)
   - `chapter-2-civil-war/data/villains-ch2-delta.csv`
   - `chapter-2-civil-war/data/new-characters.csv`
   - same for Ch 3, Ch 4
- [ ] **F5.** Create a template `story.html` for Chapter 2 (one-off; copy & adapt per kingdom). Should include: faction-split banner, three-beat layout, animal-stirring callout, Void Maw sign callout, new-characters card grid.
- [ ] **F6.** Update `chapter-2-civil-war/index.html` from placeholder → chapter landing (28-kingdom tile grid).
- [ ] **F7.** Update `chapter-3-rise-of-beasts/index.html` → 6 Dominants + 22 absorbed.
- [ ] **F8.** Update `chapter-4-the-great-epic/index.html` → the convergence.

---

## Stage 2 — Chapter 2 Civil War Stories (production order from `03-chapter-2-civil-war.md` §4)

Write in clusters. Within each cluster, sub-tasks per kingdom are: **(a) story.html prose** | **(b) identity.html Ch 2 update** | **(c) faction insignia / new-character portraits brief** | **(d) hero/villain CSV delta row** | **(e) Void Maw sign one-liner added to chapter-level sign log**.

### Cluster 2.A — Karnataka Pilot
- [ ] **2A.1** Karnataka — `Vijayanagara Reborn` — write `story.html` (the pilot — defines voice & length)
- [ ] **2A.2** Karnataka — identity & faction-insignia brief
- [ ] **2A.3** Karnataka — CSV delta rows (Tungabhadra Ch2; Bhoomi-Takshaka Ch2; Hampi-of-the-Bronze new; Krishnadevaraya-Bhrata new; 3rd Herald new)
- [ ] **2A.4** Karnataka — Void Maw sign 3 logged in `chapter-2-civil-war/maw-signs.md`
- [ ] **2A.5** REVIEW with user — voice, pace, length. Sign-off needed before continuing cluster work.

### Cluster 2.B — Maharashtra + Goa
- [ ] **2B.1** Goa — `Samudra-Dvipa` — story.html (HERO DEATH arc)
- [ ] **2B.2** Goa — identity update; "kingdom occupied" template
- [ ] **2B.3** Goa — CSV delta (Sagaradeva → deceased; Ferreira-de-Sangam new)
- [ ] **2B.4** Maharashtra — `Swarajya Sahyadri` — story.html (double-bond arc)
- [ ] **2B.5** Maharashtra — identity update with both tattoos forming
- [ ] **2B.6** Maharashtra — CSV delta (Shivagati Ch2; Vanaraksha Ch2; Tanaji-the-Second new)
- [ ] **2B.7** Void Maw signs from Maharashtra + Goa logged

### Cluster 2.C — UP + MP (Bloodline B internal)
- [ ] **2C.1** UP — `Ganga-Simhasana` — story.html (the abdication arc)
- [ ] **2C.2** UP — identity update; Yamunadatta added
- [ ] **2C.3** UP — CSV delta (Gangaputra Ch2; Adharma Ch2; Yamunadatta new; Vidura-Babu new)
- [ ] **2C.4** MP — `Hridaya-Sthana` — story.html (twelve courts dissolved)
- [ ] **2C.5** MP — identity update; Sutrakara introduced
- [ ] **2C.6** MP — CSV delta (Dvadashashringa Ch2; Adharma-Kendra Ch2; Sutrakara new)

### Cluster 2.D — NE (Chandravamsha + Vana-Kula northeast)
- [ ] **2D.1** Assam — `Ganda-Kshetra` — story.html (the suppressed coven; Bhairavi-Aaee lineage reveal)
- [ ] **2D.2** Assam — identity update
- [ ] **2D.3** Assam — CSV delta (Kamalavarna Ch2; Kama-Mara Ch2; Bhairavi-Aaee new)
- [ ] **2D.4** Meghalaya — `Megha-Maata` — story.html
- [ ] **2D.5** Meghalaya — identity update; U-Mawkynrew added
- [ ] **2D.6** Meghalaya — CSV delta
- [ ] **2D.7** Manipur — `Sangai-Nata` — story.html (the dance rebellion)
- [ ] **2D.8** Manipur — identity update; Sangaputra introduced
- [ ] **2D.9** Manipur — CSV delta
- [ ] **2D.10** Nagaland — `Dzukou-Rashtra` — story.html (the pure-lineage wars)
- [ ] **2D.11** Nagaland — identity update; Khrieo-Mama added
- [ ] **2D.12** Nagaland — CSV delta
- [ ] **2D.13** Sikkim — `Beyul-Kshetra` — story.html (the refugee council)
- [ ] **2D.14** Sikkim — identity update; Pema-Chöden introduced
- [ ] **2D.15** Sikkim — CSV delta
- [ ] **2D.16** Arunachal — `Arunodaya-Kshetra` — story.html (the night-cultists)
- [ ] **2D.17** Arunachal — identity update; First Herald + Tani-of-the-Veil introduced
- [ ] **2D.18** Arunachal — CSV delta (note: First Herald → new-characters.csv with `type: herald`)
- [ ] **2D.19** Mizoram — `Tlawmngaihna-Desh` — story.html (HERO DEATH)
- [ ] **2D.20** Mizoram — identity update; Tlangvala marked deceased; Hmangaihi introduced
- [ ] **2D.21** Mizoram — CSV delta
- [ ] **2D.22** Tripura — `Tri-Pura` — story.html (HERO FALL; Triputra inherits)
- [ ] **2D.23** Tripura — identity update; Triputra introduced
- [ ] **2D.24** Tripura — CSV delta
- [ ] **2D.25** All NE Void Maw signs logged

### Cluster 2.E — South (Karnataka already done — TN + AP + Kerala + Telangana)
- [ ] **2E.1** Kerala — `Parashurama-Kshetra` — story.html (the 109th form public; teaching Tungabhadra)
- [ ] **2E.2** Kerala — identity update; Sivakami-Acharyini introduced
- [ ] **2E.3** Kerala — CSV delta
- [ ] **2E.4** AP — `Dharmakshetra Amaravati` — story.html (Kalaniksha returns)
- [ ] **2E.5** AP — identity update; Pulakeshi-Babu introduced (lineage reveal trigger)
- [ ] **2E.6** AP — CSV delta
- [ ] **2E.7** TN — `Sangam Tamilakam` — story.html (the silenced assembly)
- [ ] **2E.8** TN — identity update; Avvaiyar-the-Younger added
- [ ] **2E.9** TN — CSV delta
- [ ] **2E.10** Telangana — `Chaya-Golkonda` — story.html (the mirror-city)
- [ ] **2E.11** Telangana — identity update; Bhagmati-Saheba added
- [ ] **2E.12** Telangana — CSV delta

### Cluster 2.F — East (Bihar + Jharkhand + Bengal + Odisha)
- [ ] **2F.1** Odisha — `Kalinga-Chakra` — story.html (the three Jagannaths; chariot pulled alone)
- [ ] **2F.2** Odisha — identity update; Subhadra-of-the-Wood introduced
- [ ] **2F.3** Odisha — CSV delta
- [ ] **2F.4** Bihar — `Vajra-Bhumi` — story.html (Nalanda burns; Maitreyi-the-Younger)
- [ ] **2F.5** Bihar — identity update
- [ ] **2F.6** Bihar — CSV delta
- [ ] **2F.7** Jharkhand — `Vana-Agni` — story.html (the coal heart; Birsa-Aaj as pivot)
- [ ] **2F.8** Jharkhand — identity update
- [ ] **2F.9** Jharkhand — CSV delta
- [ ] **2F.10** West Bengal — `Sundara-Vana` — story.html (the twin delta)
- [ ] **2F.11** West Bengal — identity update; Ganesh-Babu added
- [ ] **2F.12** West Bengal — CSV delta

### Cluster 2.G — North (Punjab + Haryana)
- [ ] **2G.1** Punjab — `Panch-Nada` — story.html (the poisoned river)
- [ ] **2G.2** Punjab — identity update; Bibi Karam-Kaur introduced
- [ ] **2G.3** Punjab — CSV delta
- [ ] **2G.4** Haryana — `Kurukshetra-Bhoomi` — story.html (the marriage fire)
- [ ] **2G.5** Haryana — identity update; Yajna-Devi added
- [ ] **2G.6** Haryana — CSV delta

### Cluster 2.H — Mountain Pact (Uttarakhand + HP + Sikkim — Sikkim already done in 2D)
- [ ] **2H.1** Uttarakhand — `Deva-Bhumi` — story.html (the pilgrim's tax)
- [ ] **2H.2** Uttarakhand — identity update; Bhairavi-Mata introduced
- [ ] **2H.3** Uttarakhand — CSV delta
- [ ] **2H.4** Himachal Pradesh — `Hima-Chhaya` — story.html (the avalanche of names)
- [ ] **2H.5** Himachal Pradesh — identity update; Lama Tashi-of-Spiti added
- [ ] **2H.6** Himachal Pradesh — CSV delta

### Cluster 2.I — Central (Chhattisgarh; MP done in 2C)
- [ ] **2I.1** Chhattisgarh — `Dandakaranya` — story.html (the forest schism)
- [ ] **2I.2** Chhattisgarh — identity update; Aranya-Putri introduced
- [ ] **2I.3** Chhattisgarh — CSV delta

### Cluster 2.J — West dryside (Gujarat + Rajasthan)
- [ ] **2J.1** Gujarat — `Simha-Dwara` — story.html (the pride vote)
- [ ] **2J.2** Gujarat — identity update; Asha-Ben introduced
- [ ] **2J.3** Gujarat — CSV delta
- [ ] **2J.4** Rajasthan — `Maru-Maya` — story.html (the forged fates)
- [ ] **2J.5** Rajasthan — identity update; Ratan-Singh-of-the-Ledger added
- [ ] **2J.6** Rajasthan — CSV delta

### Cluster 2.Z — Chapter 2 Convergence
- [ ] **2Z.1** Write the chapter-closing image — the hawk-relay message across all six regions.
- [ ] **2Z.2** Update `chapter-2-civil-war/index.html` to feature the closing image.
- [ ] **2Z.3** Write `chapter-2-civil-war/maw-signs.md` — the catalogue of 28 Void Maw signs.
- [ ] **2Z.4** Update `chapter-2-civil-war/bharatavarsha/global-map.html` — civil-war faction overlay.
- [ ] **2Z.5** REVIEW with user — Chapter 2 complete. Sign-off needed before starting Chapter 3.

---

## Stage 3 — Chapter 3 Rise of Beasts (production order from `04-chapter-3-rise-of-beasts.md` §10)

Per Regional Dominant: **(a) Beast-Rising scene** | **(b) Bargain/Battle absorption scenes** | **(c) Tattoo-3 Unity Trial** | **(d) Sanctuary leg** | **(e) Dominant page + 4 absorbed/fold pages** | **(f) CSV delta**.

- [ ] **3A** Karnataka — South Dominant story (the Sanctuary's host)
  - [ ] 3A.1 story.html (Beast-Rising + Unity Trial + Sanctuary)
  - [ ] 3A.2 absorbed fold-pages: Kerala, AP, TN, Telangana
  - [ ] 3A.3 CSV delta
- [ ] **3B** Assam — NE Dominant story
  - [ ] 3B.1 story.html
  - [ ] 3B.2 absorbed fold-pages: Meghalaya, Manipur, Nagaland, Sikkim, Arunachal, Mizoram, Tripura
  - [ ] 3B.3 CSV delta
- [ ] **3C** UP — North Dominant story
  - [ ] 3C.1 story.html (Yamunadatta as throne; Gangaputra as regent)
  - [ ] 3C.2 absorbed fold-pages: Haryana, MP-federated, Punjab-federated, Uttarakhand, HP
  - [ ] 3C.3 CSV delta
- [ ] **3D** Odisha — East Dominant story
  - [ ] 3D.1 story.html
  - [ ] 3D.2 absorbed fold-pages: Bihar, Jharkhand, West Bengal
  - [ ] 3D.3 CSV delta
- [ ] **3E** Maharashtra — West Dominant story (double-bond)
  - [ ] 3E.1 story.html
  - [ ] 3E.2 absorbed fold-pages: Goa (occupied), Gujarat, Rajasthan
  - [ ] 3E.3 CSV delta
- [ ] **3F** MP — Central Dominant story (note: MP is *also* federated with UP — handle the dual federation carefully)
  - [ ] 3F.1 story.html
  - [ ] 3F.2 absorbed fold-page: Chhattisgarh
  - [ ] 3F.3 CSV delta
- [ ] **3G** Sanctuary chapter page (the buried Hampi chamber, the seventh seat)
- [ ] **3H** Council chapter page (6 seats filled, 7th cracked)
- [ ] **3I** Global map update (6-region color-coded)
- [ ] **3J** Fourth Herald reveal page
- [ ] **3K** REVIEW with user — Chapter 3 complete.

---

## Stage 4 — Chapter 4 The Great Epic (production order from `05-chapter-4-the-great-epic.md` §9)

- [ ] **4A** Void Maw definition page (`maw.html`) — write first.
- [ ] **4B** Sanctuary update — seat forged from six regional contributions.
- [ ] **4C** Kurukshetra battlefield page.
- [ ] **4D** Maha-Adhipati arc (the spine — Tungabhadra's full Ch 4 story).
- [ ] **4E** Five other Dominants' Ch 4 stories
  - [ ] 4E.1 Gangaputra (UP) — regent's fight + the abdication restated
  - [ ] 4E.2 Jagannathi (Odisha) — Rath Yatra reborn
  - [ ] 4E.3 Shivagati (Maharashtra) — bond-broken-then-restored
  - [ ] 4E.4 Dvadashashringa (MP) — Sutrakara's silent council seat
  - [ ] 4E.5 Kamalavarna (Assam) — the matriarch's final standing
- [ ] **4F** Four Herald redemption stories
  - [ ] 4F.1 Herald 1 — Arunachal (Vana-Kula forgotten firstborn)
  - [ ] 4F.2 Herald 2 — Goa (sailor-without-ship)
  - [ ] 4F.3 Herald 3 — Karnataka (Tungabhadra's forgotten cousin-infant)
  - [ ] 4F.4 Herald 4 — Sikkim (Krodha's redemption)
- [ ] **4G** Council page — seven seats, seven faces.
- [ ] **4H** Volume I epilogue — next continent named.
- [ ] **4I** REVIEW with user — Volume I complete.

---

## Stage 5 — Volume I Wrap

- [ ] **W1.** Update the project root `index.html` to reflect Volume I complete.
- [ ] **W2.** Update `IMPLEMENTATION_PLAN.md` at repo root with Volume I done; Volume II next.
- [ ] **W3.** Generate Volume I cover image / poster (if media generation in scope).
- [ ] **W4.** Final QA pass — broken links, missing media placeholders, CSV format consistency.

---

## Per-Kingdom Atomic Task Template

When picking up any kingdom's Chapter-2 story (e.g. Karnataka — task 2A.1), use this checklist *inside* the task:

```
For kingdom: <slug>
1. Open `01-foundation-kingdoms.md` for the kingdom's Chapter-1 seed.
2. Open `03-chapter-2-civil-war.md` for the kingdom's Crack/Loss/Tattoo-2.5 spec.
3. Open `02-relationship-graph.md` for the kingdom's bloodline & cross-marriages.
4. Read the kingdom's Chapter-1 `story.html` once for voice anchoring.
5. Draft `chapter-2-civil-war/bharatavarsha/regions/<region>/<slug>/story.html`:
   a. Banner (Civil War + Kingdom + Faction subtitle)
   b. Beat 1 — The Crack (5–7 paragraphs)
   c. Beat 2 — The Loss (5–7 paragraphs)
   d. Beat 3 — The Tattoo-2.5 (4–6 paragraphs)
   e. Epilogue — Void Maw sign + bird-message (2 paragraphs)
6. Update `identity.html` with new faction + new characters.
7. Add CSV delta rows.
8. Mark task complete in this file. Commit. Move on.
```

Same template applies for Chapter 3 and Chapter 4 stories (replace beats with phases / acts as appropriate).

---

## Continuation Playbook (for the next session / Claudia)

If a session ends mid-task:
1. Don't reopen earlier completed tasks. Trust the checkmarks.
2. Open this file. Find the first unchecked item.
3. Read the file the item points to.
4. Use the **Per-Kingdom Atomic Task Template** above.
5. If you encounter a contradiction — for example, a story decision that conflicts with what an earlier task did — flag it in a new section at the bottom of this file under "Contradictions found" with file paths and line numbers. Do not silently override.
6. Commit per task, not per cluster.

---

## Estimated Effort (rough)

| Stage | Approx. tasks | Approx. session-days (one focused day per session) |
|---|---|---|
| Stage 0 | 10 decisions | 1 day (just the user) |
| Stage 1 | 8 setup tasks | 1 day |
| Stage 2 | ~110 atomic tasks (28 kingdoms × ~4 per) | 14–20 sessions |
| Stage 3 | ~50 atomic tasks | 7–10 sessions |
| Stage 4 | ~30 atomic tasks | 5–7 sessions |
| Stage 5 | 4 tasks | 1 session |

**Total: ~210 atomic tasks. ~30–40 focused sessions.** This is a Volume-I-of-six saga; it should take real time.

---

## Contradictions found

(empty for now — append here as future sessions encounter them)
