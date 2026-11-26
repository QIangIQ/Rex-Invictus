---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/divination
  - source/srd
aliases:
  - "3rd Tier Spell: Tongues"
  - "Tongues"
  - "3-D-L-TNG"
registry_id: 3-D-L-TNG
attribute_code: "3·Div·None·None·Touch·1 hour"
incantation: "Lilixa"
tier: 3
school: Divination
affinity: D
grade: L
pz_total: 134.9
pz_quantum: 2586.2
t_e: 0.05
updated: 2026-11-16
---

**Tongues** (`3-D-L-TNG`) is a 3rd Tier working of the [[Divination]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **135 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E 0.05 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Divination]]
        - **Tongues** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-D-L-TNG` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Div·None·None·Touch·1 hour` |
| Incantation | *Lilixa* |
| Affinity | D (Divination) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Divination]] |
| Casting time | 1 action |
| Range | Touch |
| Area | single point or target |
| Duration | 1 hour |
| Components | spoken (incantation), material focus. Material: A small clay model of a ziggurat |
| Ritual | no |
| Practitioner lineages | Bard, Cleric, Sorcerer, Warlock, Wizard |

### Mechanism

The subject understands any spoken language and its own speech is understood by any listener who knows a language.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Language mapping | `instant info = 1 Pz` | 1.0 |
| Upkeep: Translation for subject and 5 listeners | `0.005 Pz/s * 6 * 3600 s` | 108 |
| Pattern cost | `0.01 × Q3 × (1 + 0.00)` | 25.9 |

| Quantity | Value |
|---|---|
| Effect energy | 1.0 Pz |
| Upkeep energy | 108 Pz (0.03 Pz/s) |
| **Total draw** | **135 Pz** (202.3 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 0.0521 |
| Energy-equivalent tier T_E | 0.05 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** 1 subject plus 5 regular listeners for 1 h.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Tongues (3-D-L-TNG) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Divination | 2 | `0000000000101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | 1 hour | 0 | `0000000000001` |

### Incantation

Spoken as **Lilixa** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vililixa* · T5: *Tililixa* · T6: *Rililixa* · T7: *Mililixa* · T8: *Nililixa* · T9: *Xyililixa*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 2→0 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 | 1 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#bd8c38`.

![[Tongues (3-D-L-TNG) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| School | Divination | 0.250 | 0.999 | `#cdff00` (625 nm eq.) | source grid |
| Duration | 1 hour | 0.053 | 0.970 | `#ff1c00` (684 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.844 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.23): swatch `#da9873`, measured lines at 0.053, 0.251, 0.300, 0.883. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.13. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·D·None`; the k4 to k6 lines (None, Touch, 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·D·None` |
| Standard spectrometer detection range | 1.16 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 280 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Light, 2x Extraspection. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 2c 1d 1F 2g 1J` (Beyond, 2x Light, Life, Potential, 2x Extraspection, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 22.5 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 3rd Tier quantum of 2,586 Pz (5.2% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Divination school with aspect lean Beyond, Light, 2x Extraspection. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Divination]] |
| Affinity | [[Divination]] (D) |
| Function | [[Divination and Sensing]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Clairvoyance (3-D-L-CLR)|Clairvoyance]] (3) · [[Shannon's Coding Theorem (3-D-L-SSCT)|Shannon's Coding Theorem]] (3) · [[Arcane Eye (4-D-L-AE)|Arcane Eye]] (4) · [[Augury (2-D-L-AGR)|Augury]] (2) · [[Detect Thoughts (2-D-L-DT)|Detect Thoughts]] (2) · [[Divination (4-D-L-DVN)|Divination]] (4) · [[Find Traps (2-D-L-FT)|Find Traps]] (2) · [[Locate Animals or Plants (2-D-L-LAP)|Locate Animals or Plants]] (2).


---

## Tactical Assessment

Field interrogation, negotiation and liaison with populations whose languages are unknown.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Divination]] · [[Spell Breakdown Procedure]] · [[Parzival]]
