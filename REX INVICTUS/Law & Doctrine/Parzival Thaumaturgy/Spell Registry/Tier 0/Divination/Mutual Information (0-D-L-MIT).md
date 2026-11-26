---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-0
  - spell/divination
  - source/science-spellbook
aliases:
  - "Cantrip Spell: Mutual Information"
  - "0-D-L-MIT"
  - "Mutual Information (Science)"
registry_id: 0-D-L-MIT
attribute_code: "0·Div·None·None·60 feet·Instantaneous"
incantation: "Ciwyn"
tier: 0
school: Divination
affinity: D
grade: L
pz_total: 3.3
pz_quantum: 128.8
t_e: -3.67
updated: 2026-11-16
---

**Mutual Information** (`0-D-L-MIT`) is a Cantrip (Tier 0) working of the [[Divination]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **3.3 Pz** against a slot quantum of 129 Pz, which puts its energy-equivalent tier at T_E -3.67 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 0 Workings]]
      - [[Divination]]
        - **Mutual Information** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `0-D-L-MIT` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `0·Div·None·None·60 feet·Instantaneous` |
| Incantation | *Ciwyn* |
| Affinity | D (Divination) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | Cantrip (Tier 0) |
| School | [[Divination]] |
| Casting time | 1 Action |
| Range | 60 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Wizard, Sorcerer |

### Mechanism

Compares one chosen property of caster and target and tells both which is larger.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Comparison | `2 x instant info` | 2.0 |
| Pattern cost | `0.01 × Q0 × (1 + 0.00)` | 1.3 |

| Quantity | Value |
|---|---|
| Effect energy | 2.0 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **3.3 Pz** (4.9 kJ) |
| Slot quantum Q0 | 129 Pz |
| Field gain (draw / quantum) | 0.0255 |
| Energy-equivalent tier T_E | -3.67 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Instant information for two parties, 1 Pz each.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Mutual Information (0-D-L-MIT) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 0 | 0 | `0000000000001` |
| k2 School | Divination | 2 | `0000000000101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Ciwyn** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T1: *Siciwyn* · T2: *Hiciwyn* · T3: *Liciwyn* · T4: *Viciwyn* · T5: *Ticiwyn* · T6: *Riciwyn* · T7: *Miciwyn* · T8: *Niciwyn* · T9: *Xyiciwyn*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 | 1 |
| k2 School | 0→11 2→0 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#b9784d`.

![[Mutual Information (0-D-L-MIT) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 0 | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| School | Divination | 0.250 | 0.969 | `#cdff00` (625 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.841 | `#00fbff` (524 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 0.52. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `0·D·None`; the k4 to k6 lines (None, 60 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `0·D·None` |
| Standard spectrometer detection range | 0.18 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 6.4 Pz (0.05 × Q0) |
| Counter drawn cold (all six layers) | 12.9 Pz (0.10 × Q0) |
| Unravel after completion | 12.9 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Light, 2x Extraspection. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 2c 1d 1F 2g 1J` (Beyond, 2x Light, Life, Potential, 2x Extraspection, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 0.548 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the Cantrip (Tier 0) quantum of 129 Pz (2.6% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at Cantrip (Tier 0) up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Divination school with aspect lean Beyond, Light, 2x Extraspection. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 0 Workings]] |
| School | [[Divination]] |
| Affinity | [[Divination]] (D) |
| Function | [[Divination and Sensing]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Arcane Gravitational Lens (0-D-L-AGL)|Arcane Gravitational Lens]] (0) · [[Guidance (0-D-L-GDN)|Guidance]] (0) · [[Identify Medicinal Herbs (0-D-L-IMH)|Identify Medicinal Herbs]] (0) · [[True Strike (0-D-L-TS)|True Strike]] (0) · [[Comprehend Languages (1-D-L-CL)|Comprehend Languages]] (1) · [[Detect Evil and Good (1-D-L-DEG)|Detect Evil and Good]] (1) · [[Detect Habitat (1-D-L-DH)|Detect Habitat]] (1) · [[Detect Magic (1-D-L-DMT)|Detect Magic]] (1).


---

## Tactical Assessment

Rapid assessment of an opponent before engagement.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 0 Workings]] · [[Divination]] · [[Spell Breakdown Procedure]] · [[Parzival]]
