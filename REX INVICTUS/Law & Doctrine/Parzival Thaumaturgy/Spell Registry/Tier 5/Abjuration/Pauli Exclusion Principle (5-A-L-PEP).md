---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/abjuration
  - source/science-spellbook
aliases:
  - "5th Tier Spell: Pauli Exclusion Principle"
  - "5-A-L-PEP"
  - "Pauli Exclusion Principle (Science)"
registry_id: 5-A-L-PEP
attribute_code: "5·Abj·None·sphere (15)·Self·Up to 10 minutes"
incantation: "Ta’-Séporly"
tier: 5
school: Abjuration
affinity: A
grade: L
pz_total: 264.6
pz_quantum: 19109.4
t_e: 0.72
updated: 2026-11-16
---

**Pauli Exclusion Principle** (`5-A-L-PEP`) is a 5th Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **265 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 0.72 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Abjuration]]
        - **Pauli Exclusion Principle** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-A-L-PEP` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Abj·None·sphere (15)·Self·Up to 10 minutes` |
| Incantation | *Ta’-Séporly* |
| Affinity | A (Abjuration) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Abjuration]] |
| Casting time | 1 Action |
| Range | Self |
| Area | sphere (15) |
| Duration | Up to 10 minutes (concentration) |
| Components | somatic (glyph kata) |
| Ritual | no |
| Resistance check | strength; on success: no effect |
| Practitioner lineages | Wizard, Cleric |

### Mechanism

A white field 15 ft around the caster refuses to share space, shoving intruders to its edge and resisting entry.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Expulsions (upkeep) | `20 x 0.5 x 80 kg x 9.81 x 3 m = 2.354e+04 J / 1500` | 15.7 |
| Resisted entry (upkeep) | `10 x 500 N x 3 m = 1.5e+04 J / 1500` | 10.0 |
| Pattern cost | `0.01 × Q5 × (1 + 0.25)` | 239 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 25.7 Pz (0.0428 Pz/s) |
| **Total draw** | **265 Pz** (396.8 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 0.0138 |
| Energy-equivalent tier T_E | 0.72 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** concentration.

**Assumptions:** Twenty expulsions of an 80 kg creature over 3 m against friction (mu 0.5) plus resisted entry 500 N x 3 m ten times; real degeneracy pressure is irrelevant at this scale.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Pauli Exclusion Principle (5-A-L-PEP) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (15) | 29 | `0000000111011` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Up to 10 minutes | 15 | `0000000011111` |

### Incantation

Spoken as **Ta’-Séporly** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Rita’-Séporly* · T7: *Mita’-Séporly* · T8: *Nita’-Séporly* · T9: *Xyita’-Séporly*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 3→12 4→0 5→1 | 5 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 2→9 3→10 4→11 | 5 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#3f47be`.

![[Pauli Exclusion Principle (5-A-L-PEP) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.882 | `#ff0028` (700 nm eq.) | source grid |
| Duration | Up to 10 minutes | 0.789 | 0.959 | `#1e00ff` (463 nm eq.) | source grid |
| Area | sphere (15) | 0.806 | 0.954 | `#3400ff` (458 nm eq.) | source grid |
| Range | Self | 0.706 | 0.979 | `#0058ff` (488 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 2.42. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·A·None`; the k4 to k6 lines (sphere (15), Self, Up to 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·A·None` |
| Standard spectrometer detection range | 1.63 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 1,916 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 44.1 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 5th Tier quantum of 19,109 Pz (1.4% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 5th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 5 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Summoning and Conjured Creatures]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Planar Binding (5-A-L-PB)|Planar Binding]] (5) · [[Summon Demon Core (6-A-M-SDC)|Summon Demon Core]] (6) · [[Animate Objects (5-T-L-AO)|Animate Objects]] (5) · [[Arcane Hand (5-P-L-AH)|Arcane Hand]] (5) · [[Conjure Elemental (5-C-M-CEN)|Conjure Elemental]] (5) · [[Magic Circle (3-A-L-MC)|Magic Circle]] (3) · [[Conjure Fey (6-C-L-CFN)|Conjure Fey]] (6) · [[Conjure Magic Prism (4-C-L-CMPJ)|Conjure Magic Prism]] (4).


---

## Tactical Assessment

Personal perimeter for a caster or officer against boarding and melee rushes.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
