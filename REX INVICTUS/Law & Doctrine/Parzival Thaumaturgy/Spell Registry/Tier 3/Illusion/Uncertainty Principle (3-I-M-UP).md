---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/illusion
  - source/science-spellbook
aliases:
  - "3rd Tier Spell: Uncertainty Principle"
  - "3-I-M-UP"
  - "Uncertainty Principle (Science)"
registry_id: 3-I-M-UP
attribute_code: "3·Ill·None·None·Self·Up to 1 minute"
incantation: "Laiporse"
tier: 3
school: Illusion
affinity: I
grade: M
pz_total: 876.1
pz_quantum: 2586.2
t_e: 1.92
updated: 2026-11-16
---

**Uncertainty Principle** (`3-I-M-UP`) is a 3rd Tier working of the [[Illusion]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **876 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E 1.92 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Illusion]]
        - **Uncertainty Principle** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-I-M-UP` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Ill·None·None·Self·Up to 1 minute` |
| Incantation | *Laiporse* |
| Affinity | I (Illusion) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Illusion]] |
| Casting time | 1 Action |
| Range | Self |
| Area | single point or target |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A single coin |
| Ritual | no |
| Practitioner lineages | Wizard |

### Mechanism

Splits the caster into two equally real copies until one is observed by an attack or effect, then collapses to one at random.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Second body | `80 kg x 10 Pz/kg` | 800 |
| Body autonomy (upkeep) | `0.05 Pz/s x 60 s` | 3.0 |
| Injury avoided | `0.20 x 10` | 2.0 |
| Pattern cost | `0.01 × Q3 × (1 + 1.75)` | 71.1 |

| Quantity | Value |
|---|---|
| Effect energy | 802 Pz |
| Upkeep energy | 3.0 Pz (0.05 Pz/s) |
| **Total draw** | **876 Pz** (1,314.2 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 0.339 |
| Energy-equivalent tier T_E | 1.92 |
| Handling points | 1.75 |
| Grade score | 1.21 → M |

**Handling flags:** concentration, fragile, multi target control.

**Assumptions:** Second body 80 kg semi-living at 10 Pz/kg with summon autonomy upkeep; expected injury avoided 10 at 0.20 Pz.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Uncertainty Principle (3-I-M-UP) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Illusion | 5 | `0000000001011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Laiporse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vilaiporse* · T5: *Tilaiporse* · T6: *Rilaiporse* · T7: *Milaiporse* · T8: *Nilaiporse* · T9: *Xyilaiporse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 1→12 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#24a6bb`.

![[Uncertainty Principle (3-I-M-UP) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| School | Illusion | 0.625 | 0.949 | `#00c5ff` (512 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.929 | `#0074ff` (495 nm eq.) | source grid |
| Range | Self | 0.706 | 0.921 | `#0058ff` (488 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 2.94. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·I·None`; the k4 to k6 lines (None, Self, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·I·None` |
| Standard spectrometer detection range | 2.96 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 259 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Light, Introspection, 2x Flexibility. The working vector used by [[Recast Tension and Combination Affinity]] is `2c 1d 1F 1G 2h 1J` (2x Light, Life, Potential, Introspection, 2x Flexibility, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 146 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 3rd Tier quantum of 2,586 Pz (33.9% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Illusion school with aspect lean Light, Introspection, 2x Flexibility. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Illusion]] |
| Affinity | [[Illusion]] (I) |
| Function | [[Utility Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Pascal's Revenge (1-I-L-PSR)|Pascal's Revenge]] (1) · [[Reflection (3-A-L-RFL)|Reflection]] (3) · [[Reverb (1-I-L-RVR)|Reverb]] (1) · [[Sublimation (3-T-L-SBL)|Sublimation]] (3) · [[Synchrotron Spell (3-V-M-SSN)|Synchrotron Spell]] (3) · [[Carbon Dating (2-D-L-CDR)|Carbon Dating]] (2) · [[Magnetise (2-T-L-MGN)|Magnetise]] (2) · [[Manipulate Uncertainty (0-I-L-MU)|Manipulate Uncertainty]] (0).


---

## Tactical Assessment

Halves the chance a single strike lands on the caster and doubles their positions for a minute.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Illusion]] · [[Spell Breakdown Procedure]] · [[Parzival]]
