---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/divination
  - source/science-spellbook
aliases:
  - "1st Tier Spell: Magic Antenna"
  - "1-D-L-MAG"
  - "Magic Antenna (Science)"
registry_id: 1-D-L-MAG
attribute_code: "1·Div·None·sphere (15)·15 feet·Up to 1 hour"
incantation: "Si’-Sébalsi"
tier: 1
school: Divination
affinity: D
grade: L
pz_total: 7.0
pz_quantum: 350.0
t_e: -2.91
updated: 2026-11-16
---

**Magic Antenna** (`1-D-L-MAG`) is a 1st Tier working of the [[Divination]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **7.0 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -2.91 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Divination]]
        - **Magic Antenna** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-D-L-MAG` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Div·None·sphere (15)·15 feet·Up to 1 hour` |
| Incantation | *Si’-Sébalsi* |
| Affinity | D (Divination) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Divination]] |
| Casting time | 1 Action |
| Range | 15 feet |
| Area | sphere (15) |
| Duration | Up to 1 hour (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A small metal rod |
| Ritual | no |
| Practitioner lineages | Wizard, Sorcerer |

### Mechanism

Tunes the caster to non-visual arcane messages sent or received within 15 ft and allows them to be read.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Listening field (upkeep) | `divination 0.001 x (4.572/10): 0.0004572 Pz/s x 3600 s` | 1.6 |
| Message decoded | `instant info` | 1.0 |
| Pattern cost | `0.01 × Q1 × (1 + 0.25)` | 4.4 |

| Quantity | Value |
|---|---|
| Effect energy | 1.0 Pz |
| Upkeep energy | 1.6 Pz (0.000457 Pz/s) |
| **Total draw** | **7.0 Pz** (10.5 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.0201 |
| Energy-equivalent tier T_E | -2.91 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** concentration.

**Assumptions:** Divination rate for 4.572 m held 1 hour plus 1 Pz to read one message.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Magic Antenna (1-D-L-MAG) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Divination | 2 | `0000000000101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (15) | 29 | `0000000111011` |
| k5 Range | 15 feet | 18 | `0000000100101` |
| k6 Duration | Up to 1 hour | 12 | `0000000011001` |

### Incantation

Spoken as **Si’-Sébalsi** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisi’-Sébalsi* · T3: *Lisi’-Sébalsi* · T4: *Visi’-Sébalsi* · T5: *Tisi’-Sébalsi* · T6: *Risi’-Sébalsi* · T7: *Misi’-Sébalsi* · T8: *Nisi’-Sébalsi* · T9: *Xyisi’-Sébalsi*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 2→0 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 3→12 4→0 5→1 | 5 |
| k5 Range | 0→8 2→10 5→0 | 3 |
| k6 Duration | 0→7 3→10 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#a2a15a`.

![[Magic Antenna (1-D-L-MAG) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Divination | 0.250 | 0.989 | `#cdff00` (625 nm eq.) | source grid |
| Duration | Up to 1 hour | 0.632 | 0.868 | `#00c0ff` (511 nm eq.) | source grid |
| Area | sphere (15) | 0.806 | 0.780 | `#3400ff` (458 nm eq.) | source grid |
| Range | 15 feet | 0.206 | 0.994 | `#ffef00` (638 nm eq.) | RI half-step |

Relative luminosity scales with initial energy: log10(E) = 0.85. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·D·None`; the k4 to k6 lines (sphere (15), 15 feet, Up to 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·D·None` |
| Standard spectrometer detection range | 0.26 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.3 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Light, 2x Extraspection. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 2c 1d 1F 2g 1J` (Beyond, 2x Light, Life, Potential, 2x Extraspection, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1.2 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (2.0% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Divination school with aspect lean Beyond, Light, 2x Extraspection. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Divination]] |
| Affinity | [[Divination]] (D) |
| Function | [[Divination and Sensing]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Comprehend Languages (1-D-L-CL)|Comprehend Languages]] (1) · [[Detect Evil and Good (1-D-L-DEG)|Detect Evil and Good]] (1) · [[Detect Habitat (1-D-L-DH)|Detect Habitat]] (1) · [[Detect Magic (1-D-L-DMT)|Detect Magic]] (1) · [[Detect Poison and Disease (1-D-L-DPD)|Detect Poison and Disease]] (1) · [[Expectation Values (1-D-L-EV)|Expectation Values]] (1) · [[Hunter's Mark (1-D-L-HSM)|Hunter's Mark]] (1) · [[Identify (1-D-L-IDN)|Identify]] (1).


---

## Tactical Assessment

Signals intelligence against arcane communications at close range.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Divination]] · [[Spell Breakdown Procedure]] · [[Parzival]]
