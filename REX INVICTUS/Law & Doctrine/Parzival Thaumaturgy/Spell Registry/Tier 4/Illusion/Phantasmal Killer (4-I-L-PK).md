---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/illusion
  - source/srd
aliases:
  - "4th Tier Spell: Phantasmal Killer"
  - "Phantasmal Killer"
  - "4-I-L-PK"
registry_id: 4-I-L-PK
attribute_code: "4·Ill·Psychic·None·120 feet·Up to 1 minute"
incantation: "Vaichar-’mulse"
tier: 4
school: Illusion
affinity: I
grade: L
pz_total: 88.8
pz_quantum: 7029.9
t_e: -0.37
updated: 2026-11-16
---

**Phantasmal Killer** (`4-I-L-PK`) is a 4th Tier working of the [[Illusion]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **88.8 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E -0.37 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Illusion]]
        - **Phantasmal Killer** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-I-L-PK` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Ill·Psychic·None·120 feet·Up to 1 minute` |
| Incantation | *Vaichar-’mulse* |
| Affinity | I (Illusion) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Illusion]] |
| Casting time | 1 action |
| Range | 120 feet |
| Area | single point or target |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 4d10 psychic (mean 22) |
| Injury by tier | T4: 4d10 |
| Resistance check | will; on success: no effect |
| Practitioner lineages | Wizard |

### Mechanism

The field projects a private vision of the subject's worst fear and inflicts repeated mental injury until it shakes off the effect.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Psychic injury, 3 rounds | `3 * 22 HP * 0.02 * 0.5` | 0.66 |
| Fear hold, one subject (upkeep) | `0.005 Pz/s * 60 s` | 0.3 |
| Pattern cost | `0.01 × Q4 × (1 + 0.25)` | 87.9 |

| Quantity | Value |
|---|---|
| Effect energy | 0.66 Pz |
| Upkeep energy | 0.3 Pz (0.005 Pz/s) |
| **Total draw** | **88.8 Pz** (133.3 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 0.0126 |
| Energy-equivalent tier T_E | -0.37 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** concentration.

**Assumptions:** 4d10 = 22 per round, full value, for 3 rounds.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Phantasmal Killer (4-I-L-PK) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 4 | 4 | `0000000001001` |
| k2 School | Illusion | 5 | `0000000001011` |
| k3 Damage | Psychic | 10 | `0000000010101` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 120 feet | 3 | `0000000000111` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Vaichar-’mulse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T5: *Tivaichar-’mulse* · T6: *Rivaichar-’mulse* · T7: *Mivaichar-’mulse* · T8: *Nivaichar-’mulse* · T9: *Xyivaichar-’mulse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 3→2 | 2 |
| k2 School | 0→11 1→12 3→1 | 3 |
| k3 Damage | 0→10 2→12 4→1 | 3 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#33aa97`.

![[Phantasmal Killer (4-I-L-PK) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| Damage | Psychic | 0.714 | 0.952 | `#004dff` (486 nm eq.) | source grid |
| School | Illusion | 0.625 | 0.975 | `#00c5ff` (512 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.960 | `#0074ff` (495 nm eq.) | source grid |
| Range | 120 feet | 0.176 | 0.975 | `#ffc900` (647 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.20): swatch `#6cd6b5`, measured lines at 0.177, 0.401, 0.626, 0.685, 0.715. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.95. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·I·Psychic`; the k4 to k6 lines (None, 120 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·I·Psychic` |
| Standard spectrometer detection range | 0.94 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 703 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Dark, Potential, Introspection, Hopelessness and the school lean is Light, Introspection, 2x Flexibility. The working vector used by [[Recast Tension and Combination Affinity]] is `1F 2G 2h 1I` (Potential, 2x Introspection, 2x Flexibility, Hopelessness).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 14.8 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 4th Tier quantum of 7,030 Pz (1.3% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 4th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Illusion school with aspect lean Light, Introspection, 2x Flexibility. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 4 Workings]] |
| School | [[Illusion]] |
| Affinity | [[Illusion]] (I) |
| Function | [[Mind and Will]], [[Precision Strikes]] |
| Element | [[Psychic Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Dream (5-I-L-DRM)|Dream]] (5) · [[Feeblemind (8-E-L-FBL)|Feeblemind]] (8) · [[Vicious Mockery (0-E-L-VM)|Vicious Mockery]] (0) · [[Fear (3-I-L-FEA)|Fear]] (3) · [[Hypnotic Pattern (3-I-L-HPP)|Hypnotic Pattern]] (3) · [[Blight (4-N-L-BLG)|Blight]] (4) · [[Compulsion (4-E-L-CMP)|Compulsion]] (4) · [[Confusion (4-E-L-CNF)|Confusion]] (4).


---

## Tactical Assessment

Breaks the nerve of a single officer or champion and may disable it outright. Strong-willed subjects throw it off quickly.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Illusion]] · [[Spell Breakdown Procedure]] · [[Parzival]]
