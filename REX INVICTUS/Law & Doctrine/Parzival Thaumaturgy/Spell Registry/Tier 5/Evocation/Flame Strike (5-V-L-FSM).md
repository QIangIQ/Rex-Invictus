---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/evocation
  - source/srd
aliases:
  - "5th Tier Spell: Flame Strike"
  - "Flame Strike"
  - "5-V-L-FSM"
registry_id: 5-V-L-FSM
attribute_code: "5·Evo·Fire·cylinder (40)·60 feet·Instantaneous"
incantation: "Tuire-Xowyn"
tier: 5
school: Evocation
affinity: V
grade: L
pz_total: 6495.3
pz_quantum: 19109.4
t_e: 3.92
updated: 2026-11-16
---

**Flame Strike** (`5-V-L-FSM`) is a 5th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **6,495 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 3.92 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Evocation]]
        - **Flame Strike** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-V-L-FSM` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Evo·Fire·cylinder (40)·60 feet·Instantaneous` |
| Incantation | *Tuire-Xowyn* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | cylinder (40) |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Pinch of sulfur |
| Ritual | no |
| Injury | 4d6 fire (mean 14) |
| Injury by tier | T5: 4d6, T6: 4d6 OR 5d6, T7: 4d6 OR 6d6, T8: 4d6 OR 7d6, T9: 4d6 OR 8d6 |
| Resistance check | agility; on success: half injury |
| Practitioner lineages | Cleric |

### Mechanism

A vertical column of flame and radiant energy descends over a 3 m radius footprint, heating and searing everything in the column.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| fire column, 4d6=14 | `14 HP * kappa_fire 0.7 * S/A_c (1 x 2*pi*r*h+pi*r^2 (r=10 ft, h=40 ft) = 262.7 m^2 / 0.7)` | 3,677 |
| radiant column, 4d6=14 | `14 HP * kappa_radiant 0.5 * S/A_c (1 x 2*pi*r*h+pi*r^2 (r=10 ft, h=40 ft) = 262.7 m^2 / 0.7)` | 2,627 |
| Pattern cost | `0.01 × Q5 × (1 + 0.00)` | 191 |

| Quantity | Value |
|---|---|
| Effect energy | 6,304 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **6,495 Pz** (9,743.0 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 0.34 |
| Energy-equivalent tier T_E | 3.92 |
| Handling points | 0.00 |
| Grade score | -0.54 → L |

**Handling flags:** none.

**Assumptions:** 4d6 fire and 4d6 radiant averages; cylinder r 10 ft, h 40 ft.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Flame Strike (5-V-L-FSM) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Fire | 3 | `0000000000111` |
| k4 Area | cylinder (40) | 19 | `0000000100111` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Tuire-Xowyn** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Rituire-Xowyn* · T7: *Mituire-Xowyn* · T8: *Nituire-Xowyn* · T9: *Xyituire-Xowyn*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 | 3 |
| k4 Area | 0→9 1→10 2→11 5→1 | 4 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#40d77f`.

![[Flame Strike (5-V-L-FSM) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| Damage | Fire | 0.286 | 0.977 | `#9cff00` (614 nm eq.) | source grid |
| School | Evocation | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.882 | `#ff0028` (700 nm eq.) | source grid |
| Area | cylinder (40) | 0.528 | 1.000 | `#00ffb1` (542 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.996 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.17): swatch `#93e3a0`, measured lines at 0.004, 0.286, 0.501, 0.529, 0.589. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.81. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·V·Fire`; the k4 to k6 lines (cylinder (40), 60 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·V·Fire` |
| Standard spectrometer detection range | 8.06 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 1,911 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Energy, Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `2b 1c 3f 2j` (2x Heat, Light, 3x Energy, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1,083 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 5th Tier quantum of 19,109 Pz (34.0% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 5th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 5 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Area Destruction]] |
| Element | [[Fire Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Fire Shield (4-V-L-FSR)|Fire Shield]] (4) · [[Wall of Fire (4-V-M-WF)|Wall of Fire]] (4) · [[Delayed Blast Fireball (7-V-M-DBF)|Delayed Blast Fireball]] (7) · [[Fire Storm (7-V-L-FSS)|Fire Storm]] (7) · [[Fireball (3-V-M-FRB)|Fireball]] (3) · [[Outflows (5-A-L-OTF)|Outflows]] (5) · [[Galaxy Whirl (2-V-L-GWL)|Galaxy Whirl]] (2) · [[Supernova (8-V-L-SPR)|Supernova]] (8).


---

## Tactical Assessment

A precise vertical strike that can be dropped onto a single fire team, a gun emplacement or a hatch without spilling onto nearby friendly troops.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
