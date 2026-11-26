---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-6
  - spell/evocation
  - source/srd
aliases:
  - "6th Tier Spell: Chain Lightning"
  - "Chain Lightning"
  - "6-V-L-CLA"
registry_id: 6-V-L-CLA
attribute_code: "6·Evo·Lightning·None·150 feet·Instantaneous"
incantation: "Runin-’nosin"
tier: 6
school: Evocation
affinity: V
grade: L
pz_total: 546.4
pz_quantum: 51944.6
t_e: 1.45
updated: 2026-11-16
---

**Chain Lightning** (`6-V-L-CLA`) is a 6th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **546 Pz** against a slot quantum of 51,945 Pz, which puts its energy-equivalent tier at T_E 1.45 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 6 Workings]]
      - [[Evocation]]
        - **Chain Lightning** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `6-V-L-CLA` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `6·Evo·Lightning·None·150 feet·Instantaneous` |
| Incantation | *Runin-’nosin* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 6th Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 150 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A bit of fur; a piece of amber, glass, or a crystal rod; and three silver pins |
| Ritual | no |
| Injury | 10d8 lightning (mean 45) |
| Injury by tier | T6: 10d8 |
| Resistance check | agility; on success: half injury |
| Practitioner lineages | Sorcerer, Wizard |

### Mechanism

A bolt strikes one target and splits into three more that jump to nearby targets.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| primary and chained bolts | `45 HP * 0.3 Pz/HP (lightning) * F 0.5 * 4 target(s)/hit(s)` | 27.0 |
| Pattern cost | `0.01 × Q6 × (1 + 0.00)` | 519 |

| Quantity | Value |
|---|---|
| Effect energy | 27.0 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **546 Pz** (819.7 kJ) |
| Slot quantum Q6 | 51,945 Pz |
| Field gain (draw / quantum) | 0.0105 |
| Energy-equivalent tier T_E | 1.45 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** 4 targets at 45 average injury each; ray factor 0.5.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Chain Lightning (6-V-L-CLA) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 6 | 6 | `0000000001101` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Lightning | 5 | `0000000001011` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 150 feet | 4 | `0000000001001` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Runin-’nosin** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T7: *Mirunin-’nosin* · T8: *Nirunin-’nosin* · T9: *Xyirunin-’nosin*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 3→2 | 3 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 3→0 | 3 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 | 2 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#59cd61`.

![[Chain Lightning (6-V-L-CLA) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 6 | 0.600 | 1.000 | `#00ebff` (520 nm eq.) | source grid |
| Damage | Lightning | 0.429 | 0.985 | `#00ff25` (571 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.995 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.835 | `#ff0028` (700 nm eq.) | source grid |
| Range | 150 feet | 0.235 | 0.936 | `#e3ff00` (629 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.14): swatch `#94dd9e`, measured lines at 0.004, 0.236, 0.429, 0.501, 0.601. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.74. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `6·V·Lightning`; the k4 to k6 lines (None, 150 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `6·V·Lightning` |
| Standard spectrometer detection range | 2.34 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 2,597 Pz (0.05 × Q6) |
| Counter drawn cold (all six layers) | 5,194 Pz (0.10 × Q6) |
| Unravel after completion | 5,194 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is 2x Heat, Light, Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `3b 1c 2f 2j` (3x Heat, Light, 2x Energy, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 91.1 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 6th Tier quantum of 51,945 Pz (1.1% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 6th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 6 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Light and Radiance]], [[Precision Strikes]] |
| Element | [[Lightning Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Lightning Bolt (3-V-L-LB)|Lightning Bolt]] (3) · [[Blight (4-N-L-BLG)|Blight]] (4) · [[Sunbeam (6-V-L-SNB)|Sunbeam]] (6) · [[Arcane Sword (7-P-L-ASC)|Arcane Sword]] (7) · [[Call Lightning (3-C-L-CLL)|Call Lightning]] (3) · [[Dark Matter Sword (7-V-L-DMS)|Dark Matter Sword]] (7) · [[Electrify (1-V-L-ELC)|Electrify]] (1) · [[Guiding Bolt (1-V-L-GB)|Guiding Bolt]] (1).


---

## Tactical Assessment

Engages several dispersed soldiers or drones in one action.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 6 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
