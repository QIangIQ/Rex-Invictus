---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/conjuration
  - source/srd
aliases:
  - "4th Tier Spell: Guardian of Faith"
  - "Guardian of Faith"
  - "4-C-L-GFA"
registry_id: 4-C-L-GFA
attribute_code: "4·Con·Radiant·cylinder (10)·30 feet·8 hours"
incantation: "Venat-Xeusiniy"
tier: 4
school: Conjuration
affinity: C
grade: L
pz_total: 1595.6
pz_quantum: 7029.9
t_e: 2.52
updated: 2026-11-16
---

**Guardian of Faith** (`4-C-L-GFA`) is a 4th Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **1,596 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E 2.52 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Conjuration]]
        - **Guardian of Faith** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-C-L-GFA` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Con·Radiant·cylinder (10)·30 feet·8 hours` |
| Incantation | *Venat-Xeusiniy* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | 30 feet |
| Area | cylinder (10) |
| Duration | 8 hours |
| Components | spoken (incantation) |
| Ritual | no |
| Injury | 20 radiant (mean 0) |
| Injury by tier | T4: 20 |
| Resistance check | agility; on success: half injury |
| Practitioner lineages | Cleric |

### Mechanism

A large spectral sentinel holds a fixed point for eight hours and strikes hostile creatures that approach within 3 m until it has dealt 60 injury.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| guardian strikes, 20 radiant x 3 | `20 HP * kappa_radiant 0.5 * F 0.5 * 1 target(s) * 3 trigger(s)` | 15.0 |
| spectral guardian presence | `0.05 Pz/s (one conjured creature) = 0.05 Pz/s * 28800 s` | 1,440 |
| Pattern cost | `0.01 × Q4 × (1 + 1.00)` | 141 |

| Quantity | Value |
|---|---|
| Effect energy | 15.0 Pz |
| Upkeep energy | 1,440 Pz (0.05 Pz/s) |
| **Total draw** | **1,596 Pz** (2,393.4 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 0.227 |
| Energy-equivalent tier T_E | 2.52 |
| Handling points | 1.00 |
| Grade score | 0.26 → L |

**Handling flags:** fragile.

**Assumptions:** Three failed-check strikes exhaust the 60-injury limit; directed delivery; guardian upkeep 0.05 Pz/s for 8 h.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Guardian of Faith (4-C-L-GFA) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 4 | 4 | `0000000001001` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | Radiant | 11 | `0000000010111` |
| k4 Area | cylinder (10) | 17 | `0000000100011` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | 8 hours | 8 | `0000000010001` |

### Incantation

Spoken as **Venat-Xeusiniy** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T5: *Tivenat-Xeusiniy* · T6: *Rivenat-Xeusiniy* · T7: *Mivenat-Xeusiniy* · T8: *Nivenat-Xeusiniy* · T9: *Xyivenat-Xeusiniy*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 3→2 | 2 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 4→1 | 4 |
| k4 Area | 0→9 1→10 5→1 | 3 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 4→11 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#46c249`.

![[Guardian of Faith (4-C-L-GFA) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| Damage | Radiant | 0.786 | 0.928 | `#1900ff` (464 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.963 | `#ff8300` (662 nm eq.) | source grid |
| Duration | 8 hours | 0.474 | 0.997 | `#00ff66` (558 nm eq.) | source grid |
| Area | cylinder (10) | 0.472 | 0.997 | `#00ff60` (558 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.994 | `#91ff00` (612 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.18): swatch `#afb987`, measured lines at 0.126, 0.295, 0.401, 0.474, 0.786. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.20. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·C·Radiant`; the k4 to k6 lines (cylinder (10), 30 feet, 8 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·C·Radiant` |
| Standard spectrometer detection range | 3.99 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 991 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Life, Hope and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1b 1c 1d 1e 1F 1i 1j` (Beyond, Heat, Light, Life, Prodigious, Potential, Hope, Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 266 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 4th Tier quantum of 7,030 Pz (22.7% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 4th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 4 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Summoning and Conjured Creatures]], [[Area Destruction]] |
| Element | [[Radiant Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Summon Demon Core (6-A-M-SDC)|Summon Demon Core]] (6) · [[Solve Olber's Paradox (4-I-L-SOSP)|Solve Olber's Paradox]] (4) · [[Black Tentacles (4-C-L-BT)|Black Tentacles]] (4) · [[Burst Radiation (6-V-L-BR)|Burst Radiation]] (6) · [[Conjure Magic Prism (4-C-L-CMPJ)|Conjure Magic Prism]] (4) · [[Conjure Minor Elementals (4-C-M-CME)|Conjure Minor Elementals]] (4) · [[Conjure Woodland Beings (4-C-L-CWB)|Conjure Woodland Beings]] (4) · [[Faithful Hound (4-C-L-FH)|Faithful Hound]] (4).


---

## Tactical Assessment

An overnight sentry at a gate or corridor that needs no rest; it can absorb a small probing attack by itself.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
