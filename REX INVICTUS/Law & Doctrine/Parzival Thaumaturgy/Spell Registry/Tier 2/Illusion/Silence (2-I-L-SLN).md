---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/illusion
  - source/srd
aliases:
  - "2nd Tier Spell: Silence"
  - "Silence"
  - "2-I-L-SLN"
registry_id: 2-I-L-SLN
attribute_code: "2·Ill·None·sphere (20)·120 feet·Up to 10 minutes"
incantation: "Hai’-Somully"
tier: 2
school: Illusion
affinity: I
grade: L
pz_total: 17.2
pz_quantum: 951.4
t_e: -2.02
updated: 2026-11-16
---

**Silence** (`2-I-L-SLN`) is a 2nd Tier working of the [[Illusion]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **17.2 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E -2.02 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Illusion]]
        - **Silence** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-I-L-SLN` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Ill·None·sphere (20)·120 feet·Up to 10 minutes` |
| Incantation | *Hai’-Somully* |
| Affinity | I (Illusion) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Illusion]] |
| Casting time | 1 action |
| Range | 120 feet |
| Area | sphere (20) |
| Duration | Up to 10 minutes (concentration) |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | yes |
| Practitioner lineages | Bard, Cleric, Ranger |

### Mechanism

A sphere of damped acoustics, where no sound forms or passes and voiced workings are impossible.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| [upkeep] acoustic damping over sphere r 20 ft at 1e-3 W/m^2, 10 min | `1e-3*4*pi*(20*ft)**2*600/1500` | 0.187 |
| thunder injury absorbed, 13.5 points | `0.20*13.5` | 2.7 |
| Pattern cost | `0.01 × Q2 × (1 + 0.50)` | 14.3 |

| Quantity | Value |
|---|---|
| Effect energy | 2.7 Pz |
| Upkeep energy | 0.187 Pz (0.000311 Pz/s) |
| **Total draw** | **17.2 Pz** (25.7 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.018 |
| Energy-equivalent tier T_E | -2.02 |
| Handling points | 0.50 |
| Grade score | -0.50 → L |

**Handling flags:** concentration, ritual.

**Assumptions:** Ambient 90 dB flux; one thunder burst absorbed.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Silence (2-I-L-SLN) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Illusion | 5 | `0000000001011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (20) | 30 | `0000000111101` |
| k5 Range | 120 feet | 3 | `0000000000111` |
| k6 Duration | Up to 10 minutes | 15 | `0000000011111` |

### Incantation

Spoken as **Hai’-Somully** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihai’-Somully* · T4: *Vihai’-Somully* · T5: *Tihai’-Somully* · T6: *Rihai’-Somully* · T7: *Mihai’-Somully* · T8: *Nihai’-Somully* · T9: *Xyihai’-Somully*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 1→12 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 2→11 3→12 4→0 5→1 | 5 |
| k5 Range | 0→8 1→9 2→10 | 3 |
| k6 Duration | 0→7 1→8 2→9 3→10 4→11 | 5 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#85868f`.

![[Silence (2-I-L-SLN) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Illusion | 0.625 | 0.914 | `#00c5ff` (512 nm eq.) | source grid |
| Duration | Up to 10 minutes | 0.789 | 0.841 | `#1e00ff` (463 nm eq.) | source grid |
| Area | sphere (20) | 0.833 | 0.818 | `#5a00ff` (450 nm eq.) | source grid |
| Range | 120 feet | 0.176 | 1.000 | `#ffc900` (647 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.22): swatch `#91af9b`, measured lines at 0.177, 0.201, 0.626, 0.790, 0.834. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.23. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·I·None`; the k4 to k6 lines (sphere (20), 120 feet, Up to 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·I·None` |
| Standard spectrometer detection range | 0.41 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 95.2 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Light, Introspection, 2x Flexibility. The working vector used by [[Recast Tension and Combination Affinity]] is `2c 1d 1F 1G 2h 1J` (2x Light, Life, Potential, Introspection, 2x Flexibility, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 2.9 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (1.8% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Illusion school with aspect lean Light, Introspection, 2x Flexibility. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Illusion]] |
| Affinity | [[Illusion]] (I) |
| Function | [[Concealment and Illusion]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Arcanist's Magic Aura (2-I-L-ASMA)|Arcanist's Magic Aura]] (2) · [[Blur (2-I-L-BLR)|Blur]] (2) · [[Cloak (2-I-L-CLK)|Cloak]] (2) · [[Invisibility (2-I-L-INV)|Invisibility]] (2) · [[Mirror Image (2-I-L-MIR)|Mirror Image]] (2) · [[Alter Difraction Pattern (1-I-L-ADP)|Alter Difraction Pattern]] (1) · [[Disguise Self (1-I-L-DS)|Disguise Self]] (1) · [[Illusory Geodesic Curve (3-I-L-IGC)|Illusory Geodesic Curve]] (3).


---

## Tactical Assessment

Denies spoken casting and covers stealthy breaches.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Illusion]] · [[Spell Breakdown Procedure]] · [[Parzival]]
