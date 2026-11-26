---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/evocation
  - source/srd
aliases:
  - "3rd Tier Spell: Wind Wall"
  - "Wind Wall"
  - "3-V-L-WWN"
registry_id: 3-V-L-WWN
attribute_code: "3·Evo·Bludgeoning·line (50)·120 feet·Up to 1 minute"
incantation: "Ludeg-Lumulse"
tier: 3
school: Evocation
affinity: V
grade: L
pz_total: 3010.3
pz_quantum: 2586.2
t_e: 3.15
updated: 2026-11-16
---

**Wind Wall** (`3-V-L-WWN`) is a 3rd Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **3,010 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E 3.15 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Evocation]]
        - **Wind Wall** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-V-L-WWN` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Evo·Bludgeoning·line (50)·120 feet·Up to 1 minute` |
| Incantation | *Ludeg-Lumulse* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 120 feet |
| Area | line (50) |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A tiny fan and a feather of exotic origin |
| Ritual | no |
| Injury | 3d8 bludgeoning (mean 13.5) |
| Injury by tier | T3: 3d8 |
| Resistance check | strength; on success: half injury |
| Practitioner lineages | Druid, Ranger |

### Mechanism

A 15 m long, 4.6 m high curtain of rising wind strikes those it forms on and deflects light projectiles, gases and small fliers upward.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Initial gust injury | `13.5 * 0.46 * 139 / 0.7` | 1,236 |
| Upkeep: Upward jet, 25 m/s | `0.5 * 1.2 * 4.65 m^2 * 25^3 * 60 s / 1500` | 1,742 |
| Pattern cost | `0.01 × Q3 × (1 + 0.25)` | 32.3 |

| Quantity | Value |
|---|---|
| Effect energy | 1,236 Pz |
| Upkeep energy | 1,742 Pz (29.0 Pz/s) |
| **Total draw** | **3,010 Pz** (4,515.5 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 1.16 |
| Energy-equivalent tier T_E | 3.15 |
| Handling points | 0.25 |
| Grade score | 0.33 → L |

**Handling flags:** concentration.

**Assumptions:** 3d8 = 13.5; jet speed 25 m/s through the 1 ft thick wall section.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Wind Wall (3-V-L-WWN) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Bludgeoning | 1 | `0000000000011` |
| k4 Area | line (50) | 24 | `0000000110001` |
| k5 Range | 120 feet | 3 | `0000000000111` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Ludeg-Lumulse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Viludeg-Lumulse* · T5: *Tiludeg-Lumulse* · T6: *Riludeg-Lumulse* · T7: *Miludeg-Lumulse* · T8: *Niludeg-Lumulse* · T9: *Xyiludeg-Lumulse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 | 2 |
| k4 Area | 0→9 4→0 5→1 | 3 |
| k5 Range | 0→8 1→9 2→10 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#6ebc68`.

![[Wind Wall (3-V-L-WWN) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| Damage | Bludgeoning | 0.143 | 0.988 | `#ff9900` (657 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.980 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.929 | `#0074ff` (495 nm eq.) | source grid |
| Area | line (50) | 0.667 | 0.935 | `#008fff` (500 nm eq.) | source grid |
| Range | 120 feet | 0.176 | 0.992 | `#ffc900` (647 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 3.48. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·V·Bludgeoning`; the k4 to k6 lines (line (50), 120 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·V·Bludgeoning` |
| Standard spectrometer detection range | 5.49 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 607 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Within, Rigidity, 2x Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1b 2f 1H 3j` (Within, Heat, 2x Energy, Rigidity, 3x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 502 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 1.16 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 3rd Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Walls and Barriers]], [[Area Destruction]] |
| Element | [[Bludgeoning Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Geyser (2-V-L-GYS)|Geyser]] (2) · [[Ice Storm (4-V-L-ISE)|Ice Storm]] (4) · [[Wall of Fire (4-V-M-WF)|Wall of Fire]] (4) · [[Black Tentacles (4-C-L-BT)|Black Tentacles]] (4) · [[Blade Barrier (6-V-L-BB)|Blade Barrier]] (6) · [[Control Water (4-T-H-CWN)|Control Water]] (4) · [[Wall of Ice (6-V-M-WI)|Wall of Ice]] (6) · [[Fireball (3-V-M-FRB)|Fireball]] (3).


---

## Tactical Assessment

Shields a position from arrows, small drones and gas; heavy projectiles and gunfire at high velocity pass through.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
