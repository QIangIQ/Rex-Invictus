---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/evocation
  - source/srd
aliases:
  - "3rd Tier Spell: Lightning Bolt"
  - "Lightning Bolt"
  - "3-V-L-LB"
registry_id: 3-V-L-LB
attribute_code: "3·Evo·Lightning·line (100)·Self·Instantaneous"
incantation: "Lunin-Lopor"
tier: 3
school: Evocation
affinity: V
grade: L
pz_total: 1140.9
pz_quantum: 2586.2
t_e: 2.18
updated: 2026-11-16
---

**Lightning Bolt** (`3-V-L-LB`) is a 3rd Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **1,141 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E 2.18 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Evocation]]
        - **Lightning Bolt** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-V-L-LB` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Evo·Lightning·line (100)·Self·Instantaneous` |
| Incantation | *Lunin-Lopor* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | Self |
| Area | line (100) |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A bit of fur and a rod of amber, crystal, or glass |
| Ritual | no |
| Injury | 8d6 lightning (mean 28) |
| Injury by tier | T3: 8d6, T4: 9d6, T5: 10d6, T6: 11d6, T7: 12d6, T8: 13d6, T9: 14d6 |
| Resistance check | agility; on success: half injury |
| Practitioner lineages | Sorcerer, Wizard |

### Mechanism

The field drives an electrical discharge along a 100 ft by 5 ft channel from the caster, injuring everything in the path and igniting loose flammables.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Lightning stroke along line | `28 HP * 0.30 * (92.90 m^2 / 0.7)` | 1,115 |
| Pattern cost | `0.01 × Q3 × (1 + 0.00)` | 25.9 |

| Quantity | Value |
|---|---|
| Effect energy | 1,115 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **1,141 Pz** (1,711.3 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 0.441 |
| Energy-equivalent tier T_E | 2.18 |
| Handling points | 0.00 |
| Grade score | -0.41 → L |

**Handling flags:** none.

**Assumptions:** Line 100 ft by 5 ft; 8d6 = 28 average, full value.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Lightning Bolt (3-V-L-LB) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Lightning | 5 | `0000000001011` |
| k4 Area | line (100) | 23 | `0000000101111` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Lunin-Lopor** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vilunin-Lopor* · T5: *Tilunin-Lopor* · T6: *Rilunin-Lopor* · T7: *Milunin-Lopor* · T8: *Nilunin-Lopor* · T9: *Xyilunin-Lopor*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 3→0 | 3 |
| k4 Area | 0→9 1→10 2→11 3→12 5→1 | 5 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#42ae76`.

![[Lightning Bolt (3-V-L-LB) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| Damage | Lightning | 0.429 | 0.992 | `#00ff25` (571 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.980 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.956 | `#ff0028` (700 nm eq.) | source grid |
| Area | line (100) | 0.639 | 0.944 | `#00b5ff` (508 nm eq.) | source grid |
| Range | Self | 0.706 | 0.921 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.19): swatch `#96d79c`, measured lines at 0.004, 0.300, 0.429, 0.501, 0.639, 0.706. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.06. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·V·Lightning`; the k4 to k6 lines (line (100), Self, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·V·Lightning` |
| Standard spectrometer detection range | 3.38 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 259 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is 2x Heat, Light, Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `3b 1c 2f 2j` (3x Heat, Light, 2x Energy, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 190 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 3rd Tier quantum of 2,586 Pz (44.1% of it). |
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
| Function | [[Light and Radiance]], [[Area Destruction]] |
| Element | [[Lightning Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Call Lightning (3-C-L-CLL)|Call Lightning]] (3) · [[Moonbeam (2-V-M-MNB)|Moonbeam]] (2) · [[Voltaic Arc (5-V-L-VA)|Voltaic Arc]] (5) · [[Chain Lightning (6-V-L-CLA)|Chain Lightning]] (6) · [[Sunbeam (6-V-L-SNB)|Sunbeam]] (6) · [[Daylight (3-V-L-DYL)|Daylight]] (3) · [[Fireball (3-V-M-FRB)|Fireball]] (3) · [[Sonic Boom (3-P-L-SBN)|Sonic Boom]] (3).


---

## Tactical Assessment

Effective down corridors, streets and trenches where enemies line up. Grounded conductive armour and Faraday shielding reduce its effect.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
