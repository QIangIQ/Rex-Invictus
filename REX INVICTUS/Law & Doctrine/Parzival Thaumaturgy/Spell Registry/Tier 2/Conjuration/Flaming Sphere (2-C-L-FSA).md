---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/conjuration
  - source/srd
aliases:
  - "2nd Tier Spell: Flaming Sphere"
  - "Flaming Sphere"
  - "2-C-L-FSA"
registry_id: 2-C-L-FSA
attribute_code: "2·Con·Fire·None·60 feet·Up to 1 minute"
incantation: "Heire-’wynse"
tier: 2
school: Conjuration
affinity: C
grade: L
pz_total: 1395.0
pz_quantum: 951.4
t_e: 2.38
updated: 2026-11-16
---

**Flaming Sphere** (`2-C-L-FSA`) is a 2nd Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **1,395 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E 2.38 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Conjuration]]
        - **Flaming Sphere** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-C-L-FSA` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Con·Fire·None·60 feet·Up to 1 minute` |
| Incantation | *Heire-’wynse* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | single point or target |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A bit of tallow, a pinch of brimstone, and a dusting of powdered iron |
| Ritual | no |
| Injury | 2d6 fire (mean 7) |
| Injury by tier | T2: 2d6, T3: 3d6, T4: 4d6, T5: 5d6, T6: 6d6, T7: 7d6, T8: 8d6, T9: 9d6 |
| Practitioner lineages | Druid, Wizard |

### Mechanism

A 1.5 m ball of fire is held in place or steered about the field, heating anything within 1.5 m of it and igniting loose fuel.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| sphere heat emanation, 2d6=7 | `7 HP * kappa_fire 0.7 * S/A_c (1 x 4*pi*(7.5 ft*0.3048)^2 = 65.7 m^2 / 0.7) * 3 triggers` | 1,379 |
| sphere light (20 ft bright) | `100 W / 1500 = 0.0666667 Pz/s * 60 s` | 4.0 |
| Pattern cost | `0.01 × Q2 × (1 + 0.25)` | 11.9 |

| Quantity | Value |
|---|---|
| Effect energy | 1,379 Pz |
| Upkeep energy | 4.0 Pz (0.0667 Pz/s) |
| **Total draw** | **1,395 Pz** (2,092.4 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 1.47 |
| Energy-equivalent tier T_E | 2.38 |
| Handling points | 0.25 |
| Grade score | 0.44 → L |

**Handling flags:** concentration.

**Assumptions:** Emanation radius 7.5 ft (sphere radius plus 5 ft); 3 triggers; light 100 W for 1 minute.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Flaming Sphere (2-C-L-FSA) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | Fire | 3 | `0000000000111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Heire-’wynse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Liheire-’wynse* · T4: *Viheire-’wynse* · T5: *Tiheire-’wynse* · T6: *Riheire-’wynse* · T7: *Miheire-’wynse* · T8: *Niheire-’wynse* · T9: *Xyiheire-’wynse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 | 3 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#8ac660`.

![[Flaming Sphere (2-C-L-FSA) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| Damage | Fire | 0.286 | 0.996 | `#9cff00` (614 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.997 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.889 | `#0074ff` (495 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.927 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.17): swatch `#caa36e`, measured lines at 0.126, 0.201, 0.286, 0.589, 0.685. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.14. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·C·Fire`; the k4 to k6 lines (None, 60 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·C·Fire` |
| Standard spectrometer detection range | 3.73 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 95.9 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Energy, Movement and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1b 1c 1e 2j` (Beyond, Heat, Light, Prodigious, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 232 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 1.47 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 2nd Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Precision Strikes]] |
| Element | [[Fire Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Flame Blade (2-V-L-FBA)|Flame Blade]] (2) · [[Heat Metal (2-T-M-HM)|Heat Metal]] (2) · [[Produce Flame (0-C-L-PF)|Produce Flame]] (0) · [[Scorching Ray (2-V-L-SR)|Scorching Ray]] (2) · [[Focusing Lens (1-V-L-FLC)|Focusing Lens]] (1) · [[Hellish Rebuke (1-V-L-HR)|Hellish Rebuke]] (1) · [[Fire Bolt (0-V-L-FB)|Fire Bolt]] (0) · [[Sacred Flame (0-V-L-SF)|Sacred Flame]] (0).


---

## Tactical Assessment

A mobile area-denial charge that can be rolled down corridors and over low walls to flush defenders out of cover.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
