---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/conjuration
  - source/srd
aliases:
  - "4th Tier Spell: Faithful Hound"
  - "Faithful Hound"
  - "4-C-L-FH"
registry_id: 4-C-L-FH
attribute_code: "4·Con·Piercing·None·30 feet·8 hours"
incantation: "Veix-’usiniy"
tier: 4
school: Conjuration
affinity: C
grade: L
pz_total: 1608.4
pz_quantum: 7029.9
t_e: 2.53
updated: 2026-11-16
---

**Faithful Hound** (`4-C-L-FH`) is a 4th Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **1,608 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E 2.53 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Conjuration]]
        - **Faithful Hound** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-C-L-FH` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Con·Piercing·None·30 feet·8 hours` |
| Incantation | *Veix-’usiniy* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | 30 feet |
| Area | single point or target |
| Duration | 8 hours |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A tiny silver whistle, a piece of bone, and a thread |
| Ritual | no |
| Injury | 4d8 piercing (mean 18) |
| Injury by tier | T4: 4d8 |
| Delivery | aimed melee working |
| Practitioner lineages | Wizard |

### Mechanism

An invisible watchdog stands guard, barks at intruders who lack the password, sees invisible creatures and bites hostile visitors nearby.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| phantom hound bites: 3 x 4d8 = 18 piercing | `3*18*0.35*0.08` | 1.5 |
| upkeep: phantom autonomy for 8 h | `0.05*1*8*3600` | 1,440 |
| upkeep: perimeter sensing 30 ft for 8 h | `0.001*(30*ft/10)*8*3600` | 26.3 |
| Pattern cost | `0.01 × Q4 × (1 + 1.00)` | 141 |

| Quantity | Value |
|---|---|
| Effect energy | 1.5 Pz |
| Upkeep energy | 1,466 Pz (0.0509 Pz/s) |
| **Total draw** | **1,608 Pz** (2,412.7 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 0.229 |
| Energy-equivalent tier T_E | 2.53 |
| Handling points | 1.00 |
| Grade score | 0.26 → L |

**Handling flags:** fragile.

**Assumptions:** Massless phantom; 3 bites expected; autonomy rate 0.05 Pz/s.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Faithful Hound (4-C-L-FH) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 4 | 4 | `0000000001001` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | Piercing | 8 | `0000000010001` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | 8 hours | 8 | `0000000010001` |

### Incantation

Spoken as **Veix-’usiniy** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T5: *Tiveix-’usiniy* · T6: *Riveix-’usiniy* · T7: *Miveix-’usiniy* · T8: *Niveix-’usiniy* · T9: *Xyiveix-’usiniy*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 3→2 | 2 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 4→1 | 2 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 4→11 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#4ee643`.

![[Faithful Hound (4-C-L-FH) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| Damage | Piercing | 0.571 | 0.985 | `#00ffec` (529 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.963 | `#ff8300` (662 nm eq.) | source grid |
| Duration | 8 hours | 0.474 | 0.997 | `#00ff66` (558 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.994 | `#91ff00` (612 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.16): swatch `#bdc47e`, measured lines at 0.126, 0.295, 0.401, 0.474, 0.572. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.21. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·C·Piercing`; the k4 to k6 lines (None, 30 feet, 8 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·C·Piercing` |
| Standard spectrometer detection range | 4.01 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 996 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Beyond, Cold, Hopelessness, Movement and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `2a 1B 1e 1F 1I 2j` (2x Beyond, Cold, Prodigious, Potential, Hopelessness, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 268 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 4th Tier quantum of 7,030 Pz (22.9% of it). |
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
| Function | [[Summoning and Conjured Creatures]], [[Precision Strikes]] |
| Element | [[Piercing Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Conjure Magic Prism (4-C-L-CMPJ)|Conjure Magic Prism]] (4) · [[Conjure Minor Elementals (4-C-M-CME)|Conjure Minor Elementals]] (4) · [[Conjure Woodland Beings (4-C-L-CWB)|Conjure Woodland Beings]] (4) · [[Dimension Door (4-P-L-DD)|Dimension Door]] (4) · [[Guardian of Faith (4-C-L-GFA)|Guardian of Faith]] (4) · [[Magic Polarising Filter (4-C-L-MPF)|Magic Polarising Filter]] (4) · [[Spiritual Weapon (2-P-L-SW)|Spiritual Weapon]] (2) · [[Arcane Singularity (3-C-L-ASA)|Arcane Singularity]] (3).


---

## Tactical Assessment

A guard post that sees invisible and phased intruders.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
