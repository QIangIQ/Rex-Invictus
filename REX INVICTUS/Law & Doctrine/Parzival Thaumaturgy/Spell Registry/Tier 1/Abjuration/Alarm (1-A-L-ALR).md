---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/abjuration
  - source/srd
aliases:
  - "1st Tier Spell: Alarm"
  - "Alarm"
  - "1-A-L-ALR"
registry_id: 1-A-L-ALR
attribute_code: "1·Abj·None·cube (20)·30 feet·8 hours"
incantation: "Sa’-Bousiniy"
tier: 1
school: Abjuration
affinity: A
grade: L
pz_total: 32.6
pz_quantum: 350.0
t_e: -1.37
updated: 2026-11-16
---

**Alarm** (`1-A-L-ALR`) is a 1st Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **32.6 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -1.37 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Abjuration]]
        - **Alarm** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-A-L-ALR` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Abj·None·cube (20)·30 feet·8 hours` |
| Incantation | *Sa’-Bousiniy* |
| Affinity | A (Abjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Abjuration]] |
| Casting time | 1 minute |
| Range | 30 feet |
| Area | cube (20) |
| Duration | 8 hours |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A tiny bell and a piece of fine silver wire |
| Ritual | yes |
| Practitioner lineages | Ranger, Wizard |

### Mechanism

A sensing lattice is laid across a doorway or a cube up to 6 m on a side and reports any intrusion to the caster mentally or as a bell tone.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| instant information | `1 * 1 Pz` | 1.0 |
| audible bell | `~1 W acoustic * 10 s / 1500` | 0.0067 |
| ward sensing upkeep | `0.001 Pz/s * (9.14 m / 10) * 28800 s` | 26.3 |
| Pattern cost | `0.01 × Q1 × (1 + 0.50)` | 5.2 |

| Quantity | Value |
|---|---|
| Effect energy | 1.0 Pz |
| Upkeep energy | 26.3 Pz (0.0009 Pz/s) |
| **Total draw** | **32.6 Pz** (48.9 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.0931 |
| Energy-equivalent tier T_E | -1.37 |
| Handling points | 0.50 |
| Grade score | -0.50 → L |

**Handling flags:** ritual, long cast.

**Assumptions:** Sensing range taken as the 9.14 m anchoring distance; one trigger per night; bell tone about 1 W for 10 s; 8 h duration.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Alarm (1-A-L-ALR) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | cube (20) | 9 | `0000000010011` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | 8 hours | 8 | `0000000010001` |

### Incantation

Spoken as **Sa’-Bousiniy** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisa’-Bousiniy* · T3: *Lisa’-Bousiniy* · T4: *Visa’-Bousiniy* · T5: *Tisa’-Bousiniy* · T6: *Risa’-Bousiniy* · T7: *Misa’-Bousiniy* · T8: *Nisa’-Bousiniy* · T9: *Xyisa’-Bousiniy*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 4→0 | 3 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 4→11 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#aeaa1b`.

![[Alarm (1-A-L-ALR) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.995 | `#ff0028` (700 nm eq.) | source grid |
| Duration | 8 hours | 0.474 | 0.933 | `#00ff66` (558 nm eq.) | source grid |
| Area | cube (20) | 0.250 | 0.989 | `#cdff00` (625 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.981 | `#91ff00` (612 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.13): swatch `#e87b48`, measured lines at 0.007, 0.101, 0.251, 0.295, 0.474. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.51. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·A·None`; the k4 to k6 lines (cube (20), 30 feet, 8 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·A·None` |
| Standard spectrometer detection range | 0.57 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 40.3 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 5.4 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (9.3% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Linking and Triggers]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Tripwire (0-A-L-TRP)|Tripwire]] (0) · [[Glyph of Warding (3-A-H-GWY)|Glyph of Warding]] (3) · [[Magic Link (1-P-L-MLK)|Magic Link]] (1) · [[Magic Mouth (2-I-L-MMG)|Magic Mouth]] (2) · [[Transfiguration Inheritance (2-T-L-TI)|Transfiguration Inheritance]] (2) · [[Arcane Ward (1-A-L-AW)|Arcane Ward]] (1) · [[Faraday Cage (1-A-L-FCR)|Faraday Cage]] (1) · [[Mage Armor (1-P-L-MA)|Mage Armor]] (1).


---

## Tactical Assessment

A field-deployable tripwire that leaves no electronic signature, suited to securing a perimeter or a bivouac overnight.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
