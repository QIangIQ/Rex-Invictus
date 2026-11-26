---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-9
  - spell/transmutation
  - source/science-spellbook
aliases:
  - "9th Tier Spell: Weave Warp"
  - "9-T-L-WWA"
  - "Weave Warp (Science)"
registry_id: 9-T-L-WWA
attribute_code: "9·Tra·None·sphere (300)·Self·1 hour"
incantation: "Xyie’-Soapora"
tier: 9
school: Transmutation
affinity: T
grade: L
pz_total: 1056557.0
pz_quantum: 1043335.3
t_e: 9.01
updated: 2026-11-16
---

**Weave Warp** (`9-T-L-WWA`) is a 9th Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **1.06 MPz Pz** against a slot quantum of 1.04 MPz Pz, which puts its energy-equivalent tier at T_E 9.01 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 9 Workings]]
      - [[Transmutation]]
        - **Weave Warp** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `9-T-L-WWA` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `9·Tra·None·sphere (300)·Self·1 hour` |
| Incantation | *Xyie’-Soapora* |
| Affinity | T (Transmutation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 9th Tier |
| School | [[Transmutation]] |
| Casting time | 1 Action |
| Range | Self |
| Area | sphere (300) |
| Duration | 1 hour |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A piece of thread |
| Ritual | no |
| Resistance check | constitution; on success: no effect |
| Practitioner lineages | Wizard |

### Mechanism

The caster dumps their full field return back into the ambient field, scrambling every caster's access within 300 ft for an hour.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Field return reinjected | `Q9 = 350 x e^8` | 1.04 MPz |
| Access suppression, 10 casters (upkeep) | `enchantment 0.005 x 10: 0.05 Pz/s x 3600 s` | 180 |
| Pattern cost | `0.01 × Q9 × (1 + 0.25)` | 13,042 |

| Quantity | Value |
|---|---|
| Effect energy | 1.04 MPz Pz |
| Upkeep energy | 180 Pz (0.05 Pz/s) |
| **Total draw** | **1.06 MPz Pz** (1,584,835.5 kJ) |
| Slot quantum Q9 | 1.04 MPz Pz |
| Field gain (draw / quantum) | 1.01 |
| Energy-equivalent tier T_E | 9.01 |
| Handling points | 0.25 |
| Grade score | 0.26 → L |

**Handling flags:** save or suck.

**Assumptions:** Text says the caster exerts all they can, taken as one full tier-9 field return (1,043,203 Pz); suppression of 10 casters at the enchantment rate for 1 hour.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Weave Warp (9-T-L-WWA) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 9 | 9 | `0000000010011` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (300) | 41 | `0000001010011` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | 1 hour | 0 | `0000000000001` |

### Incantation

Spoken as **Xyie’-Soapora** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 4→3 | 3 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 4→0 6→2 | 4 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 | 1 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#8d16d8`.

![[Weave Warp (9-T-L-WWA) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 9 | 0.900 | 1.000 | `#b600ff` (430 nm eq.) | source grid |
| School | Transmutation | 0.875 | 1.000 | `#9600ff` (438 nm eq.) | source grid |
| Duration | 1 hour | 0.053 | 0.698 | `#ff1c00` (684 nm eq.) | source grid |
| Area | sphere (300) | 0.875 | 1.000 | `#9600ff` (438 nm eq.) | RI half-step |
| Range | Self | 0.706 | 0.981 | `#0058ff` (488 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 6.02. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `9·T·None`; the k4 to k6 lines (sphere (300), Self, 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `9·T·None` |
| Standard spectrometer detection range | 102.79 km (r = 1 km × √(E/100 Pz)) |
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
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 176,093 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 9th Tier quantum of 1.04 MPz Pz (101.3% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 9th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 9 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Utility Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Multiverse Exploration (9-D-L-MEL)|Multiverse Exploration]] (9) · [[Create Chimera (6-T-L-CCE)|Create Chimera]] (6) · [[Alter Biome (9-T-X-AB)|Alter Biome]] (9) · [[Enhance Potion (5-T-L-EP)|Enhance Potion]] (5) · [[Shapechange (9-T-L-SHP)|Shapechange]] (9) · [[Time Stop (9-T-M-TSM)|Time Stop]] (9) · [[True Polymorph (9-T-L-TPU)|True Polymorph]] (9) · [[Animal Shapes (8-T-M-ASM)|Animal Shapes]] (8).


---

## Tactical Assessment

Strategic counter-magic: grounds enemy casters around a position, including one's own.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 9 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
