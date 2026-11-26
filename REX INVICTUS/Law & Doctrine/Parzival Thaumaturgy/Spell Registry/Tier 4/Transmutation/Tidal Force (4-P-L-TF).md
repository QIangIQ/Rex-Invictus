---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/transmutation
  - source/science-spellbook
aliases:
  - "4th Tier Spell: Tidal Force"
  - "4-P-L-TF"
  - "Tidal Force (Science)"
registry_id: 4-P-L-TF
attribute_code: "4·Tra·Force·None·150 feet·Instantaneous"
incantation: "Vieton-’nosin"
tier: 4
school: Transmutation
affinity: P
grade: L
pz_total: 74.5
pz_quantum: 7029.9
t_e: -0.55
updated: 2026-11-16
---

**Tidal Force** (`4-P-L-TF`) is a 4th Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **74.5 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E -0.55 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Transmutation]]
        - **Tidal Force** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-P-L-TF` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Tra·Force·None·150 feet·Instantaneous` |
| Incantation | *Vieton-’nosin* |
| Affinity | P (Pure field construct) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Transmutation]] |
| Casting time | 1 Action |
| Range | 150 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A black pearl |
| Ritual | no |
| Injury | 6d6 force (mean 21) |
| Injury by tier | T4: 6d6, T5: 7d6, T6: 8d6, T7: 9d6, T8: 10d6, T9: 11d6 |
| Resistance check | strength; on success: half injury |
| Practitioner lineages | Wizard, Sorcerer |

### Mechanism

Applies a steep force gradient across one target, stretching and tearing it.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Differential force | `21 HP x 0.4 (force) x F 0.5` | 4.2 |
| Pattern cost | `0.01 × Q4 × (1 + 0.00)` | 70.3 |

| Quantity | Value |
|---|---|
| Effect energy | 4.2 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **74.5 Pz** (111.7 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 0.0106 |
| Energy-equivalent tier T_E | -0.55 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Force 6d6 = 21 on one target, directed F 0.5.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Tidal Force (4-P-L-TF) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 4 | 4 | `0000000001001` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | Force | 4 | `0000000001001` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 150 feet | 4 | `0000000001001` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Vieton-’nosin** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T5: *Tivieton-’nosin* · T6: *Rivieton-’nosin* · T7: *Mivieton-’nosin* · T8: *Nivieton-’nosin* · T9: *Xyivieton-’nosin*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 3→2 | 2 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 3→0 | 2 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 | 2 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#879e37`.

![[Tidal Force (4-P-L-TF) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| Damage | Force | 0.357 | 0.999 | `#3bff00` (593 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.893 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.923 | `#ff0028` (700 nm eq.) | source grid |
| Range | 150 feet | 0.235 | 0.987 | `#e3ff00` (629 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 1.87. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·T·Force`; the k4 to k6 lines (None, 150 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·T·Force` |
| Standard spectrometer detection range | 0.86 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 703 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Beyond, Introspection, 2x Movement and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1d 1G 2h 3j` (Beyond, Life, Introspection, 2x Flexibility, 3x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 12.4 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 4th Tier quantum of 7,030 Pz (1.1% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 4th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 4 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Pure]] (P) |
| Function | [[Precision Strikes]] |
| Element | [[Force Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Dimension Door (4-P-L-DD)|Dimension Door]] (4) · [[Planetary Rings (4-P-L-PR)|Planetary Rings]] (4) · [[Spiritual Weapon (2-P-L-SW)|Spiritual Weapon]] (2) · [[Stress (Battle) (0-P-L-SB)|Stress (Battle)]] (0) · [[Arcane Sword (7-P-L-ASC)|Arcane Sword]] (7) · [[Magic Missile (1-P-L-MM)|Magic Missile]] (1) · [[Blight (4-N-L-BLG)|Blight]] (4) · [[Cool Metal (2-T-L-CM)|Cool Metal]] (2).


---

## Tactical Assessment

Anti-materiel and anti-personnel strike; can tear 10 ft sections of structures.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
