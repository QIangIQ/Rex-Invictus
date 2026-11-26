---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/illusion
  - source/science-spellbook
aliases:
  - "3rd Tier Spell: Illusory Geodesic Curve"
  - "3-I-L-IGC"
  - "Illusory Geodesic Curve (Science)"
registry_id: 3-I-L-IGC
attribute_code: "3·Ill·None·sphere (30)·30 feet·1 hour or until dispelled"
incantation: "Lai’-Sorusinbal"
tier: 3
school: Illusion
affinity: I
grade: L
pz_total: 50.1
pz_quantum: 2586.2
t_e: -0.94
updated: 2026-11-16
---

**Illusory Geodesic Curve** (`3-I-L-IGC`) is a 3rd Tier working of the [[Illusion]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **50.1 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E -0.94 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Illusion]]
        - **Illusory Geodesic Curve** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-I-L-IGC` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Ill·None·sphere (30)·30 feet·1 hour or until dispelled` |
| Incantation | *Lai’-Sorusinbal* |
| Affinity | I (Illusion) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Illusion]] |
| Casting time | 1 Action |
| Range | 30 feet |
| Area | sphere (30) |
| Duration | 1 hour or until dispelled |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Resistance check | intellect; on success: no effect |
| Practitioner lineages | Wizard |

### Mechanism

An object projects a false curvature over 30 ft so movement toward it feels uphill and movement away is hurried.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Curvature illusion (upkeep) | `illusion rate x 3203 m^3: 0.00640512 Pz/s x 3600 s` | 23.1 |
| Perception hold, 4 creatures (upkeep) | `enchantment 0.005 x 4: 0.02 Pz/s x 60 s` | 1.2 |
| Pattern cost | `0.01 × Q3 × (1 + 0.00)` | 25.9 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 24.3 Pz (0.00674 Pz/s) |
| **Total draw** | **50.1 Pz** (75.2 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 0.0194 |
| Energy-equivalent tier T_E | -0.94 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Illusion volume 3203 m^3 for 1 hour plus enchantment on 4 affected creatures for 1 minute.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Illusory Geodesic Curve (3-I-L-IGC) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Illusion | 5 | `0000000001011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (30) | 31 | `0000000111111` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | 1 hour or until dispelled | 20 | `0000000101001` |

### Incantation

Spoken as **Lai’-Sorusinbal** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vilai’-Sorusinbal* · T5: *Tilai’-Sorusinbal* · T6: *Rilai’-Sorusinbal* · T7: *Milai’-Sorusinbal* · T8: *Nilai’-Sorusinbal* · T9: *Xyilai’-Sorusinbal*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 1→12 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 2→11 3→12 4→0 5→1 | 6 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 3→10 5→12 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#869f60`.

![[Illusory Geodesic Curve (3-I-L-IGC) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| School | Illusion | 0.625 | 0.949 | `#00c5ff` (512 nm eq.) | source grid |
| Duration | 1 hour or until dispelled | 0.079 | 0.976 | `#ff4200` (676 nm eq.) | RI half-step |
| Area | sphere (30) | 0.861 | 0.854 | `#8000ff` (442 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 1.000 | `#91ff00` (612 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 1.70. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·I·None`; the k4 to k6 lines (sphere (30), 30 feet, 1 hour or until dispelled) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·I·None` |
| Standard spectrometer detection range | 0.71 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 263 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Light, Introspection, 2x Flexibility. The working vector used by [[Recast Tension and Combination Affinity]] is `2c 1d 1F 1G 2h 1J` (2x Light, Life, Potential, Introspection, 2x Flexibility, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 8.4 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 3rd Tier quantum of 2,586 Pz (1.9% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Illusion school with aspect lean Light, Introspection, 2x Flexibility. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Illusion]] |
| Affinity | [[Illusion]] (I) |
| Function | [[Concealment and Illusion]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Major Image (3-I-L-MIJ)|Major Image]] (3) · [[Arcanist's Magic Aura (2-I-L-ASMA)|Arcanist's Magic Aura]] (2) · [[Blur (2-I-L-BLR)|Blur]] (2) · [[Cloak (2-I-L-CLK)|Cloak]] (2) · [[Greater Invisibility (4-I-L-GIE)|Greater Invisibility]] (4) · [[Hallucinatory Terrain (4-I-M-HT)|Hallucinatory Terrain]] (4) · [[Invisibility (2-I-L-INV)|Invisibility]] (2) · [[Mirror Image (2-I-L-MIR)|Mirror Image]] (2).


---

## Tactical Assessment

Slows assaults on a defended point and speeds retreats from it.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Illusion]] · [[Spell Breakdown Procedure]] · [[Parzival]]
