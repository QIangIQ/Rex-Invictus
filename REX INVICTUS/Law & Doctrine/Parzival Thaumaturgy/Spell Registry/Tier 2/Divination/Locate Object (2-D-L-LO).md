---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/divination
  - source/srd
aliases:
  - "2nd Tier Spell: Locate Object"
  - "Locate Object"
  - "2-D-L-LO"
registry_id: 2-D-L-LO
attribute_code: "2·Div·None·None·Self·Up to 10 minutes"
incantation: "Hiporly"
tier: 2
school: Divination
affinity: D
grade: L
pz_total: 31.2
pz_quantum: 951.4
t_e: -1.42
updated: 2026-11-16
---

**Locate Object** (`2-D-L-LO`) is a 2nd Tier working of the [[Divination]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **31.2 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E -1.42 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Divination]]
        - **Locate Object** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-D-L-LO` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Div·None·None·Self·Up to 10 minutes` |
| Incantation | *Hiporly* |
| Affinity | D (Divination) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Divination]] |
| Casting time | 1 action |
| Range | Self |
| Area | single point or target |
| Duration | Up to 10 minutes (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A forked twig |
| Ritual | no |
| Practitioner lineages | Bard, Cleric, Druid, Paladin, Ranger, Wizard |

### Mechanism

The field holds a directional lock on a known object or the nearest object of a named kind within 1000 ft. Any lead sheet in the path blocks the trace.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Acquisition (instant info) | `instant info = 1 Pz` | 1.0 |
| Direction sense, 1000 ft (upkeep) | `0.001 Pz/s * (304.8 m / 10) * 600 s` | 18.3 |
| Pattern cost | `0.01 × Q2 × (1 + 0.25)` | 11.9 |

| Quantity | Value |
|---|---|
| Effect energy | 1.0 Pz |
| Upkeep energy | 18.3 Pz (0.0305 Pz/s) |
| **Total draw** | **31.2 Pz** (46.8 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.0328 |
| Energy-equivalent tier T_E | -1.42 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** concentration.

**Assumptions:** Range 1000 ft held for 10 minutes.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Locate Object (2-D-L-LO) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Divination | 2 | `0000000000101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Up to 10 minutes | 15 | `0000000011111` |

### Incantation

Spoken as **Hiporly** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihiporly* · T4: *Vihiporly* · T5: *Tihiporly* · T6: *Rihiporly* · T7: *Mihiporly* · T8: *Nihiporly* · T9: *Xyihiporly*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 2→0 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 2→9 3→10 4→11 | 5 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#829875`.

![[Locate Object (2-D-L-LO) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Divination | 0.250 | 0.999 | `#cdff00` (625 nm eq.) | source grid |
| Duration | Up to 10 minutes | 0.789 | 0.841 | `#1e00ff` (463 nm eq.) | source grid |
| Range | Self | 0.706 | 0.880 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.19): swatch `#b8ab85`, measured lines at 0.201, 0.251, 0.706, 0.790. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.49. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·D·None`; the k4 to k6 lines (None, Self, Up to 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·D·None` |
| Standard spectrometer detection range | 0.56 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 98.8 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Light, 2x Extraspection. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 2c 1d 1F 2g 1J` (Beyond, 2x Light, Life, Potential, 2x Extraspection, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 5.2 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (3.3% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Divination school with aspect lean Beyond, Light, 2x Extraspection. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Divination]] |
| Affinity | [[Divination]] (D) |
| Function | [[Divination and Sensing]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Augury (2-D-L-AGR)|Augury]] (2) · [[Detect Thoughts (2-D-L-DT)|Detect Thoughts]] (2) · [[Find Traps (2-D-L-FT)|Find Traps]] (2) · [[Locate Animals or Plants (2-D-L-LAP)|Locate Animals or Plants]] (2) · [[Radar (2-D-L-RDR)|Radar]] (2) · [[See Invisibility (2-D-L-SIE)|See Invisibility]] (2) · [[Clairvoyance (3-D-L-CLR)|Clairvoyance]] (3) · [[Comprehend Languages (1-D-L-CL)|Comprehend Languages]] (1).


---

## Tactical Assessment

Finds caches, stolen equipment and dropped items in a search area. Lead-lined containers defeat it.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Divination]] · [[Spell Breakdown Procedure]] · [[Parzival]]
