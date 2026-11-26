---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/conjuration
  - source/srd
aliases:
  - "5th Tier Spell: Cloudkill"
  - "Cloudkill"
  - "5-C-L-CLD"
registry_id: 5-C-L-CLD
attribute_code: "5·Con·Poison·sphere (20)·120 feet·Up to 10 minutes"
incantation: "Tenis-Somully"
tier: 5
school: Conjuration
affinity: C
grade: L
pz_total: 4117.1
pz_quantum: 19109.4
t_e: 3.46
updated: 2026-11-16
---

**Cloudkill** (`5-C-L-CLD`) is a 5th Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **4,117 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 3.46 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Conjuration]]
        - **Cloudkill** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-C-L-CLD` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Con·Poison·sphere (20)·120 feet·Up to 10 minutes` |
| Incantation | *Tenis-Somully* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | 120 feet |
| Area | sphere (20) |
| Duration | Up to 10 minutes (concentration) |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 5d8 poison (mean 22.5) |
| Injury by tier | T5: 5d8, T6: 6d8, T7: 7d8, T8: 8d8, T9: 9d8 |
| Resistance check | constitution; on success: half injury |
| Practitioner lineages | Sorcerer, Wizard |

### Mechanism

A dense toxic fog fills a 6 m radius sphere, rolls away from the caster and sinks into low ground.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| toxic fog | `22.5 HP * 0.05 Pz/HP (poison) * (sphere 20 ft: 4*pi*6.096^2 = 466.982 m^2 / 0.7 m^2) * 3 triggers` | 2,252 |
| conjured dense gas | `948.9 m^3 * 1.5 kg/m^3 * 1 Pz/kg` | 1,423 |
| cloud drift | `0.5*1423 kg*(0.508 m/s)^2 per 6 s * 600 s / 1500` | 12.2 |
| Pattern cost | `0.01 × Q5 × (1 + 1.25)` | 430 |

| Quantity | Value |
|---|---|
| Effect energy | 3,675 Pz |
| Upkeep energy | 12.2 Pz (0.0204 Pz/s) |
| **Total draw** | **4,117 Pz** (6,175.6 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 0.215 |
| Energy-equivalent tier T_E | 3.46 |
| Handling points | 1.25 |
| Grade score | 0.48 → L |

**Handling flags:** concentration, fragile.

**Assumptions:** 3 triggers; gas density 1.5 kg/m^3.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Cloudkill (5-C-L-CLD) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | Poison | 9 | `0000000010011` |
| k4 Area | sphere (20) | 30 | `0000000111101` |
| k5 Range | 120 feet | 3 | `0000000000111` |
| k6 Duration | Up to 10 minutes | 15 | `0000000011111` |

### Incantation

Spoken as **Tenis-Somully** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Ritenis-Somully* · T7: *Mitenis-Somully* · T8: *Nitenis-Somully* · T9: *Xyitenis-Somully*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 4→1 | 3 |
| k4 Area | 0→9 2→11 3→12 4→0 5→1 | 5 |
| k5 Range | 0→8 1→9 2→10 | 3 |
| k6 Duration | 0→7 1→8 2→9 3→10 4→11 | 5 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#668097`.

![[Cloudkill (5-C-L-CLD) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| Damage | Poison | 0.643 | 0.990 | `#00afff` (507 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.932 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Up to 10 minutes | 0.789 | 0.959 | `#1e00ff` (463 nm eq.) | source grid |
| Area | sphere (20) | 0.833 | 0.946 | `#5a00ff` (450 nm eq.) | source grid |
| Range | 120 feet | 0.176 | 0.949 | `#ffc900` (647 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.14): swatch `#94ab94`, measured lines at 0.126, 0.177, 0.501, 0.644, 0.790, 0.834. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.61. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·C·Poison`; the k4 to k6 lines (sphere (20), 120 feet, Up to 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·C·Poison` |
| Standard spectrometer detection range | 6.42 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 1,913 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Within, Cold, Death, Diminutive and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1B 1D 1F 1j` (Cold, Death, Potential, Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 686 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 5th Tier quantum of 19,109 Pz (21.5% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 5th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 5 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Area Destruction]] |
| Element | [[Poison Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Insect Plague (5-C-L-IP)|Insect Plague]] (5) · [[Supersonic Omnidirectional Jet (5-C-M-SOJ)|Supersonic Omnidirectional Jet]] (5) · [[Black Tentacles (4-C-L-BT)|Black Tentacles]] (4) · [[Guardian of Faith (4-C-L-GFA)|Guardian of Faith]] (4) · [[Wall of Thorns (6-C-L-WT)|Wall of Thorns]] (6) · [[Call Lightning (3-C-L-CLL)|Call Lightning]] (3) · [[Cone of Cold (5-V-L-CC)|Cone of Cold]] (5) · [[Flame Strike (5-V-L-FSM)|Flame Strike]] (5).


---

## Tactical Assessment

Area denial and bunker clearing; harms even sealed breathing.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
