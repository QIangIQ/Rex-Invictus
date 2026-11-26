---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/evocation
  - source/srd
aliases:
  - "5th Tier Spell: Arcane Hand"
  - "Arcane Hand"
  - "5-P-L-AH"
registry_id: 5-P-L-AH
attribute_code: "5·Evo·None·None·120 feet·Up to 1 minute"
incantation: "Tumulse"
tier: 5
school: Evocation
affinity: P
grade: L
pz_total: 452.1
pz_quantum: 19109.4
t_e: 1.26
updated: 2026-11-16
---

**Arcane Hand** (`5-P-L-AH`) is a 5th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **452 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 1.26 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Evocation]]
        - **Arcane Hand** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-P-L-AH` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Evo·None·None·120 feet·Up to 1 minute` |
| Incantation | *Tumulse* |
| Affinity | P (Pure field construct) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 120 feet |
| Area | single point or target |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: An eggshell and a snakeskin glove |
| Ritual | no |
| Practitioner lineages | Wizard |

### Mechanism

A large hand of force is projected and driven by the caster's own hand motions to strike, shove, grapple or block.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| fist strikes | `18 HP * 0.4 Pz/HP (force) * F 0.08 * 10 target(s)/hit(s)` | 5.8 |
| structural absorption | `60 points * 0.20 Pz/point` | 12.0 |
| hover of force construct | `0.02 * 177 kg * 9.81 * 60 s / 1500` | 1.4 |
| autonomy upkeep | `0.05 Pz/s * 60 s` | 3.0 |
| Pattern cost | `0.01 × Q5 × (1 + 1.25)` | 430 |

| Quantity | Value |
|---|---|
| Effect energy | 17.8 Pz |
| Upkeep energy | 4.4 Pz (0.0732 Pz/s) |
| **Total draw** | **452 Pz** (678.2 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 0.0237 |
| Energy-equivalent tier T_E | 1.26 |
| Handling points | 1.25 |
| Grade score | 0.25 → L |

**Handling flags:** concentration, fragile.

**Assumptions:** Fist used each round for 10 rounds at 18 average injury; hand mass equivalent 177 kg from its strength rating; hand durability 60 points.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Arcane Hand (5-P-L-AH) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 120 feet | 3 | `0000000000111` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Tumulse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Ritumulse* · T7: *Mitumulse* · T8: *Nitumulse* · T9: *Xyitumulse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#3dcf86`.

![[Arcane Hand (5-P-L-AH) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| School | Evocation | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.983 | `#0074ff` (495 nm eq.) | source grid |
| Range | 120 feet | 0.176 | 0.949 | `#ffc900` (647 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.13): swatch `#86e4a9`, measured lines at 0.177, 0.501, 0.685. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.66. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·V·None`; the k4 to k6 lines (None, 120 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·V·None` |
| Standard spectrometer detection range | 2.13 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 1,912 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1b 1c 1d 1f` (Heat, Light, Life, Energy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 75.4 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 5th Tier quantum of 19,109 Pz (2.4% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 5th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 5 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Pure]] (P) |
| Function | [[Summoning and Conjured Creatures]], [[Divination and Sensing]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Arcane Singularity (3-C-L-ASA)|Arcane Singularity]] (3) · [[Animate Objects (5-T-L-AO)|Animate Objects]] (5) · [[Arcane Sword (7-P-L-ASC)|Arcane Sword]] (7) · [[Awaken (5-T-H-AWK)|Awaken]] (5) · [[Commune (5-D-L-CMMM)|Commune]] (5) · [[Commune With Nature (5-D-L-CN)|Commune With Nature]] (5) · [[Conjure Elemental (5-C-M-CEN)|Conjure Elemental]] (5) · [[Contact Other Plane (5-D-L-COP)|Contact Other Plane]] (5).


---

## Tactical Assessment

A versatile close-support manipulator for crushing light cover, restraining a target or screening the caster.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
