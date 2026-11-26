---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-7
  - spell/transmutation
  - source/srd
aliases:
  - "7th Tier Spell: Reverse Gravity"
  - "Reverse Gravity"
  - "7-T-L-RG"
registry_id: 7-T-L-RG
attribute_code: "7·Tra·None·cylinder (50)·100 feet·Up to 1 minute"
incantation: "Mie’-Xisponse"
tier: 7
school: Transmutation
affinity: T
grade: L
pz_total: 2354.2
pz_quantum: 141200.1
t_e: 2.91
updated: 2026-11-16
---

**Reverse Gravity** (`7-T-L-RG`) is a 7th Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **2,354 Pz** against a slot quantum of 141,200 Pz, which puts its energy-equivalent tier at T_E 2.91 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 7 Workings]]
      - [[Transmutation]]
        - **Reverse Gravity** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `7-T-L-RG` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `7·Tra·None·cylinder (50)·100 feet·Up to 1 minute` |
| Incantation | *Mie’-Xisponse* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 7th Tier |
| School | [[Transmutation]] |
| Casting time | 1 action |
| Range | 100 feet |
| Area | cylinder (50) |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A lodestone and iron filings |
| Ritual | no |
| Resistance check | agility; on success: other |
| Practitioner lineages | Druid, Sorcerer, Wizard |

### Mechanism

Local gravity inside a tall cylinder is inverted, lifting all unanchored mass to the top or into any ceiling. When the field ends the mass falls back.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| raise 8 Medium creatures + 500 kg loose objects 100 ft | `(8*80+500)*g*(100*ft)/1500` | 227 |
| [upkeep] hold 1140 kg at the top, 1 min | `0.02*1140*g*60/1500` | 8.9 |
| Pattern cost | `0.01 × Q7 × (1 + 0.50)` | 2,118 |

| Quantity | Value |
|---|---|
| Effect energy | 227 Pz |
| Upkeep energy | 8.9 Pz (0.149 Pz/s) |
| **Total draw** | **2,354 Pz** (3,531.3 kJ) |
| Slot quantum Q7 | 141,200 Pz |
| Field gain (draw / quantum) | 0.0167 |
| Energy-equivalent tier T_E | 2.91 |
| Handling points | 0.50 |
| Grade score | -0.50 → L |

**Handling flags:** concentration, save or suck.

**Assumptions:** 8 creatures plus 500 kg of loose objects; full 100 ft lift; hover upkeep at 0.02 m*g.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Reverse Gravity (7-T-L-RG) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 7 | 7 | `0000000001111` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | cylinder (50) | 21 | `0000000101011` |
| k5 Range | 100 feet | 2 | `0000000000101` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Mie’-Xisponse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T8: *Nimie’-Xisponse* · T9: *Xyimie’-Xisponse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 3→2 | 4 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 3→12 5→1 | 4 |
| k5 Range | 0→8 2→10 | 2 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#4b75d1`.

![[Reverse Gravity (7-T-L-RG) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 7 | 0.700 | 1.000 | `#005eff` (490 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.985 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 1.000 | `#0074ff` (495 nm eq.) | source grid |
| Area | cylinder (50) | 0.583 | 0.993 | `#00fffc` (525 nm eq.) | source grid |
| Range | 100 feet | 0.118 | 0.844 | `#ff7800` (665 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.22): swatch `#4c9cd1`, measured lines at 0.118, 0.584, 0.685, 0.701, 0.876. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.37. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `7·T·None`; the k4 to k6 lines (cylinder (50), 100 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `7·T·None` |
| Standard spectrometer detection range | 4.85 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 7,060 Pz (0.05 × Q7) |
| Counter drawn cold (all six layers) | 14,120 Pz (0.10 × Q7) |
| Unravel after completion | 14,122 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 392 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 7th Tier quantum of 141,200 Pz (1.7% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 7th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 7 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Movement and Flight]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Sequester (7-T-L-SQS)|Sequester]] (7) · [[Wind Walk (6-T-L-WWD)|Wind Walk]] (6) · [[Telekinesis (5-P-L-TLK)|Telekinesis]] (5) · [[Freefall (4-T-L-FRF)|Freefall]] (4) · [[Etherealness (7-T-L-ETH)|Etherealness]] (7) · [[Fly (3-T-L-FLY)|Fly]] (3) · [[Gaseous Form (3-T-M-GF)|Gaseous Form]] (3) · [[Haste (3-T-L-HST)|Haste]] (3).


---

## Tactical Assessment

Strips troops from the ground, smashes them into ceilings and drops them again, good against vehicles in hangars as well.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 7 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
