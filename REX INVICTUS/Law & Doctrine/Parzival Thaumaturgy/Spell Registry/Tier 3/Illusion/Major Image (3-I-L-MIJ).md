---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/illusion
  - source/srd
aliases:
  - "3rd Tier Spell: Major Image"
  - "Major Image"
  - "3-I-L-MIJ"
registry_id: 3-I-L-MIJ
attribute_code: "3·Ill·None·None·120 feet·Up to 10 minutes"
incantation: "Laimully"
tier: 3
school: Illusion
affinity: I
grade: L
pz_total: 93.0
pz_quantum: 2586.2
t_e: -0.33
updated: 2026-11-16
---

**Major Image** (`3-I-L-MIJ`) is a 3rd Tier working of the [[Illusion]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **93.0 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E -0.33 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Illusion]]
        - **Major Image** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-I-L-MIJ` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Ill·None·None·120 feet·Up to 10 minutes` |
| Incantation | *Laimully* |
| Affinity | I (Illusion) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Illusion]] |
| Casting time | 1 action |
| Range | 120 feet |
| Area | single point or target |
| Duration | Up to 10 minutes (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A bit of fleece |
| Ritual | no |
| Practitioner lineages | Bard, Sorcerer, Warlock, Wizard |

### Mechanism

The field projects a mobile illusion up to a 20 ft cube with matching sound, smell and mild temperature. It carries no substance and anything passing through reveals it.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Illusion volume, 20 ft cube (upkeep) | `0.002 Pz/s * (226.5 m^3/1000) * 600 s` | 0.272 |
| Sound simulation (upkeep) | `1 W / 1500 * 600 s` | 0.4 |
| Thermal simulation (upkeep) | `100 W / 1500 * 600 s` | 40.0 |
| Visible light output (upkeep) | `50 W / 1500 * 600 s` | 20.0 |
| Pattern cost | `0.01 × Q3 × (1 + 0.25)` | 32.3 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 60.7 Pz (0.101 Pz/s) |
| **Total draw** | **93.0 Pz** (139.5 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 0.036 |
| Energy-equivalent tier T_E | -0.33 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** concentration.

**Assumptions:** 20 ft cube for 10 minutes; 1 W sound, 100 W simulated warmth, 50 W light.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Major Image (3-I-L-MIJ) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Illusion | 5 | `0000000001011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 120 feet | 3 | `0000000000111` |
| k6 Duration | Up to 10 minutes | 15 | `0000000011111` |

### Incantation

Spoken as **Laimully** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vilaimully* · T5: *Tilaimully* · T6: *Rilaimully* · T7: *Milaimully* · T8: *Nilaimully* · T9: *Xyilaimully*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 1→12 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 | 3 |
| k6 Duration | 0→7 1→8 2→9 3→10 4→11 | 5 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#6da77a`.

![[Major Image (3-I-L-MIJ) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| School | Illusion | 0.625 | 0.949 | `#00c5ff` (512 nm eq.) | source grid |
| Duration | Up to 10 minutes | 0.789 | 0.887 | `#1e00ff` (463 nm eq.) | source grid |
| Range | 120 feet | 0.176 | 0.992 | `#ffc900` (647 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.20): swatch `#8fc5a1`, measured lines at 0.177, 0.300, 0.626, 0.790. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.97. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·I·None`; the k4 to k6 lines (None, 120 feet, Up to 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·I·None` |
| Standard spectrometer detection range | 0.96 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 271 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Light, Introspection, 2x Flexibility. The working vector used by [[Recast Tension and Combination Affinity]] is `2c 1d 1F 1G 2h 1J` (2x Light, Life, Potential, Introspection, 2x Flexibility, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 15.5 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 3rd Tier quantum of 2,586 Pz (3.6% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Illusion school with aspect lean Light, Introspection, 2x Flexibility. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Illusion]] |
| Affinity | [[Illusion]] (I) |
| Function | [[Concealment and Illusion]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Illusory Geodesic Curve (3-I-L-IGC)|Illusory Geodesic Curve]] (3) · [[Arcanist's Magic Aura (2-I-L-ASMA)|Arcanist's Magic Aura]] (2) · [[Blur (2-I-L-BLR)|Blur]] (2) · [[Cloak (2-I-L-CLK)|Cloak]] (2) · [[Greater Invisibility (4-I-L-GIE)|Greater Invisibility]] (4) · [[Hallucinatory Terrain (4-I-M-HT)|Hallucinatory Terrain]] (4) · [[Invisibility (2-I-L-INV)|Invisibility]] (2) · [[Mirror Image (2-I-L-MIR)|Mirror Image]] (2).


---

## Tactical Assessment

Creates decoy vehicles, false positions and phantom troops to draw fire or mislead observers. Physical probing or careful inspection exposes it.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Illusion]] · [[Spell Breakdown Procedure]] · [[Parzival]]
