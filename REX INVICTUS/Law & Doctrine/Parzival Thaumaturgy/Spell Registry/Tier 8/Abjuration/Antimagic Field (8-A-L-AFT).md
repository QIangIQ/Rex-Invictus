---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-8
  - spell/abjuration
  - source/srd
aliases:
  - "8th Tier Spell: Antimagic Field"
  - "Antimagic Field"
  - "8-A-L-AFT"
registry_id: 8-A-L-AFT
attribute_code: "8·Abj·None·sphere (10)·Self·Up to 1 hour"
incantation: "Na’-Seporsi"
tier: 8
school: Abjuration
affinity: A
grade: L
pz_total: 432991.9
pz_quantum: 383821.6
t_e: 8.12
updated: 2026-11-16
---

**Antimagic Field** (`8-A-L-AFT`) is a 8th Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **432,992 Pz** against a slot quantum of 383,822 Pz, which puts its energy-equivalent tier at T_E 8.12 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 8 Workings]]
      - [[Abjuration]]
        - **Antimagic Field** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `8-A-L-AFT` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `8·Abj·None·sphere (10)·Self·Up to 1 hour` |
| Incantation | *Na’-Seporsi* |
| Affinity | A (Abjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 8th Tier |
| School | [[Abjuration]] |
| Casting time | 1 action |
| Range | Self |
| Area | sphere (10) |
| Duration | Up to 1 hour (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A pinch of powdered iron or iron filings |
| Ritual | no |
| Practitioner lineages | Cleric, Wizard |

### Mechanism

A 3 m radius sphere around the caster cancels ambient field return, suppressing workings, summoned bodies, enchanted items and translocation inside it.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| field charging | `118.61 m^3 * 10 Pz/m^3` | 1,186 |
| suppression upkeep | `118.61 m^3 * 1 Pz/s/m^3 * 3600 s` | 427,008 |
| Pattern cost | `0.01 × Q8 × (1 + 0.25)` | 4,798 |

| Quantity | Value |
|---|---|
| Effect energy | 1,186 Pz |
| Upkeep energy | 427,008 Pz (119 Pz/s) |
| **Total draw** | **432,992 Pz** (649,487.8 kJ) |
| Slot quantum Q8 | 383,822 Pz |
| Field gain (draw / quantum) | 1.13 |
| Energy-equivalent tier T_E | 8.12 |
| Handling points | 0.25 |
| Grade score | 0.31 → L |

**Handling flags:** concentration.

**Assumptions:** Order-of-magnitude estimate: 1 Pz/s per cubic metre of nulled volume for 1 h plus 10 Pz/m^3 to establish; no physical analogue exists.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Antimagic Field (8-A-L-AFT) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 8 | 8 | `0000000010001` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (10) | 27 | `0000000110111` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Up to 1 hour | 12 | `0000000011001` |

### Incantation

Spoken as **Na’-Seporsi** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T9: *Xyina’-Seporsi*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 4→3 | 2 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 2→11 4→0 5→1 | 5 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 3→10 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#303fdd`.

![[Antimagic Field (8-A-L-AFT) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 8 | 0.800 | 1.000 | `#2900ff` (460 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.726 | `#ff0028` (700 nm eq.) | source grid |
| Duration | Up to 1 hour | 0.632 | 0.986 | `#00c0ff` (511 nm eq.) | source grid |
| Area | sphere (10) | 0.750 | 0.999 | `#0017ff` (475 nm eq.) | source grid |
| Range | Self | 0.706 | 0.996 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.13): swatch `#429bc3`, measured lines at 0.006, 0.632, 0.706, 0.751, 0.801. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 5.64. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `8·A·None`; the k4 to k6 lines (sphere (10), Self, Up to 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `8·A·None` |
| Standard spectrometer detection range | 65.80 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 19,191 Pz (0.05 × Q8) |
| Counter drawn cold (all six layers) | 38,382 Pz (0.10 × Q8) |
| Unravel after completion | 123,784 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 72,165 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 1.13 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 8th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 8th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 8 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Negation and Counterspell]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Mind Blank (8-A-L-MB)|Mind Blank]] (8) · [[Forbiddance (6-A-L-FRBB)|Forbiddance]] (6) · [[Glibness (8-T-L-GLB)|Glibness]] (8) · [[Globe of Invulnerability (6-A-L-GIO)|Globe of Invulnerability]] (6) · [[Antilife Shell (5-A-L-ASI)|Antilife Shell]] (5) · [[Dispel Evil and Good (5-A-L-DEGP)|Dispel Evil and Good]] (5) · [[Arcane Insulation (4-A-L-AI)|Arcane Insulation]] (4) · [[Banishment (4-A-M-BNS)|Banishment]] (4).


---

## Tactical Assessment

A mobile null zone that strips enemy casters and enchanted equipment, and blocks teleport insertions into a command post.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 8 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
