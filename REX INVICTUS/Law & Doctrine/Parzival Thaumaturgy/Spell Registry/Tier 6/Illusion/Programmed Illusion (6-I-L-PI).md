---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-6
  - spell/illusion
  - source/srd
aliases:
  - "6th Tier Spell: Programmed Illusion"
  - "Programmed Illusion"
  - "6-I-L-PI"
registry_id: 6-I-L-PI
attribute_code: "6·Ill·None·cube (30)·120 feet·Until dispelled"
incantation: "Rai’-Bormulis"
tier: 6
school: Illusion
affinity: I
grade: L
pz_total: 697.4
pz_quantum: 51944.6
t_e: 1.69
updated: 2026-11-16
---

**Programmed Illusion** (`6-I-L-PI`) is a 6th Tier working of the [[Illusion]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **697 Pz** against a slot quantum of 51,945 Pz, which puts its energy-equivalent tier at T_E 1.69 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 6 Workings]]
      - [[Illusion]]
        - **Programmed Illusion** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `6-I-L-PI` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `6·Ill·None·cube (30)·120 feet·Until dispelled` |
| Incantation | *Rai’-Bormulis* |
| Affinity | I (Illusion) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 6th Tier |
| School | [[Illusion]] |
| Casting time | 1 action |
| Range | 120 feet |
| Area | cube (30) |
| Duration | Until dispelled |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A bit of fleece and jade dust worth at least 25 gp |
| Ritual | no |
| Practitioner lineages | Bard, Wizard |

### Mechanism

A scripted sensory performance is stored dormant and released when a set visual or acoustic condition is met nearby, then rearms after ten minutes.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| one 5 min performance, 30 ft cube illusion volume | `0.002*((30*ft)**3/1000)*300` | 0.459 |
| performance sound, 1 W for 300 s | `1*300/1500` | 0.2 |
| [upkeep] dormant trigger watch over 30 ft margin, 30-day reference | `0.01*(dormant watch)  [C4]` | 47.4 |
| Pattern cost | `0.01 × Q6 × (1 + 0.25)` | 649 |

| Quantity | Value |
|---|---|
| Effect energy | 0.659 Pz |
| Upkeep energy | 47.4 Pz (0.00183 Pz/s) |
| **Total draw** | **697 Pz** (1,046.1 kJ) |
| Slot quantum Q6 | 51,945 Pz |
| Field gain (draw / quantum) | 0.0134 |
| Energy-equivalent tier T_E | 1.69 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

Calibration applied: C4 (Dormant patterns), see [[Parzival Energy Budget#Registry calibration rules]].

**Handling flags:** costly material.

**Assumptions:** One activation; dormant upkeep counted over a 30-day reference window since the effect is open-ended; watch range 60 ft from the cube centre.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Programmed Illusion (6-I-L-PI) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 6 | 6 | `0000000001101` |
| k2 School | Illusion | 5 | `0000000001011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | cube (30) | 12 | `0000000011001` |
| k5 Range | 120 feet | 3 | `0000000000111` |
| k6 Duration | Until dispelled | 11 | `0000000010111` |

### Incantation

Spoken as **Rai’-Bormulis** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T7: *Mirai’-Bormulis* · T8: *Nirai’-Bormulis* · T9: *Xyirai’-Bormulis*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 3→2 | 3 |
| k2 School | 0→11 1→12 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 3→12 4→0 | 3 |
| k5 Range | 0→8 1→9 2→10 | 3 |
| k6 Duration | 0→7 1→8 2→9 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#41e49b`.

![[Programmed Illusion (6-I-L-PI) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 6 | 0.600 | 1.000 | `#00ebff` (520 nm eq.) | source grid |
| School | Illusion | 0.625 | 1.000 | `#00c5ff` (512 nm eq.) | source grid |
| Duration | Until dispelled | 0.579 | 1.000 | `#00fff7` (526 nm eq.) | source grid |
| Area | cube (30) | 0.333 | 0.965 | `#5bff00` (600 nm eq.) | source grid |
| Range | 120 feet | 0.176 | 0.914 | `#ffc900` (647 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.21): swatch `#6edfb6`, measured lines at 0.177, 0.334, 0.580, 0.600, 0.625. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.84. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `6·I·None`; the k4 to k6 lines (cube (30), 120 feet, Until dispelled) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `6·I·None` |
| Standard spectrometer detection range | 2.64 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 2,597 Pz (0.05 × Q6) |
| Counter drawn cold (all six layers) | 5,194 Pz (0.10 × Q6) |
| Unravel after completion | 5,204 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Light, Introspection, 2x Flexibility. The working vector used by [[Recast Tension and Combination Affinity]] is `2c 1d 1F 1G 2h 1J` (2x Light, Life, Potential, Introspection, 2x Flexibility, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 116 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 6th Tier quantum of 51,945 Pz (1.3% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Endures independently once set, which places it under the decay clause of ULMTU-XIII. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIII]] | Lex Impermanentiae | Long-lived patterns drift toward reversion unless refreshed from a source that satisfies ULMTU-I. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 6th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Illusion school with aspect lean Light, Introspection, 2x Flexibility. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 6 Workings]] |
| School | [[Illusion]] |
| Affinity | [[Illusion]] (I) |
| Function | [[Linking and Triggers]], [[Concealment and Illusion]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Mirage Arcane (7-I-M-MAR)|Mirage Arcane]] (7) · [[Mislead (5-I-L-MSL)|Mislead]] (5) · [[Project Image (7-I-L-PIO)|Project Image]] (7) · [[Seeming (5-I-L-SMN)|Seeming]] (5) · [[Contingency (6-V-L-CNTI)|Contingency]] (6) · [[Greater Invisibility (4-I-L-GIE)|Greater Invisibility]] (4) · [[Hallucinatory Terrain (4-I-M-HT)|Hallucinatory Terrain]] (4) · [[Delayed Blast Fireball (7-V-M-DBF)|Delayed Blast Fireball]] (7).


---

## Tactical Assessment

A cheap sentry and deception device: false patrols, warnings or decoys triggered by intruders.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 6 Workings]] · [[Illusion]] · [[Spell Breakdown Procedure]] · [[Parzival]]
