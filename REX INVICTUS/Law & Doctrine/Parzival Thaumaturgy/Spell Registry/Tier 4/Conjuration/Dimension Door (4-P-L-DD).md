---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/conjuration
  - source/srd
aliases:
  - "4th Tier Spell: Dimension Door"
  - "Dimension Door"
  - "4-P-L-DD"
registry_id: 4-P-L-DD
attribute_code: "4·Con·Force·None·500 feet·Instantaneous"
incantation: "Veton-’sin"
tier: 4
school: Conjuration
affinity: P
grade: L
pz_total: 72.7
pz_quantum: 7029.9
t_e: -0.57
updated: 2026-11-16
---

**Dimension Door** (`4-P-L-DD`) is a 4th Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **72.7 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E -0.57 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Conjuration]]
        - **Dimension Door** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-P-L-DD` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Con·Force·None·500 feet·Instantaneous` |
| Incantation | *Veton-’sin* |
| Affinity | P (Pure field construct) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | 500 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation) |
| Ritual | no |
| Injury | 4d6 force (mean 14) |
| Injury by tier | T4: 4d6 |
| Practitioner lineages | Bard, Sorcerer, Warlock, Wizard |

### Mechanism

The caster and one companion jump to any point within 500 ft. Arriving inside a solid object aborts the jump and injures both.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| teleport 2 x 80 kg over 500 ft | `0.01*2*80*15*(500*ft)/J` | 2.4 |
| Pattern cost | `0.01 × Q4 × (1 + 0.00)` | 70.3 |

| Quantity | Value |
|---|---|
| Effect energy | 2.4 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **72.7 Pz** (109.1 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 0.0103 |
| Energy-equivalent tier T_E | -0.57 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Two 80 kg travellers with gear; failure injury excluded.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Dimension Door (4-P-L-DD) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 4 | 4 | `0000000001001` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | Force | 4 | `0000000001001` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 500 feet | 8 | `0000000010001` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Veton-’sin** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T5: *Tiveton-’sin* · T6: *Riveton-’sin* · T7: *Miveton-’sin* · T8: *Niveton-’sin* · T9: *Xyiveton-’sin*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 3→2 | 2 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 3→0 | 2 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 4→12 | 2 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#6eb61b`.

![[Dimension Door (4-P-L-DD) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| Damage | Force | 0.357 | 0.999 | `#3bff00` (593 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.963 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.923 | `#ff0028` (700 nm eq.) | source grid |
| Range | 500 feet | 0.471 | 0.998 | `#00ff60` (559 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.16): swatch `#cfb26c`, measured lines at 0.004, 0.126, 0.358, 0.401, 0.471. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.86. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·C·Force`; the k4 to k6 lines (None, 500 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·C·Force` |
| Standard spectrometer detection range | 0.85 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 703 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Beyond, Introspection, 2x Movement and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `2a 1e 1F 1G 3j` (2x Beyond, Prodigious, Potential, Introspection, 3x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 12.1 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 4th Tier quantum of 7,030 Pz (1.0% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 4th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 4 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Pure]] (P) |
| Function | [[Teleportation and Planar Travel]], [[Precision Strikes]] |
| Element | [[Force Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Tidal Force (4-P-L-TF)|Tidal Force]] (4) · [[Faithful Hound (4-C-L-FH)|Faithful Hound]] (4) · [[Secret Chest (4-C-M-SCC)|Secret Chest]] (4) · [[Spiritual Weapon (2-P-L-SW)|Spiritual Weapon]] (2) · [[Arcane Sword (7-P-L-ASC)|Arcane Sword]] (7) · [[Magic Missile (1-P-L-MM)|Magic Missile]] (1) · [[Teleportation Circle (5-C-M-TC)|Teleportation Circle]] (5) · [[Tree Stride (5-C-L-TSE)|Tree Stride]] (5).


---

## Tactical Assessment

Short-range extraction or insertion across walls and obstacles.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
