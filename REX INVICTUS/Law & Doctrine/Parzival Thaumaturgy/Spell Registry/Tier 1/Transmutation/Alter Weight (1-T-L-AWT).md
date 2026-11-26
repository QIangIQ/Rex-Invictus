---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/transmutation
  - source/science-spellbook
aliases:
  - "1st Tier Spell: Alter Weight"
  - "1-T-L-AWT"
  - "Alter Weight (Science)"
registry_id: 1-T-L-AWT
attribute_code: "1·Tra·None·None·30 feet·Up to 1 hour"
incantation: "Sieusinsi"
tier: 1
school: Transmutation
affinity: T
grade: L
pz_total: 223.8
pz_quantum: 350.0
t_e: 0.55
updated: 2026-11-16
---

**Alter Weight** (`1-T-L-AWT`) is a 1st Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **224 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E 0.55 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Transmutation]]
        - **Alter Weight** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-T-L-AWT` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Tra·None·None·30 feet·Up to 1 hour` |
| Incantation | *Sieusinsi* |
| Affinity | T (Transmutation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Transmutation]] |
| Casting time | 1 Action |
| Range | 30 feet |
| Area | single point or target |
| Duration | Up to 1 hour (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A scale of any size |
| Ritual | no |
| Resistance check | strength; on success: no effect |
| Practitioner lineages | Wizard, Sorcerer, Bard, Druid |

### Mechanism

Scales the effective weight of an object up to the size of a 30 ft cube by 2^n, with n from 1 to 4, for as long as the caster holds the pattern.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Weight change held (upkeep) | `0.02 x 100 kg x 9.81 x 4.66 x 3600 s / 1500` | 219 |
| Pattern cost | `0.01 × Q1 × (1 + 0.25)` | 4.4 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 219 Pz (0.061 Pz/s) |
| **Total draw** | **224 Pz** (335.7 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.639 |
| Energy-equivalent tier T_E | 0.55 |
| Handling points | 0.25 |
| Grade score | 0.03 → L |

**Handling flags:** concentration.

**Assumptions:** Object 100 kg; average 2.5 doublings (factor 5.66, extra 4.66 times weight); holding the extra load costs the hover rate 0.02*m*g on the added weight for 1 hour.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Alter Weight (1-T-L-AWT) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Up to 1 hour | 12 | `0000000011001` |

### Incantation

Spoken as **Sieusinsi** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisieusinsi* · T3: *Lisieusinsi* · T4: *Visieusinsi* · T5: *Tisieusinsi* · T6: *Risieusinsi* · T7: *Misieusinsi* · T8: *Nisieusinsi* · T9: *Xyisieusinsi*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 3→10 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#8d8e72`.

![[Alter Weight (1-T-L-AWT) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.741 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Up to 1 hour | 0.632 | 0.868 | `#00c0ff` (511 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.981 | `#91ff00` (612 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 2.35. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·T·None`; the k4 to k6 lines (None, 30 feet, Up to 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·T·None` |
| Standard spectrometer detection range | 1.50 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 78.9 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 37.3 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (63.9% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Utility Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Arcane Gyroscope (1-T-L-AG)|Arcane Gyroscope]] (1) · [[Vapour Deposition (1-T-L-VD)|Vapour Deposition]] (1) · [[Magnetise (2-T-L-MGN)|Magnetise]] (2) · [[Momentum Transfer (2-T-L-MT)|Momentum Transfer]] (2) · [[Ladder Operation (1-E-L-LOD)|Ladder Operation]] (1) · [[Pascal's Revenge (1-I-L-PSR)|Pascal's Revenge]] (1) · [[Reverb (1-I-L-RVR)|Reverb]] (1) · [[Sublimation (3-T-L-SBL)|Sublimation]] (3).


---

## Tactical Assessment

Pins weapons to the ground, collapses supports by overloading them, or lightens heavy loads for transport and bridging.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
