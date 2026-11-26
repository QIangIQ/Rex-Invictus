---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-9
  - spell/illusion
  - source/srd
aliases:
  - "9th Tier Spell: Weird"
  - "Weird"
  - "9-I-L-WRD"
registry_id: 9-I-L-WRD
attribute_code: "9·Ill·None·sphere (30)·120 feet·Up to 1 minute"
incantation: "Xyai’-Sormulse"
tier: 9
school: Illusion
affinity: I
grade: L
pz_total: 20242.8
pz_quantum: 1043335.3
t_e: 5.06
updated: 2026-11-16
---

**Weird** (`9-I-L-WRD`) is a 9th Tier working of the [[Illusion]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **20,243 Pz** against a slot quantum of 1.04 MPz Pz, which puts its energy-equivalent tier at T_E 5.06 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 9 Workings]]
      - [[Illusion]]
        - **Weird** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `9-I-L-WRD` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `9·Ill·None·sphere (30)·120 feet·Up to 1 minute` |
| Incantation | *Xyai’-Sormulse* |
| Affinity | I (Illusion) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 9th Tier |
| School | [[Illusion]] |
| Casting time | 1 action |
| Range | 120 feet |
| Area | sphere (30) |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Resistance check | will; on success: no effect |
| Practitioner lineages | Wizard |

### Mechanism

Each creature in a 9 m sphere sees an individually tailored phantom of its worst fear, which paralyses with dread and inflicts repeated psychic injury.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Psychic injury, 3 triggers | `22 * 0.02 * 1051 / 0.7 * 3` | 1,981 |
| Upkeep: Individual fear projections, 10 creatures | `0.005 * 10 * 60 s` | 3.0 |
| Upkeep: Illusion volume | `0.002 * (3203/1000) * 60` | 0.384 |
| Pattern cost | `0.01 × Q9 × (1 + 0.75)` | 18,258 |

| Quantity | Value |
|---|---|
| Effect energy | 1,981 Pz |
| Upkeep energy | 3.4 Pz (0.0564 Pz/s) |
| **Total draw** | **20,243 Pz** (30,364.1 kJ) |
| Slot quantum Q9 | 1.04 MPz Pz |
| Field gain (draw / quantum) | 0.0194 |
| Energy-equivalent tier T_E | 5.06 |
| Handling points | 0.75 |
| Grade score | -0.25 → L |

**Handling flags:** concentration, multi target control.

**Assumptions:** 4d10 = 22; 10 creatures; 3 triggers. Physical cost far below tier; complexity dominates.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Weird (9-I-L-WRD) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 9 | 9 | `0000000010011` |
| k2 School | Illusion | 5 | `0000000001011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (30) | 31 | `0000000111111` |
| k5 Range | 120 feet | 3 | `0000000000111` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Xyai’-Sormulse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 4→3 | 3 |
| k2 School | 0→11 1→12 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 2→11 3→12 4→0 5→1 | 6 |
| k5 Range | 0→8 1→9 2→10 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#6b61d5`.

![[Weird (9-I-L-WRD) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 9 | 0.900 | 1.000 | `#b600ff` (430 nm eq.) | source grid |
| School | Illusion | 0.625 | 0.963 | `#00c5ff` (512 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.977 | `#0074ff` (495 nm eq.) | source grid |
| Area | sphere (30) | 0.861 | 0.999 | `#8000ff` (442 nm eq.) | source grid |
| Range | 120 feet | 0.176 | 0.770 | `#ffc900` (647 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 4.31. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `9·I·None`; the k4 to k6 lines (sphere (30), 120 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `9·I·None` |
| Standard spectrometer detection range | 14.23 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 52,167 Pz (0.05 × Q9) |
| Counter drawn cold (all six layers) | 104,334 Pz (0.10 × Q9) |
| Unravel after completion | 104,334 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Light, Introspection, 2x Flexibility. The working vector used by [[Recast Tension and Combination Affinity]] is `2c 1d 1F 1G 2h 1J` (2x Light, Life, Potential, Introspection, 2x Flexibility, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 3,374 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 9th Tier quantum of 1.04 MPz Pz (1.9% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 9th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Illusion school with aspect lean Light, Introspection, 2x Flexibility. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 9 Workings]] |
| School | [[Illusion]] |
| Affinity | [[Illusion]] (I) |
| Function | [[Mind and Will]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Power Word Kill (9-E-L-PWK)|Power Word Kill]] (9) · [[Antipathy-Sympathy (8-E-L-ASP)|Antipathy/Sympathy]] (8) · [[Dominate Monster (8-E-L-DMM)|Dominate Monster]] (8) · [[Feeblemind (8-E-L-FBL)|Feeblemind]] (8) · [[Gravitational Wave (8-V-L-GWV)|Gravitational Wave]] (8) · [[Power Word Stun (8-E-L-PWS)|Power Word Stun]] (8) · [[Divine Word (7-V-L-DWV)|Divine Word]] (7) · [[Dream (5-I-L-DRM)|Dream]] (5).


---

## Tactical Assessment

Mass morale collapse against formations; physically cheap, its cost lies in pattern complexity.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 9 Workings]] · [[Illusion]] · [[Spell Breakdown Procedure]] · [[Parzival]]
