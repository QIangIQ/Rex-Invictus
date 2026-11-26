---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/divination
  - source/srd
aliases:
  - "5th Tier Spell: Commune"
  - "Commune"
  - "5-D-L-CMMM"
registry_id: 5-D-L-CMMM
attribute_code: "5·Div·None·None·Self·1 minute"
incantation: "Tipore"
tier: 5
school: Divination
affinity: D
grade: L
pz_total: 295.6
pz_quantum: 19109.4
t_e: 0.83
updated: 2026-11-16
---

**Commune** (`5-D-L-CMMM`) is a 5th Tier working of the [[Divination]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **296 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 0.83 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Divination]]
        - **Commune** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-D-L-CMMM` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Div·None·None·Self·1 minute` |
| Incantation | *Tipore* |
| Affinity | D (Divination) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Divination]] |
| Casting time | 1 minute |
| Range | Self |
| Area | single point or target |
| Duration | 1 minute |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Incense and a vial of holy or unholy water |
| Ritual | yes |
| Practitioner lineages | Cleric |

### Mechanism

The caster opens a link to a patron entity and receives yes or no answers to up to three questions.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| instant information | `3 * 1 Pz` | 3.0 |
| cross-plane contact | `0.1 Pz/s*60  [C2]` | 6.0 |
| Pattern cost | `0.01 × Q5 × (1 + 0.50)` | 287 |

| Quantity | Value |
|---|---|
| Effect energy | 9.0 Pz |
| Upkeep energy | 0 Pz (100 Pz/s) |
| **Total draw** | **296 Pz** (443.5 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 0.0155 |
| Energy-equivalent tier T_E | 0.83 |
| Handling points | 0.50 |
| Grade score | -0.50 → L |

Calibration applied: C2 (Sympathetic link saturation), see [[Parzival Energy Budget#Registry calibration rules]].

**Handling flags:** ritual, long cast.

**Assumptions:** Contact distance 1e6 m equivalent; 60 s; 3 questions.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Commune (5-D-L-CMMM) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Divination | 2 | `0000000000101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | 1 minute | 1 | `0000000000011` |

### Incantation

Spoken as **Tipore** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Ritipore* · T7: *Mitipore* · T8: *Nitipore* · T9: *Xyitipore*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 2→0 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#70af64`.

![[Commune (5-D-L-CMMM) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| School | Divination | 0.250 | 0.969 | `#cdff00` (625 nm eq.) | source grid |
| Duration | 1 minute | 0.105 | 0.925 | `#ff6300` (668 nm eq.) | source grid |
| Range | Self | 0.706 | 0.979 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.14): swatch `#aec18a`, measured lines at 0.106, 0.251, 0.501, 0.706. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.47. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·D·None`; the k4 to k6 lines (None, Self, 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·D·None` |
| Standard spectrometer detection range | 1.72 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 1,911 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Light, 2x Extraspection. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 2c 1d 1F 2g 1J` (Beyond, 2x Light, Life, Potential, 2x Extraspection, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 49.3 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 5th Tier quantum of 19,109 Pz (1.5% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 5th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Divination school with aspect lean Beyond, Light, 2x Extraspection. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 5 Workings]] |
| School | [[Divination]] |
| Affinity | [[Divination]] (D) |
| Function | [[Divination and Sensing]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Commune With Nature (5-D-L-CN)|Commune With Nature]] (5) · [[Contact Other Plane (5-D-L-COP)|Contact Other Plane]] (5) · [[Legend Lore (5-D-L-LLG)|Legend Lore]] (5) · [[Scrying (5-D-L-SCR)|Scrying]] (5) · [[Telepathic Bond (5-D-L-TB)|Telepathic Bond]] (5) · [[Arcane Eye (4-D-L-AE)|Arcane Eye]] (4) · [[Divination (4-D-L-DVN)|Divination]] (4) · [[Find the Path (6-D-L-FP)|Find the Path]] (6).


---

## Tactical Assessment

High-confidence intelligence for planning.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Divination]] · [[Spell Breakdown Procedure]] · [[Parzival]]
