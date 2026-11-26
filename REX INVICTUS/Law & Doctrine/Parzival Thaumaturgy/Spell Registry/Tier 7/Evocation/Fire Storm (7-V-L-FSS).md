---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-7
  - spell/evocation
  - source/srd
aliases:
  - "7th Tier Spell: Fire Storm"
  - "Fire Storm"
  - "7-V-L-FSS"
registry_id: 7-V-L-FSS
attribute_code: "7·Evo·Fire·cube (100)·150 feet·Instantaneous"
incantation: "Muire-Binosin"
tier: 7
school: Evocation
affinity: V
grade: L
pz_total: 18689.6
pz_quantum: 141200.1
t_e: 4.98
updated: 2026-11-16
---

**Fire Storm** (`7-V-L-FSS`) is a 7th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **18,690 Pz** against a slot quantum of 141,200 Pz, which puts its energy-equivalent tier at T_E 4.98 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 7 Workings]]
      - [[Evocation]]
        - **Fire Storm** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `7-V-L-FSS` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `7·Evo·Fire·cube (100)·150 feet·Instantaneous` |
| Incantation | *Muire-Binosin* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 7th Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 150 feet |
| Area | cube (100) |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 7d10 fire (mean 38.5) |
| Injury by tier | T7: 7d10 |
| Resistance check | agility; on success: half injury |
| Practitioner lineages | Cleric, Druid, Sorcerer |

### Mechanism

Sheets of flame fill up to ten connected 3 m cells, delivering an intense heat pulse to everything inside while optionally sparing plant life.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| ten 10-ft cubes of flame, 7d10=38.5 | `38.5 HP * kappa_fire 0.7 * S/A_c (10 x 4*pi*(0.62*10 ft*0.3048)^2 = 44.9 m^2 / 0.7)` | 17,278 |
| Pattern cost | `0.01 × Q7 × (1 + 0.00)` | 1,412 |

| Quantity | Value |
|---|---|
| Effect energy | 17,278 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **18,690 Pz** (28,034.4 kJ) |
| Slot quantum Q7 | 141,200 Pz |
| Field gain (draw / quantum) | 0.132 |
| Energy-equivalent tier T_E | 4.98 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** 7d10 avg 38.5 fire; exposure surface summed per cube (10 cubes).

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Fire Storm (7-V-L-FSS) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 7 | 7 | `0000000001111` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Fire | 3 | `0000000000111` |
| k4 Area | cube (100) | 6 | `0000000001101` |
| k5 Range | 150 feet | 4 | `0000000001001` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Muire-Binosin** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T8: *Nimuire-Binosin* · T9: *Xyimuire-Binosin*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 3→2 | 4 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 | 3 |
| k4 Area | 0→9 2→11 3→12 | 3 |
| k5 Range | 0→8 3→11 | 2 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#8cb14d`.

![[Fire Storm (7-V-L-FSS) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 7 | 0.700 | 1.000 | `#005eff` (490 nm eq.) | source grid |
| Damage | Fire | 0.286 | 0.918 | `#9cff00` (614 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.980 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.783 | `#ff0028` (700 nm eq.) | source grid |
| Area | cube (100) | 0.167 | 0.867 | `#ffb900` (650 nm eq.) | source grid |
| Range | 150 feet | 0.235 | 0.898 | `#e3ff00` (629 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.17): swatch `#97c697`, measured lines at 0.004, 0.167, 0.236, 0.286, 0.501, 0.701. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.27. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `7·V·Fire`; the k4 to k6 lines (cube (100), 150 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `7·V·Fire` |
| Standard spectrometer detection range | 13.67 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 7,060 Pz (0.05 × Q7) |
| Counter drawn cold (all six layers) | 14,120 Pz (0.10 × Q7) |
| Unravel after completion | 14,120 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Energy, Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `2b 1c 3f 2j` (2x Heat, Light, 3x Energy, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 3,115 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 7th Tier quantum of 141,200 Pz (13.2% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 7th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 7 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Area Destruction]] |
| Element | [[Fire Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Delayed Blast Fireball (7-V-M-DBF)|Delayed Blast Fireball]] (7) · [[Supernova (8-V-L-SPR)|Supernova]] (8) · [[Eruption (9-V-M-ERP)|Eruption]] (9) · [[Flame Strike (5-V-L-FSM)|Flame Strike]] (5) · [[Meteor Swarm (9-V-L-MST)|Meteor Swarm]] (9) · [[Thermonuclear Fireball (9-P-L-TFE)|Thermonuclear Fireball]] (9) · [[Fire Shield (4-V-L-FSR)|Fire Shield]] (4) · [[Incendiary Cloud (8-C-M-IC)|Incendiary Cloud]] (8).


---

## Tactical Assessment

A shapeable area-denial weapon that can follow a trench, a corridor or a column of vehicles exactly, with no blast spill onto adjacent friendly positions.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 7 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
