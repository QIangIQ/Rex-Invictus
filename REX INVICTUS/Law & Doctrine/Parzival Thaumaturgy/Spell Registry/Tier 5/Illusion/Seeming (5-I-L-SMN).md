---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/illusion
  - source/srd
aliases:
  - "5th Tier Spell: Seeming"
  - "Seeming"
  - "5-I-L-SMN"
registry_id: 5-I-L-SMN
attribute_code: "5·Ill·None·None·30 feet·8 hours"
incantation: "Taiusiniy"
tier: 5
school: Illusion
affinity: I
grade: L
pz_total: 287.8
pz_quantum: 19109.4
t_e: 0.80
updated: 2026-11-16
---

**Seeming** (`5-I-L-SMN`) is a 5th Tier working of the [[Illusion]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **288 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 0.80 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Illusion]]
        - **Seeming** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-I-L-SMN` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Ill·None·None·30 feet·8 hours` |
| Incantation | *Taiusiniy* |
| Affinity | I (Illusion) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Illusion]] |
| Casting time | 1 action |
| Range | 30 feet |
| Area | single point or target |
| Duration | 8 hours |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Bard, Sorcerer, Wizard |

### Mechanism

An optical overlay is applied to many creatures, reshaping their apparent bodies and equipment for hours.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| [upkeep] illusory overlays on 10 creatures, ~2 m^3 each, 8 h | `0.002*(10*2/1000)*28800` | 1.2 |
| Pattern cost | `0.01 × Q5 × (1 + 0.50)` | 287 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 1.2 Pz (4e-05 Pz/s) |
| **Total draw** | **288 Pz** (431.7 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 0.0151 |
| Energy-equivalent tier T_E | 0.80 |
| Handling points | 0.50 |
| Grade score | -0.50 → L |

**Handling flags:** multi target control.

**Assumptions:** Ten targets; illusion envelope 2 m^3 each; light redirection treated as lossless.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Seeming (5-I-L-SMN) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Illusion | 5 | `0000000001011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | 8 hours | 8 | `0000000010001` |

### Incantation

Spoken as **Taiusiniy** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Ritaiusiniy* · T7: *Mitaiusiniy* · T8: *Nitaiusiniy* · T9: *Xyitaiusiniy*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 1→12 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 4→11 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#23f07c`.

![[Seeming (5-I-L-SMN) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| School | Illusion | 0.625 | 0.992 | `#00c5ff` (512 nm eq.) | source grid |
| Duration | 8 hours | 0.474 | 1.000 | `#00ff66` (558 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.979 | `#91ff00` (612 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.22): swatch `#7cefb4`, measured lines at 0.295, 0.474, 0.501, 0.626. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.46. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·I·None`; the k4 to k6 lines (None, 30 feet, 8 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·I·None` |
| Standard spectrometer detection range | 1.70 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 1,911 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Light, Introspection, 2x Flexibility. The working vector used by [[Recast Tension and Combination Affinity]] is `2c 1d 1F 1G 2h 1J` (2x Light, Life, Potential, Introspection, 2x Flexibility, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 48.0 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 5th Tier quantum of 19,109 Pz (1.5% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 5th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Illusion school with aspect lean Light, Introspection, 2x Flexibility. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 5 Workings]] |
| School | [[Illusion]] |
| Affinity | [[Illusion]] (I) |
| Function | [[Concealment and Illusion]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Mislead (5-I-L-MSL)|Mislead]] (5) · [[Greater Invisibility (4-I-L-GIE)|Greater Invisibility]] (4) · [[Hallucinatory Terrain (4-I-M-HT)|Hallucinatory Terrain]] (4) · [[Programmed Illusion (6-I-L-PI)|Programmed Illusion]] (6) · [[Illusory Geodesic Curve (3-I-L-IGC)|Illusory Geodesic Curve]] (3) · [[Major Image (3-I-L-MIJ)|Major Image]] (3) · [[Mirage Arcane (7-I-M-MAR)|Mirage Arcane]] (7) · [[Project Image (7-I-L-PIO)|Project Image]] (7).


---

## Tactical Assessment

Mass disguise for an infiltration team or for passing a checkpoint as another unit.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Illusion]] · [[Spell Breakdown Procedure]] · [[Parzival]]
