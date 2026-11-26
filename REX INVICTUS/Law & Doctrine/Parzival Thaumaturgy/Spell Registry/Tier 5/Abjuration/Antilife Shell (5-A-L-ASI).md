---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/abjuration
  - source/srd
aliases:
  - "5th Tier Spell: Antilife Shell"
  - "Antilife Shell"
  - "5-A-L-ASI"
registry_id: 5-A-L-ASI
attribute_code: "5·Abj·None·sphere (10)·Self·Up to 1 hour"
incantation: "Ta’-Seporsi"
tier: 5
school: Abjuration
affinity: A
grade: L
pz_total: 553.6
pz_quantum: 19109.4
t_e: 1.46
updated: 2026-11-16
---

**Antilife Shell** (`5-A-L-ASI`) is a 5th Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **554 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 1.46 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Abjuration]]
        - **Antilife Shell** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-A-L-ASI` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Abj·None·sphere (10)·Self·Up to 1 hour` |
| Incantation | *Ta’-Seporsi* |
| Affinity | A (Abjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Abjuration]] |
| Casting time | 1 action |
| Range | Self |
| Area | sphere (10) |
| Duration | Up to 1 hour (concentration) |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Druid |

### Mechanism

A 3 m radius barrier around the caster refuses passage to living creatures, while ranged attacks and workings still pass through.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| melee absorption | `150 points prevented * 0.20 Pz/point` | 30.0 |
| repulsion of charges | `10 contacts * 0.5*80 kg*(9 m/s)^2 / 1500` | 21.6 |
| barrier upkeep | `0.005 Pz/s * 4 creatures held off * 3600 s` | 72.0 |
| Pattern cost | `0.01 × Q5 × (1 + 1.25)` | 430 |

| Quantity | Value |
|---|---|
| Effect energy | 51.6 Pz |
| Upkeep energy | 72.0 Pz (0.02 Pz/s) |
| **Total draw** | **554 Pz** (830.3 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 0.029 |
| Energy-equivalent tier T_E | 1.46 |
| Handling points | 1.25 |
| Grade score | 0.25 → L |

**Handling flags:** concentration, fragile.

**Assumptions:** 10 rounds of 15 points per round of melee prevented; 10 charging contacts at 9 m/s; 4 creatures held for 1 h.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Antilife Shell (5-A-L-ASI) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (10) | 27 | `0000000110111` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Up to 1 hour | 12 | `0000000011001` |

### Incantation

Spoken as **Ta’-Seporsi** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Rita’-Seporsi* · T7: *Mita’-Seporsi* · T8: *Nita’-Seporsi* · T9: *Xyita’-Seporsi*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 2→11 4→0 5→1 | 5 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 3→10 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#2e72bf`.

![[Antilife Shell (5-A-L-ASI) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.882 | `#ff0028` (700 nm eq.) | source grid |
| Duration | Up to 1 hour | 0.632 | 0.991 | `#00c0ff` (511 nm eq.) | source grid |
| Area | sphere (10) | 0.750 | 0.969 | `#0017ff` (475 nm eq.) | source grid |
| Range | Self | 0.706 | 0.979 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.13): swatch `#6cb9a6`, measured lines at 0.007, 0.501, 0.632, 0.706, 0.750. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.74. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·A·None`; the k4 to k6 lines (sphere (10), Self, Up to 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·A·None` |
| Standard spectrometer detection range | 2.35 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 1,925 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 92.3 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 5th Tier quantum of 19,109 Pz (2.9% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 5th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 5 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Negation and Counterspell]], [[Necromantic and Soul Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Dispel Evil and Good (5-A-L-DEGP)|Dispel Evil and Good]] (5) · [[Arcane Insulation (4-A-L-AI)|Arcane Insulation]] (4) · [[Banishment (4-A-M-BNS)|Banishment]] (4) · [[Forbiddance (6-A-L-FRBB)|Forbiddance]] (6) · [[Glibness (8-T-L-GLB)|Glibness]] (8) · [[Globe of Invulnerability (6-A-L-GIO)|Globe of Invulnerability]] (6) · [[Private Sanctum (4-A-L-PSI)|Private Sanctum]] (4) · [[Beacon of Hope (3-A-L-BHA)|Beacon of Hope]] (3).


---

## Tactical Assessment

A personal exclusion zone against boarders and close assault; it collapses if the caster drives an enemy into it.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
