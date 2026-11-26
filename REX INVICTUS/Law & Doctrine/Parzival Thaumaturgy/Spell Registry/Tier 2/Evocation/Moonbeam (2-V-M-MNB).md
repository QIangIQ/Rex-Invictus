---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/evocation
  - source/srd
aliases:
  - "2nd Tier Spell: Moonbeam"
  - "Moonbeam"
  - "2-V-M-MNB"
registry_id: 2-V-M-MNB
attribute_code: "2·Evo·Radiant·cylinder (5)·120 feet·Up to 1 minute"
incantation: "Hunat-Xumulse"
tier: 2
school: Evocation
affinity: V
grade: M
pz_total: 2936.3
pz_quantum: 951.4
t_e: 3.13
updated: 2026-11-16
---

**Moonbeam** (`2-V-M-MNB`) is a 2nd Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **2,936 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E 3.13 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Evocation]]
        - **Moonbeam** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-V-M-MNB` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Evo·Radiant·cylinder (5)·120 feet·Up to 1 minute` |
| Incantation | *Hunat-Xumulse* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 120 feet |
| Area | cylinder (5) |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Several seeds of any moonseed plant and a piece of opalescent feldspar |
| Ritual | no |
| Injury | 2d10 radiant (mean 11) |
| Injury by tier | T2: 2d10, T3: 3d10, T4: 4d10, T5: 5d10, T6: 6d10, T7: 7d10, T8: 8d10, T9: 9d10 |
| Resistance check | constitution; on success: half injury |
| Practitioner lineages | Druid |

### Mechanism

The field drops a pale column of light 5 ft in radius and 40 ft high that burns creatures entering or staying in it, and can be moved 60 ft each round. Shapechangers caught in it are forced back to their true form.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Radiant burn, 3 exposures | `3 * 11 HP * 0.50 * (124.0 m^2 / 0.7)` | 2,924 |
| Dim light in column (upkeep) | `10 W / 1500 * 60 s` | 0.4 |
| Pattern cost | `0.01 × Q2 × (1 + 0.25)` | 11.9 |

| Quantity | Value |
|---|---|
| Effect energy | 2,924 Pz |
| Upkeep energy | 0.4 Pz (0.00667 Pz/s) |
| **Total draw** | **2,936 Pz** (4,404.4 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 3.09 |
| Energy-equivalent tier T_E | 3.13 |
| Handling points | 0.25 |
| Grade score | 0.81 → M |

**Handling flags:** concentration.

**Assumptions:** Cylinder 5 ft radius, 40 ft high; 2d10 = 11 per exposure, full value; 3 exposures; 10 W of dim light.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Moonbeam (2-V-M-MNB) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Radiant | 11 | `0000000010111` |
| k4 Area | cylinder (5) | 20 | `0000000101001` |
| k5 Range | 120 feet | 3 | `0000000000111` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Hunat-Xumulse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihunat-Xumulse* · T4: *Vihunat-Xumulse* · T5: *Tihunat-Xumulse* · T6: *Rihunat-Xumulse* · T7: *Mihunat-Xumulse* · T8: *Nihunat-Xumulse* · T9: *Xyihunat-Xumulse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 4→1 | 4 |
| k4 Area | 0→9 3→12 5→1 | 3 |
| k5 Range | 0→8 1→9 2→10 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#5eb589`.

![[Moonbeam (2-V-M-MNB) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| Damage | Radiant | 0.786 | 0.842 | `#1900ff` (464 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.956 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.889 | `#0074ff` (495 nm eq.) | source grid |
| Area | cylinder (5) | 0.556 | 0.939 | `#00ffd7` (533 nm eq.) | source grid |
| Range | 120 feet | 0.176 | 1.000 | `#ffc900` (647 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.20): swatch `#94c19b`, measured lines at 0.177, 0.201, 0.501, 0.556, 0.685, 0.786. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.47. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·V·Radiant`; the k4 to k6 lines (cylinder (5), 120 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·V·Radiant` |
| Standard spectrometer detection range | 5.42 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 95.2 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Life, Hope and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `2b 1c 1d 2f 1i 1j` (2x Heat, Light, Life, 2x Energy, Hope, Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 489 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 3.09 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 2nd Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
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
| Function | [[Light and Radiance]], [[Area Destruction]] |
| Element | [[Radiant Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Sunbeam (6-V-L-SNB)|Sunbeam]] (6) · [[Guiding Bolt (1-V-L-GB)|Guiding Bolt]] (1) · [[Lightning Bolt (3-V-L-LB)|Lightning Bolt]] (3) · [[Sacred Flame (0-V-L-SF)|Sacred Flame]] (0) · [[Sunburst (8-V-L-SNBB)|Sunburst]] (8) · [[Call Lightning (3-C-L-CLL)|Call Lightning]] (3) · [[Bohr's Model (2-P-L-BSM)|Bohr's Model]] (2) · [[Branding Smite (2-V-L-BS)|Branding Smite]] (2).


---

## Tactical Assessment

Harasses a defended position or chokepoint over a minute, and unmasks infiltrators using altered forms. Damage per exposure is modest.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
