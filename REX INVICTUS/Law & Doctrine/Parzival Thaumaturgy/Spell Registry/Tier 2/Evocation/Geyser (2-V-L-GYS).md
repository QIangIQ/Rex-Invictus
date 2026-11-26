---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/evocation
  - source/rex-invictus
aliases:
  - "2nd Tier Spell: Geyser"
  - "Geyser"
  - "2-V-L-GYS"
registry_id: 2-V-L-GYS
attribute_code: "2·Evo·Bludgeoning·cylinder (5)·60 feet·Instantaneous"
incantation: "Hudeg-Xuwyn"
tier: 2
school: Evocation
affinity: V
grade: L
pz_total: 466.6
pz_quantum: 951.4
t_e: 1.29
updated: 2026-11-16
---

**Geyser** (`2-V-L-GYS`) is a 2nd Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Rex Invictus original working. Its modelled draw is **467 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E 1.29 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Evocation]]
        - **Geyser** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-V-L-GYS` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Evo·Bludgeoning·cylinder (5)·60 feet·Instantaneous` |
| Incantation | *Hudeg-Xuwyn* |
| Affinity | V (Evocation) |
| Source | Rex Invictus |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | cylinder (5) |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 3d6 bludgeoning (mean 10.5) |
| Injury by tier | T2: 3d6, T3: 4d6 |
| Resistance check | strength; on success: half injury |
| Practitioner lineages | Wizard, Sorcerer, Druid |

### Effect

A column of pressurized fluid erupts from a point on the ground, 5 feet in radius and 20 feet high. Creatures in it take 3d6 bludgeoning injury and are thrown off their feet unless they pass a strength check. Loose liquid in the column is flung outward and sprayed across a 20 m radius.

### Mechanism

A short evocation pulse that pressurizes a vertical column. It throws whatever liquid lies in the column upward and outward, which makes it the dispersal stage of most liquid combinations.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| column impact, 10.5 injury, cylinder r 1.5 m h 6.1 m | `10.5*0.46*(2*pi*1.524*6.096+pi*1.524^2)/0.7` | 453 |
| lifting 100 kg of local water 6 m | `100*9.81*6.096/1500` | 4.0 |
| Pattern cost | `0.01 × Q2 × (1 + 0.00)` | 9.5 |

| Quantity | Value |
|---|---|
| Effect energy | 457 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **467 Pz** (699.9 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.49 |
| Energy-equivalent tier T_E | 1.29 |
| Handling points | 0.00 |
| Grade score | -0.36 → L |

**Handling flags:** none.

**Assumptions:** Average 3d6 = 10.5; cylinder fluence surface; 100 kg of ambient water raised to the column height.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Geyser (2-V-L-GYS) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Bludgeoning | 1 | `0000000000011` |
| k4 Area | cylinder (5) | 20 | `0000000101001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Hudeg-Xuwyn** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihudeg-Xuwyn* · T4: *Vihudeg-Xuwyn* · T5: *Tihudeg-Xuwyn* · T6: *Rihudeg-Xuwyn* · T7: *Mihudeg-Xuwyn* · T8: *Nihudeg-Xuwyn* · T9: *Xyihudeg-Xuwyn*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 | 2 |
| k4 Area | 0→9 3→12 5→1 | 3 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#82be69`.

![[Geyser (2-V-L-GYS) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| Damage | Bludgeoning | 0.143 | 0.998 | `#ff9900` (657 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.956 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.980 | `#ff0028` (700 nm eq.) | source grid |
| Area | cylinder (5) | 0.556 | 0.939 | `#00ffd7` (533 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.927 | `#00fbff` (524 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 2.67. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·V·Bludgeoning`; the k4 to k6 lines (cylinder (5), 60 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·V·Bludgeoning` |
| Standard spectrometer detection range | 2.16 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 95.1 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Within, Rigidity, 2x Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1b 2f 1H 3j` (Within, Heat, 2x Energy, Rigidity, 3x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 77.8 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (49.0% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Terrain and Matter Shaping]], [[Area Destruction]] |
| Element | [[Bludgeoning Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Ice Storm (4-V-L-ISE)|Ice Storm]] (4) · [[Control Water (4-T-H-CWN)|Control Water]] (4) · [[Wind Wall (3-V-L-WWN)|Wind Wall]] (3) · [[Black Tentacles (4-C-L-BT)|Black Tentacles]] (4) · [[Bohr's Model (2-P-L-BSM)|Bohr's Model]] (2) · [[Galaxy Whirl (2-V-L-GWL)|Galaxy Whirl]] (2) · [[Moonbeam (2-V-M-MNB)|Moonbeam]] (2) · [[Shatter (2-V-L-SHT)|Shatter]] (2).


---

## Tactical Assessment

Alone it knocks down a squad in a doorway. In combinations it spreads conjured fluid over a wide area in a single second.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
