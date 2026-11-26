---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/evocation
  - source/srd
aliases:
  - "1st Tier Spell: Guiding Bolt"
  - "Guiding Bolt"
  - "1-V-L-GB"
registry_id: 1-V-L-GB
attribute_code: "1·Evo·Radiant·None·120 feet·1 round"
incantation: "Sunat-’muli"
tier: 1
school: Evocation
affinity: V
grade: L
pz_total: 7.0
pz_quantum: 350.0
t_e: -2.91
updated: 2026-11-16
---

**Guiding Bolt** (`1-V-L-GB`) is a 1st Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **7.0 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -2.91 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Evocation]]
        - **Guiding Bolt** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-V-L-GB` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Evo·Radiant·None·120 feet·1 round` |
| Incantation | *Sunat-’muli* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 120 feet |
| Area | single point or target |
| Duration | 1 round |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 4d6 radiant (mean 14) |
| Injury by tier | T1: 4d6, T2: 5d6, T3: 6d6, T4: 7d6, T5: 8d6, T6: 9d6, T7: 10d6, T8: 11d6, T9: 12d6 |
| Delivery | aimed ranged working |
| Practitioner lineages | Cleric |

### Mechanism

A radiant bolt strikes one target and leaves a faint glow on it that makes the next attack against it easier.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| radiant bolt, 4d6=14 | `14 HP * kappa_radiant 0.5 * F 0.5 * 1 target(s) * 1 trigger(s)` | 3.5 |
| marking glow | `5 W * 6 s / 1500` | 0.02 |
| Pattern cost | `0.01 × Q1 × (1 + 0.00)` | 3.5 |

| Quantity | Value |
|---|---|
| Effect energy | 3.5 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **7.0 Pz** (10.5 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.0201 |
| Energy-equivalent tier T_E | -2.91 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** 4d6 avg 14 radiant, ray delivery; marking glow 5 W for one round.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Guiding Bolt (1-V-L-GB) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Radiant | 11 | `0000000010111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 120 feet | 3 | `0000000000111` |
| k6 Duration | 1 round | 2 | `0000000000101` |

### Incantation

Spoken as **Sunat-’muli** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisunat-’muli* · T3: *Lisunat-’muli* · T4: *Visunat-’muli* · T5: *Tisunat-’muli* · T6: *Risunat-’muli* · T7: *Misunat-’muli* · T8: *Nisunat-’muli* · T9: *Xyisunat-’muli*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 4→1 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 | 3 |
| k6 Duration | 0→7 2→9 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#a69546`.

![[Guiding Bolt (1-V-L-GB) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| Damage | Radiant | 0.786 | 0.790 | `#1900ff` (464 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.923 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | 1 round | 0.158 | 0.998 | `#ffae00` (653 nm eq.) | source grid |
| Range | 120 feet | 0.176 | 0.997 | `#ffc900` (647 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.18): swatch `#b69d77`, measured lines at 0.101, 0.159, 0.177, 0.501, 0.786. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 0.85. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·V·Radiant`; the k4 to k6 lines (None, 120 feet, 1 round) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·V·Radiant` |
| Standard spectrometer detection range | 0.26 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.0 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Life, Hope and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `2b 1c 1d 2f 1i 1j` (2x Heat, Light, Life, 2x Energy, Hope, Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1.2 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (2.0% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Light and Radiance]], [[Precision Strikes]] |
| Element | [[Radiant Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Sacred Flame (0-V-L-SF)|Sacred Flame]] (0) · [[Divine Favor (1-V-L-DF)|Divine Favor]] (1) · [[Branding Smite (2-V-L-BS)|Branding Smite]] (2) · [[Moonbeam (2-V-M-MNB)|Moonbeam]] (2) · [[Electrify (1-V-L-ELC)|Electrify]] (1) · [[Faerie Fire (1-V-L-FF)|Faerie Fire]] (1) · [[Focusing Lens (1-V-L-FLC)|Focusing Lens]] (1) · [[Hellish Rebuke (1-V-L-HR)|Hellish Rebuke]] (1).


---

## Tactical Assessment

A strike that also designates a target for the rest of the team, like a laser marker.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
