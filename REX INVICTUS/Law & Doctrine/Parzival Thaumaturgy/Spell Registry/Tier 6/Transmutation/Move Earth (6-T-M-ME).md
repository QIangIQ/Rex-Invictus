---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-6
  - spell/transmutation
  - source/srd
aliases:
  - "6th Tier Spell: Move Earth"
  - "Move Earth"
  - "6-T-M-ME"
registry_id: 6-T-M-ME
attribute_code: "6·Tra·None·cone (40)·120 feet·Up to 2 hours"
incantation: "Rie’-Némulay"
tier: 6
school: Transmutation
affinity: T
grade: M
pz_total: 174049.3
pz_quantum: 51944.6
t_e: 7.21
updated: 2026-11-16
---

**Move Earth** (`6-T-M-ME`) is a 6th Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **174,049 Pz** against a slot quantum of 51,945 Pz, which puts its energy-equivalent tier at T_E 7.21 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 6 Workings]]
      - [[Transmutation]]
        - **Move Earth** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `6-T-M-ME` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `6·Tra·None·cone (40)·120 feet·Up to 2 hours` |
| Incantation | *Rie’-Némulay* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 6th Tier |
| School | [[Transmutation]] |
| Casting time | 1 action |
| Range | 120 feet |
| Area | cone (40) |
| Duration | Up to 2 hours (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: An iron blade and a small bag containing a mixture of soils--clay, loam, and sand |
| Ritual | no |
| Practitioner lineages | Druid, Sorcerer, Wizard |

### Mechanism

Over each 10 minute cycle the field reshapes loose soil in a 40 ft square, raising, lowering, trenching or piling it by up to 20 ft. Natural rock and masonry are untouched.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Soil reshaping, one 40 ft square per 10 minutes (upkeep) | `(12.192 m^2 * 6.096 m / 2 * 1600 kg/m^3) * 9.81 * 3.048 m / 1500 / 600 s * 7200 s` | 173,400 |
| Pattern cost | `0.01 × Q6 × (1 + 0.25)` | 649 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 173,400 Pz (24.1 Pz/s) |
| **Total draw** | **174,049 Pz** (261,074.0 kJ) |
| Slot quantum Q6 | 51,945 Pz |
| Field gain (draw / quantum) | 3.35 |
| Energy-equivalent tier T_E | 7.21 |
| Handling points | 0.25 |
| Grade score | 0.85 → M |

**Handling flags:** concentration.

**Assumptions:** Each cycle moves half the square's area times 20 ft of soil at 1600 kg/m^3 through an average 10 ft; 12 cycles in 2 hours; the area value in the record is ignored as a data error.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Move Earth (6-T-M-ME) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 6 | 6 | `0000000001101` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | cone (40) | 3 | `0000000000111` |
| k5 Range | 120 feet | 3 | `0000000000111` |
| k6 Duration | Up to 2 hours | 16 | `0000000100001` |

### Incantation

Spoken as **Rie’-Némulay** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T7: *Mirie’-Némulay* · T8: *Nirie’-Némulay* · T9: *Xyirie’-Némulay*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 3→2 | 3 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 2→11 | 3 |
| k5 Range | 0→8 1→9 2→10 | 3 |
| k6 Duration | 0→7 5→12 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#93659e`.

![[Move Earth (6-T-M-ME) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 6 | 0.600 | 1.000 | `#00ebff` (520 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.963 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Up to 2 hours | 0.842 | 0.971 | `#6500ff` (447 nm eq.) | source grid |
| Area | cone (40) | 0.083 | 0.875 | `#ff4800` (675 nm eq.) | source grid |
| Range | 120 feet | 0.176 | 0.914 | `#ffc900` (647 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.20): swatch `#6b91c4`, measured lines at 0.084, 0.177, 0.601, 0.843, 0.876. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 5.24. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `6·T·None`; the k4 to k6 lines (cone (40), 120 feet, Up to 2 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `6·T·None` |
| Standard spectrometer detection range | 41.72 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 2,597 Pz (0.05 × Q6) |
| Counter drawn cold (all six layers) | 5,194 Pz (0.10 × Q6) |
| Unravel after completion | 39,874 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 29,008 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 3.35 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 6th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 6th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 6 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Terrain and Matter Shaping]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Passwall (5-T-L-PSS)|Passwall]] (5) · [[Control Water (4-T-H-CWN)|Control Water]] (4) · [[Control Weather (8-T-H-CWT)|Control Weather]] (8) · [[Fabricate (4-T-L-FBR)|Fabricate]] (4) · [[Freefall (4-T-L-FRF)|Freefall]] (4) · [[Stone Shape (4-T-M-SSO)|Stone Shape]] (4) · [[Alter Biome (9-T-X-AB)|Alter Biome]] (9) · [[Creation (5-I-L-CRT)|Creation]] (5).


---

## Tactical Assessment

Digs trenches and berms, fills tank traps and builds revetments without engineers or machines over two hours. It is too slow to trap or injure troops directly.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 6 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
