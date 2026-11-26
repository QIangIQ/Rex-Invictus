---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/evocation
  - source/srd
aliases:
  - "1st Tier Spell: Burning Hands"
  - "Burning Hands"
  - "1-V-L-BH"
registry_id: 1-V-L-BH
attribute_code: "1·Evo·Fire·cone (15)·Self·Instantaneous"
incantation: "Suire-Nupor"
tier: 1
school: Evocation
affinity: V
grade: L
pz_total: 149.7
pz_quantum: 350.0
t_e: 0.15
updated: 2026-11-16
---

**Burning Hands** (`1-V-L-BH`) is a 1st Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **150 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E 0.15 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Evocation]]
        - **Burning Hands** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-V-L-BH` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Evo·Fire·cone (15)·Self·Instantaneous` |
| Incantation | *Suire-Nupor* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | Self |
| Area | cone (15) |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 3d6 fire (mean 10.5) |
| Injury by tier | T1: 3d6, T2: 4d6, T3: 5d6, T4: 6d6, T5: 7d6, T6: 8d6, T7: 9d6, T8: 10d6, T9: 11d6 |
| Resistance check | agility; on success: half injury |
| Practitioner lineages | Sorcerer, Wizard |

### Mechanism

A thin fan of flame sprays from the caster's hands over a 4.6 m cone and ignites loose flammables.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| flame sheet | `10.5 HP * 0.7 Pz/HP (fire) * (cone 15 ft: 0.666*4.572^2 = 13.922 m^2 / 0.7 m^2)` | 146 |
| Pattern cost | `0.01 × Q1 × (1 + 0.00)` | 3.5 |

| Quantity | Value |
|---|---|
| Effect energy | 146 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **150 Pz** (224.5 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.428 |
| Energy-equivalent tier T_E | 0.15 |
| Handling points | 0.00 |
| Grade score | -0.42 → L |

**Handling flags:** none.

**Assumptions:** Average 10.5 injury; one-shot.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Burning Hands (1-V-L-BH) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Fire | 3 | `0000000000111` |
| k4 Area | cone (15) | 1 | `0000000000011` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Suire-Nupor** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisuire-Nupor* · T3: *Lisuire-Nupor* · T4: *Visuire-Nupor* · T5: *Tisuire-Nupor* · T6: *Risuire-Nupor* · T7: *Misuire-Nupor* · T8: *Nisuire-Nupor* · T9: *Xyisuire-Nupor*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 | 3 |
| k4 Area | 0→9 1→10 | 2 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#9f7142`.

![[Burning Hands (1-V-L-BH) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| Damage | Fire | 0.286 | 0.983 | `#9cff00` (614 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.923 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.995 | `#ff0028` (700 nm eq.) | source grid |
| Area | cone (15) | 0.028 | 0.997 | `#ff0003` (692 nm eq.) | source grid |
| Range | Self | 0.706 | 0.832 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.14): swatch `#b99d70`, measured lines at 0.004, 0.028, 0.101, 0.286, 0.501, 0.706. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.18. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·V·Fire`; the k4 to k6 lines (cone (15), Self, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·V·Fire` |
| Standard spectrometer detection range | 1.22 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.0 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Energy, Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `2b 1c 3f 2j` (2x Heat, Light, 3x Energy, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 24.9 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (42.8% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Area Destruction]] |
| Element | [[Fire Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Kilonova (1-V-M-KLN)|Kilonova]] (1) · [[Galaxy Whirl (2-V-L-GWL)|Galaxy Whirl]] (2) · [[Fireball (3-V-M-FRB)|Fireball]] (3) · [[Fire Shield (4-V-L-FSR)|Fire Shield]] (4) · [[Wall of Fire (4-V-M-WF)|Wall of Fire]] (4) · [[Blast (1-V-L-BLS)|Blast]] (1) · [[Faerie Fire (1-V-L-FF)|Faerie Fire]] (1) · [[Flame Strike (5-V-L-FSM)|Flame Strike]] (5).


---

## Tactical Assessment

Short-range clearing of rooms and trenches.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
