---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/illusion
  - source/srd
aliases:
  - "3rd Tier Spell: Hypnotic Pattern"
  - "Hypnotic Pattern"
  - "3-I-L-HPP"
registry_id: 3-I-L-HPP
attribute_code: "3·Ill·None·None·120 feet·Up to 1 minute"
incantation: "Laimulse"
tier: 3
school: Illusion
affinity: I
grade: L
pz_total: 67.5
pz_quantum: 2586.2
t_e: -0.65
updated: 2026-11-16
---

**Hypnotic Pattern** (`3-I-L-HPP`) is a 3rd Tier working of the [[Illusion]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **67.5 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E -0.65 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Illusion]]
        - **Hypnotic Pattern** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-I-L-HPP` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Ill·None·None·120 feet·Up to 1 minute` |
| Incantation | *Laimulse* |
| Affinity | I (Illusion) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Illusion]] |
| Casting time | 1 action |
| Range | 120 feet |
| Area | single point or target |
| Duration | Up to 1 minute (concentration) |
| Components | somatic (glyph kata), material focus. Material: A glowing stick of incense or a crystal vial filled with phosphorescent material |
| Ritual | no |
| Resistance check | will; on success: no effect |
| Practitioner lineages | Bard, Sorcerer, Warlock, Wizard |

### Mechanism

A brief luminous interference pattern fills a 30 ft cube and imprints a looping visual stimulus on every viewer's attention circuits. The field then holds those viewers in a motionless stupor until injury or a shove breaks the loop.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Pattern flash (instant info) | `instant info = 1 Pz` | 1.0 |
| Illusion volume, 1 round flash | `0.002 Pz/s * (764.6 m^3/1000) * 6 s` | 0.00918 |
| Stupor hold on 6 creatures (upkeep) | `0.005 Pz/s * 6 * 60 s` | 1.8 |
| Pattern cost | `0.01 × Q3 × (1 + 1.50)` | 64.7 |

| Quantity | Value |
|---|---|
| Effect energy | 1.0 Pz |
| Upkeep energy | 1.8 Pz (0.03 Pz/s) |
| **Total draw** | **67.5 Pz** (101.2 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 0.0261 |
| Energy-equivalent tier T_E | -0.65 |
| Handling points | 1.50 |
| Grade score | 0.50 → L |

**Handling flags:** concentration, fragile, save or suck.

**Assumptions:** 30 ft cube = 764.6 m^3; flash lasts one 6 s round; 6 creatures held for the full 1 minute.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Hypnotic Pattern (3-I-L-HPP) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Illusion | 5 | `0000000001011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 120 feet | 3 | `0000000000111` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Laimulse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vilaimulse* · T5: *Tilaimulse* · T6: *Rilaimulse* · T7: *Milaimulse* · T8: *Nilaimulse* · T9: *Xyilaimulse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 1→12 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#65c17b`.

![[Hypnotic Pattern (3-I-L-HPP) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| School | Illusion | 0.625 | 0.949 | `#00c5ff` (512 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.929 | `#0074ff` (495 nm eq.) | source grid |
| Range | 120 feet | 0.176 | 0.992 | `#ffc900` (647 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.19): swatch `#90cd9f`, measured lines at 0.177, 0.300, 0.626, 0.685. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.83. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·I·None`; the k4 to k6 lines (None, 120 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·I·None` |
| Standard spectrometer detection range | 0.82 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 259 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Light, Introspection, 2x Flexibility. The working vector used by [[Recast Tension and Combination Affinity]] is `2c 1d 1F 1G 2h 1J` (2x Light, Life, Potential, Introspection, 2x Flexibility, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 11.2 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 3rd Tier quantum of 2,586 Pz (2.6% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Illusion school with aspect lean Light, Introspection, 2x Flexibility. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Illusion]] |
| Affinity | [[Illusion]] (I) |
| Function | [[Mind and Will]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Fear (3-I-L-FEA)|Fear]] (3) · [[Phantasmal Killer (4-I-L-PK)|Phantasmal Killer]] (4) · [[Beacon of Hope (3-A-L-BHA)|Beacon of Hope]] (3) · [[Bestow Curse (3-N-L-BC)|Bestow Curse]] (3) · [[Dream (5-I-L-DRM)|Dream]] (5) · [[Spirit Guardians (3-C-M-SGR)|Spirit Guardians]] (3) · [[Calm Emotions (2-E-L-CE)|Calm Emotions]] (2) · [[Compulsion (4-E-L-CMP)|Compulsion]] (4).


---

## Tactical Assessment

Effective against massed infantry or crowds without optical filtering; one burst can freeze a squad in place. Sensor-protected troops, drones and armoured optics defeat it.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Illusion]] · [[Spell Breakdown Procedure]] · [[Parzival]]
