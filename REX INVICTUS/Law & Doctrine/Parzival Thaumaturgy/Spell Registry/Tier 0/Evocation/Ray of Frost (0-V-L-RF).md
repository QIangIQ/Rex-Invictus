---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-0
  - spell/evocation
  - source/srd
aliases:
  - "Cantrip Spell: Ray of Frost"
  - "Ray of Frost"
  - "0-V-L-RF"
registry_id: 0-V-L-RF
attribute_code: "0·Evo·Cold·None·60 feet·Instantaneous"
incantation: "Culod-’wyn"
tier: 0
school: Evocation
affinity: V
grade: L
pz_total: 3.3
pz_quantum: 128.8
t_e: -3.66
updated: 2026-11-16
---

**Ray of Frost** (`0-V-L-RF`) is a Cantrip (Tier 0) working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **3.3 Pz** against a slot quantum of 129 Pz, which puts its energy-equivalent tier at T_E -3.66 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 0 Workings]]
      - [[Evocation]]
        - **Ray of Frost** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `0-V-L-RF` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `0·Evo·Cold·None·60 feet·Instantaneous` |
| Incantation | *Culod-’wyn* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | Cantrip (Tier 0) |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 1d8 cold (mean 4.5) |
| Injury by caster maturity bands | T1: 1d8, T5: 2d8, T11: 3d8, T17: 4d8 |
| Delivery | aimed ranged working |
| Practitioner lineages | Sorcerer, Wizard |

### Mechanism

A chilled beam pulls heat from a target and stiffens its limbs for a few seconds.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| 1d8 cold (4.5), directed | `4.5*0.90*0.5` | 2.0 |
| Pattern cost | `0.01 × Q0 × (1 + 0.00)` | 1.3 |

| Quantity | Value |
|---|---|
| Effect energy | 2.0 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **3.3 Pz** (5.0 kJ) |
| Slot quantum Q0 | 129 Pz |
| Field gain (draw / quantum) | 0.0257 |
| Energy-equivalent tier T_E | -3.66 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Base 1d8; directed F 0.5; slowing effect costed as negligible.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Ray of Frost (0-V-L-RF) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 0 | 0 | `0000000000001` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Cold | 2 | `0000000000101` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Culod-’wyn** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T1: *Siculod-’wyn* · T2: *Hiculod-’wyn* · T3: *Liculod-’wyn* · T4: *Viculod-’wyn* · T5: *Ticulod-’wyn* · T6: *Riculod-’wyn* · T7: *Miculod-’wyn* · T8: *Niculod-’wyn* · T9: *Xyiculod-’wyn*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 | 1 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 2→12 | 2 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#a19058`.

![[Ray of Frost (0-V-L-RF) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 0 | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| Damage | Cold | 0.214 | 0.977 | `#fffa00` (636 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.882 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.841 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.21): swatch `#b7a371`, measured lines at 0.005, 0.215, 0.501, 0.589. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 0.52. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `0·V·Cold`; the k4 to k6 lines (None, 60 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `0·V·Cold` |
| Standard spectrometer detection range | 0.18 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 6.4 Pz (0.05 × Q0) |
| Counter drawn cold (all six layers) | 12.9 Pz (0.10 × Q0) |
| Unravel after completion | 12.9 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is 2x Cold, 2x Death and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1B 2D 2f 1j` (Cold, 2x Death, 2x Energy, Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 0.552 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the Cantrip (Tier 0) quantum of 129 Pz (2.6% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at Cantrip (Tier 0) up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 0 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Precision Strikes]] |
| Element | [[Cold and Ice Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Chill Touch (0-N-L-CT)|Chill Touch]] (0) · [[Cool Metal (2-T-L-CM)|Cool Metal]] (2) · [[Eldritch Blast (0-P-L-EB)|Eldritch Blast]] (0) · [[Fire Bolt (0-V-L-FB)|Fire Bolt]] (0) · [[Radiation Poisoning (0-V-L-RP)|Radiation Poisoning]] (0) · [[Sacred Flame (0-V-L-SF)|Sacred Flame]] (0) · [[Shocking Grasp (0-V-L-SG)|Shocking Grasp]] (0) · [[Divine Favor (1-V-L-DF)|Divine Favor]] (1).


---

## Tactical Assessment

A cheap ranged attack that also slows pursuers.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 0 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
