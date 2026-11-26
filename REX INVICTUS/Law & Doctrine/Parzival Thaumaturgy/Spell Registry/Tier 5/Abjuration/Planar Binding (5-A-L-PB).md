---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/abjuration
  - source/srd
aliases:
  - "5th Tier Spell: Planar Binding"
  - "Planar Binding"
  - "5-A-L-PB"
registry_id: 5-A-L-PB
attribute_code: "5·Abj·None·None·60 feet·24 hours"
incantation: "Tawynl"
tier: 5
school: Abjuration
affinity: A
grade: L
pz_total: 767.4
pz_quantum: 19109.4
t_e: 1.79
updated: 2026-11-16
---

**Planar Binding** (`5-A-L-PB`) is a 5th Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **767 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 1.79 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Abjuration]]
        - **Planar Binding** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-A-L-PB` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Abj·None·None·60 feet·24 hours` |
| Incantation | *Tawynl* |
| Affinity | A (Abjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Abjuration]] |
| Casting time | 1 hour |
| Range | 60 feet |
| Area | single point or target |
| Duration | 24 hours |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A jewel worth at least 1,000 gp, which the spell consumes |
| Ritual | no |
| Resistance check | presence; on success: no effect |
| Practitioner lineages | Bard, Cleric, Druid, Wizard |

### Mechanism

A compulsion lattice is fixed onto an already present extraplanar entity, overriding its intent with the caster's instructions for one day and extending any summoning that holds it here.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| compulsion imprint at casting, instant information | `1` | 1.0 |
| [upkeep] enchantment hold on 1 creature, 24 h | `0.005*86400` | 432 |
| Pattern cost | `0.01 × Q5 × (1 + 0.75)` | 334 |

| Quantity | Value |
|---|---|
| Effect energy | 1.0 Pz |
| Upkeep energy | 432 Pz (0.005 Pz/s) |
| **Total draw** | **767 Pz** (1,151.1 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 0.0402 |
| Energy-equivalent tier T_E | 1.79 |
| Handling points | 0.75 |
| Grade score | -0.25 → L |

**Handling flags:** costly material, consumed material, long cast.

**Assumptions:** One bound creature; full 24 h held; standard enchantment rate; binding circle prepared separately.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Planar Binding (5-A-L-PB) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | 24 hours | 5 | `0000000001011` |

### Incantation

Spoken as **Tawynl** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Ritawynl* · T7: *Mitawynl* · T8: *Nitawynl* · T9: *Xyitawynl*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 3→10 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#58c36e`.

![[Planar Binding (5-A-L-PB) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.882 | `#ff0028` (700 nm eq.) | source grid |
| Duration | 24 hours | 0.316 | 0.983 | `#76ff00` (605 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.996 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.21): swatch `#a3be87`, measured lines at 0.007, 0.316, 0.501, 0.589. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.89. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·A·None`; the k4 to k6 lines (None, 60 feet, 24 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·A·None` |
| Standard spectrometer detection range | 2.77 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 1,997 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 128 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 5th Tier quantum of 19,109 Pz (4.0% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
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

Similar workings: [[Pauli Exclusion Principle (5-A-L-PEP)|Pauli Exclusion Principle]] (5) · [[Summon Demon Core (6-A-M-SDC)|Summon Demon Core]] (6) · [[Animate Objects (5-T-L-AO)|Animate Objects]] (5) · [[Arcane Hand (5-P-L-AH)|Arcane Hand]] (5) · [[Conjure Elemental (5-C-M-CEN)|Conjure Elemental]] (5) · [[Magic Circle (3-A-L-MC)|Magic Circle]] (3) · [[Conjure Fey (6-C-L-CFN)|Conjure Fey]] (6) · [[Conjure Magic Prism (4-C-L-CMPJ)|Conjure Magic Prism]] (4).


---

## Tactical Assessment

Converts a summoned entity into a bound guard, courier or strike asset for a full day. Hostile bound entities exploit loose orders, so instructions are drafted like legal orders of operation.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
