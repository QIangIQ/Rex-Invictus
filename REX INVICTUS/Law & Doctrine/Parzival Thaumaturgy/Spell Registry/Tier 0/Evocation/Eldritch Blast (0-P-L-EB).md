---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-0
  - spell/evocation
  - source/srd
aliases:
  - "Cantrip Spell: Eldritch Blast"
  - "Eldritch Blast"
  - "0-P-L-EB"
registry_id: 0-P-L-EB
attribute_code: "0·Evo·Force·None·120 feet·Instantaneous"
incantation: "Cuton-’mul"
tier: 0
school: Evocation
affinity: P
grade: L
pz_total: 2.4
pz_quantum: 128.8
t_e: -3.99
updated: 2026-11-16
---

**Eldritch Blast** (`0-P-L-EB`) is a Cantrip (Tier 0) working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **2.4 Pz** against a slot quantum of 129 Pz, which puts its energy-equivalent tier at T_E -3.99 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 0 Workings]]
      - [[Evocation]]
        - **Eldritch Blast** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `0-P-L-EB` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `0·Evo·Force·None·120 feet·Instantaneous` |
| Incantation | *Cuton-’mul* |
| Affinity | P (Pure field construct) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | Cantrip (Tier 0) |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 120 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 1d10 force (mean 5.5) |
| Injury by caster maturity bands | T1: 1d10, T5: 1d10, T11: 1d10, T17: 1d10 |
| Delivery | aimed ranged working |
| Practitioner lineages | Warlock |

### Mechanism

A beam of crackling force strikes one target; experienced casters split it into several beams.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| 1d10 = 5.5 force, beam | `5.5*0.40*0.5` | 1.1 |
| Pattern cost | `0.01 × Q0 × (1 + 0.00)` | 1.3 |

| Quantity | Value |
|---|---|
| Effect energy | 1.1 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **2.4 Pz** (3.6 kJ) |
| Slot quantum Q0 | 129 Pz |
| Field gain (draw / quantum) | 0.0185 |
| Energy-equivalent tier T_E | -3.99 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** One beam at base strength; more beams scale linearly.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Eldritch Blast (0-P-L-EB) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 0 | 0 | `0000000000001` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Force | 4 | `0000000001001` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 120 feet | 3 | `0000000000111` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Cuton-’mul** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T1: *Sicuton-’mul* · T2: *Hicuton-’mul* · T3: *Licuton-’mul* · T4: *Vicuton-’mul* · T5: *Ticuton-’mul* · T6: *Ricuton-’mul* · T7: *Micuton-’mul* · T8: *Nicuton-’mul* · T9: *Xyicuton-’mul*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 | 1 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 3→0 | 2 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#a9892a`.

![[Eldritch Blast (0-P-L-EB) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 0 | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| Damage | Force | 0.357 | 0.938 | `#3bff00` (593 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.882 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| Range | 120 feet | 0.176 | 0.985 | `#ffc900` (647 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.16): swatch `#c8a067`, measured lines at 0.005, 0.177, 0.358, 0.501. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 0.38. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `0·V·Force`; the k4 to k6 lines (None, 120 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `0·V·Force` |
| Standard spectrometer detection range | 0.15 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 6.4 Pz (0.05 × Q0) |
| Counter drawn cold (all six layers) | 12.9 Pz (0.10 × Q0) |
| Unravel after completion | 12.9 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Beyond, Introspection, 2x Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1b 2f 1G 3j` (Beyond, Heat, 2x Energy, Introspection, 3x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 0.398 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the Cantrip (Tier 0) quantum of 129 Pz (1.9% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at Cantrip (Tier 0) up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 0 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Pure]] (P) |
| Function | [[Precision Strikes]] |
| Element | [[Force Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Magic Missile (1-P-L-MM)|Magic Missile]] (1) · [[Spiritual Weapon (2-P-L-SW)|Spiritual Weapon]] (2) · [[Stress (Battle) (0-P-L-SB)|Stress (Battle)]] (0) · [[Fire Bolt (0-V-L-FB)|Fire Bolt]] (0) · [[Radiation Poisoning (0-V-L-RP)|Radiation Poisoning]] (0) · [[Ray of Frost (0-V-L-RF)|Ray of Frost]] (0) · [[Sacred Flame (0-V-L-SF)|Sacred Flame]] (0) · [[Shocking Grasp (0-V-L-SG)|Shocking Grasp]] (0).


---

## Tactical Assessment

Reliable long-range harassment fire for a caster.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 0 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
