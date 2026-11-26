---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/evocation
  - source/srd
aliases:
  - "1st Tier Spell: Thunderwave"
  - "Thunderwave"
  - "1-V-L-THN"
registry_id: 1-V-L-THN
attribute_code: "1·Evo·Thunder·cube (15)·Self·Instantaneous"
incantation: "Suder-Bépor"
tier: 1
school: Evocation
affinity: V
grade: L
pz_total: 784.8
pz_quantum: 350.0
t_e: 1.81
updated: 2026-11-16
---

**Thunderwave** (`1-V-L-THN`) is a 1st Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **785 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E 1.81 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Evocation]]
        - **Thunderwave** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-V-L-THN` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Evo·Thunder·cube (15)·Self·Instantaneous` |
| Incantation | *Suder-Bépor* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | Self |
| Area | cube (15) |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 2d8 thunder (mean 9) |
| Injury by tier | T1: 2d8, T2: 3d8, T3: 4d8, T4: 5d8, T5: 6d8, T6: 7d8, T7: 8d8, T8: 9d8, T9: 10d8 |
| Resistance check | constitution; on success: half injury |
| Practitioner lineages | Bard, Druid, Sorcerer, Wizard |

### Mechanism

A pressure wave expands from the caster through a 4.6 m cube, concussing and shoving creatures and loose objects with a boom heard 90 m away.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Thunder wave | `9 HP * 0.60 * 101.0 m^2 / 0.7` | 779 |
| Shoving 3 creatures 10 ft | `3 * 0.5 * 80 kg * 9.81 * 3.048 m / 1500` | 2.4 |
| Pattern cost | `0.01 × Q1 × (1 + 0.00)` | 3.5 |

| Quantity | Value |
|---|---|
| Effect energy | 781 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **785 Pz** (1,177.2 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 2.24 |
| Energy-equivalent tier T_E | 1.81 |
| Handling points | 0.00 |
| Grade score | 0.40 → L |

**Handling flags:** none.

**Assumptions:** 2d8 = 9; push resisted by friction coefficient 0.5; 3 creatures.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Thunderwave (1-V-L-THN) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Thunder | 13 | `0000000011011` |
| k4 Area | cube (15) | 7 | `0000000001111` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Suder-Bépor** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisuder-Bépor* · T3: *Lisuder-Bépor* · T4: *Visuder-Bépor* · T5: *Tisuder-Bépor* · T6: *Risuder-Bépor* · T7: *Misuder-Bépor* · T8: *Nisuder-Bépor* · T9: *Xyisuder-Bépor*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 3→0 4→1 | 4 |
| k4 Area | 0→9 1→10 2→11 3→12 | 4 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#a87266`.

![[Thunderwave (1-V-L-THN) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| Damage | Thunder | 0.929 | 0.709 | `#dc00ff` (421 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.923 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.995 | `#ff0028` (700 nm eq.) | source grid |
| Area | cube (15) | 0.194 | 0.996 | `#ffdf00` (642 nm eq.) | source grid |
| Range | Self | 0.706 | 0.832 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.23): swatch `#a39088`, measured lines at 0.004, 0.101, 0.195, 0.501, 0.706, 0.929. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.89. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·V·Thunder`; the k4 to k6 lines (cube (15), Self, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·V·Thunder` |
| Standard spectrometer detection range | 2.80 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.0 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is 2x Heat, Dark, Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `3b 1C 2f 2j` (3x Heat, Dark, 2x Energy, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 131 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 2.24 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 1st Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Area Destruction]] |
| Element | [[Thunder and Concussion Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Blast (1-V-L-BLS)|Blast]] (1) · [[Shatter (2-V-L-SHT)|Shatter]] (2) · [[Burning Hands (1-V-L-BH)|Burning Hands]] (1) · [[Kilonova (1-V-M-KLN)|Kilonova]] (1) · [[Resonant Shatter (1-V-L-RSO)|Resonant Shatter]] (1) · [[Bohr's Model (2-P-L-BSM)|Bohr's Model]] (2) · [[Galaxy Whirl (2-V-L-GWL)|Galaxy Whirl]] (2) · [[Geyser (2-V-L-GYS)|Geyser]] (2).


---

## Tactical Assessment

A close-quarters breaking tool for clearing a doorway, at the cost of announcing the caster's position.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
