---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-6
  - spell/evocation
  - source/srd
aliases:
  - "6th Tier Spell: Blade Barrier"
  - "Blade Barrier"
  - "6-V-L-BB"
registry_id: 6-V-L-BB
attribute_code: "6·Evo·Slashing·line (100)·90 feet·Up to 10 minutes"
incantation: "Rusih-Loylarly"
tier: 6
school: Evocation
affinity: V
grade: L
pz_total: 21971.9
pz_quantum: 51944.6
t_e: 5.14
updated: 2026-11-16
---

**Blade Barrier** (`6-V-L-BB`) is a 6th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **21,972 Pz** against a slot quantum of 51,945 Pz, which puts its energy-equivalent tier at T_E 5.14 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 6 Workings]]
      - [[Evocation]]
        - **Blade Barrier** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `6-V-L-BB` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `6·Evo·Slashing·line (100)·90 feet·Up to 10 minutes` |
| Incantation | *Rusih-Loylarly* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 6th Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 90 feet |
| Area | line (100) |
| Duration | Up to 10 minutes (concentration) |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 6d10 slashing (mean 33) |
| Injury by tier | T6: 6d10 |
| Resistance check | agility; on success: half injury |
| Practitioner lineages | Cleric |

### Mechanism

A wall of whirling energy blades up to 30 m long and 6 m high gives heavy cover and lacerates anything passing through.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| blade wall | `33 HP * 0.4 Pz/HP (slashing) * (wall 2*30.48*6.096 = 371.612 m^2 / 0.7 m^2) * 3 triggers` | 21,023 |
| rotor drag upkeep | `0.5 Pz/s * 600 s` | 300 |
| Pattern cost | `0.01 × Q6 × (1 + 0.25)` | 649 |

| Quantity | Value |
|---|---|
| Effect energy | 21,023 Pz |
| Upkeep energy | 300 Pz (0.5 Pz/s) |
| **Total draw** | **21,972 Pz** (32,957.9 kJ) |
| Slot quantum Q6 | 51,945 Pz |
| Field gain (draw / quantum) | 0.423 |
| Energy-equivalent tier T_E | 5.14 |
| Handling points | 0.25 |
| Grade score | -0.18 → L |

**Handling flags:** concentration.

**Assumptions:** Used the 6.1 m wall height for the line surface; 3 triggers; blade spin losses about 750 W.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Blade Barrier (6-V-L-BB) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 6 | 6 | `0000000001101` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Slashing | 12 | `0000000011001` |
| k4 Area | line (100) | 23 | `0000000101111` |
| k5 Range | 90 feet | 11 | `0000000010111` |
| k6 Duration | Up to 10 minutes | 15 | `0000000011111` |

### Incantation

Spoken as **Rusih-Loylarly** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T7: *Mirusih-Loylarly* · T8: *Nirusih-Loylarly* · T9: *Xyirusih-Loylarly*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 3→2 | 3 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 3→0 4→1 | 3 |
| k4 Area | 0→9 1→10 2→11 3→12 5→1 | 5 |
| k5 Range | 0→8 1→9 2→10 4→12 | 4 |
| k6 Duration | 0→7 1→8 2→9 3→10 4→11 | 5 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#188deb`.

![[Blade Barrier (6-V-L-BB) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 6 | 0.600 | 1.000 | `#00ebff` (520 nm eq.) | source grid |
| Damage | Slashing | 0.857 | 0.967 | `#7b00ff` (443 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.995 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Up to 10 minutes | 0.789 | 0.982 | `#1e00ff` (463 nm eq.) | source grid |
| Area | line (100) | 0.639 | 0.999 | `#00b5ff` (508 nm eq.) | source grid |
| Range | 90 feet | 0.647 | 0.999 | `#00aaff` (506 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.14): swatch `#4cd3d4`, measured lines at 0.501, 0.601, 0.645, 0.790, 0.858. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.34. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `6·V·Slashing`; the k4 to k6 lines (line (100), 90 feet, Up to 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `6·V·Slashing` |
| Standard spectrometer detection range | 14.82 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 2,597 Pz (0.05 × Q6) |
| Counter drawn cold (all six layers) | 5,194 Pz (0.10 × Q6) |
| Unravel after completion | 5,254 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Cold, Rigidity, 2x Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `2f 1H 3j` (2x Energy, Rigidity, 3x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 3,662 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 6th Tier quantum of 51,945 Pz (42.3% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
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
| Function | [[Walls and Barriers]], [[Area Destruction]] |
| Element | [[Slashing Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Wall of Ice (6-V-M-WI)|Wall of Ice]] (6) · [[Wall of Fire (4-V-M-WF)|Wall of Fire]] (4) · [[Wall of Thorns (6-C-L-WT)|Wall of Thorns]] (6) · [[Wind Wall (3-V-L-WWN)|Wind Wall]] (3) · [[Absolute Zero (6-V-L-AZ)|Absolute Zero]] (6) · [[Burst Radiation (6-V-L-BR)|Burst Radiation]] (6) · [[Freezing Sphere (6-V-M-FSZ)|Freezing Sphere]] (6) · [[Sunbeam (6-V-L-SNB)|Sunbeam]] (6).


---

## Tactical Assessment

A cutting barrier that blocks infantry assault lanes for ten minutes.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 6 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
