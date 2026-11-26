---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/divination
  - source/srd
aliases:
  - "1st Tier Spell: Comprehend Languages"
  - "Comprehend Languages"
  - "1-D-L-CL"
registry_id: 1-D-L-CL
attribute_code: "1·Div·None·None·Self·1 hour"
incantation: "Sipora"
tier: 1
school: Divination
affinity: D
grade: L
pz_total: 23.4
pz_quantum: 350.0
t_e: -1.71
updated: 2026-11-16
---

**Comprehend Languages** (`1-D-L-CL`) is a 1st Tier working of the [[Divination]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **23.4 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -1.71 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Divination]]
        - **Comprehend Languages** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-D-L-CL` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Div·None·None·Self·1 hour` |
| Incantation | *Sipora* |
| Affinity | D (Divination) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Divination]] |
| Casting time | 1 action |
| Range | Self |
| Area | single point or target |
| Duration | 1 hour |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A pinch of soot and salt |
| Ritual | yes |
| Practitioner lineages | Bard, Sorcerer, Warlock, Wizard |

### Mechanism

The caster understands the literal meaning of any spoken language heard, and written text touched, for an hour.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| instant information | `1 * 1 Pz` | 1.0 |
| translation upkeep | `0.005 Pz/s * 1 creature(s) * 3600 s` | 18.0 |
| Pattern cost | `0.01 × Q1 × (1 + 0.25)` | 4.4 |

| Quantity | Value |
|---|---|
| Effect energy | 1.0 Pz |
| Upkeep energy | 18.0 Pz (0.005 Pz/s) |
| **Total draw** | **23.4 Pz** (35.1 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.0668 |
| Energy-equivalent tier T_E | -1.71 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** ritual.

**Assumptions:** Self; 1 h.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Comprehend Languages (1-D-L-CL) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Divination | 2 | `0000000000101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | 1 hour | 0 | `0000000000001` |

### Incantation

Spoken as **Sipora** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisipora* · T3: *Lisipora* · T4: *Visipora* · T5: *Tisipora* · T6: *Risipora* · T7: *Misipora* · T8: *Nisipora* · T9: *Xyisipora*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 2→0 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 | 1 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#ba7437`.

![[Comprehend Languages (1-D-L-CL) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Divination | 0.250 | 0.989 | `#cdff00` (625 nm eq.) | source grid |
| Duration | 1 hour | 0.053 | 0.999 | `#ff1c00` (684 nm eq.) | source grid |
| Range | Self | 0.706 | 0.832 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.14): swatch `#db8257`, measured lines at 0.053, 0.101, 0.251, 0.706. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.37. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·D·None`; the k4 to k6 lines (None, Self, 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·D·None` |
| Standard spectrometer detection range | 0.48 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 38.6 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Light, 2x Extraspection. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 2c 1d 1F 2g 1J` (Beyond, 2x Light, Life, Potential, 2x Extraspection, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 3.9 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (6.7% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
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

Similar workings: [[Detect Evil and Good (1-D-L-DEG)|Detect Evil and Good]] (1) · [[Detect Habitat (1-D-L-DH)|Detect Habitat]] (1) · [[Detect Magic (1-D-L-DMT)|Detect Magic]] (1) · [[Detect Poison and Disease (1-D-L-DPD)|Detect Poison and Disease]] (1) · [[Expectation Values (1-D-L-EV)|Expectation Values]] (1) · [[Hunter's Mark (1-D-L-HSM)|Hunter's Mark]] (1) · [[Identify (1-D-L-IDN)|Identify]] (1) · [[Magic Antenna (1-D-L-MAG)|Magic Antenna]] (1).


---

## Tactical Assessment

Field translation of captured documents.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Divination]] · [[Spell Breakdown Procedure]] · [[Parzival]]
