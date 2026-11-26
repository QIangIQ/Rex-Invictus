---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/divination
  - source/srd
aliases:
  - "2nd Tier Spell: Locate Animals or Plants"
  - "Locate Animals or Plants"
  - "2-D-L-LAP"
registry_id: 2-D-L-LAP
attribute_code: "2·Div·None·None·Self·Instantaneous"
incantation: "Hipor"
tier: 2
school: Divination
affinity: D
grade: L
pz_total: 17.7
pz_quantum: 951.4
t_e: -1.98
updated: 2026-11-16
---

**Locate Animals or Plants** (`2-D-L-LAP`) is a 2nd Tier working of the [[Divination]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **17.7 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E -1.98 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Divination]]
        - **Locate Animals or Plants** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-D-L-LAP` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Div·None·None·Self·Instantaneous` |
| Incantation | *Hipor* |
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
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A bit of fur from a bloodhound |
| Ritual | yes |
| Practitioner lineages | Bard, Druid, Ranger |

### Mechanism

The field sweeps the surrounding biosphere out to 5 miles and returns direction and distance to the nearest specimen of a named animal or plant kind.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Result (instant info) | `instant info = 1 Pz` | 1.0 |
| Search sweep, 5 mile radius for one round | `0.001 Pz/s * (8046.7 m / 10) * 6 s` | 4.8 |
| Pattern cost | `0.01 × Q2 × (1 + 0.25)` | 11.9 |

| Quantity | Value |
|---|---|
| Effect energy | 5.8 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **17.7 Pz** (26.6 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.0186 |
| Energy-equivalent tier T_E | -1.98 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** ritual.

**Assumptions:** Single sweep over one 6 s round at a 5 mile range.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Locate Animals or Plants (2-D-L-LAP) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Divination | 2 | `0000000000101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Hipor** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihipor* · T4: *Vihipor* · T5: *Tihipor* · T6: *Rihipor* · T7: *Mihipor* · T8: *Nihipor* · T9: *Xyihipor*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]]. This attribute set is shared with other workings, so the glyph carries 1 centre dot(s) to tell it apart.

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 2→0 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#b79244`.

![[Locate Animals or Plants (2-D-L-LAP) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Divination | 0.250 | 0.999 | `#cdff00` (625 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.980 | `#ff0028` (700 nm eq.) | source grid |
| Range | Self | 0.706 | 0.880 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.19): swatch `#d79c68`, measured lines at 0.004, 0.201, 0.251, 0.706. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.25. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·D·None`; the k4 to k6 lines (None, Self, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·D·None` |
| Standard spectrometer detection range | 0.42 km (r = 1 km × √(E/100 Pz)) |
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
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 3.0 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (1.9% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
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

Similar workings: [[Augury (2-D-L-AGR)|Augury]] (2) · [[Detect Thoughts (2-D-L-DT)|Detect Thoughts]] (2) · [[Find Traps (2-D-L-FT)|Find Traps]] (2) · [[Locate Object (2-D-L-LO)|Locate Object]] (2) · [[Radar (2-D-L-RDR)|Radar]] (2) · [[See Invisibility (2-D-L-SIE)|See Invisibility]] (2) · [[Clairvoyance (3-D-L-CLR)|Clairvoyance]] (3) · [[Comprehend Languages (1-D-L-CL)|Comprehend Languages]] (1).


---

## Tactical Assessment

Helps foragers, trackers and scouts find water sources, pack animals or rare medicinal species. It locates kinds, not individuals.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Divination]] · [[Spell Breakdown Procedure]] · [[Parzival]]
