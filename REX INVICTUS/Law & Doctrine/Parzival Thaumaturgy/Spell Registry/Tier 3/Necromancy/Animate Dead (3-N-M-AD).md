---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/necromancy
  - source/srd
aliases:
  - "3rd Tier Spell: Animate Dead"
  - "Animate Dead"
  - "3-N-M-AD"
registry_id: 3-N-M-AD
attribute_code: "3·Nec·None·None·10 feet·Instantaneous"
incantation: "Louspul"
tier: 3
school: Necromancy
affinity: N
grade: M
pz_total: 5165.3
pz_quantum: 2586.2
t_e: 3.69
updated: 2026-11-16
---

**Animate Dead** (`3-N-M-AD`) is a 3rd Tier working of the [[Necromancy (School)|Necromancy]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **5,165 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E 3.69 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Necromancy (School)|Necromancy]]
        - **Animate Dead** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-N-M-AD` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Nec·None·None·10 feet·Instantaneous` |
| Incantation | *Louspul* |
| Affinity | N (Necromancy) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Necromancy (School)\|Necromancy]] |
| Casting time | 1 minute |
| Range | 10 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A drop of blood, a piece of flesh, and a pinch of bone dust |
| Ritual | no |
| Practitioner lineages | Cleric, Wizard |

### Mechanism

A corpse or skeleton is threaded with an autonomous motor pattern that obeys the caster for a day before control lapses.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| corpse animation | `80 kg * 10 Pz/kg (semi-living)` | 800 |
| control upkeep | `0.05 Pz/s * 1 creature * 86400 s` | 4,320 |
| Pattern cost | `0.01 × Q3 × (1 + 0.75)` | 45.3 |

| Quantity | Value |
|---|---|
| Effect energy | 800 Pz |
| Upkeep energy | 4,320 Pz (0.05 Pz/s) |
| **Total draw** | **5,165 Pz** (7,747.9 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 2 |
| Energy-equivalent tier T_E | 3.69 |
| Handling points | 0.75 |
| Grade score | 1.10 → M |

**Handling flags:** multi target control, long cast.

**Assumptions:** Medium corpse 80 kg at 10 Pz/kg; control sustained at 0.05 Pz/s for 24 h.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Animate Dead (3-N-M-AD) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Necromancy | 6 | `0000000001101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 10 feet | 1 | `0000000000011` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Louspul** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vilouspul* · T5: *Tilouspul* · T6: *Rilouspul* · T7: *Milouspul* · T8: *Nilouspul* · T9: *Xyilouspul*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 2→0 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 | 2 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#a45146`.

![[Animate Dead (3-N-M-AD) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| School | Necromancy | 0.750 | 0.904 | `#0017ff` (475 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.956 | `#ff0028` (700 nm eq.) | source grid |
| Range | 10 feet | 0.059 | 0.971 | `#ff2700` (682 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.13): swatch `#969284`, measured lines at 0.004, 0.059, 0.300, 0.751. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.71. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·N·None`; the k4 to k6 lines (None, 10 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·N·None` |
| Standard spectrometer detection range | 7.19 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 1,123 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Dark, 2x Death. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1D 1F 1J` (Within, Death, Potential, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 861 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 2.00 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 3rd Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Necromancy school with aspect lean Within, Dark, 2x Death. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Necromancy (School)\|Necromancy]] |
| Affinity | [[Necromancy (School)\|Necromancy]] (N) |
| Function | [[Summoning and Conjured Creatures]], [[Necromantic and Soul Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Create Undead (6-N-L-CU)|Create Undead]] (6) · [[Speak with Dead (3-N-L-SDE)|Speak with Dead]] (3) · [[Vampiric Touch (3-N-L-VT)|Vampiric Touch]] (3) · [[Blight (4-N-L-BLG)|Blight]] (4) · [[Clone (8-N-L-CLN)|Clone]] (8) · [[Gentle Repose (2-N-H-GR)|Gentle Repose]] (2) · [[Arcane Singularity (3-C-L-ASA)|Arcane Singularity]] (3) · [[Beacon of Hope (3-A-L-BHA)|Beacon of Hope]] (3).


---

## Tactical Assessment

Expendable labor and sentries in contaminated zones; renewal can keep up to four bodies under control.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Necromancy (School)|Necromancy]] · [[Spell Breakdown Procedure]] · [[Parzival]]
