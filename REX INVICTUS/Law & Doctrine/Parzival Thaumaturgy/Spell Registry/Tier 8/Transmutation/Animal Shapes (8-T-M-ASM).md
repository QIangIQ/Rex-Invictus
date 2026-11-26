---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-8
  - spell/transmutation
  - source/srd
aliases:
  - "8th Tier Spell: Animal Shapes"
  - "Animal Shapes"
  - "8-T-M-ASM"
registry_id: 8-T-M-ASM
attribute_code: "8·Tra·None·None·30 feet·Up to 24 hours"
incantation: "Nieusinyi"
tier: 8
school: Transmutation
affinity: T
grade: M
pz_total: 40635.1
pz_quantum: 383821.6
t_e: 5.75
updated: 2026-11-16
---

**Animal Shapes** (`8-T-M-ASM`) is a 8th Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **40,635 Pz** against a slot quantum of 383,822 Pz, which puts its energy-equivalent tier at T_E 5.75 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 8 Workings]]
      - [[Transmutation]]
        - **Animal Shapes** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `8-T-M-ASM` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `8·Tra·None·None·30 feet·Up to 24 hours` |
| Incantation | *Nieusinyi* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 8th Tier |
| School | [[Transmutation]] |
| Casting time | 1 action |
| Range | 30 feet |
| Area | single point or target |
| Duration | Up to 24 hours (concentration) |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Druid |

### Mechanism

Several willing bodies are rebuilt into large animal forms, with gear absorbed into the new structure, and each can be reshaped again while the field holds.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| added living mass | `4 targets * 320 kg added tissue * 10 Pz/kg` | 12,800 |
| body sustainment upkeep | `0.05 Pz/s * 4 bodies * 86400 s` | 17,280 |
| Pattern cost | `0.01 × Q8 × (1 + 1.75)` | 10,555 |

| Quantity | Value |
|---|---|
| Effect energy | 12,800 Pz |
| Upkeep energy | 17,280 Pz (0.2 Pz/s) |
| **Total draw** | **40,635 Pz** (60,952.6 kJ) |
| Slot quantum Q8 | 383,822 Pz |
| Field gain (draw / quantum) | 0.106 |
| Energy-equivalent tier T_E | 5.75 |
| Handling points | 1.75 |
| Grade score | 0.75 → M |

**Handling flags:** concentration, fragile, multi target control.

**Assumptions:** 4 willing targets; each grows from 80 kg to about 400 kg; 10 Pz/kg for added tissue; 0.05 Pz/s per sustained body for 24 h.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Animal Shapes (8-T-M-ASM) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 8 | 8 | `0000000010001` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Up to 24 hours | 17 | `0000000100011` |

### Incantation

Spoken as **Nieusinyi** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T9: *Xyinieusinyi*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 4→3 | 2 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 5→12 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#7f39c5`.

![[Animal Shapes (8-T-M-ASM) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 8 | 0.800 | 1.000 | `#2900ff` (460 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.997 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Up to 24 hours | 0.895 | 0.996 | `#b100ff` (432 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.880 | `#91ff00` (612 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.13): swatch `#507ee3`, measured lines at 0.295, 0.801, 0.875, 0.895. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.61. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `8·T·None`; the k4 to k6 lines (None, 30 feet, Up to 24 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `8·T·None` |
| Standard spectrometer detection range | 20.16 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 19,191 Pz (0.05 × Q8) |
| Counter drawn cold (all six layers) | 38,382 Pz (0.10 × Q8) |
| Unravel after completion | 41,838 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 6,773 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 8th Tier quantum of 383,822 Pz (10.6% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 8th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 8 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Transformation]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Shapechange (9-T-L-SHP)|Shapechange]] (9) · [[True Polymorph (9-T-L-TPU)|True Polymorph]] (9) · [[Flesh to Stone (6-T-L-FSE)|Flesh to Stone]] (6) · [[Control Weather (8-T-H-CWT)|Control Weather]] (8) · [[Glibness (8-T-L-GLB)|Glibness]] (8) · [[Magic Jar (6-N-H-MJ)|Magic Jar]] (6) · [[Polymorph (4-T-L-PLY)|Polymorph]] (4) · [[Alter Biome (9-T-X-AB)|Alter Biome]] (9).


---

## Tactical Assessment

Converts a squad into fast, terrain-capable beasts for reconnaissance or pursuit over a full day.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 8 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
