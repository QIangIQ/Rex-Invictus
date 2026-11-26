---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/abjuration
  - source/science-spellbook
aliases:
  - "4th Tier Spell: Raman Scattering"
  - "4-A-L-RSM"
  - "Raman Scattering (Science)"
registry_id: 4-A-L-RSM
attribute_code: "4·Abj·None·None·60 feet·Instantaneous"
incantation: "Vawyn"
tier: 4
school: Abjuration
affinity: A
grade: L
pz_total: 102.6
pz_quantum: 7029.9
t_e: -0.23
updated: 2026-11-16
---

**Raman Scattering** (`4-A-L-RSM`) is a 4th Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **103 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E -0.23 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Abjuration]]
        - **Raman Scattering** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-A-L-RSM` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Abj·None·None·60 feet·Instantaneous` |
| Incantation | *Vawyn* |
| Affinity | A (Abjuration) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Abjuration]] |
| Casting time | 1 reaction, which you take when you see a creature within 60 feet target you with a spell they cast. |
| Range | 60 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Wizard, Sorcerer |

### Mechanism

Absorbs a working aimed at the caster and re-emits it at its originator at half strength.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Incoming working absorbed | `28 HP x 0.7 x 0.5` | 9.8 |
| Working re-emitted at half | `0.5 x 9.8` | 4.9 |
| Pattern cost | `0.01 × Q4 × (1 + 0.25)` | 87.9 |

| Quantity | Value |
|---|---|
| Effect energy | 14.7 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **103 Pz** (153.9 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 0.0146 |
| Energy-equivalent tier T_E | -0.23 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** reaction cast.

**Assumptions:** Reference incoming 8d6 = 28 fire ray (F 0.5, 9.8 Pz) absorbed fully and returned at half.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Raman Scattering (4-A-L-RSM) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 4 | 4 | `0000000001001` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Vawyn** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T5: *Tivawyn* · T6: *Rivawyn* · T7: *Mivawyn* · T8: *Nivawyn* · T9: *Xyivawyn*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 3→2 | 2 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#7a8354`.

![[Raman Scattering (4-A-L-RSM) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.923 | `#ff0028` (700 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.923 | `#ff0028` (700 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.982 | `#00fbff` (524 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 2.01. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·A·None`; the k4 to k6 lines (None, 60 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·A·None` |
| Standard spectrometer detection range | 1.01 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 703 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 17.1 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 4th Tier quantum of 7,030 Pz (1.5% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 4th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 4 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Utility Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Reflection (3-A-L-RFL)|Reflection]] (3) · [[Moderator (2-A-L-MDR)|Moderator]] (2) · [[Enhance Potion (5-T-L-EP)|Enhance Potion]] (5) · [[Sublimation (3-T-L-SBL)|Sublimation]] (3) · [[Synchrotron Spell (3-V-M-SSN)|Synchrotron Spell]] (3) · [[Uncertainty Principle (3-I-M-UP)|Uncertainty Principle]] (3) · [[Arcane Insulation (4-A-L-AI)|Arcane Insulation]] (4) · [[Banishment (4-A-M-BNS)|Banishment]] (4).


---

## Tactical Assessment

Counter-casting shield for commanders targeted by enemy casters.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
