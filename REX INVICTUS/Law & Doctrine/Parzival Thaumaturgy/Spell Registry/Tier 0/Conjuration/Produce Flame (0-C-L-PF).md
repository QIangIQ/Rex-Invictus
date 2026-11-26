---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-0
  - spell/conjuration
  - source/srd
aliases:
  - "Cantrip Spell: Produce Flame"
  - "Produce Flame"
  - "0-C-L-PF"
registry_id: 0-C-L-PF
attribute_code: "0·Con·Fire·None·Self·10 minutes"
incantation: "Ceire-’pors"
tier: 0
school: Conjuration
affinity: C
grade: L
pz_total: 12.9
pz_quantum: 128.8
t_e: -2.30
updated: 2026-11-16
---

**Produce Flame** (`0-C-L-PF`) is a Cantrip (Tier 0) working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **12.9 Pz** against a slot quantum of 129 Pz, which puts its energy-equivalent tier at T_E -2.30 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 0 Workings]]
      - [[Conjuration]]
        - **Produce Flame** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `0-C-L-PF` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `0·Con·Fire·None·Self·10 minutes` |
| Incantation | *Ceire-’pors* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | Cantrip (Tier 0) |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | Self |
| Area | single point or target |
| Duration | 10 minutes |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 1d8 fire (mean 4.5) |
| Injury by caster maturity bands | T1: 1d8, T5: 2d8, T11: 3d8, T17: 4d8 |
| Delivery | aimed ranged working |
| Practitioner lineages | Druid |

### Mechanism

A contained flame sits in the palm as a light source and can be launched once at a nearby target.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| hurled flame, 1d8 fire (4.5), directed | `4.5*0.70*0.5` | 1.6 |
| [upkeep] hand flame light, 10 ft bright (25 W), 10 min | `100*(10/20)**2*600/1500` | 10.0 |
| Pattern cost | `0.01 × Q0 × (1 + 0.00)` | 1.3 |

| Quantity | Value |
|---|---|
| Effect energy | 1.6 Pz |
| Upkeep energy | 10.0 Pz (0.0167 Pz/s) |
| **Total draw** | **12.9 Pz** (19.3 kJ) |
| Slot quantum Q0 | 129 Pz |
| Field gain (draw / quantum) | 0.0999 |
| Energy-equivalent tier T_E | -2.30 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Light scaled from 100 W per 20 ft radius; one throw; base 1d8.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Produce Flame (0-C-L-PF) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 0 | 0 | `0000000000001` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | Fire | 3 | `0000000000111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | 10 minutes | 4 | `0000000001001` |

### Incantation

Spoken as **Ceire-’pors** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T1: *Siceire-’pors* · T2: *Hiceire-’pors* · T3: *Liceire-’pors* · T4: *Viceire-’pors* · T5: *Ticeire-’pors* · T6: *Riceire-’pors* · T7: *Miceire-’pors* · T8: *Niceire-’pors* · T9: *Xyiceire-’pors*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 | 1 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 | 3 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 3→10 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#b29232`.

![[Produce Flame (0-C-L-PF) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 0 | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| Damage | Fire | 0.286 | 0.960 | `#9cff00` (614 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.992 | `#ff8300` (662 nm eq.) | source grid |
| Duration | 10 minutes | 0.263 | 0.966 | `#bdff00` (621 nm eq.) | source grid |
| Range | Self | 0.706 | 0.779 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.21): swatch `#db8155`, measured lines at 0.006, 0.126, 0.264, 0.286, 0.706. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.11. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `0·C·Fire`; the k4 to k6 lines (None, Self, 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `0·C·Fire` |
| Standard spectrometer detection range | 0.36 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 6.4 Pz (0.05 × Q0) |
| Counter drawn cold (all six layers) | 12.9 Pz (0.10 × Q0) |
| Unravel after completion | 14.9 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Energy, Movement and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1b 1c 1e 2j` (Beyond, Heat, Light, Prodigious, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 2.1 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the Cantrip (Tier 0) quantum of 129 Pz (10.0% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at Cantrip (Tier 0) up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 0 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Precision Strikes]] |
| Element | [[Fire Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Fire Bolt (0-V-L-FB)|Fire Bolt]] (0) · [[Flaming Sphere (2-C-L-FSA)|Flaming Sphere]] (2) · [[Sacred Flame (0-V-L-SF)|Sacred Flame]] (0) · [[Focusing Lens (1-V-L-FLC)|Focusing Lens]] (1) · [[Hellish Rebuke (1-V-L-HR)|Hellish Rebuke]] (1) · [[Acid Splash (0-C-L-AS)|Acid Splash]] (0) · [[Flame Blade (2-V-L-FBA)|Flame Blade]] (2) · [[Heat Metal (2-T-M-HM)|Heat Metal]] (2).


---

## Tactical Assessment

A hands-free light and a minor improvised attack; the flame marks the user's position at night.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 0 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
