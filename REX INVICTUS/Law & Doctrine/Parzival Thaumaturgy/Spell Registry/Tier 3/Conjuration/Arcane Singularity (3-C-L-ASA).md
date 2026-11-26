---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/conjuration
  - source/science-spellbook
aliases:
  - "3rd Tier Spell: Arcane Singularity"
  - "3-C-L-ASA"
  - "Arcane Singularity (Science)"
registry_id: 3-C-L-ASA
attribute_code: "3·Con·None·sphere (60)·30 feet·Up to 1 minute"
incantation: "Le’-Siusinse"
tier: 3
school: Conjuration
affinity: C
grade: L
pz_total: 686.1
pz_quantum: 2586.2
t_e: 1.67
updated: 2026-11-16
---

**Arcane Singularity** (`3-C-L-ASA`) is a 3rd Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **686 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E 1.67 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Conjuration]]
        - **Arcane Singularity** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-C-L-ASA` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Con·None·sphere (60)·30 feet·Up to 1 minute` |
| Incantation | *Le’-Siusinse* |
| Affinity | C (Conjuration) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Conjuration]] |
| Casting time | 1 Action |
| Range | 30 feet |
| Area | sphere (60) |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Wizard |

### Mechanism

Hangs a small dark attractor over a target creature that captures workings passing within 60 ft and pulls their aim onto that creature.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Retargeting captured working (upkeep) | `0.05 x 13075 Pz x 1 per minute` | 654 |
| Pattern cost | `0.01 × Q3 × (1 + 0.25)` | 32.3 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 654 Pz (10.9 Pz/s) |
| **Total draw** | **686 Pz** (1,029.2 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 0.265 |
| Energy-equivalent tier T_E | 1.67 |
| Handling points | 0.25 |
| Grade score | -0.41 → L |

**Handling flags:** concentration.

**Assumptions:** One reference tier-3 area working (13,076 Pz) captured per minute, at 5% of its energy to retarget.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Arcane Singularity (3-C-L-ASA) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (60) | 35 | `0000001000111` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Le’-Siusinse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vile’-Siusinse* · T5: *Tile’-Siusinse* · T6: *Rile’-Siusinse* · T7: *Mile’-Siusinse* · T8: *Nile’-Siusinse* · T9: *Xyile’-Siusinse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 2→11 6→2 | 4 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#9c9e59`.

![[Arcane Singularity (3-C-L-ASA) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.985 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.929 | `#0074ff` (495 nm eq.) | source grid |
| Area | sphere (60) | 0.972 | 0.798 | `#ff00e5` (408 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 1.000 | `#91ff00` (612 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 2.84. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·C·None`; the k4 to k6 lines (sphere (60), 30 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·C·None` |
| Standard spectrometer detection range | 2.62 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 389 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 114 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 3rd Tier quantum of 2,586 Pz (26.5% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Summoning and Conjured Creatures]], [[Divination and Sensing]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Arcane Hand (5-P-L-AH)|Arcane Hand]] (5) · [[Conjure Animals (3-C-M-CA)|Conjure Animals]] (3) · [[Spirit Guardians (3-C-M-SGR)|Spirit Guardians]] (3) · [[Stinking Cloud (3-C-M-SCI)|Stinking Cloud]] (3) · [[Conjure Magic Prism (4-C-L-CMPJ)|Conjure Magic Prism]] (4) · [[Conjure Minor Elementals (4-C-M-CME)|Conjure Minor Elementals]] (4) · [[Conjure Woodland Beings (4-C-L-CWB)|Conjure Woodland Beings]] (4) · [[Faithful Hound (4-C-L-FH)|Faithful Hound]] (4).


---

## Tactical Assessment

Area protection for a convoy or position that turns incoming fire onto a designated enemy.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
