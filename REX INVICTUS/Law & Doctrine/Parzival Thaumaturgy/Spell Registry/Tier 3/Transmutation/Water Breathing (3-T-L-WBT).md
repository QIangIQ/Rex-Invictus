---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/transmutation
  - source/srd
aliases:
  - "3rd Tier Spell: Water Breathing"
  - "Water Breathing"
  - "3-T-L-WBT"
registry_id: 3-T-L-WBT
attribute_code: "3·Tra·None·None·30 feet·24 hours"
incantation: "Lieusinl"
tier: 3
school: Transmutation
affinity: T
grade: L
pz_total: 1232.3
pz_quantum: 2586.2
t_e: 2.26
updated: 2026-11-16
---

**Water Breathing** (`3-T-L-WBT`) is a 3rd Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **1,232 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E 2.26 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Transmutation]]
        - **Water Breathing** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-T-L-WBT` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Tra·None·None·30 feet·24 hours` |
| Incantation | *Lieusinl* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Transmutation]] |
| Casting time | 1 action |
| Range | 30 feet |
| Area | single point or target |
| Duration | 24 hours |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A short piece of reed or straw |
| Ritual | yes |
| Practitioner lineages | Druid, Ranger, Sorcerer, Wizard |

### Mechanism

Up to ten subjects gain the ability to draw dissolved oxygen from water for a day while keeping normal air breathing.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Upkeep: Oxygen extraction pumping, 10 creatures | `10 * 180 m^3 water * 1000 Pa / 1500` | 1,200 |
| Pattern cost | `0.01 × Q3 × (1 + 0.25)` | 32.3 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 1,200 Pz (0.0139 Pz/s) |
| **Total draw** | **1,232 Pz** (1,848.5 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 0.477 |
| Energy-equivalent tier T_E | 2.26 |
| Handling points | 0.25 |
| Grade score | -0.12 → L |

**Handling flags:** ritual.

**Assumptions:** 0.35 L/min O2 per person; 4 mg/L usable O2; 1 kPa membrane head.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Water Breathing (3-T-L-WBT) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | 24 hours | 5 | `0000000001011` |

### Incantation

Spoken as **Lieusinl** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vilieusinl* · T5: *Tilieusinl* · T6: *Rilieusinl* · T7: *Milieusinl* · T8: *Nilieusinl* · T9: *Xyilieusinl*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 3→10 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#89c638`.

![[Water Breathing (3-T-L-WBT) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.848 | `#9600ff` (438 nm eq.) | source grid |
| Duration | 24 hours | 0.316 | 1.000 | `#76ff00` (605 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 1.000 | `#91ff00` (612 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 3.09. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·T·None`; the k4 to k6 lines (None, 30 feet, 24 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·T·None` |
| Standard spectrometer detection range | 3.51 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 499 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 205 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 3rd Tier quantum of 2,586 Pz (47.7% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Movement and Flight]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Fly (3-T-L-FLY)|Fly]] (3) · [[Gaseous Form (3-T-M-GF)|Gaseous Form]] (3) · [[Haste (3-T-L-HST)|Haste]] (3) · [[Slow (3-T-L-SLW)|Slow]] (3) · [[Water Walk (3-T-L-WW)|Water Walk]] (3) · [[Accelerate (2-T-L-ACC)|Accelerate]] (2) · [[Freefall (4-T-L-FRF)|Freefall]] (4) · [[Levitate (2-T-L-LVT)|Levitate]] (2).


---

## Tactical Assessment

Underwater infiltration, harbour operations and survival after ditching.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
