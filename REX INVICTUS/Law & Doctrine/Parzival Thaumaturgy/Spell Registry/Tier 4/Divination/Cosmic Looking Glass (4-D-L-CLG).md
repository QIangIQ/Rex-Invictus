---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/divination
  - source/science-spellbook
aliases:
  - "4th Tier Spell: Cosmic Looking Glass"
  - "4-D-L-CLG"
  - "Cosmic Looking Glass (Science)"
registry_id: 4-D-L-CLG
attribute_code: "4·Div·None·sphere (15)·30 feet·10 minutes"
incantation: "Vi’-Séusins"
tier: 4
school: Divination
affinity: D
grade: L
pz_total: 106.9
pz_quantum: 7029.9
t_e: -0.19
updated: 2026-11-16
---

**Cosmic Looking Glass** (`4-D-L-CLG`) is a 4th Tier working of the [[Divination]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **107 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E -0.19 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Divination]]
        - **Cosmic Looking Glass** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-D-L-CLG` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Div·None·sphere (15)·30 feet·10 minutes` |
| Incantation | *Vi’-Séusins* |
| Affinity | D (Divination) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Divination]] |
| Casting time | 1 minute |
| Range | 30 feet |
| Area | sphere (15) |
| Duration | 10 minutes |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A looking glass |
| Ritual | yes |
| Practitioner lineages | Wizard, Sorcerer, Warlock, Bard |

### Mechanism

Projects a still image of a 30 ft wide area exactly as it was at a stated past moment.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Past image retrieved | `instant info` | 1.0 |
| Still image held (upkeep) | `illusion rate x 400 m^3: 0.00080064 Pz/s x 600 s` | 0.48 |
| Pattern cost | `0.01 × Q4 × (1 + 0.50)` | 105 |

| Quantity | Value |
|---|---|
| Effect energy | 1.0 Pz |
| Upkeep energy | 0.48 Pz (0.000801 Pz/s) |
| **Total draw** | **107 Pz** (160.4 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 0.0152 |
| Energy-equivalent tier T_E | -0.19 |
| Handling points | 0.50 |
| Grade score | -0.50 → L |

**Handling flags:** ritual, long cast.

**Assumptions:** Illusion volume 400 m^3 held 10 minutes plus 1 Pz of retrieved information; the reach into the past is assumed to cost no more than ordinary divination.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Cosmic Looking Glass (4-D-L-CLG) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 4 | 4 | `0000000001001` |
| k2 School | Divination | 2 | `0000000000101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (15) | 29 | `0000000111011` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | 10 minutes | 4 | `0000000001001` |

### Incantation

Spoken as **Vi’-Séusins** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T5: *Tivi’-Séusins* · T6: *Rivi’-Séusins* · T7: *Mivi’-Séusins* · T8: *Nivi’-Séusins* · T9: *Xyivi’-Séusins*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 3→2 | 2 |
| k2 School | 0→11 2→0 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 3→12 4→0 5→1 | 5 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 3→10 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#76cf2f`.

![[Cosmic Looking Glass (4-D-L-CLG) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| School | Divination | 0.250 | 0.989 | `#cdff00` (625 nm eq.) | source grid |
| Duration | 10 minutes | 0.263 | 0.991 | `#bdff00` (621 nm eq.) | source grid |
| Area | sphere (15) | 0.806 | 0.921 | `#3400ff` (458 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.994 | `#91ff00` (612 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 2.03. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·D·None`; the k4 to k6 lines (sphere (15), 30 feet, 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·D·None` |
| Standard spectrometer detection range | 1.03 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 703 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Light, 2x Extraspection. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 2c 1d 1F 2g 1J` (Beyond, 2x Light, Life, Potential, 2x Extraspection, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 17.8 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 4th Tier quantum of 7,030 Pz (1.5% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 4th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Divination school with aspect lean Beyond, Light, 2x Extraspection. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 4 Workings]] |
| School | [[Divination]] |
| Affinity | [[Divination]] (D) |
| Function | [[Concealment and Illusion]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Greater Invisibility (4-I-L-GIE)|Greater Invisibility]] (4) · [[Hallucinatory Terrain (4-I-M-HT)|Hallucinatory Terrain]] (4) · [[Radar (2-D-L-RDR)|Radar]] (2) · [[See Invisibility (2-D-L-SIE)|See Invisibility]] (2) · [[Illusory Geodesic Curve (3-I-L-IGC)|Illusory Geodesic Curve]] (3) · [[Major Image (3-I-L-MIJ)|Major Image]] (3) · [[Mislead (5-I-L-MSL)|Mislead]] (5) · [[Nondetection (3-A-L-NND)|Nondetection]] (3).


---

## Tactical Assessment

Crime scene and battlefield reconstruction; checks what stood at a location before an attack.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Divination]] · [[Spell Breakdown Procedure]] · [[Parzival]]
