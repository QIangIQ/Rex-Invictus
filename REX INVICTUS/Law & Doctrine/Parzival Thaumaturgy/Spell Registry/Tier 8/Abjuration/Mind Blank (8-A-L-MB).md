---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-8
  - spell/abjuration
  - source/srd
aliases:
  - "8th Tier Spell: Mind Blank"
  - "Mind Blank"
  - "8-A-L-MB"
registry_id: 8-A-L-MB
attribute_code: "8·Abj·None·None·Touch·24 hours"
incantation: "Nalixl"
tier: 8
school: Abjuration
affinity: A
grade: L
pz_total: 4290.2
pz_quantum: 383821.6
t_e: 3.51
updated: 2026-11-16
---

**Mind Blank** (`8-A-L-MB`) is a 8th Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **4,290 Pz** against a slot quantum of 383,822 Pz, which puts its energy-equivalent tier at T_E 3.51 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 8 Workings]]
      - [[Abjuration]]
        - **Mind Blank** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `8-A-L-MB` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `8·Abj·None·None·Touch·24 hours` |
| Incantation | *Nalixl* |
| Affinity | A (Abjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 8th Tier |
| School | [[Abjuration]] |
| Casting time | 1 action |
| Range | Touch |
| Area | single point or target |
| Duration | 24 hours |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Bard, Wizard |

### Mechanism

For a day the field seals one willing creature against psychic injury, emotion and thought reading, remote sensing and control, even by workings of the highest order.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Mental shielding, one subject (upkeep) | `0.005 Pz/s * 86400 s` | 432 |
| Psychic absorption (upkeep) | `0.20 Pz * 100 HP / 86400 s * 86400 s` | 20.0 |
| Pattern cost | `0.01 × Q8 × (1 + 0.00)` | 3,838 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 452 Pz (0.00523 Pz/s) |
| **Total draw** | **4,290 Pz** (6,435.3 kJ) |
| Slot quantum Q8 | 383,822 Pz |
| Field gain (draw / quantum) | 0.0112 |
| Energy-equivalent tier T_E | 3.51 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** One subject for 24 hours; 100 units of psychic injury absorbed; low physical cost, as the effect is informational.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Mind Blank (8-A-L-MB) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 8 | 8 | `0000000010001` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | 24 hours | 5 | `0000000001011` |

### Incantation

Spoken as **Nalixl** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T9: *Xyinalixl*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 4→3 | 2 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 3→10 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#863e94`.

![[Mind Blank (8-A-L-MB) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 8 | 0.800 | 1.000 | `#2900ff` (460 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.726 | `#ff0028` (700 nm eq.) | source grid |
| Duration | 24 hours | 0.316 | 0.889 | `#76ff00` (605 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.997 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.20): swatch `#7178b3`, measured lines at 0.006, 0.316, 0.801, 0.883. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.63. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `8·A·None`; the k4 to k6 lines (None, Touch, 24 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `8·A·None` |
| Standard spectrometer detection range | 6.55 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 19,191 Pz (0.05 × Q8) |
| Counter drawn cold (all six layers) | 38,382 Pz (0.10 × Q8) |
| Unravel after completion | 38,473 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 715 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 8th Tier quantum of 383,822 Pz (1.1% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 8th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 8 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Wards and Shields]], [[Negation and Counterspell]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Globe of Invulnerability (6-A-L-GIO)|Globe of Invulnerability]] (6) · [[Antimagic Field (8-A-L-AFT)|Antimagic Field]] (8) · [[Holy Aura (8-A-L-HA)|Holy Aura]] (8) · [[Nondetection (3-A-L-NND)|Nondetection]] (3) · [[Forbiddance (6-A-L-FRBB)|Forbiddance]] (6) · [[Glibness (8-T-L-GLB)|Glibness]] (8) · [[Guards and Wards (6-A-L-GWA)|Guards and Wards]] (6) · [[Antilife Shell (5-A-L-ASI)|Antilife Shell]] (5).


---

## Tactical Assessment

Protects heads of state, commanders and agents carrying secrets against interrogation, tracking and mental control. It does not protect against physical harm.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 8 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
