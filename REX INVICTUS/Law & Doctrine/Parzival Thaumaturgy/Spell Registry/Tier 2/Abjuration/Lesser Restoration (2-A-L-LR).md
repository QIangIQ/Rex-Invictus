---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/abjuration
  - source/srd
aliases:
  - "2nd Tier Spell: Lesser Restoration"
  - "Lesser Restoration"
  - "2-A-L-LR"
registry_id: 2-A-L-LR
attribute_code: "2·Abj·None·None·Touch·Instantaneous"
incantation: "Halix"
tier: 2
school: Abjuration
affinity: A
grade: L
pz_total: 12.5
pz_quantum: 951.4
t_e: -2.33
updated: 2026-11-16
---

**Lesser Restoration** (`2-A-L-LR`) is a 2nd Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **12.5 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E -2.33 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Abjuration]]
        - **Lesser Restoration** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-A-L-LR` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Abj·None·None·Touch·Instantaneous` |
| Incantation | *Halix* |
| Affinity | A (Abjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Abjuration]] |
| Casting time | 1 action |
| Range | Touch |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Bard, Cleric, Druid, Paladin, Ranger |

### Mechanism

A touch clears one disease or one disabling impairment such as blindness, deafness, paralysis or poisoning. The field work is comparable to a small wound repair.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Clearing one disease or condition (healing equivalent) | `10 HP equivalent * 0.30` | 3.0 |
| Pattern cost | `0.01 × Q2 × (1 + 0.00)` | 9.5 |

| Quantity | Value |
|---|---|
| Effect energy | 3.0 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **12.5 Pz** (18.8 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.0132 |
| Energy-equivalent tier T_E | -2.33 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Removing one condition valued as 10 units of healing.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Lesser Restoration (2-A-L-LR) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Halix** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihalix* · T4: *Vihalix* · T5: *Tihalix* · T6: *Rihalix* · T7: *Mihalix* · T8: *Nihalix* · T9: *Xyihalix*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#e93e4a`.

![[Lesser Restoration (2-A-L-LR) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.980 | `#ff0028` (700 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.980 | `#ff0028` (700 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.792 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.19): swatch `#db4f51`, measured lines at 0.006, 0.201, 0.883. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.10. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·A·None`; the k4 to k6 lines (None, Touch, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·A·None` |
| Standard spectrometer detection range | 0.35 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 95.1 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 2.1 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (1.3% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Healing and Restoration]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Remove Curse (3-A-L-RC)|Remove Curse]] (3) · [[Prayer of Healing (2-V-L-PH)|Prayer of Healing]] (2) · [[Thomson's Plum Pudding (2-T-L-TSPP)|Thomson's Plum Pudding]] (2) · [[Cure Wounds (1-V-L-CW)|Cure Wounds]] (1) · [[Goodberry (1-T-L-GDB)|Goodberry]] (1) · [[Greater Restoration (5-A-L-GRE)|Greater Restoration]] (5) · [[Healing Word (1-V-L-HW)|Healing Word]] (1) · [[Mass Healing Word (3-V-L-MHW)|Mass Healing Word]] (3).


---

## Tactical Assessment

Field medicine for chemical and biological exposure and for restoring a blinded or paralysed soldier to action. One condition per use.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
