---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/enchantment
  - source/science-spellbook
aliases:
  - "3rd Tier Spell: Fourier Transform"
  - "3-E-L-FTU"
  - "Fourier Transform (Science)"
registry_id: 3-E-L-FTU
attribute_code: "3·Enc·None·None·Touch·until used or short rest"
incantation: "Lolixbay"
tier: 3
school: Enchantment
affinity: E
grade: L
pz_total: 43.9
pz_quantum: 2586.2
t_e: -1.08
updated: 2026-11-16
---

**Fourier Transform** (`3-E-L-FTU`) is a 3rd Tier working of the [[Enchantment]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **43.9 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E -1.08 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Enchantment]]
        - **Fourier Transform** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-E-L-FTU` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Enc·None·None·Touch·until used or short rest` |
| Incantation | *Lolixbay* |
| Affinity | E (Enchantment) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Enchantment]] |
| Casting time | 1 Bonus Action |
| Range | Touch |
| Area | single point or target |
| Duration | until used or short rest |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Wizard |

### Mechanism

Lets one creature swap the count and size of a multi-die result once, reshaping its spread of outcomes.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Reciprocal-space hold (upkeep) | `enchantment rate: 0.005 Pz/s x 3600 s` | 18.0 |
| Pattern cost | `0.01 × Q3 × (1 + 0.00)` | 25.9 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 18.0 Pz (0.005 Pz/s) |
| **Total draw** | **43.9 Pz** (65.8 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 0.017 |
| Energy-equivalent tier T_E | -1.08 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Enchantment rate for up to 1 hour until used.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Fourier Transform (3-E-L-FTU) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Enchantment | 3 | `0000000000111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | until used or short rest | 26 | `0000000110101` |

### Incantation

Spoken as **Lolixbay** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vilolixbay* · T5: *Tilolixbay* · T6: *Rilolixbay* · T7: *Milolixbay* · T8: *Nilolixbay* · T9: *Xyilolixbay*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 1→12 2→0 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 2→9 4→11 5→12 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#8b8b6c`.

![[Fourier Transform (3-E-L-FTU) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| School | Enchantment | 0.375 | 0.997 | `#20ff00` (588 nm eq.) | source grid |
| Duration | until used or short rest | 0.974 | 0.797 | `#ff00df` (408 nm eq.) | RI half-step |
| Range | Touch | 0.882 | 0.844 | `#9b00ff` (435 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 1.64. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·E·None`; the k4 to k6 lines (None, Touch, until used or short rest) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·E·None` |
| Standard spectrometer detection range | 0.66 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 262 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Introspection, Flexibility, Hope. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1G 1h 1i 1J` (Within, Light, Life, Potential, Introspection, Flexibility, Hope, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 7.3 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 3rd Tier quantum of 2,586 Pz (1.7% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Enchantment school with aspect lean Within, Introspection, Flexibility, Hope. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Enchantment]] |
| Affinity | [[Enchantment]] (E) |
| Function | [[Transformation]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Arcane Redirection (3-A-L-AR)|Arcane Redirection]] (3) · [[Chemical Transition (3-T-L-CTE)|Chemical Transition]] (3) · [[Gaseous Form (3-T-M-GF)|Gaseous Form]] (3) · [[Alter Self (2-T-L-AST)|Alter Self]] (2) · [[Enlarge-Reduce (2-T-M-ERL)|Enlarge/Reduce]] (2) · [[Polymorph (4-T-L-PLY)|Polymorph]] (4) · [[Temporary Magic Prism (2-C-L-TMP)|Temporary Magic Prism]] (2) · [[Crystalise (1-T-L-CRY)|Crystalise]] (1).


---

## Tactical Assessment

Variance control on a planned action.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Enchantment]] · [[Spell Breakdown Procedure]] · [[Parzival]]
