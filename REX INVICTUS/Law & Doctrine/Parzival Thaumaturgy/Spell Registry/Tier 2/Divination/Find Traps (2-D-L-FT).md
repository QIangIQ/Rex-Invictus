---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/divination
  - source/srd
aliases:
  - "2nd Tier Spell: Find Traps"
  - "Find Traps"
  - "2-D-L-FT"
registry_id: 2-D-L-FT
attribute_code: "2·Div·None·None·120 feet·Instantaneous"
incantation: "Himul"
tier: 2
school: Divination
affinity: D
grade: L
pz_total: 10.5
pz_quantum: 951.4
t_e: -2.50
updated: 2026-11-16
---

**Find Traps** (`2-D-L-FT`) is a 2nd Tier working of the [[Divination]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **10.5 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E -2.50 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Divination]]
        - **Find Traps** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-D-L-FT` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Div·None·None·120 feet·Instantaneous` |
| Incantation | *Himul* |
| Affinity | D (Divination) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Divination]] |
| Casting time | 1 action |
| Range | 120 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Cleric, Druid, Ranger |

### Mechanism

A brief divination sweep across line of sight within 36 m registers deliberate harmful mechanisms and wards and returns their general nature, without positions.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| trap-presence divination | `instant info` | 1.0 |
| line-of-sight sweep | `0.001 Pz/s * (36.6 m / 10) * 6 s` | 0.0219 |
| Pattern cost | `0.01 × Q2 × (1 + 0.00)` | 9.5 |

| Quantity | Value |
|---|---|
| Effect energy | 1.0 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **10.5 Pz** (15.8 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.0111 |
| Energy-equivalent tier T_E | -2.50 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Instant information 1 Pz plus a one-round sweep at the divination rate over 120 ft.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Find Traps (2-D-L-FT) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Divination | 2 | `0000000000101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 120 feet | 3 | `0000000000111` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Himul** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihimul* · T4: *Vihimul* · T5: *Tihimul* · T6: *Rihimul* · T7: *Mihimul* · T8: *Nihimul* · T9: *Xyihimul*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 2→0 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#f2ad09`.

![[Find Traps (2-D-L-FT) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Divination | 0.250 | 0.999 | `#cdff00` (625 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.980 | `#ff0028` (700 nm eq.) | source grid |
| Range | 120 feet | 0.176 | 1.000 | `#ffc900` (647 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.17): swatch `#ff904d`, measured lines at 0.004, 0.177, 0.201, 0.251. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.02. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·D·None`; the k4 to k6 lines (None, 120 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·D·None` |
| Standard spectrometer detection range | 0.32 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 95.1 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Light, 2x Extraspection. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 2c 1d 1F 2g 1J` (Beyond, 2x Light, Life, Potential, 2x Extraspection, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1.8 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (1.1% of it). |
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

Similar workings: [[Augury (2-D-L-AGR)|Augury]] (2) · [[Detect Thoughts (2-D-L-DT)|Detect Thoughts]] (2) · [[Locate Animals or Plants (2-D-L-LAP)|Locate Animals or Plants]] (2) · [[Locate Object (2-D-L-LO)|Locate Object]] (2) · [[Radar (2-D-L-RDR)|Radar]] (2) · [[See Invisibility (2-D-L-SIE)|See Invisibility]] (2) · [[Clairvoyance (3-D-L-CLR)|Clairvoyance]] (3) · [[Comprehend Languages (1-D-L-CL)|Comprehend Languages]] (1).


---

## Tactical Assessment

A quick go or no-go check before entering a corridor, vehicle bay or doorway; it flags mines, booby traps and ward glyphs but not structural decay.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Divination]] · [[Spell Breakdown Procedure]] · [[Parzival]]
