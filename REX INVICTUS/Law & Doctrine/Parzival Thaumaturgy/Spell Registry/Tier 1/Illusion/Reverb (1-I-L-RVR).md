---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/illusion
  - source/science-spellbook
aliases:
  - "1st Tier Spell: Reverb"
  - "1-I-L-RVR"
  - "Reverb (Science)"
registry_id: 1-I-L-RVR
attribute_code: "1·Ill·None·sphere (120)·Touch·10 minutes"
incantation: "Sai’-Seilixs"
tier: 1
school: Illusion
affinity: I
grade: L
pz_total: 3.5
pz_quantum: 350.0
t_e: -3.59
updated: 2026-11-16
---

**Reverb** (`1-I-L-RVR`) is a 1st Tier working of the [[Illusion]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **3.5 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -3.59 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Illusion]]
        - **Reverb** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-I-L-RVR` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Ill·None·sphere (120)·Touch·10 minutes` |
| Incantation | *Sai’-Seilixs* |
| Affinity | I (Illusion) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Illusion]] |
| Casting time | 1 Action |
| Range | Touch |
| Area | sphere (120) |
| Duration | 10 minutes |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A hollow shell |
| Ritual | no |
| Practitioner lineages | Wizard, Sorcerer, Warlock, Bard |

### Mechanism

Carries one creature's voice clearly through an indoor space or to everyone within 120 ft outdoors.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Voice carried (upkeep) | `0.1 W x 600 s = 60 J / 1500` | 0.04 |
| Pattern cost | `0.01 × Q1 × (1 + 0.00)` | 3.5 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 0.04 Pz (6.7e-05 Pz/s) |
| **Total draw** | **3.5 Pz** (5.3 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.0101 |
| Energy-equivalent tier T_E | -3.59 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Acoustic output 0.1 W for 10 minutes.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Reverb (1-I-L-RVR) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Illusion | 5 | `0000000001011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (120) | 39 | `0000001001111` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | 10 minutes | 4 | `0000000001001` |

### Incantation

Spoken as **Sai’-Seilixs** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisai’-Seilixs* · T3: *Lisai’-Seilixs* · T4: *Visai’-Seilixs* · T5: *Tisai’-Seilixs* · T6: *Risai’-Seilixs* · T7: *Misai’-Seilixs* · T8: *Nisai’-Seilixs* · T9: *Xyisai’-Seilixs*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 1→12 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 2→11 3→12 6→2 | 5 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 3→10 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#84758b`.

![[Reverb (1-I-L-RVR) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Illusion | 0.625 | 0.871 | `#00c5ff` (512 nm eq.) | source grid |
| Duration | 10 minutes | 0.263 | 0.987 | `#bdff00` (621 nm eq.) | source grid |
| Area | sphere (120) | 0.792 | 0.787 | `#1e00ff` (462 nm eq.) | RI half-step |
| Range | Touch | 0.882 | 0.736 | `#9b00ff` (435 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 0.55. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·I·None`; the k4 to k6 lines (sphere (120), Touch, 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·I·None` |
| Standard spectrometer detection range | 0.19 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.0 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Light, Introspection, 2x Flexibility. The working vector used by [[Recast Tension and Combination Affinity]] is `2c 1d 1F 1G 2h 1J` (2x Light, Life, Potential, Introspection, 2x Flexibility, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 0.59 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (1.0% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Illusion school with aspect lean Light, Introspection, 2x Flexibility. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Illusion]] |
| Affinity | [[Illusion]] (I) |
| Function | [[Utility Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Pascal's Revenge (1-I-L-PSR)|Pascal's Revenge]] (1) · [[Manipulate Uncertainty (0-I-L-MU)|Manipulate Uncertainty]] (0) · [[Alter Weight (1-T-L-AWT)|Alter Weight]] (1) · [[Arcane Gyroscope (1-T-L-AG)|Arcane Gyroscope]] (1) · [[Ladder Operation (1-E-L-LOD)|Ladder Operation]] (1) · [[Uncertainty Principle (3-I-M-UP)|Uncertainty Principle]] (3) · [[Vapour Deposition (1-T-L-VD)|Vapour Deposition]] (1) · [[Volcanum (1-D-L-VLC)|Volcanum]] (1).


---

## Tactical Assessment

Battlefield address without equipment.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Illusion]] · [[Spell Breakdown Procedure]] · [[Parzival]]
