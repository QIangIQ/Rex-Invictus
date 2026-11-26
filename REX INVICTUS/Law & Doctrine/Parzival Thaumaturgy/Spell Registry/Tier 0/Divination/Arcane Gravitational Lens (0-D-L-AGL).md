---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-0
  - spell/divination
  - source/science-spellbook
aliases:
  - "Cantrip Spell: Arcane Gravitational Lens"
  - "0-D-L-AGL"
  - "Arcane Gravitational Lens (Science)"
registry_id: 0-D-L-AGL
attribute_code: "0·Div·None·None·15 feet·Up to 1 minute"
incantation: "Cibalse"
tier: 0
school: Divination
affinity: D
grade: L
pz_total: 1.6
pz_quantum: 128.8
t_e: -4.37
updated: 2026-11-16
---

**Arcane Gravitational Lens** (`0-D-L-AGL`) is a Cantrip (Tier 0) working of the [[Divination]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **1.6 Pz** against a slot quantum of 129 Pz, which puts its energy-equivalent tier at T_E -4.37 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 0 Workings]]
      - [[Divination]]
        - **Arcane Gravitational Lens** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `0-D-L-AGL` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `0·Div·None·None·15 feet·Up to 1 minute` |
| Incantation | *Cibalse* |
| Affinity | D (Divination) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | Cantrip (Tier 0) |
| School | [[Divination]] |
| Casting time | 1 Action |
| Range | 15 feet |
| Area | single point or target |
| Duration | Up to 1 minute (concentration) |
| Components | none |
| Ritual | no |
| Practitioner lineages | Wizard, Sorcerer, Warlock |

### Mechanism

Curves light around an opaque corner within 15 ft so the caster sees past it without extending sight range.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Light path bending (upkeep) | `divination 0.001 x (range 4.572 m /10): 0.0004572 Pz/s x 60 s` | 0.0274 |
| Pattern cost | `0.01 × Q0 × (1 + 0.25)` | 1.6 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 0.0274 Pz (0.000457 Pz/s) |
| **Total draw** | **1.6 Pz** (2.5 kJ) |
| Slot quantum Q0 | 129 Pz |
| Field gain (draw / quantum) | 0.0127 |
| Energy-equivalent tier T_E | -4.37 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** concentration.

**Assumptions:** Divination rate 0.001 Pz/s x (4.572 m / 10) held for 1 minute.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Arcane Gravitational Lens (0-D-L-AGL) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 0 | 0 | `0000000000001` |
| k2 School | Divination | 2 | `0000000000101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 15 feet | 18 | `0000000100101` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Cibalse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T1: *Sicibalse* · T2: *Hicibalse* · T3: *Licibalse* · T4: *Vicibalse* · T5: *Ticibalse* · T6: *Ricibalse* · T7: *Micibalse* · T8: *Nicibalse* · T9: *Xyicibalse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 | 1 |
| k2 School | 0→11 2→0 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 5→0 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#bc9940`.

![[Arcane Gravitational Lens (0-D-L-AGL) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 0 | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| School | Divination | 0.250 | 0.969 | `#cdff00` (625 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.791 | `#0074ff` (495 nm eq.) | source grid |
| Range | 15 feet | 0.206 | 0.979 | `#ffef00` (638 nm eq.) | RI half-step |

Relative luminosity scales with initial energy: log10(E) = 0.21. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `0·D·None`; the k4 to k6 lines (None, 15 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `0·D·None` |
| Standard spectrometer detection range | 0.13 km (r = 1 km × √(E/100 Pz)) |
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
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 0.273 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the Cantrip (Tier 0) quantum of 129 Pz (1.3% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
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

Similar workings: [[Guidance (0-D-L-GDN)|Guidance]] (0) · [[Identify Medicinal Herbs (0-D-L-IMH)|Identify Medicinal Herbs]] (0) · [[Mutual Information (0-D-L-MIT)|Mutual Information]] (0) · [[True Strike (0-D-L-TS)|True Strike]] (0) · [[Comprehend Languages (1-D-L-CL)|Comprehend Languages]] (1) · [[Detect Evil and Good (1-D-L-DEG)|Detect Evil and Good]] (1) · [[Detect Habitat (1-D-L-DH)|Detect Habitat]] (1) · [[Detect Magic (1-D-L-DMT)|Detect Magic]] (1).


---

## Tactical Assessment

Safe room clearing and corner observation without exposing a head or a camera mast.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 0 Workings]] · [[Divination]] · [[Spell Breakdown Procedure]] · [[Parzival]]
