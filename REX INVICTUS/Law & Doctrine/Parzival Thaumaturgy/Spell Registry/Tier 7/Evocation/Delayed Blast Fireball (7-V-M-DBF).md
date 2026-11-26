---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-7
  - spell/evocation
  - source/srd
aliases:
  - "7th Tier Spell: Delayed Blast Fireball"
  - "Delayed Blast Fireball"
  - "7-V-M-DBF"
registry_id: 7-V-M-DBF
attribute_code: "7·Evo·Fire·sphere (20)·150 feet·Up to 1 minute"
incantation: "Muire-Sonosinse"
tier: 7
school: Evocation
affinity: V
grade: M
pz_total: 39134.6
pz_quantum: 141200.1
t_e: 5.72
updated: 2026-11-16
---

**Delayed Blast Fireball** (`7-V-M-DBF`) is a 7th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **39,135 Pz** against a slot quantum of 141,200 Pz, which puts its energy-equivalent tier at T_E 5.72 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 7 Workings]]
      - [[Evocation]]
        - **Delayed Blast Fireball** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `7-V-M-DBF` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `7·Evo·Fire·sphere (20)·150 feet·Up to 1 minute` |
| Incantation | *Muire-Sonosinse* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 7th Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 150 feet |
| Area | sphere (20) |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A tiny ball of bat guano and sulfur |
| Ritual | no |
| Injury | 12d6 fire (mean 42) |
| Injury by tier | T7: 12d6, T8: 13d6, T9: 14d6 |
| Resistance check | agility; on success: half injury |
| Practitioner lineages | Sorcerer, Wizard |

### Mechanism

A bead of fire held at a chosen point gains strength each round and detonates into a 20 ft sphere of flame when released or disturbed. It can be touched and thrown before it bursts.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| base detonation 12d6=42 fire, 20 ft sphere | `42*0.70*(4*pi*(20*ft)**2/Ac)` | 19,613 |
| upkeep: charge growth +1d6 per round for 10 rounds (35 more) | `35*0.70*(4*pi*(20*ft)**2/Ac)` | 16,344 |
| Pattern cost | `0.01 × Q7 × (1 + 1.25)` | 3,177 |

| Quantity | Value |
|---|---|
| Effect energy | 19,613 Pz |
| Upkeep energy | 16,344 Pz (272 Pz/s) |
| **Total draw** | **39,135 Pz** (58,701.9 kJ) |
| Slot quantum Q7 | 141,200 Pz |
| Field gain (draw / quantum) | 0.277 |
| Energy-equivalent tier T_E | 5.72 |
| Handling points | 1.25 |
| Grade score | 0.61 → M |

**Handling flags:** concentration, fragile.

**Assumptions:** Point-source fluence model, S/Ac = 667; full 10 rounds of growth counted as upkeep.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Delayed Blast Fireball (7-V-M-DBF) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 7 | 7 | `0000000001111` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Fire | 3 | `0000000000111` |
| k4 Area | sphere (20) | 30 | `0000000111101` |
| k5 Range | 150 feet | 4 | `0000000001001` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Muire-Sonosinse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T8: *Nimuire-Sonosinse* · T9: *Xyimuire-Sonosinse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 3→2 | 4 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 | 3 |
| k4 Area | 0→9 2→11 3→12 4→0 5→1 | 5 |
| k5 Range | 0→8 3→11 | 2 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#4b9f9b`.

![[Delayed Blast Fireball (7-V-M-DBF) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 7 | 0.700 | 1.000 | `#005eff` (490 nm eq.) | source grid |
| Damage | Fire | 0.286 | 0.918 | `#9cff00` (614 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.980 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 1.000 | `#0074ff` (495 nm eq.) | source grid |
| Area | sphere (20) | 0.833 | 0.991 | `#5a00ff` (450 nm eq.) | source grid |
| Range | 150 feet | 0.235 | 0.898 | `#e3ff00` (629 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.15): swatch `#76d2b4`, measured lines at 0.236, 0.286, 0.501, 0.685, 0.701, 0.834. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.59. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `7·V·Fire`; the k4 to k6 lines (sphere (20), 150 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `7·V·Fire` |
| Standard spectrometer detection range | 19.78 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 7,060 Pz (0.05 × Q7) |
| Counter drawn cold (all six layers) | 14,120 Pz (0.10 × Q7) |
| Unravel after completion | 17,389 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Energy, Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `2b 1c 3f 2j` (2x Heat, Light, 3x Energy, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 6,522 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 7th Tier quantum of 141,200 Pz (27.7% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 7th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 7 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Linking and Triggers]], [[Area Destruction]] |
| Element | [[Fire Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Fire Storm (7-V-L-FSS)|Fire Storm]] (7) · [[Supernova (8-V-L-SPR)|Supernova]] (8) · [[Eruption (9-V-M-ERP)|Eruption]] (9) · [[Flame Strike (5-V-L-FSM)|Flame Strike]] (5) · [[Meteor Swarm (9-V-L-MST)|Meteor Swarm]] (9) · [[Thermonuclear Fireball (9-P-L-TFE)|Thermonuclear Fireball]] (9) · [[Fire Shield (4-V-L-FSR)|Fire Shield]] (4) · [[Incendiary Cloud (8-C-M-IC)|Incendiary Cloud]] (8).


---

## Tactical Assessment

A timed area charge for ambushes and denial of chokepoints; disruption of the caster sets it off early.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 7 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
