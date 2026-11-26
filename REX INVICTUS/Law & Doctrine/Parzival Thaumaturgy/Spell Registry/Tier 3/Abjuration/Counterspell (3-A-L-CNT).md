---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/abjuration
  - source/srd
aliases:
  - "3rd Tier Spell: Counterspell"
  - "Counterspell"
  - "3-A-L-CNT"
registry_id: 3-A-L-CNT
attribute_code: "3·Abj·None·None·60 feet·Instantaneous"
incantation: "Lawyn"
tier: 3
school: Abjuration
affinity: A
grade: L
pz_total: 59.2
pz_quantum: 2586.2
t_e: -0.78
updated: 2026-11-16
---

**Counterspell** (`3-A-L-CNT`) is a 3rd Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **59.2 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E -0.78 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Abjuration]]
        - **Counterspell** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-A-L-CNT` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Abj·None·None·60 feet·Instantaneous` |
| Incantation | *Lawyn* |
| Affinity | A (Abjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Abjuration]] |
| Casting time | 1 reaction |
| Range | 60 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Sorcerer, Warlock, Wizard |

### Mechanism

The caster injects a counter-phase field into another working while it is still forming, collapsing patterns up to the third tier outright and contesting stronger ones.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| counter-phase disruption of a tier-3 pattern | `0.01*Q(3)` | 25.9 |
| target pattern recognition (instant info) | `1` | 1.0 |
| Pattern cost | `0.01 × Q3 × (1 + 0.25)` | 32.3 |

| Quantity | Value |
|---|---|
| Effect energy | 26.9 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **59.2 Pz** (88.8 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 0.0229 |
| Energy-equivalent tier T_E | -0.78 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** reaction cast.

**Assumptions:** Disrupting energy equals the target pattern-holding cost 0.01*Q3; stronger targets resolved by a contest with no extra energy modeled.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Counterspell (3-A-L-CNT) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Lawyn** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vilawyn* · T5: *Tilawyn* · T6: *Rilawyn* · T7: *Milawyn* · T8: *Nilawyn* · T9: *Xyilawyn*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#a28052`.

![[Counterspell (3-A-L-CNT) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.956 | `#ff0028` (700 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.956 | `#ff0028` (700 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.959 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.15): swatch `#ce8a5d`, measured lines at 0.006, 0.301, 0.589. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.77. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·A·None`; the k4 to k6 lines (None, 60 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·A·None` |
| Standard spectrometer detection range | 0.77 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 259 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 9.9 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 3rd Tier quantum of 2,586 Pz (2.3% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Negation and Counterspell]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Dispel Magic (3-A-L-DM)|Dispel Magic]] (3) · [[Nondetection (3-A-L-NND)|Nondetection]] (3) · [[Remove Curse (3-A-L-RC)|Remove Curse]] (3) · [[Arcane Insulation (4-A-L-AI)|Arcane Insulation]] (4) · [[Arcane Lock (2-A-L-AL)|Arcane Lock]] (2) · [[Banishment (4-A-M-BNS)|Banishment]] (4) · [[Private Sanctum (4-A-L-PSI)|Private Sanctum]] (4) · [[Antilife Shell (5-A-L-ASI)|Antilife Shell]] (5).


---

## Tactical Assessment

The standard reactive defence in caster duels and against field artillery; it forces opponents to layer workings or saturate defenders.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
