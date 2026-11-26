---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/abjuration
  - source/srd
aliases:
  - "4th Tier Spell: Death Ward"
  - "Death Ward"
  - "4-A-L-DW"
registry_id: 4-A-L-DW
attribute_code: "4·Abj·None·None·Touch·8 hours"
incantation: "Valixiy"
tier: 4
school: Abjuration
affinity: A
grade: L
pz_total: 218.3
pz_quantum: 7029.9
t_e: 0.53
updated: 2026-11-16
---

**Death Ward** (`4-A-L-DW`) is a 4th Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **218 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E 0.53 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Abjuration]]
        - **Death Ward** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-A-L-DW` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Abj·None·None·Touch·8 hours` |
| Incantation | *Valixiy* |
| Affinity | A (Abjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Abjuration]] |
| Casting time | 1 action |
| Range | Touch |
| Area | single point or target |
| Duration | 8 hours |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Cleric, Paladin |

### Mechanism

A touch places a one-use guard on a creature that holds it at the edge of consciousness when it would otherwise fall, or cancels one instant killing effect.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| absorb the lethal blow overflow, 20 injury points | `0.20*20` | 4.0 |
| upkeep: sentinel coupling to 1 creature for 8 h | `0.005*1*8*3600` | 144 |
| Pattern cost | `0.01 × Q4 × (1 + 0.00)` | 70.3 |

| Quantity | Value |
|---|---|
| Effect energy | 4.0 Pz |
| Upkeep energy | 144 Pz (0.005 Pz/s) |
| **Total draw** | **218 Pz** (327.4 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 0.0311 |
| Energy-equivalent tier T_E | 0.53 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Expected overflow absorbed 20 points at 0.20 Pz each; watch coupling at enchantment rate for 8 h.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Death Ward (4-A-L-DW) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 4 | 4 | `0000000001001` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | 8 hours | 8 | `0000000010001` |

### Incantation

Spoken as **Valixiy** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T5: *Tivalixiy* · T6: *Rivalixiy* · T7: *Mivalixiy* · T8: *Nivalixiy* · T9: *Xyivalixiy*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 3→2 | 2 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 4→11 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#61855f`.

![[Death Ward (4-A-L-DW) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.923 | `#ff0028` (700 nm eq.) | source grid |
| Duration | 8 hours | 0.474 | 0.997 | `#00ff66` (558 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.890 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.15): swatch `#a79f8c`, measured lines at 0.007, 0.401, 0.474, 0.883. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.34. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·A·None`; the k4 to k6 lines (None, Touch, 8 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·A·None` |
| Standard spectrometer detection range | 1.48 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 732 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 36.4 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 4th Tier quantum of 7,030 Pz (3.1% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 4th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 4 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Wards and Shields]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Stoneskin (4-A-L-STN)|Stoneskin]] (4) · [[Bulwark (3-A-L-BLW)|Bulwark]] (3) · [[Glyph of Warding (3-A-H-GWY)|Glyph of Warding]] (3) · [[Nondetection (3-A-L-NND)|Nondetection]] (3) · [[Protection From Energy (3-A-L-PE)|Protection From Energy]] (3) · [[Aid (2-A-L-AID)|Aid]] (2) · [[Fire Shield (4-V-L-FSR)|Fire Shield]] (4) · [[Globe of Invulnerability (6-A-L-GIO)|Globe of Invulnerability]] (6).


---

## Tactical Assessment

Standard protection for commanders and high-risk operators before an engagement.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
