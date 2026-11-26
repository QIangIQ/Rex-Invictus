---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-6
  - spell/divination
  - source/srd
aliases:
  - "6th Tier Spell: Find the Path"
  - "Find the Path"
  - "6-D-L-FP"
registry_id: 6-D-L-FP
attribute_code: "6·Div·None·None·Self·Up to 24 hours"
incantation: "Riporyi"
tier: 6
school: Divination
affinity: D
grade: L
pz_total: 9550.0
pz_quantum: 51944.6
t_e: 4.31
updated: 2026-11-16
---

**Find the Path** (`6-D-L-FP`) is a 6th Tier working of the [[Divination]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **9,550 Pz** against a slot quantum of 51,945 Pz, which puts its energy-equivalent tier at T_E 4.31 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 6 Workings]]
      - [[Divination]]
        - **Find the Path** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `6-D-L-FP` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `6·Div·None·None·Self·Up to 24 hours` |
| Incantation | *Riporyi* |
| Affinity | D (Divination) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 6th Tier |
| School | [[Divination]] |
| Casting time | 1 minute |
| Range | Self |
| Area | single point or target |
| Duration | Up to 24 hours (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A set of divinatory tools--such as bones, ivory sticks, cards, teeth, or carved runes--worth 100gp and an object from the location you wish to find |
| Ritual | no |
| Practitioner lineages | Bard, Cleric, Druid |

### Mechanism

A sustained divination resolves the bearing and distance to a known fixed location and evaluates each branching route for shortest length as it is encountered.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| initial fix on destination | `instant info` | 1.0 |
| continuous route divination | `0.1 Pz/s*86400  [C2]` | 8,640 |
| Pattern cost | `0.01 × Q6 × (1 + 0.75)` | 909 |

| Quantity | Value |
|---|---|
| Effect energy | 8,641 Pz |
| Upkeep energy | 0 Pz (1.0 Pz/s) |
| **Total draw** | **9,550 Pz** (14,325.0 kJ) |
| Slot quantum Q6 | 51,945 Pz |
| Field gain (draw / quantum) | 0.184 |
| Energy-equivalent tier T_E | 4.31 |
| Handling points | 0.75 |
| Grade score | -0.10 → L |

Calibration applied: C2 (Sympathetic link saturation), see [[Parzival Energy Budget#Registry calibration rules]].

**Handling flags:** concentration, costly material, long cast.

**Assumptions:** Effective search radius 10 km for the divination power law; full 24 h of sustained focus.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Find the Path (6-D-L-FP) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 6 | 6 | `0000000001101` |
| k2 School | Divination | 2 | `0000000000101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Up to 24 hours | 17 | `0000000100011` |

### Incantation

Spoken as **Riporyi** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T7: *Miriporyi* · T8: *Niriporyi* · T9: *Xyiriporyi*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 3→2 | 3 |
| k2 School | 0→11 2→0 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 5→12 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#5d90c1`.

![[Find the Path (6-D-L-FP) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 6 | 0.600 | 1.000 | `#00ebff` (520 nm eq.) | source grid |
| School | Divination | 0.250 | 0.941 | `#cdff00` (625 nm eq.) | source grid |
| Duration | Up to 24 hours | 0.895 | 0.957 | `#b100ff` (432 nm eq.) | source grid |
| Range | Self | 0.706 | 0.994 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.17): swatch `#81bcb3`, measured lines at 0.251, 0.601, 0.706, 0.895. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.98. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `6·D·None`; the k4 to k6 lines (None, Self, Up to 24 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `6·D·None` |
| Standard spectrometer detection range | 9.77 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 2,597 Pz (0.05 × Q6) |
| Counter drawn cold (all six layers) | 5,194 Pz (0.10 × Q6) |
| Unravel after completion | 5,194 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Light, 2x Extraspection. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 2c 1d 1F 2g 1J` (Beyond, 2x Light, Life, Potential, 2x Extraspection, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1,592 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 6th Tier quantum of 51,945 Pz (18.4% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 6th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Divination school with aspect lean Beyond, Light, 2x Extraspection. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 6 Workings]] |
| School | [[Divination]] |
| Affinity | [[Divination]] (D) |
| Function | [[Divination and Sensing]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[True Seeing (6-D-L-TSU)|True Seeing]] (6) · [[Commune (5-D-L-CMMM)|Commune]] (5) · [[Commune With Nature (5-D-L-CN)|Commune With Nature]] (5) · [[Contact Other Plane (5-D-L-COP)|Contact Other Plane]] (5) · [[Legend Lore (5-D-L-LLG)|Legend Lore]] (5) · [[Scrying (5-D-L-SCR)|Scrying]] (5) · [[Telepathic Bond (5-D-L-TB)|Telepathic Bond]] (5) · [[Arcane Eye (4-D-L-AE)|Arcane Eye]] (4).


---

## Tactical Assessment

Navigation that ignores jamming, map denial and spoofed satellite positioning; useful for infiltration teams and for finding a way out of deliberately confusing terrain or orbital habitats.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 6 Workings]] · [[Divination]] · [[Spell Breakdown Procedure]] · [[Parzival]]
