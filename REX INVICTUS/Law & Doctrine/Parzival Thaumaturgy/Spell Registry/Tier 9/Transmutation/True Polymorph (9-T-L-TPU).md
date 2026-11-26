---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-9
  - spell/transmutation
  - source/srd
aliases:
  - "9th Tier Spell: True Polymorph"
  - "True Polymorph"
  - "9-T-L-TPU"
registry_id: 9-T-L-TPU
attribute_code: "9·Tra·None·None·30 feet·Up to 1 hour"
incantation: "Xyieusinsi"
tier: 9
school: Transmutation
affinity: T
grade: L
pz_total: 66263.4
pz_quantum: 1043335.3
t_e: 6.24
updated: 2026-11-16
---

**True Polymorph** (`9-T-L-TPU`) is a 9th Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **66,263 Pz** against a slot quantum of 1.04 MPz Pz, which puts its energy-equivalent tier at T_E 6.24 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 9 Workings]]
      - [[Transmutation]]
        - **True Polymorph** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `9-T-L-TPU` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `9·Tra·None·None·30 feet·Up to 1 hour` |
| Incantation | *Xyieusinsi* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 9th Tier |
| School | [[Transmutation]] |
| Casting time | 1 action |
| Range | 30 feet |
| Area | single point or target |
| Duration | Up to 1 hour (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A drop of mercury, a dollop of gum arabic, and a wisp of smoke |
| Ritual | no |
| Practitioner lineages | Bard, Warlock, Wizard |

### Mechanism

Matter and pattern of a creature or object are rewritten into another creature or object, becoming permanent if held for a full hour.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Object restructured into Huge creature | `10 Pz/kg * 4000 kg` | 40,000 |
| Upkeep: Animation of created creature for 1 h | `0.05 Pz/s * 3600 s` | 180 |
| Pattern cost | `0.01 × Q9 × (1 + 1.50)` | 26,083 |

| Quantity | Value |
|---|---|
| Effect energy | 40,000 Pz |
| Upkeep energy | 180 Pz (0.05 Pz/s) |
| **Total draw** | **66,263 Pz** (99,395.1 kJ) |
| Slot quantum Q9 | 1.04 MPz Pz |
| Field gain (draw / quantum) | 0.0635 |
| Energy-equivalent tier T_E | 6.24 |
| Handling points | 1.50 |
| Grade score | 0.50 → L |

**Handling flags:** concentration, fragile, save or suck.

**Assumptions:** Largest case: object into a 4000 kg creature; living matter at 10 Pz/kg; permanence costed within pattern.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[True Polymorph (9-T-L-TPU) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 9 | 9 | `0000000010011` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Up to 1 hour | 12 | `0000000011001` |

### Incantation

Spoken as **Xyieusinsi** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 4→3 | 3 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 3→10 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#7768c7`.

![[True Polymorph (9-T-L-TPU) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 9 | 0.900 | 1.000 | `#b600ff` (430 nm eq.) | source grid |
| School | Transmutation | 0.875 | 1.000 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Up to 1 hour | 0.632 | 0.965 | `#00c0ff` (511 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.832 | `#91ff00` (612 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 4.82. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `9·T·None`; the k4 to k6 lines (None, 30 feet, Up to 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `9·T·None` |
| Standard spectrometer detection range | 25.74 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 52,167 Pz (0.05 × Q9) |
| Counter drawn cold (all six layers) | 104,334 Pz (0.10 × Q9) |
| Unravel after completion | 104,370 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 11,044 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 9th Tier quantum of 1.04 MPz Pz (6.4% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 9th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 9 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Transformation]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Shapechange (9-T-L-SHP)|Shapechange]] (9) · [[Animal Shapes (8-T-M-ASM)|Animal Shapes]] (8) · [[Flesh to Stone (6-T-L-FSE)|Flesh to Stone]] (6) · [[Alter Biome (9-T-X-AB)|Alter Biome]] (9) · [[Time Stop (9-T-M-TSM)|Time Stop]] (9) · [[Weave Warp (9-T-L-WWA)|Weave Warp]] (9) · [[Control Weather (8-T-H-CWT)|Control Weather]] (8) · [[Glibness (8-T-L-GLB)|Glibness]] (8).


---

## Tactical Assessment

Neutralises a commander by turning them into an inert object, or turns materiel into a loyal heavy combatant.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 9 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
