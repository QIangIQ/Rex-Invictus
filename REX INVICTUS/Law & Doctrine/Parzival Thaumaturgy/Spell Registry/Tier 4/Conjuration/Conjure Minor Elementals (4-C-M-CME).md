---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/conjuration
  - source/srd
aliases:
  - "4th Tier Spell: Conjure Minor Elementals"
  - "Conjure Minor Elementals"
  - "4-C-M-CME"
registry_id: 4-C-M-CME
attribute_code: "4·Con·None·None·90 feet·Up to 1 hour"
incantation: "Veylarsi"
tier: 4
school: Conjuration
affinity: C
grade: M
pz_total: 2780.6
pz_quantum: 7029.9
t_e: 3.07
updated: 2026-11-16
---

**Conjure Minor Elementals** (`4-C-M-CME`) is a 4th Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **2,781 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E 3.07 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Conjuration]]
        - **Conjure Minor Elementals** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-C-M-CME` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Con·None·None·90 feet·Up to 1 hour` |
| Incantation | *Veylarsi* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Conjuration]] |
| Casting time | 1 minute |
| Range | 90 feet |
| Area | single point or target |
| Duration | Up to 1 hour (concentration) |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Druid, Wizard |

### Mechanism

The field assembles several small elemental bodies, from one larger body up to eight minor ones, and binds them to a shared command channel. They hold position and defend themselves when no orders arrive.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| 8 small elemental bodies | `10*8*15` | 1,200 |
| upkeep: autonomy of 8 creatures for 1 h | `0.05*8*3600` | 1,440 |
| Pattern cost | `0.01 × Q4 × (1 + 1.00)` | 141 |

| Quantity | Value |
|---|---|
| Effect energy | 1,200 Pz |
| Upkeep energy | 1,440 Pz (0.4 Pz/s) |
| **Total draw** | **2,781 Pz** (4,170.9 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 0.396 |
| Energy-equivalent tier T_E | 3.07 |
| Handling points | 1.00 |
| Grade score | 0.54 → M |

**Handling flags:** concentration, multi target control, long cast.

**Assumptions:** Eight-body option chosen as the most demanding: 15 kg each; one 200 kg body would cost 2000 + 180 Pz instead.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Conjure Minor Elementals (4-C-M-CME) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 4 | 4 | `0000000001001` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 90 feet | 11 | `0000000010111` |
| k6 Duration | Up to 1 hour | 12 | `0000000011001` |

### Incantation

Spoken as **Veylarsi** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T5: *Tiveylarsi* · T6: *Riveylarsi* · T7: *Miveylarsi* · T8: *Niveylarsi* · T9: *Xyiveylarsi*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 3→2 | 2 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 4→12 | 4 |
| k6 Duration | 0→7 3→10 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#3ebb7e`.

![[Conjure Minor Elementals (4-C-M-CME) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.963 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Up to 1 hour | 0.632 | 0.974 | `#00c0ff` (511 nm eq.) | source grid |
| Range | 90 feet | 0.647 | 0.970 | `#00aaff` (506 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.15): swatch `#a5ba87`, measured lines at 0.126, 0.401, 0.632, 0.647. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.44. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·C·None`; the k4 to k6 lines (None, 90 feet, Up to 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·C·None` |
| Standard spectrometer detection range | 5.27 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 991 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 463 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 4th Tier quantum of 7,030 Pz (39.6% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
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
| Affinity | [[Conjuration]] (C) |
| Function | [[Summoning and Conjured Creatures]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Conjure Magic Prism (4-C-L-CMPJ)|Conjure Magic Prism]] (4) · [[Conjure Woodland Beings (4-C-L-CWB)|Conjure Woodland Beings]] (4) · [[Faithful Hound (4-C-L-FH)|Faithful Hound]] (4) · [[Guardian of Faith (4-C-L-GFA)|Guardian of Faith]] (4) · [[Magic Polarising Filter (4-C-L-MPF)|Magic Polarising Filter]] (4) · [[Arcane Singularity (3-C-L-ASA)|Arcane Singularity]] (3) · [[Conjure Animals (3-C-M-CA)|Conjure Animals]] (3) · [[Conjure Elemental (5-C-M-CEN)|Conjure Elemental]] (5).


---

## Tactical Assessment

Eight minor bodies saturate a small area, screen a squad or trigger enemy sensors and traps at low cost per unit.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
