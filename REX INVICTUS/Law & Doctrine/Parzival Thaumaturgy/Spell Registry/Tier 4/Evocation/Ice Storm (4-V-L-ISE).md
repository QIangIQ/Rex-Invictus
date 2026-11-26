---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/evocation
  - source/srd
aliases:
  - "4th Tier Spell: Ice Storm"
  - "Ice Storm"
  - "4-V-L-ISE"
registry_id: 4-V-L-ISE
attribute_code: "4·Evo·Bludgeoning·cylinder (20)·300 feet·Instantaneous"
incantation: "Vudeg-Xésphin"
tier: 4
school: Evocation
affinity: V
grade: L
pz_total: 15640.3
pz_quantum: 7029.9
t_e: 4.80
updated: 2026-11-16
---

**Ice Storm** (`4-V-L-ISE`) is a 4th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **15,640 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E 4.80 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Evocation]]
        - **Ice Storm** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-V-L-ISE` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Evo·Bludgeoning·cylinder (20)·300 feet·Instantaneous` |
| Incantation | *Vudeg-Xésphin* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 300 feet |
| Area | cylinder (20) |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A pinch of dust and a few drops of water |
| Ritual | no |
| Injury | 2d8 bludgeoning (mean 9) |
| Injury by tier | T4: 2d8, T5: 3d8, T6: 4d8, T7: 5d8, T8: 6d8, T9: 7d8 |
| Resistance check | agility; on success: half injury |
| Practitioner lineages | Druid, Sorcerer, Wizard |

### Mechanism

The field condenses and drives dense ice pellets down through a 20 ft radius, 40 ft high column, combining impact and deep chilling. The settled hail remains as a slick layer for a short time.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Hail impact (bludgeoning) | `9 HP * 0.46 * (583.7 m^2 / 0.7)` | 3,452 |
| Cold injury | `14 HP * 0.90 * (583.7 m^2 / 0.7)` | 10,510 |
| Hailstone ground cover (conjured ice) | `3 Pz/kg * (pi*6.096^2 m^2 * 0.01 m * 917 kg/m^3 * 0.5 packing = 535 kg)` | 1,606 |
| Pattern cost | `0.01 × Q4 × (1 + 0.00)` | 70.3 |

| Quantity | Value |
|---|---|
| Effect energy | 15,570 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **15,640 Pz** (23,460.4 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 2.22 |
| Energy-equivalent tier T_E | 4.80 |
| Handling points | 0.00 |
| Grade score | 0.40 → L |

**Handling flags:** none.

**Assumptions:** Cylinder 20 ft radius, 40 ft height; injury averages 2d8 = 9 impact and 4d6 = 14 cold, full value; hail layer 1 cm over the base at half packing density.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Ice Storm (4-V-L-ISE) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 4 | 4 | `0000000001001` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Bludgeoning | 1 | `0000000000011` |
| k4 Area | cylinder (20) | 18 | `0000000100101` |
| k5 Range | 300 feet | 6 | `0000000001101` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Vudeg-Xésphin** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T5: *Tivudeg-Xésphin* · T6: *Rivudeg-Xésphin* · T7: *Mivudeg-Xésphin* · T8: *Nivudeg-Xésphin* · T9: *Xyivudeg-Xésphin*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 3→2 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 | 2 |
| k4 Area | 0→9 2→11 5→1 | 3 |
| k5 Range | 0→8 2→10 3→11 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#5cc635`.

![[Ice Storm (4-V-L-ISE) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| Damage | Bludgeoning | 0.143 | 0.967 | `#ff9900` (657 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.995 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.923 | `#ff0028` (700 nm eq.) | source grid |
| Area | cylinder (20) | 0.500 | 0.995 | `#00ff8b` (550 nm eq.) | source grid |
| Range | 300 feet | 0.353 | 0.999 | `#40ff00` (594 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.19): swatch `#b5ce85`, measured lines at 0.004, 0.143, 0.354, 0.401, 0.501. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.19. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·V·Bludgeoning`; the k4 to k6 lines (cylinder (20), 300 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·V·Bludgeoning` |
| Standard spectrometer detection range | 12.51 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 703 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Within, Rigidity, 2x Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1b 2f 1H 3j` (Within, Heat, 2x Energy, Rigidity, 3x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 2,607 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 2.22 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 4th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 4th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 4 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Terrain and Matter Shaping]], [[Area Destruction]] |
| Element | [[Bludgeoning Workings]], [[Cold and Ice Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Control Water (4-T-H-CWN)|Control Water]] (4) · [[Geyser (2-V-L-GYS)|Geyser]] (2) · [[Cone of Cold (5-V-L-CC)|Cone of Cold]] (5) · [[Wind Wall (3-V-L-WWN)|Wind Wall]] (3) · [[Absolute Zero (6-V-L-AZ)|Absolute Zero]] (6) · [[Black Tentacles (4-C-L-BT)|Black Tentacles]] (4) · [[Freezing Sphere (6-V-M-FSZ)|Freezing Sphere]] (6) · [[Wall of Ice (6-V-M-WI)|Wall of Ice]] (6).


---

## Tactical Assessment

A fire-support option against troops in the open or under light cover, with a lingering mobility penalty on the impact zone. Overhead protection and vehicle hulls reduce its effect considerably.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
