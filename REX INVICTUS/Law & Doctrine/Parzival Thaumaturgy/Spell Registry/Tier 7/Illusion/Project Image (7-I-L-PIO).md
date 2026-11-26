---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-7
  - spell/illusion
  - source/srd
aliases:
  - "7th Tier Spell: Project Image"
  - "Project Image"
  - "7-I-L-PIO"
registry_id: 7-I-L-PIO
attribute_code: "7·Ill·None·None·500 miles·Up to 24 hours"
incantation: "Maiqulyi"
tier: 7
school: Illusion
affinity: I
grade: L
pz_total: 12170.1
pz_quantum: 141200.1
t_e: 4.55
updated: 2026-11-16
---

**Project Image** (`7-I-L-PIO`) is a 7th Tier working of the [[Illusion]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **12,170 Pz** against a slot quantum of 141,200 Pz, which puts its energy-equivalent tier at T_E 4.55 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 7 Workings]]
      - [[Illusion]]
        - **Project Image** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `7-I-L-PIO` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `7·Ill·None·None·500 miles·Up to 24 hours` |
| Incantation | *Maiqulyi* |
| Affinity | I (Illusion) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 7th Tier |
| School | [[Illusion]] |
| Casting time | 1 action |
| Range | 500 miles |
| Area | single point or target |
| Duration | Up to 24 hours (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A small replica of you made from materials worth at least 5 gp |
| Ritual | no |
| Practitioner lineages | Bard, Wizard |

### Mechanism

A remote illusory body of the caster is projected to a known site and linked to the caster's senses and voice across hundreds of miles.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| illusory body copy, ~0.5 m^3 for 24 h | `0.002*(0.5/1000)*86400` | 0.0864 |
| [upkeep] two-way sensory link at 500 miles, 24 h | `0.1 Pz/s*86400  [C2]` | 8,640 |
| Pattern cost | `0.01 × Q7 × (1 + 1.50)` | 3,530 |

| Quantity | Value |
|---|---|
| Effect energy | 0.0864 Pz |
| Upkeep energy | 8,640 Pz (80.5 Pz/s) |
| **Total draw** | **12,170 Pz** (18,255.1 kJ) |
| Slot quantum Q7 | 141,200 Pz |
| Field gain (draw / quantum) | 0.0862 |
| Energy-equivalent tier T_E | 4.55 |
| Handling points | 1.50 |
| Grade score | 0.50 → L |

Calibration applied: C2 (Sympathetic link saturation), see [[Parzival Energy Budget#Registry calibration rules]].

**Handling flags:** concentration, costly material, fragile.

**Assumptions:** Full 500 mile range and full 24 h held; linear divination range rate; the long range makes upkeep dominate.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Project Image (7-I-L-PIO) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 7 | 7 | `0000000001111` |
| k2 School | Illusion | 5 | `0000000001011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 500 miles | 9 | `0000000010011` |
| k6 Duration | Up to 24 hours | 17 | `0000000100011` |

### Incantation

Spoken as **Maiqulyi** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T8: *Nimaiqulyi* · T9: *Xyimaiqulyi*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 3→2 | 4 |
| k2 School | 0→11 1→12 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 4→12 | 3 |
| k6 Duration | 0→7 1→8 5→12 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#2b88eb`.

![[Project Image (7-I-L-PIO) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 7 | 0.700 | 1.000 | `#005eff` (490 nm eq.) | source grid |
| School | Illusion | 0.625 | 0.997 | `#00c5ff` (512 nm eq.) | source grid |
| Duration | Up to 24 hours | 0.895 | 0.981 | `#b100ff` (432 nm eq.) | source grid |
| Range | 500 miles | 0.529 | 0.986 | `#00ffb1` (541 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.21): swatch `#3ecedb`, measured lines at 0.530, 0.626, 0.701, 0.895. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.09. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `7·I·None`; the k4 to k6 lines (None, 500 miles, Up to 24 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `7·I·None` |
| Standard spectrometer detection range | 11.03 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 7,060 Pz (0.05 × Q7) |
| Counter drawn cold (all six layers) | 14,120 Pz (0.10 × Q7) |
| Unravel after completion | 15,848 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Light, Introspection, 2x Flexibility. The working vector used by [[Recast Tension and Combination Affinity]] is `2c 1d 1F 1G 2h 1J` (2x Light, Life, Potential, Introspection, 2x Flexibility, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 2,028 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 7th Tier quantum of 141,200 Pz (8.6% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 7th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Illusion school with aspect lean Light, Introspection, 2x Flexibility. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 7 Workings]] |
| School | [[Illusion]] |
| Affinity | [[Illusion]] (I) |
| Function | [[Concealment and Illusion]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Mirage Arcane (7-I-M-MAR)|Mirage Arcane]] (7) · [[Programmed Illusion (6-I-L-PI)|Programmed Illusion]] (6) · [[Dream of the Blue Veil (7-C-M-DBV)|Dream of the Blue Veil]] (7) · [[Mislead (5-I-L-MSL)|Mislead]] (5) · [[Seeming (5-I-L-SMN)|Seeming]] (5) · [[Sequester (7-T-L-SQS)|Sequester]] (7) · [[Greater Invisibility (4-I-L-GIE)|Greater Invisibility]] (4) · [[Hallucinatory Terrain (4-I-M-HT)|Hallucinatory Terrain]] (4).


---

## Tactical Assessment

Remote command presence, negotiation and reconnaissance with no risk to the operator. The image collapses on any hit.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 7 Workings]] · [[Illusion]] · [[Spell Breakdown Procedure]] · [[Parzival]]
