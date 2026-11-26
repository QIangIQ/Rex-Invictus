---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-0
  - spell/illusion
  - source/science-spellbook
aliases:
  - "Cantrip Spell: Manipulate Uncertainty"
  - "0-I-L-MU"
  - "Manipulate Uncertainty (Science)"
registry_id: 0-I-L-MU
attribute_code: "0·Ill·None·None·Self·until the end of your turn"
incantation: "Caiporbas"
tier: 0
school: Illusion
affinity: I
grade: L
pz_total: 1.3
pz_quantum: 128.8
t_e: -4.58
updated: 2026-11-16
---

**Manipulate Uncertainty** (`0-I-L-MU`) is a Cantrip (Tier 0) working of the [[Illusion]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **1.3 Pz** against a slot quantum of 129 Pz, which puts its energy-equivalent tier at T_E -4.58 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 0 Workings]]
      - [[Illusion]]
        - **Manipulate Uncertainty** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `0-I-L-MU` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `0·Ill·None·None·Self·until the end of your turn` |
| Incantation | *Caiporbas* |
| Affinity | I (Illusion) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | Cantrip (Tier 0) |
| School | [[Illusion]] |
| Casting time | 1 Bonus Action |
| Range | Self |
| Area | single point or target |
| Duration | until the end of your turn |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A game die |
| Ritual | no |
| Practitioner lineages | Wizard |

### Mechanism

Trades accuracy for impact on the caster's strikes this turn.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Probability skew (upkeep) | `enchantment rate: 0.005 Pz/s x 6 s` | 0.03 |
| Pattern cost | `0.01 × Q0 × (1 + 0.00)` | 1.3 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 0.03 Pz (0.005 Pz/s) |
| **Total draw** | **1.3 Pz** (2.0 kJ) |
| Slot quantum Q0 | 129 Pz |
| Field gain (draw / quantum) | 0.0102 |
| Energy-equivalent tier T_E | -4.58 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Self enchantment for one round.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Manipulate Uncertainty (0-I-L-MU) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 0 | 0 | `0000000000001` |
| k2 School | Illusion | 5 | `0000000001011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | until the end of your turn | 24 | `0000000110001` |

### Incantation

Spoken as **Caiporbas** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T1: *Sicaiporbas* · T2: *Hicaiporbas* · T3: *Licaiporbas* · T4: *Vicaiporbas* · T5: *Ticaiporbas* · T6: *Ricaiporbas* · T7: *Micaiporbas* · T8: *Nicaiporbas* · T9: *Xyicaiporbas*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 | 1 |
| k2 School | 0→11 1→12 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 4→11 5→12 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#8047b6`.

![[Manipulate Uncertainty (0-I-L-MU) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 0 | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| School | Illusion | 0.625 | 0.823 | `#00c5ff` (512 nm eq.) | source grid |
| Duration | until the end of your turn | 0.974 | 0.622 | `#ff00df` (408 nm eq.) | RI half-step |
| Range | Self | 0.706 | 0.779 | `#0058ff` (488 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 0.12. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `0·I·None`; the k4 to k6 lines (None, Self, until the end of your turn) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `0·I·None` |
| Standard spectrometer detection range | 0.11 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 6.4 Pz (0.05 × Q0) |
| Counter drawn cold (all six layers) | 12.9 Pz (0.10 × Q0) |
| Unravel after completion | 12.9 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Light, Introspection, 2x Flexibility. The working vector used by [[Recast Tension and Combination Affinity]] is `2c 1d 1F 1G 2h 1J` (2x Light, Life, Potential, Introspection, 2x Flexibility, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 0.22 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the Cantrip (Tier 0) quantum of 129 Pz (1.0% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at Cantrip (Tier 0) up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Illusion school with aspect lean Light, Introspection, 2x Flexibility. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 0 Workings]] |
| School | [[Illusion]] |
| Affinity | [[Illusion]] (I) |
| Function | [[Utility Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Pascal's Revenge (1-I-L-PSR)|Pascal's Revenge]] (1) · [[Reverb (1-I-L-RVR)|Reverb]] (1) · [[Aquire Funding (0-C-L-AFU)|Aquire Funding]] (0) · [[Alter Weight (1-T-L-AWT)|Alter Weight]] (1) · [[Arcane Gyroscope (1-T-L-AG)|Arcane Gyroscope]] (1) · [[Ladder Operation (1-E-L-LOD)|Ladder Operation]] (1) · [[Uncertainty Principle (3-I-M-UP)|Uncertainty Principle]] (3) · [[Vapour Deposition (1-T-L-VD)|Vapour Deposition]] (1).


---

## Tactical Assessment

Fine control of hit probability for a marksman.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 0 Workings]] · [[Illusion]] · [[Spell Breakdown Procedure]] · [[Parzival]]
