---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-6
  - spell/transmutation
  - source/srd
aliases:
  - "6th Tier Spell: Flesh to Stone"
  - "Flesh to Stone"
  - "6-T-L-FSE"
registry_id: 6-T-L-FSE
attribute_code: "6·Tra·None·None·60 feet·Up to 1 minute"
incantation: "Riewynse"
tier: 6
school: Transmutation
affinity: T
grade: L
pz_total: 1019.5
pz_quantum: 51944.6
t_e: 2.07
updated: 2026-11-16
---

**Flesh to Stone** (`6-T-L-FSE`) is a 6th Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **1,019 Pz** against a slot quantum of 51,945 Pz, which puts its energy-equivalent tier at T_E 2.07 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 6 Workings]]
      - [[Transmutation]]
        - **Flesh to Stone** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `6-T-L-FSE` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `6·Tra·None·None·60 feet·Up to 1 minute` |
| Incantation | *Riewynse* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 6th Tier |
| School | [[Transmutation]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | single point or target |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A pinch of lime, water, and earth |
| Ritual | no |
| Resistance check | constitution; on success: no effect |
| Practitioner lineages | Warlock, Wizard |

### Mechanism

The field converts living tissue progressively to mineral, first stiffening the body and then completing the change if the target's resistance fails repeatedly.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| petrification of 80 kg body | `3 Pz/kg * 80 kg (structured solid)` | 240 |
| progressive binding | `0.005 Pz/s = 0.005 Pz/s * 60 s` | 0.3 |
| Pattern cost | `0.01 × Q6 × (1 + 0.50)` | 779 |

| Quantity | Value |
|---|---|
| Effect energy | 240 Pz |
| Upkeep energy | 0.3 Pz (0.005 Pz/s) |
| **Total draw** | **1,019 Pz** (1,529.2 kJ) |
| Slot quantum Q6 | 51,945 Pz |
| Field gain (draw / quantum) | 0.0196 |
| Energy-equivalent tier T_E | 2.07 |
| Handling points | 0.50 |
| Grade score | -0.50 → L |

**Handling flags:** concentration, save or suck.

**Assumptions:** 80 kg target fully converted at 3 Pz/kg; binding upkeep at enchantment rate.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Flesh to Stone (6-T-L-FSE) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 6 | 6 | `0000000001101` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Riewynse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T7: *Miriewynse* · T8: *Niriewynse* · T9: *Xyiriewynse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 3→2 | 3 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#2497ff`.

![[Flesh to Stone (6-T-L-FSE) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 6 | 0.600 | 1.000 | `#00ebff` (520 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.963 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.996 | `#0074ff` (495 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 1.000 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.17): swatch `#42b9e1`, measured lines at 0.596, 0.685, 0.876. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.01. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `6·T·None`; the k4 to k6 lines (None, 60 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `6·T·None` |
| Standard spectrometer detection range | 3.19 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 2,597 Pz (0.05 × Q6) |
| Counter drawn cold (all six layers) | 5,194 Pz (0.10 × Q6) |
| Unravel after completion | 5,195 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 170 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 6th Tier quantum of 51,945 Pz (2.0% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 6th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 6 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Transformation]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Animal Shapes (8-T-M-ASM)|Animal Shapes]] (8) · [[Magic Jar (6-N-H-MJ)|Magic Jar]] (6) · [[Polymorph (4-T-L-PLY)|Polymorph]] (4) · [[Chemical Transition (3-T-L-CTE)|Chemical Transition]] (3) · [[Gaseous Form (3-T-M-GF)|Gaseous Form]] (3) · [[Shapechange (9-T-L-SHP)|Shapechange]] (9) · [[True Polymorph (9-T-L-TPU)|True Polymorph]] (9) · [[Alter Self (2-T-L-AST)|Alter Self]] (2).


---

## Tactical Assessment

Takes a single high-value target out permanently if sustained for the full minute; the result can be stored, transported or held as a hostage.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 6 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
