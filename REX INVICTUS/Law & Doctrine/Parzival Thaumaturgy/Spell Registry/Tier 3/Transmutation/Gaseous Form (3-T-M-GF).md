---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/transmutation
  - source/srd
aliases:
  - "3rd Tier Spell: Gaseous Form"
  - "Gaseous Form"
  - "3-T-M-GF"
registry_id: 3-T-M-GF
attribute_code: "3·Tra·None·None·Touch·Up to 1 hour"
incantation: "Lielixsi"
tier: 3
school: Transmutation
affinity: T
grade: M
pz_total: 910.9
pz_quantum: 2586.2
t_e: 1.96
updated: 2026-11-16
---

**Gaseous Form** (`3-T-M-GF`) is a 3rd Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **911 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E 1.96 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Transmutation]]
        - **Gaseous Form** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-T-M-GF` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Tra·None·None·Touch·Up to 1 hour` |
| Incantation | *Lielixsi* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Transmutation]] |
| Casting time | 1 action |
| Range | Touch |
| Area | single point or target |
| Duration | Up to 1 hour (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A bit of gauze and a wisp of smoke |
| Ritual | no |
| Practitioner lineages | Sorcerer, Warlock, Wizard |

### Mechanism

Converts a willing creature and its gear into a coherent drifting mist that moves at 3 m/s, passes through cracks and resists ordinary injury.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| dispersal and reassembly of 80 kg body | `10 Pz/kg * 80 kg` | 800 |
| nonmagical injury halving | `0.20 Pz * (10 rounds * 15 HP/round * 50% = 75 HP)` | 15.0 |
| suspension of mist body | `0.02 * 80 kg * 9.81 / 1500 = 0.010464 Pz/s * 3600 s` | 37.7 |
| Pattern cost | `0.01 × Q3 × (1 + 1.25)` | 58.2 |

| Quantity | Value |
|---|---|
| Effect energy | 815 Pz |
| Upkeep energy | 37.7 Pz (0.0105 Pz/s) |
| **Total draw** | **911 Pz** (1,366.3 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 0.352 |
| Energy-equivalent tier T_E | 1.96 |
| Handling points | 1.25 |
| Grade score | 0.73 → M |

**Handling flags:** concentration, fragile.

**Assumptions:** 80 kg target restructured at the living-matter rate; full hour of hover; 10 rounds of halved incoming injury.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Gaseous Form (3-T-M-GF) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Up to 1 hour | 12 | `0000000011001` |

### Incantation

Spoken as **Lielixsi** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vilielixsi* · T5: *Tilielixsi* · T6: *Rilielixsi* · T7: *Milielixsi* · T8: *Nilielixsi* · T9: *Xyilielixsi*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 3→10 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#6d78b8`.

![[Gaseous Form (3-T-M-GF) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.848 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Up to 1 hour | 0.632 | 0.947 | `#00c0ff` (511 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.844 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.17): swatch `#7699c9`, measured lines at 0.300, 0.632, 0.878. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.96. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·T·None`; the k4 to k6 lines (None, Touch, Up to 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·T·None` |
| Standard spectrometer detection range | 3.02 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 266 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 152 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 3rd Tier quantum of 2,586 Pz (35.2% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Movement and Flight]], [[Transformation]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Chemical Transition (3-T-L-CTE)|Chemical Transition]] (3) · [[Fly (3-T-L-FLY)|Fly]] (3) · [[Haste (3-T-L-HST)|Haste]] (3) · [[Slow (3-T-L-SLW)|Slow]] (3) · [[Water Breathing (3-T-L-WBT)|Water Breathing]] (3) · [[Water Walk (3-T-L-WW)|Water Walk]] (3) · [[Accelerate (2-T-L-ACC)|Accelerate]] (2) · [[Alter Self (2-T-L-AST)|Alter Self]] (2).


---

## Tactical Assessment

An escape and infiltration tool: agents can pass under doors, through vents and past guards, though they arrive unable to act or carry tools.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
