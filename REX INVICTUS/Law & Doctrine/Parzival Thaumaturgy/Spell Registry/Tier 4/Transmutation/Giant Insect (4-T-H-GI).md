---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/transmutation
  - source/srd
aliases:
  - "4th Tier Spell: Giant Insect"
  - "Giant Insect"
  - "4-T-H-GI"
registry_id: 4-T-H-GI
attribute_code: "4·Tra·None·None·30 feet·Up to 10 minutes"
incantation: "Vieusinly"
tier: 4
school: Transmutation
affinity: T
grade: H
pz_total: 6283.3
pz_quantum: 7029.9
t_e: 3.89
updated: 2026-11-16
---

**Giant Insect** (`4-T-H-GI`) is a 4th Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **6,283 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E 3.89 and its handling grade at **High**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Transmutation]]
        - **Giant Insect** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-T-H-GI` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Tra·None·None·30 feet·Up to 10 minutes` |
| Incantation | *Vieusinly* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Transmutation]] |
| Casting time | 1 action |
| Range | 30 feet |
| Area | single point or target |
| Duration | Up to 10 minutes (concentration) |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Druid |

### Mechanism

Enlarges small arthropods into giant obedient forms that act on the caster's command for up to ten minutes.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| growth of 3 giant spiders | `10 Pz/kg * 3 * 200 kg` | 6,000 |
| animation and obedience, 3 creatures | `3 * 0.05 Pz/s = 0.15 Pz/s * 600 s` | 90.0 |
| Pattern cost | `0.01 × Q4 × (1 + 1.75)` | 193 |

| Quantity | Value |
|---|---|
| Effect energy | 6,000 Pz |
| Upkeep energy | 90.0 Pz (0.15 Pz/s) |
| **Total draw** | **6,283 Pz** (9,425.0 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 0.894 |
| Energy-equivalent tier T_E | 3.89 |
| Handling points | 1.75 |
| Grade score | 1.69 → H |

**Handling flags:** concentration, fragile, multi target control.

**Assumptions:** Three spiders option chosen as the largest added mass, 200 kg each; living matter 10 Pz/kg; upkeep 0.05 Pz/s each for 10 min.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Giant Insect (4-T-H-GI) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 4 | 4 | `0000000001001` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Up to 10 minutes | 15 | `0000000011111` |

### Incantation

Spoken as **Vieusinly** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T5: *Tivieusinly* · T6: *Rivieusinly* · T7: *Mivieusinly* · T8: *Nivieusinly* · T9: *Xyivieusinly*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 3→2 | 2 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 2→9 3→10 4→11 | 5 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#508579`.

![[Giant Insect (4-T-H-GI) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.893 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Up to 10 minutes | 0.789 | 0.927 | `#1e00ff` (463 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.994 | `#91ff00` (612 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.18): swatch `#7caac1`, measured lines at 0.295, 0.401, 0.790, 0.876. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.80. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·T·None`; the k4 to k6 lines (None, 30 feet, Up to 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·T·None` |
| Standard spectrometer detection range | 7.93 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 721 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1,047 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 4th Tier quantum of 7,030 Pz (89.4% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 4th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 4 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Summoning and Conjured Creatures]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|High]] |

Similar workings: [[Animate Objects (5-T-L-AO)|Animate Objects]] (5) · [[Conjure Magic Prism (4-C-L-CMPJ)|Conjure Magic Prism]] (4) · [[Conjure Minor Elementals (4-C-M-CME)|Conjure Minor Elementals]] (4) · [[Conjure Woodland Beings (4-C-L-CWB)|Conjure Woodland Beings]] (4) · [[Faithful Hound (4-C-L-FH)|Faithful Hound]] (4) · [[Guardian of Faith (4-C-L-GFA)|Guardian of Faith]] (4) · [[Magic Polarising Filter (4-C-L-MPF)|Magic Polarising Filter]] (4) · [[Thomson's Plum Pudding (2-T-L-TSPP)|Thomson's Plum Pudding]] (2).


---

## Tactical Assessment

Turns local fauna into shock troops or sentries, giving a lone caster a squad of expendable combatants.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
