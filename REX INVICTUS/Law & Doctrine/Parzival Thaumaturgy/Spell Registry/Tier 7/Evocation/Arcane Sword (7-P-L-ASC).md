---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-7
  - spell/evocation
  - source/srd
aliases:
  - "7th Tier Spell: Arcane Sword"
  - "Arcane Sword"
  - "7-P-L-ASC"
registry_id: 7-P-L-ASC
attribute_code: "7·Evo·Force·None·60 feet·Up to 1 minute"
incantation: "Muton-’wynse"
tier: 7
school: Evocation
affinity: P
grade: L
pz_total: 2126.3
pz_quantum: 141200.1
t_e: 2.80
updated: 2026-11-16
---

**Arcane Sword** (`7-P-L-ASC`) is a 7th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **2,126 Pz** against a slot quantum of 141,200 Pz, which puts its energy-equivalent tier at T_E 2.80 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 7 Workings]]
      - [[Evocation]]
        - **Arcane Sword** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `7-P-L-ASC` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `7·Evo·Force·None·60 feet·Up to 1 minute` |
| Incantation | *Muton-’wynse* |
| Affinity | P (Pure field construct) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 7th Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | single point or target |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A miniature platinum sword with a grip and pommel of copper and zinc, worth 250 gp |
| Ritual | no |
| Injury | 3d10 force (mean 16.5) |
| Injury by tier | T7: 3d10 |
| Delivery | aimed melee working |
| Practitioner lineages | Bard, Wizard |

### Mechanism

A blade-shaped plane of force hovers and strikes at the caster's direction, relocating up to 6 m per round.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| sword strikes | `16.5 HP * 0.4 Pz/HP (force) * F 0.08 * 10 target(s)/hit(s)` | 5.3 |
| autonomy upkeep | `0.05 Pz/s * 60 s` | 3.0 |
| Pattern cost | `0.01 × Q7 × (1 + 0.50)` | 2,118 |

| Quantity | Value |
|---|---|
| Effect energy | 5.3 Pz |
| Upkeep energy | 3.0 Pz (0.05 Pz/s) |
| **Total draw** | **2,126 Pz** (3,189.4 kJ) |
| Slot quantum Q7 | 141,200 Pz |
| Field gain (draw / quantum) | 0.0151 |
| Energy-equivalent tier T_E | 2.80 |
| Handling points | 0.50 |
| Grade score | -0.50 → L |

**Handling flags:** concentration, costly material.

**Assumptions:** One strike per round for 10 rounds at 16.5 average injury; focused factor 0.08.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Arcane Sword (7-P-L-ASC) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 7 | 7 | `0000000001111` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Force | 4 | `0000000001001` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Muton-’wynse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T8: *Nimuton-’wynse* · T9: *Xyimuton-’wynse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 3→2 | 4 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 3→0 | 2 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#0bc1b6`.

![[Arcane Sword (7-P-L-ASC) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 7 | 0.700 | 1.000 | `#005eff` (490 nm eq.) | source grid |
| Damage | Force | 0.357 | 0.943 | `#3bff00` (593 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.980 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 1.000 | `#0074ff` (495 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.994 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.13): swatch `#5fe7c2`, measured lines at 0.358, 0.501, 0.589, 0.685, 0.701. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.33. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `7·V·Force`; the k4 to k6 lines (None, 60 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `7·V·Force` |
| Standard spectrometer detection range | 4.61 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 7,060 Pz (0.05 × Q7) |
| Counter drawn cold (all six layers) | 14,120 Pz (0.10 × Q7) |
| Unravel after completion | 14,121 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Beyond, Introspection, 2x Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1b 2f 1G 3j` (Beyond, Heat, 2x Energy, Introspection, 3x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 354 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 7th Tier quantum of 141,200 Pz (1.5% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 7th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 7 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Pure]] (P) |
| Function | [[Summoning and Conjured Creatures]], [[Precision Strikes]] |
| Element | [[Force Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Spiritual Weapon (2-P-L-SW)|Spiritual Weapon]] (2) · [[Dark Matter Sword (7-V-L-DMS)|Dark Matter Sword]] (7) · [[Chain Lightning (6-V-L-CLA)|Chain Lightning]] (6) · [[Dimension Door (4-P-L-DD)|Dimension Door]] (4) · [[Faithful Hound (4-C-L-FH)|Faithful Hound]] (4) · [[Gravitational Wave (8-V-L-GWV)|Gravitational Wave]] (8) · [[Lance of Longinus (8-V-L-LL)|Lance of Longinus]] (8) · [[Tidal Force (4-P-L-TF)|Tidal Force]] (4).


---

## Tactical Assessment

A remote cutting tool that pursues targets around cover while the caster stays back.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 7 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
