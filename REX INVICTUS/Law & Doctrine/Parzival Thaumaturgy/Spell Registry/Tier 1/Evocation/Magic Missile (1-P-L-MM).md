---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/evocation
  - source/srd
aliases:
  - "1st Tier Spell: Magic Missile"
  - "Magic Missile"
  - "1-P-L-MM"
registry_id: 1-P-L-MM
attribute_code: "1·Evo·Force·None·120 feet·Instantaneous"
incantation: "Suton-’mul"
tier: 1
school: Evocation
affinity: P
grade: L
pz_total: 5.6
pz_quantum: 350.0
t_e: -3.14
updated: 2026-11-16
---

**Magic Missile** (`1-P-L-MM`) is a 1st Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **5.6 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -3.14 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Evocation]]
        - **Magic Missile** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-P-L-MM` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Evo·Force·None·120 feet·Instantaneous` |
| Incantation | *Suton-’mul* |
| Affinity | P (Pure field construct) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 120 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 3d4 + 3 force (mean 10.5) |
| Injury by tier | T1: 3d4 + 3, T2: 4d4 + 4, T3: 5d4 + 5, T4: 6d4 + 6, T5: 7d4 + 7, T6: 8d4 + 8, T7: 9d4 + 9, T8: 10d4 + 10, T9: 11d4 + 11 |
| Practitioner lineages | Sorcerer, Wizard |

### Mechanism

The field launches three force darts that fly straight from the caster's hand and burst on impact. They suffer no drop and no wind drift, but in Rex Invictus they do not track: the source's never-miss behaviour is not canon. Tracking needs a separate guidance working bound to the dart ([[Practical Magical Combat#Exploiting basic workings]]).

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Three force darts | `3 * 3.5 HP * 0.40 * 0.5 (bolt)` | 2.1 |
| Pattern cost | `0.01 × Q1 × (1 + 0.00)` | 3.5 |

| Quantity | Value |
|---|---|
| Effect energy | 2.1 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **5.6 Pz** (8.4 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.016 |
| Energy-equivalent tier T_E | -3.14 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Each dart 1d4 + 1 = 3.5; three darts.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Magic Missile (1-P-L-MM) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Force | 4 | `0000000001001` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 120 feet | 3 | `0000000000111` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Suton-’mul** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisuton-’mul* · T3: *Lisuton-’mul* · T4: *Visuton-’mul* · T5: *Tisuton-’mul* · T6: *Risuton-’mul* · T7: *Misuton-’mul* · T8: *Nisuton-’mul* · T9: *Xyisuton-’mul*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 3→0 | 2 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#a79e22`.

![[Magic Missile (1-P-L-MM) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| Damage | Force | 0.357 | 0.967 | `#3bff00` (593 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.923 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.995 | `#ff0028` (700 nm eq.) | source grid |
| Range | 120 feet | 0.176 | 0.997 | `#ffc900` (647 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.20): swatch `#cea366`, measured lines at 0.004, 0.101, 0.177, 0.358, 0.501. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 0.75. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·V·Force`; the k4 to k6 lines (None, 120 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·V·Force` |
| Standard spectrometer detection range | 0.24 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.0 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Beyond, Introspection, 2x Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1b 2f 1G 3j` (Beyond, Heat, 2x Energy, Introspection, 3x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 0.933 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (1.6% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Pure]] (P) |
| Function | [[Precision Strikes]] |
| Element | [[Force Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Eldritch Blast (0-P-L-EB)|Eldritch Blast]] (0) · [[Spiritual Weapon (2-P-L-SW)|Spiritual Weapon]] (2) · [[Stress (Battle) (0-P-L-SB)|Stress (Battle)]] (0) · [[Divine Favor (1-V-L-DF)|Divine Favor]] (1) · [[Electrify (1-V-L-ELC)|Electrify]] (1) · [[Focusing Lens (1-V-L-FLC)|Focusing Lens]] (1) · [[Guiding Bolt (1-V-L-GB)|Guiding Bolt]] (1) · [[Hellish Rebuke (1-V-L-HR)|Hellish Rebuke]] (1).


---

## Tactical Assessment

A cheap, flat-shooting dart for drones, lightly protected targets and fuzed payloads (the carrier of the [[Skymark Flare (MM-LK-AL-LT-SK)|Skymark Flare]] and the [[Anti-Mage Primer (SP-TI-MM-DM-SH-AC-BL-AL)|Anti-Mage Primer]]). It is weak in high-tier combat: under ULMTU-XII a caster of far greater knowledge or power can undo or alter it outright, and a pre-loaded counter costs almost nothing.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
