---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/transmutation
  - source/srd
aliases:
  - "3rd Tier Spell: Haste"
  - "Haste"
  - "3-T-L-HST"
registry_id: 3-T-L-HST
attribute_code: "3·Tra·None·None·30 feet·Up to 1 minute"
incantation: "Lieusinse"
tier: 3
school: Transmutation
affinity: T
grade: L
pz_total: 51.3
pz_quantum: 2586.2
t_e: -0.92
updated: 2026-11-16
---

**Haste** (`3-T-L-HST`) is a 3rd Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **51.3 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E -0.92 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Transmutation]]
        - **Haste** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-T-L-HST` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Tra·None·None·30 feet·Up to 1 minute` |
| Incantation | *Lieusinse* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Transmutation]] |
| Casting time | 1 action |
| Range | 30 feet |
| Area | single point or target |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A shaving of licorice root |
| Ritual | no |
| Practitioner lineages | Sorcerer, Wizard |

### Mechanism

Accelerates one creature's movement and action cycle for up to a minute, followed by a short crash when the field drops.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| defence bonus absorption | `0.20 Pz * (10% of 15 HP/round * 10 rounds = 15 HP)` | 3.0 |
| extra metabolic and kinetic power | `400 W / 1500 = 0.266667 Pz/s * 60 s` | 16.0 |
| Pattern cost | `0.01 × Q3 × (1 + 0.25)` | 32.3 |

| Quantity | Value |
|---|---|
| Effect energy | 3.0 Pz |
| Upkeep energy | 16.0 Pz (0.267 Pz/s) |
| **Total draw** | **51.3 Pz** (77.0 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 0.0198 |
| Energy-equivalent tier T_E | -0.92 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** concentration.

**Assumptions:** Additional 400 W of mechanical and metabolic output for 1 minute; improved defence absorbs 10% of incoming injury.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Haste (3-T-L-HST) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Lieusinse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vilieusinse* · T5: *Tilieusinse* · T6: *Rilieusinse* · T7: *Milieusinse* · T8: *Nilieusinse* · T9: *Xyilieusinse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#6da377`.

![[Haste (3-T-L-HST) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.848 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.929 | `#0074ff` (495 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 1.000 | `#91ff00` (612 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.18): swatch `#8fa9b2`, measured lines at 0.299, 0.685, 0.876. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.71. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·T·None`; the k4 to k6 lines (None, 30 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·T·None` |
| Standard spectrometer detection range | 0.72 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 262 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 8.6 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 3rd Tier quantum of 2,586 Pz (2.0% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Movement and Flight]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Fly (3-T-L-FLY)|Fly]] (3) · [[Gaseous Form (3-T-M-GF)|Gaseous Form]] (3) · [[Slow (3-T-L-SLW)|Slow]] (3) · [[Water Breathing (3-T-L-WBT)|Water Breathing]] (3) · [[Water Walk (3-T-L-WW)|Water Walk]] (3) · [[Accelerate (2-T-L-ACC)|Accelerate]] (2) · [[Freefall (4-T-L-FRF)|Freefall]] (4) · [[Levitate (2-T-L-LVT)|Levitate]] (2).


---

## Tactical Assessment

Doubles the output of an elite soldier or vehicle crew member for a single engagement; the after-effect makes timing important.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
