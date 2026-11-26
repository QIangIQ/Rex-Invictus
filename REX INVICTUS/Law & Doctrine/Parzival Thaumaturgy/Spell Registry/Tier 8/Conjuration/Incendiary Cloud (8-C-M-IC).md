---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-8
  - spell/conjuration
  - source/srd
aliases:
  - "8th Tier Spell: Incendiary Cloud"
  - "Incendiary Cloud"
  - "8-C-M-IC"
registry_id: 8-C-M-IC
attribute_code: "8·Con·Fire·sphere (20)·150 feet·Up to 1 minute"
incantation: "Neire-Sonosinse"
tier: 8
school: Conjuration
affinity: C
grade: M
pz_total: 93836.0
pz_quantum: 383821.6
t_e: 6.59
updated: 2026-11-16
---

**Incendiary Cloud** (`8-C-M-IC`) is a 8th Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **93,836 Pz** against a slot quantum of 383,822 Pz, which puts its energy-equivalent tier at T_E 6.59 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 8 Workings]]
      - [[Conjuration]]
        - **Incendiary Cloud** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `8-C-M-IC` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `8·Con·Fire·sphere (20)·150 feet·Up to 1 minute` |
| Incantation | *Neire-Sonosinse* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 8th Tier |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | 150 feet |
| Area | sphere (20) |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 10d8 fire (mean 45) |
| Injury by tier | T8: 10d8 |
| Resistance check | agility; on success: half injury |
| Practitioner lineages | Sorcerer, Wizard |

### Mechanism

The field fills a 20 ft radius sphere with dense smoke carrying white-hot embers and drifts it 10 ft per round away from the caster. Anyone inside or entering is burned repeatedly until wind disperses it or the field lapses.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Ember burst on appearance | `45 HP * 0.70 * (467.0 m^2 / 0.7)` | 21,010 |
| Repeat exposure, 3 rounds | `3 * 45 HP * 0.70 * (467.0 m^2 / 0.7)` | 63,040 |
| Conjured smoke mass | `1 Pz/kg * (948.9 m^3 * 1.2 kg/m^3)` | 1,139 |
| Pattern cost | `0.01 × Q8 × (1 + 1.25)` | 8,636 |

| Quantity | Value |
|---|---|
| Effect energy | 85,200 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **93,836 Pz** (140,754.0 kJ) |
| Slot quantum Q8 | 383,822 Pz |
| Field gain (draw / quantum) | 0.244 |
| Energy-equivalent tier T_E | 6.59 |
| Handling points | 1.25 |
| Grade score | 0.55 → M |

**Handling flags:** concentration, fragile.

**Assumptions:** Sphere 20 ft radius; 10d8 = 45 fire per exposure, full value; one initial burst plus 3 further exposures; smoke at air density.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Incendiary Cloud (8-C-M-IC) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 8 | 8 | `0000000010001` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | Fire | 3 | `0000000000111` |
| k4 Area | sphere (20) | 30 | `0000000111101` |
| k5 Range | 150 feet | 4 | `0000000001001` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Neire-Sonosinse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T9: *Xyineire-Sonosinse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 4→3 | 2 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 | 3 |
| k4 Area | 0→9 2→11 3→12 4→0 5→1 | 5 |
| k5 Range | 0→8 3→11 | 2 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#78778a`.

![[Incendiary Cloud (8-C-M-IC) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 8 | 0.800 | 1.000 | `#2900ff` (460 nm eq.) | source grid |
| Damage | Fire | 0.286 | 0.876 | `#9cff00` (614 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.796 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.993 | `#0074ff` (495 nm eq.) | source grid |
| Area | sphere (20) | 0.833 | 0.999 | `#5a00ff` (450 nm eq.) | source grid |
| Range | 150 feet | 0.235 | 0.853 | `#e3ff00` (629 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.19): swatch `#929a99`, measured lines at 0.126, 0.236, 0.286, 0.685, 0.801, 0.834. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.97. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `8·C·Fire`; the k4 to k6 lines (sphere (20), 150 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `8·C·Fire` |
| Standard spectrometer detection range | 30.63 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 19,191 Pz (0.05 × Q8) |
| Counter drawn cold (all six layers) | 38,382 Pz (0.10 × Q8) |
| Unravel after completion | 38,382 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Energy, Movement and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1b 1c 1e 2j` (Beyond, Heat, Light, Prodigious, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 15,639 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 8th Tier quantum of 383,822 Pz (24.4% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 8th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 8 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Area Destruction]] |
| Element | [[Fire Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Supernova (8-V-L-SPR)|Supernova]] (8) · [[Delayed Blast Fireball (7-V-M-DBF)|Delayed Blast Fireball]] (7) · [[Eruption (9-V-M-ERP)|Eruption]] (9) · [[Fire Storm (7-V-L-FSS)|Fire Storm]] (7) · [[Meteor Swarm (9-V-L-MST)|Meteor Swarm]] (9) · [[Starburst (9-A-L-STR)|Starburst]] (9) · [[Thermonuclear Fireball (9-P-L-TFE)|Thermonuclear Fireball]] (9) · [[Flame Strike (5-V-L-FSM)|Flame Strike]] (5).


---

## Tactical Assessment

An area-denial weapon for clearing trenches, buildings and dug-in positions, with the added effect of blocking sight lines. Strong wind or forced ventilation shortens its life.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 8 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
