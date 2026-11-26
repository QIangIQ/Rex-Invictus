---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/evocation
  - source/science-spellbook
aliases:
  - "3rd Tier Spell: Synchrotron Spell"
  - "3-V-M-SSN"
  - "Synchrotron Spell (Science)"
registry_id: 3-V-M-SSN
attribute_code: "3·Evo·None·None·Self·Up to 1 round"
incantation: "Lupores"
tier: 3
school: Evocation
affinity: V
grade: M
pz_total: 719.4
pz_quantum: 2586.2
t_e: 1.72
updated: 2026-11-16
---

**Synchrotron Spell** (`3-V-M-SSN`) is a 3rd Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **719 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E 1.72 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Evocation]]
        - **Synchrotron Spell** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-V-M-SSN` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Evo·None·None·Self·Up to 1 round` |
| Incantation | *Lupores* |
| Affinity | V (Evocation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Evocation]] |
| Casting time | 1 reaction, which you take immediately after you cast a spell that requires a spell attack or a saving throw on your turn |
| Range | Self |
| Area | single point or target |
| Duration | Up to 1 round (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A circular tube |
| Ritual | no |
| Practitioner lineages | Wizard |

### Mechanism

Holds a just-cast working in orbit around the caster for a round, charging its aim before release.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Containment loss (upkeep) | `0.05 x 13075` | 654 |
| Aim refinement | `instant info` | 1.0 |
| Pattern cost | `0.01 × Q3 × (1 + 1.50)` | 64.7 |

| Quantity | Value |
|---|---|
| Effect energy | 1.0 Pz |
| Upkeep energy | 654 Pz (109 Pz/s) |
| **Total draw** | **719 Pz** (1,079.1 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 0.278 |
| Energy-equivalent tier T_E | 1.72 |
| Handling points | 1.50 |
| Grade score | 0.86 → M |

**Handling flags:** concentration, reaction cast, fragile.

**Assumptions:** Reference held working the 8d6 fire 20 ft sphere (13075 Pz); containment loss 5% for the round; the aim gain is information (1 Pz).

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Synchrotron Spell (3-V-M-SSN) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Up to 1 round | 14 | `0000000011101` |

### Incantation

Spoken as **Lupores** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vilupores* · T5: *Tilupores* · T6: *Rilupores* · T7: *Milupores* · T8: *Nilupores* · T9: *Xyilupores*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 2→9 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#24a49e`.

![[Synchrotron Spell (3-V-M-SSN) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.980 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Up to 1 round | 0.737 | 0.909 | `#002dff` (479 nm eq.) | source grid |
| Range | Self | 0.706 | 0.921 | `#0058ff` (488 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 2.86. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·V·None`; the k4 to k6 lines (None, Self, Up to 1 round) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·V·None` |
| Standard spectrometer detection range | 2.68 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 389 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1b 1c 1d 1f` (Heat, Light, Life, Energy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 120 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 3rd Tier quantum of 2,586 Pz (27.8% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Utility Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Universal Expansion (2-V-L-UE)|Universal Expansion]] (2) · [[Reflection (3-A-L-RFL)|Reflection]] (3) · [[Sublimation (3-T-L-SBL)|Sublimation]] (3) · [[Uncertainty Principle (3-I-M-UP)|Uncertainty Principle]] (3) · [[Carbon Dating (2-D-L-CDR)|Carbon Dating]] (2) · [[Magnetise (2-T-L-MGN)|Magnetise]] (2) · [[Moderator (2-A-L-MDR)|Moderator]] (2) · [[Momentum Transfer (2-T-L-MT)|Momentum Transfer]] (2).


---

## Tactical Assessment

Turns a routine strike into a near-certain hit at the cost of a round's delay.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
