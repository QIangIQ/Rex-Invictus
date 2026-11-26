---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/transmutation
  - source/srd
aliases:
  - "4th Tier Spell: Control Water"
  - "Control Water"
  - "4-T-H-CWN"
registry_id: 4-T-H-CWN
attribute_code: "4·Tra·Bludgeoning·cube (100)·300 feet·Up to 10 minutes"
incantation: "Viedeg-Bisphinly"
tier: 4
school: Transmutation
affinity: T
grade: H
pz_total: 225874.2
pz_quantum: 7029.9
t_e: 7.47
updated: 2026-11-16
---

**Control Water** (`4-T-H-CWN`) is a 4th Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **225,874 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E 7.47 and its handling grade at **High**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Transmutation]]
        - **Control Water** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-T-H-CWN` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Tra·Bludgeoning·cube (100)·300 feet·Up to 10 minutes` |
| Incantation | *Viedeg-Bisphinly* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Transmutation]] |
| Casting time | 1 action |
| Range | 300 feet |
| Area | cube (100) |
| Duration | Up to 10 minutes (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A drop of water and a pinch of dust |
| Ritual | no |
| Injury | 2d8 bludgeoning (mean 9) |
| Injury by tier | T4: 2d8 |
| Resistance check | strength; on success: half injury |
| Practitioner lineages | Cleric, Druid, Wizard |

### Mechanism

The field takes control of free water in a cube up to 100 ft on a side and can raise its level, part it into a trench, redirect its flow or spin a whirlpool. The modes can be switched each round.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| flood: raise 20 ft layer over 100 ft square (rho*A*H*g*H/2) | `1000*(100*ft)**2*(20*ft)*g*(20*ft)/2/J` | 112,893 |
| upkeep: hold elevated water: 1% of lift energy per round for 10 min | `0.01*1000*(100*ft)**2*(20*ft)*g*(20*ft)/2/J*100` | 112,893 |
| Pattern cost | `0.01 × Q4 × (1 + 0.25)` | 87.9 |

| Quantity | Value |
|---|---|
| Effect energy | 112,893 Pz |
| Upkeep energy | 112,893 Pz (188 Pz/s) |
| **Total draw** | **225,874 Pz** (338,811.3 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 32.1 |
| Energy-equivalent tier T_E | 7.47 |
| Handling points | 0.25 |
| Grade score | 1.98 → H |

**Handling flags:** concentration.

**Assumptions:** Flood mode as the maximum case: 5.66e6 kg raised with mean lift H/2; holding losses 1% of lift energy per round (no static work in ideal hold); whirlpool damage (2d8 bludgeoning, about 12 Pz over 3 rounds) omitted as smaller.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Control Water (4-T-H-CWN) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 4 | 4 | `0000000001001` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | Bludgeoning | 1 | `0000000000011` |
| k4 Area | cube (100) | 6 | `0000000001101` |
| k5 Range | 300 feet | 6 | `0000000001101` |
| k6 Duration | Up to 10 minutes | 15 | `0000000011111` |

### Incantation

Spoken as **Viedeg-Bisphinly** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T5: *Tiviedeg-Bisphinly* · T6: *Riviedeg-Bisphinly* · T7: *Miviedeg-Bisphinly* · T8: *Niviedeg-Bisphinly* · T9: *Xyiviedeg-Bisphinly*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 3→2 | 2 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 | 2 |
| k4 Area | 0→9 2→11 3→12 | 3 |
| k5 Range | 0→8 2→10 3→11 | 3 |
| k6 Duration | 0→7 1→8 2→9 3→10 4→11 | 5 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#7d9150`.

![[Control Water (4-T-H-CWN) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| Damage | Bludgeoning | 0.143 | 0.967 | `#ff9900` (657 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.893 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Up to 10 minutes | 0.789 | 0.927 | `#1e00ff` (463 nm eq.) | source grid |
| Area | cube (100) | 0.167 | 0.973 | `#ffb900` (650 nm eq.) | source grid |
| Range | 300 feet | 0.353 | 0.999 | `#40ff00` (594 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.15): swatch `#95a1a5`, measured lines at 0.143, 0.167, 0.354, 0.401, 0.790, 0.876. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 5.35. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·T·Bludgeoning`; the k4 to k6 lines (cube (100), 300 feet, Up to 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·T·Bludgeoning` |
| Standard spectrometer detection range | 47.53 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 23,282 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Within, Rigidity, 2x Movement and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1d 1h 3j` (Within, Life, Flexibility, 3x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 37,646 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 32.13 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 4th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 4th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 4 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Terrain and Matter Shaping]], [[Area Destruction]] |
| Element | [[Bludgeoning Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|High]] |

Similar workings: [[Ice Storm (4-V-L-ISE)|Ice Storm]] (4) · [[Geyser (2-V-L-GYS)|Geyser]] (2) · [[Black Tentacles (4-C-L-BT)|Black Tentacles]] (4) · [[Supersonic Omnidirectional Jet (5-C-M-SOJ)|Supersonic Omnidirectional Jet]] (5) · [[Wind Wall (3-V-L-WWN)|Wind Wall]] (3) · [[Fabricate (4-T-L-FBR)|Fabricate]] (4) · [[Freefall (4-T-L-FRF)|Freefall]] (4) · [[Planetary Rings (4-P-L-PR)|Planetary Rings]] (4).


---

## Tactical Assessment

Riverine and littoral control: flooding positions, opening crossings, capsizing small craft or swamping landing operations.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
