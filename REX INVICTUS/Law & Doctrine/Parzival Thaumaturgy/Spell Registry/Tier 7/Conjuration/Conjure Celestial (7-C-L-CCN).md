---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-7
  - spell/conjuration
  - source/srd
aliases:
  - "7th Tier Spell: Conjure Celestial"
  - "Conjure Celestial"
  - "7-C-L-CCN"
registry_id: 7-C-L-CCN
attribute_code: "7·Con·None·None·90 feet·Up to 1 hour"
incantation: "Meylarsi"
tier: 7
school: Conjuration
affinity: C
grade: L
pz_total: 3298.0
pz_quantum: 141200.1
t_e: 3.24
updated: 2026-11-16
---

**Conjure Celestial** (`7-C-L-CCN`) is a 7th Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **3,298 Pz** against a slot quantum of 141,200 Pz, which puts its energy-equivalent tier at T_E 3.24 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 7 Workings]]
      - [[Conjuration]]
        - **Conjure Celestial** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `7-C-L-CCN` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `7·Con·None·None·90 feet·Up to 1 hour` |
| Incantation | *Meylarsi* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 7th Tier |
| School | [[Conjuration]] |
| Casting time | 1 minute |
| Range | 90 feet |
| Area | single point or target |
| Duration | Up to 1 hour (concentration) |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Cleric |

### Mechanism

A celestial entity is called and follows the caster's commands for an hour.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| conjured body | `100 kg * 10 Pz/kg` | 1,000 |
| autonomy upkeep | `0.05 Pz/s * 3600 s` | 180 |
| Pattern cost | `0.01 × Q7 × (1 + 0.50)` | 2,118 |

| Quantity | Value |
|---|---|
| Effect energy | 1,000 Pz |
| Upkeep energy | 180 Pz (0.05 Pz/s) |
| **Total draw** | **3,298 Pz** (4,947.0 kJ) |
| Slot quantum Q7 | 141,200 Pz |
| Field gain (draw / quantum) | 0.0234 |
| Energy-equivalent tier T_E | 3.24 |
| Handling points | 0.50 |
| Grade score | -0.50 → L |

**Handling flags:** concentration, long cast.

**Assumptions:** 100 kg body; 1 h.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Conjure Celestial (7-C-L-CCN) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 7 | 7 | `0000000001111` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 90 feet | 11 | `0000000010111` |
| k6 Duration | Up to 1 hour | 12 | `0000000011001` |

### Incantation

Spoken as **Meylarsi** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T8: *Nimeylarsi* · T9: *Xyimeylarsi*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 3→2 | 4 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 4→12 | 4 |
| k6 Duration | 0→7 3→10 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#3893c6`.

![[Conjure Celestial (7-C-L-CCN) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 7 | 0.700 | 1.000 | `#005eff` (490 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.848 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Up to 1 hour | 0.632 | 0.998 | `#00c0ff` (511 nm eq.) | source grid |
| Range | 90 feet | 0.647 | 0.999 | `#00aaff` (506 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.14): swatch `#6fb3a5`, measured lines at 0.126, 0.632, 0.648, 0.701. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.52. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `7·C·None`; the k4 to k6 lines (None, 90 feet, Up to 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `7·C·None` |
| Standard spectrometer detection range | 5.74 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 7,060 Pz (0.05 × Q7) |
| Counter drawn cold (all six layers) | 14,120 Pz (0.10 × Q7) |
| Unravel after completion | 14,156 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 550 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 7th Tier quantum of 141,200 Pz (2.3% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 7th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 7 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Summoning and Conjured Creatures]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Conjure Fey (6-C-L-CFN)|Conjure Fey]] (6) · [[Instant Summons (6-C-L-ISS)|Instant Summons]] (6) · [[Planar Ally (6-C-L-PA)|Planar Ally]] (6) · [[Arcane Sword (7-P-L-ASC)|Arcane Sword]] (7) · [[Conjure Elemental (5-C-M-CEN)|Conjure Elemental]] (5) · [[Simulacrum (7-I-M-SML)|Simulacrum]] (7) · [[Clone (8-N-L-CLN)|Clone]] (8) · [[Conjure Magic Prism (4-C-L-CMPJ)|Conjure Magic Prism]] (4).


---

## Tactical Assessment

A powerful ally for an hour.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 7 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
