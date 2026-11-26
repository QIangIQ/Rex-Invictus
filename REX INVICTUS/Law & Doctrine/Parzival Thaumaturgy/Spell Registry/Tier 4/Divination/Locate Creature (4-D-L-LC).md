---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/divination
  - source/srd
aliases:
  - "4th Tier Spell: Locate Creature"
  - "Locate Creature"
  - "4-D-L-LC"
registry_id: 4-D-L-LC
attribute_code: "4·Div·None·None·Self·Up to 1 hour"
incantation: "Viporsi"
tier: 4
school: Divination
affinity: D
grade: L
pz_total: 198.6
pz_quantum: 7029.9
t_e: 0.43
updated: 2026-11-16
---

**Locate Creature** (`4-D-L-LC`) is a 4th Tier working of the [[Divination]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **199 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E 0.43 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Divination]]
        - **Locate Creature** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-D-L-LC` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Div·None·None·Self·Up to 1 hour` |
| Incantation | *Viporsi* |
| Affinity | D (Divination) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Divination]] |
| Casting time | 1 action |
| Range | Self |
| Area | single point or target |
| Duration | Up to 1 hour (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A bit of fur from a bloodhound |
| Ritual | no |
| Practitioner lineages | Bard, Cleric, Druid, Paladin, Ranger, Wizard |

### Mechanism

The field holds a directional lock on a known creature or the nearest of a known kind within 1000 ft, including its direction of motion. Running water 10 ft wide blocks the trace, as does a changed form.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Acquisition (instant info) | `instant info = 1 Pz` | 1.0 |
| Direction sense, 1000 ft (upkeep) | `0.001 Pz/s * (304.8 m / 10) * 3600 s` | 110 |
| Pattern cost | `0.01 × Q4 × (1 + 0.25)` | 87.9 |

| Quantity | Value |
|---|---|
| Effect energy | 1.0 Pz |
| Upkeep energy | 110 Pz (0.0305 Pz/s) |
| **Total draw** | **199 Pz** (297.9 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 0.0282 |
| Energy-equivalent tier T_E | 0.43 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** concentration.

**Assumptions:** Range 1000 ft held for 1 hour.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Locate Creature (4-D-L-LC) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 4 | 4 | `0000000001001` |
| k2 School | Divination | 2 | `0000000000101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Up to 1 hour | 12 | `0000000011001` |

### Incantation

Spoken as **Viporsi** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T5: *Tiviporsi* · T6: *Riviporsi* · T7: *Miviporsi* · T8: *Niviporsi* · T9: *Xyiviporsi*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 3→2 | 2 |
| k2 School | 0→11 2→0 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 3→10 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#33c67d`.

![[Locate Creature (4-D-L-LC) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| School | Divination | 0.250 | 0.989 | `#cdff00` (625 nm eq.) | source grid |
| Duration | Up to 1 hour | 0.632 | 0.974 | `#00c0ff` (511 nm eq.) | source grid |
| Range | Self | 0.706 | 0.954 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.19): swatch `#a1d39a`, measured lines at 0.251, 0.401, 0.632, 0.706. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.30. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·D·None`; the k4 to k6 lines (None, Self, Up to 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·D·None` |
| Standard spectrometer detection range | 1.41 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 725 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Light, 2x Extraspection. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 2c 1d 1F 2g 1J` (Beyond, 2x Light, Life, Potential, 2x Extraspection, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 33.1 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 4th Tier quantum of 7,030 Pz (2.8% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 4th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Divination school with aspect lean Beyond, Light, 2x Extraspection. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 4 Workings]] |
| School | [[Divination]] |
| Affinity | [[Divination]] (D) |
| Function | [[Divination and Sensing]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Arcane Eye (4-D-L-AE)|Arcane Eye]] (4) · [[Divination (4-D-L-DVN)|Divination]] (4) · [[Clairvoyance (3-D-L-CLR)|Clairvoyance]] (3) · [[Commune (5-D-L-CMMM)|Commune]] (5) · [[Commune With Nature (5-D-L-CN)|Commune With Nature]] (5) · [[Contact Other Plane (5-D-L-COP)|Contact Other Plane]] (5) · [[Legend Lore (5-D-L-LLG)|Legend Lore]] (5) · [[Scrying (5-D-L-SCR)|Scrying]] (5).


---

## Tactical Assessment

Used in searches for fugitives and missing personnel within a building or compound. A river crossing or a disguise by shape alteration breaks contact.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Divination]] · [[Spell Breakdown Procedure]] · [[Parzival]]
