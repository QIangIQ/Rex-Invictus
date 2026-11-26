---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/abjuration
  - source/srd
aliases:
  - "5th Tier Spell: Greater Restoration"
  - "Greater Restoration"
  - "5-A-L-GRE"
registry_id: 5-A-L-GRE
attribute_code: "5·Abj·None·None·Touch·Instantaneous"
incantation: "Talix"
tier: 5
school: Abjuration
affinity: A
grade: L
pz_total: 296.6
pz_quantum: 19109.4
t_e: 0.83
updated: 2026-11-16
---

**Greater Restoration** (`5-A-L-GRE`) is a 5th Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **297 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 0.83 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Abjuration]]
        - **Greater Restoration** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-A-L-GRE` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Abj·None·None·Touch·Instantaneous` |
| Incantation | *Talix* |
| Affinity | A (Abjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Abjuration]] |
| Casting time | 1 action |
| Range | Touch |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Diamond dust worth at least 100gp, which the spell consumes |
| Ritual | no |
| Practitioner lineages | Bard, Cleric, Druid |

### Mechanism

A positive-energy pulse corrects one lasting impairment in a touched creature, such as a curse, petrification, charm, reduced capacity or deep fatigue.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| tissue and nervous repair | `0.30 Pz * 30 HP-equivalent` | 9.0 |
| pattern correction | `instant info` | 1.0 |
| Pattern cost | `0.01 × Q5 × (1 + 0.50)` | 287 |

| Quantity | Value |
|---|---|
| Effect energy | 10.0 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **297 Pz** (445.0 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 0.0155 |
| Energy-equivalent tier T_E | 0.83 |
| Handling points | 0.50 |
| Grade score | -0.50 → L |

**Handling flags:** costly material, consumed material.

**Assumptions:** Repair equivalent to 30 points of healing; one informational correction.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Greater Restoration (5-A-L-GRE) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Talix** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Ritalix* · T7: *Mitalix* · T8: *Nitalix* · T9: *Xyitalix*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#a04578`.

![[Greater Restoration (5-A-L-GRE) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.882 | `#ff0028` (700 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.882 | `#ff0028` (700 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.930 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.18): swatch `#9f8085`, measured lines at 0.006, 0.501, 0.883. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.47. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·A·None`; the k4 to k6 lines (None, Touch, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·A·None` |
| Standard spectrometer detection range | 1.72 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 1,911 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 49.4 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 5th Tier quantum of 19,109 Pz (1.6% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 5th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 5 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Healing and Restoration]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Mass Cure Wounds (5-C-L-MCW)|Mass Cure Wounds]] (5) · [[Raise Dead (5-N-M-RD)|Raise Dead]] (5) · [[Reincarnate (5-T-M-RNC)|Reincarnate]] (5) · [[Remove Curse (3-A-L-RC)|Remove Curse]] (3) · [[Heal (6-V-L-HEA)|Heal]] (6) · [[Heroes' Feast (6-C-L-HF)|Heroes' Feast]] (6) · [[Lesser Restoration (2-A-L-LR)|Lesser Restoration]] (2) · [[Antilife Shell (5-A-L-ASI)|Antilife Shell]] (5).


---

## Tactical Assessment

Returns specialists to duty after debilitating enemy workings; an important countermeasure in a field-caster medical corps.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
