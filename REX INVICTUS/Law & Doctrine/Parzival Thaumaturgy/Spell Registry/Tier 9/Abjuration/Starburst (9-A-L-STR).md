---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-9
  - spell/abjuration
  - source/science-spellbook
aliases:
  - "9th Tier Spell: Starburst"
  - "9-A-L-STR"
  - "Starburst (Science)"
registry_id: 9-A-L-STR
attribute_code: "9·Abj·Fire·sphere (20)·1 mile·Instantaneous"
incantation: "Xyaire-Soyp"
tier: 9
school: Abjuration
affinity: A
grade: L
pz_total: 309848.4
pz_quantum: 1043335.3
t_e: 7.79
updated: 2026-11-16
---

**Starburst** (`9-A-L-STR`) is a 9th Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **309,848 Pz** against a slot quantum of 1.04 MPz Pz, which puts its energy-equivalent tier at T_E 7.79 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 9 Workings]]
      - [[Abjuration]]
        - **Starburst** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `9-A-L-STR` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `9·Abj·Fire·sphere (20)·1 mile·Instantaneous` |
| Incantation | *Xyaire-Soyp* |
| Affinity | A (Abjuration) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 9th Tier |
| School | [[Abjuration]] |
| Casting time | 1 Action |
| Range | 1 mile |
| Area | sphere (20) |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A small sweet food item |
| Ritual | no |
| Injury | 9d6 fire (mean 31.5) |
| Injury by tier | T9: 9d6 |
| Resistance check | agility; on success: half injury |
| Practitioner lineages | Wizard |

### Mechanism

Twenty star-like fireballs erupt at chosen points within a mile, each filling a 20 ft radius.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Twenty fireballs | `31.5 HP x 0.7 (fire) x S/A_c, S = sphere r=6.096 m = 467.0 m^2 x 20` | 294,198 |
| Pattern cost | `0.01 × Q9 × (1 + 0.50)` | 15,650 |

| Quantity | Value |
|---|---|
| Effect energy | 294,198 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **309,848 Pz** (464,772.7 kJ) |
| Slot quantum Q9 | 1.04 MPz Pz |
| Field gain (draw / quantum) | 0.297 |
| Energy-equivalent tier T_E | 7.79 |
| Handling points | 0.50 |
| Grade score | -0.11 → L |

**Handling flags:** multi target control.

**Assumptions:** Fire 9d6 = 31.5 over twenty 20 ft spheres.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Starburst (9-A-L-STR) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 9 | 9 | `0000000010011` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | Fire | 3 | `0000000000111` |
| k4 Area | sphere (20) | 30 | `0000000111101` |
| k5 Range | 1 mile | 0 | `0000000000001` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Xyaire-Soyp** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 4→3 | 3 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 | 3 |
| k4 Area | 0→9 2→11 3→12 4→0 5→1 | 5 |
| k5 Range | 0→8 | 1 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#bc2b7a`.

![[Starburst (9-A-L-STR) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 9 | 0.900 | 1.000 | `#b600ff` (430 nm eq.) | source grid |
| Damage | Fire | 0.286 | 0.828 | `#9cff00` (614 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.667 | `#ff0028` (700 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.667 | `#ff0028` (700 nm eq.) | source grid |
| Area | sphere (20) | 0.833 | 0.998 | `#5a00ff` (450 nm eq.) | source grid |
| Range | 1 mile | 0.000 | 0.667 | `#ff0028` (700 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 5.49. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `9·A·Fire`; the k4 to k6 lines (sphere (20), 1 mile, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `9·A·Fire` |
| Standard spectrometer detection range | 55.66 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 52,167 Pz (0.05 × Q9) |
| Counter drawn cold (all six layers) | 104,334 Pz (0.10 × Q9) |
| Unravel after completion | 104,334 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Energy, Movement and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1b 1c 1f 1H 1i` (Within, Heat, Light, Energy, Rigidity, Hope).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 51,641 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 9th Tier quantum of 1.04 MPz Pz (29.7% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 9th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 9 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Area Destruction]] |
| Element | [[Fire Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Eruption (9-V-M-ERP)|Eruption]] (9) · [[Meteor Swarm (9-V-L-MST)|Meteor Swarm]] (9) · [[Thermonuclear Fireball (9-P-L-TFE)|Thermonuclear Fireball]] (9) · [[Incendiary Cloud (8-C-M-IC)|Incendiary Cloud]] (8) · [[Supernova (8-V-L-SPR)|Supernova]] (8) · [[Delayed Blast Fireball (7-V-M-DBF)|Delayed Blast Fireball]] (7) · [[Fire Storm (7-V-L-FSS)|Fire Storm]] (7) · [[Outflows (5-A-L-OTF)|Outflows]] (5).


---

## Tactical Assessment

Strategic saturation strike against dispersed formations.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 9 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
