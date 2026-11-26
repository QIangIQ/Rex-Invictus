---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/transmutation
  - source/srd
aliases:
  - "5th Tier Spell: Telekinesis"
  - "Telekinesis"
  - "5-P-L-TLK"
registry_id: 5-P-L-TLK
attribute_code: "5·Tra·None·sphere (30)·60 feet·Up to 10 minutes"
incantation: "Tie’-Sorwynly"
tier: 5
school: Transmutation
affinity: P
grade: L
pz_total: 2987.0
pz_quantum: 19109.4
t_e: 3.14
updated: 2026-11-16
---

**Telekinesis** (`5-P-L-TLK`) is a 5th Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **2,987 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 3.14 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Transmutation]]
        - **Telekinesis** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-P-L-TLK` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Tra·None·sphere (30)·60 feet·Up to 10 minutes` |
| Incantation | *Tie’-Sorwynly* |
| Affinity | P (Pure field construct) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Transmutation]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | sphere (30) |
| Duration | Up to 10 minutes (concentration) |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Sorcerer, Wizard |

### Mechanism

The caster exerts a directed force field able to move up to 450 kg by 9 m per round, hold it suspended, or perform fine manipulation.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| First 30 ft lift of 1000 lb | `453.6 kg * 9.81 * 9.144 m / 1500` | 27.1 |
| Upkeep: Repeated 30 ft moves, 99 rounds | `27.13 Pz * 99` | 2,685 |
| Upkeep: Suspension of load | `0.02 * 453.6 kg * 9.81 * 600 s / 1500` | 35.6 |
| Pattern cost | `0.01 × Q5 × (1 + 0.25)` | 239 |

| Quantity | Value |
|---|---|
| Effect energy | 27.1 Pz |
| Upkeep energy | 2,721 Pz (4.6 Pz/s) |
| **Total draw** | **2,987 Pz** (4,480.5 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 0.156 |
| Energy-equivalent tier T_E | 3.14 |
| Handling points | 0.25 |
| Grade score | -0.68 → L |

**Handling flags:** concentration.

**Assumptions:** Maximum load moved vertically 30 ft every round for 10 min.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Telekinesis (5-P-L-TLK) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (30) | 31 | `0000000111111` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Up to 10 minutes | 15 | `0000000011111` |

### Incantation

Spoken as **Tie’-Sorwynly** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Ritie’-Sorwynly* · T7: *Mitie’-Sorwynly* · T8: *Nitie’-Sorwynly* · T9: *Xyitie’-Sorwynly*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 2→11 3→12 4→0 5→1 | 6 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 2→9 3→10 4→11 | 5 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#3b68e6`.

![[Telekinesis (5-P-L-TLK) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.932 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Up to 10 minutes | 0.789 | 0.959 | `#1e00ff` (463 nm eq.) | source grid |
| Area | sphere (30) | 0.861 | 0.937 | `#8000ff` (442 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.996 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.23): swatch `#4eafdd`, measured lines at 0.501, 0.589, 0.790, 0.872. One or more predicted lines have no measured counterpart; the plate may merge overlapping lines.

Relative luminosity scales with initial energy: log10(E) = 3.48. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·T·None`; the k4 to k6 lines (sphere (30), 60 feet, Up to 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·T·None` |
| Standard spectrometer detection range | 5.47 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 2,455 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 498 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 5th Tier quantum of 19,109 Pz (15.6% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 5th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 5 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Pure]] (P) |
| Function | [[Movement and Flight]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Freefall (4-T-L-FRF)|Freefall]] (4) · [[Wind Walk (6-T-L-WWD)|Wind Walk]] (6) · [[Fly (3-T-L-FLY)|Fly]] (3) · [[Gaseous Form (3-T-M-GF)|Gaseous Form]] (3) · [[Haste (3-T-L-HST)|Haste]] (3) · [[Reverse Gravity (7-T-L-RG)|Reverse Gravity]] (7) · [[Sequester (7-T-L-SQS)|Sequester]] (7) · [[Slow (3-T-L-SLW)|Slow]] (3).


---

## Tactical Assessment

Lifts vehicles, barricades and prisoners, strips weapons from hands, and operates mechanisms at range.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
