---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/abjuration
  - source/srd
aliases:
  - "2nd Tier Spell: Pass Without Trace"
  - "Pass Without Trace"
  - "2-A-L-PWT"
registry_id: 2-A-L-PWT
attribute_code: "2·Abj·None·None·Self·Up to 1 hour"
incantation: "Haporsi"
tier: 2
school: Abjuration
affinity: A
grade: L
pz_total: 49.4
pz_quantum: 951.4
t_e: -0.96
updated: 2026-11-16
---

**Pass Without Trace** (`2-A-L-PWT`) is a 2nd Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **49.4 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E -0.96 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Abjuration]]
        - **Pass Without Trace** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-A-L-PWT` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Abj·None·None·Self·Up to 1 hour` |
| Incantation | *Haporsi* |
| Affinity | A (Abjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Abjuration]] |
| Casting time | 1 action |
| Range | Self |
| Area | single point or target |
| Duration | Up to 1 hour (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Ashes from a burned leaf of mistletoe and a sprig of spruce |
| Ritual | no |
| Practitioner lineages | Druid, Ranger |

### Mechanism

A veil of shadow and sound damping surrounds the caster's group within 30 ft for up to an hour, and their footprints and other traces are erased.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Shadow and silence veil, 30 ft radius (upkeep) | `0.002 Pz/s * (3203 m^3/1000) * 3600 s` | 23.1 |
| Track erasure, 6 walkers (upkeep) | `1 J/step * 6 * 1 step/s / 1500 * 3600 s` | 14.4 |
| Pattern cost | `0.01 × Q2 × (1 + 0.25)` | 11.9 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 37.5 Pz (0.0104 Pz/s) |
| **Total draw** | **49.4 Pz** (74.0 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.0519 |
| Energy-equivalent tier T_E | -0.96 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** concentration.

**Assumptions:** Six walkers stepping once per second; veil volume a 30 ft radius sphere; 1 hour.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Pass Without Trace (2-A-L-PWT) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Up to 1 hour | 12 | `0000000011001` |

### Incantation

Spoken as **Haporsi** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihaporsi* · T4: *Vihaporsi* · T5: *Tihaporsi* · T6: *Rihaporsi* · T7: *Mihaporsi* · T8: *Nihaporsi* · T9: *Xyihaporsi*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 3→10 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#858083`.

![[Pass Without Trace (2-A-L-PWT) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.980 | `#ff0028` (700 nm eq.) | source grid |
| Duration | Up to 1 hour | 0.632 | 0.911 | `#00c0ff` (511 nm eq.) | source grid |
| Range | Self | 0.706 | 0.880 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.20): swatch `#ae8b71`, measured lines at 0.007, 0.201, 0.632, 0.706. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.69. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·A·None`; the k4 to k6 lines (None, Self, Up to 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·A·None` |
| Standard spectrometer detection range | 0.70 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 103 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 8.2 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (5.2% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Concealment and Illusion]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Nondetection (3-A-L-NND)|Nondetection]] (3) · [[Arcanist's Magic Aura (2-I-L-ASMA)|Arcanist's Magic Aura]] (2) · [[Blur (2-I-L-BLR)|Blur]] (2) · [[Cloak (2-I-L-CLK)|Cloak]] (2) · [[Darkness (2-V-L-DRK)|Darkness]] (2) · [[Invisibility (2-I-L-INV)|Invisibility]] (2) · [[Mirror Image (2-I-L-MIR)|Mirror Image]] (2) · [[Misted Leap (2-C-L-ML)|Misted Leap]] (2).


---

## Tactical Assessment

Supports patrols and infiltration teams moving through observed ground, and frustrates trackers and dogs. Electronic and thermal sensors are not addressed.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
