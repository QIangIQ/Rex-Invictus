---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-0
  - spell/conjuration
  - source/srd
aliases:
  - "Cantrip Spell: Mage Hand"
  - "Mage Hand"
  - "0-P-L-MH"
registry_id: 0-P-L-MH
attribute_code: "0·Con·None·None·30 feet·1 minute"
incantation: "Ceusine"
tier: 0
school: Conjuration
affinity: P
grade: L
pz_total: 3.1
pz_quantum: 128.8
t_e: -3.74
updated: 2026-11-16
---

**Mage Hand** (`0-P-L-MH`) is a Cantrip (Tier 0) working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **3.1 Pz** against a slot quantum of 129 Pz, which puts its energy-equivalent tier at T_E -3.74 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 0 Workings]]
      - [[Conjuration]]
        - **Mage Hand** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `0-P-L-MH` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `0·Con·None·None·30 feet·1 minute` |
| Incantation | *Ceusine* |
| Affinity | P (Pure field construct) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | Cantrip (Tier 0) |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | 30 feet |
| Area | single point or target |
| Duration | 1 minute |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Bard, Sorcerer, Warlock, Wizard |

### Mechanism

The field projects a manipulator able to carry up to 10 lb and perform simple handling within 30 ft of the caster for a minute.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Lifts and moves, 10 uses | `10 * 4.536 kg * 9.81 * 1.5 m / 1500` | 0.445 |
| Hover support for load (upkeep) | `0.02 * 4.536 kg * 9.81 / 1500 * 60 s` | 0.0356 |
| Pattern cost | `0.01 × Q0 × (1 + 1.00)` | 2.6 |

| Quantity | Value |
|---|---|
| Effect energy | 0.445 Pz |
| Upkeep energy | 0.0356 Pz (0.000593 Pz/s) |
| **Total draw** | **3.1 Pz** (4.6 kJ) |
| Slot quantum Q0 | 129 Pz |
| Field gain (draw / quantum) | 0.0237 |
| Energy-equivalent tier T_E | -3.74 |
| Handling points | 1.00 |
| Grade score | 0.00 → L |

**Handling flags:** fragile.

**Assumptions:** Load at the 10 lb maximum lifted 1.5 m on each of 10 uses; held aloft for the minute.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Mage Hand (0-P-L-MH) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 0 | 0 | `0000000000001` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | 1 minute | 1 | `0000000000011` |

### Incantation

Spoken as **Ceusine** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T1: *Siceusine* · T2: *Hiceusine* · T3: *Liceusine* · T4: *Viceusine* · T5: *Ticeusine* · T6: *Riceusine* · T7: *Miceusine* · T8: *Niceusine* · T9: *Xyiceusine*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 | 1 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#e4770a`.

![[Mage Hand (0-P-L-MH) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 0 | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.992 | `#ff8300` (662 nm eq.) | source grid |
| Duration | 1 minute | 0.105 | 0.994 | `#ff6300` (668 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.958 | `#91ff00` (612 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.19): swatch `#fb6133`, measured lines at 0.006, 0.106, 0.126, 0.295. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 0.49. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `0·C·None`; the k4 to k6 lines (None, 30 feet, 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `0·C·None` |
| Standard spectrometer detection range | 0.17 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 6.4 Pz (0.05 × Q0) |
| Counter drawn cold (all six layers) | 12.9 Pz (0.10 × Q0) |
| Unravel after completion | 12.9 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 0.509 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the Cantrip (Tier 0) quantum of 129 Pz (2.4% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at Cantrip (Tier 0) up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 0 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Pure]] (P) |
| Function | [[Movement and Flight]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Floating Disk (1-P-M-FD)|Floating Disk]] (1) · [[Expeditious Retreat (1-T-L-ER)|Expeditious Retreat]] (1) · [[Feather Fall (1-T-L-FFA)|Feather Fall]] (1) · [[Jump (1-T-L-JMP)|Jump]] (1) · [[Longstrider (1-T-L-LNG)|Longstrider]] (1) · [[Skyward (1-T-L-SKY)|Skyward]] (1) · [[Accelerate (2-T-L-ACC)|Accelerate]] (2) · [[Acid Splash (0-C-L-AS)|Acid Splash]] (0).


---

## Tactical Assessment

Handles suspect packages, triggers mechanisms and retrieves items from exposed positions without risking a hand. It cannot strike or carry heavy loads.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 0 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
