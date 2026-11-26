---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/divination
  - source/srd
aliases:
  - "1st Tier Spell: Identify"
  - "Identify"
  - "1-D-L-IDN"
registry_id: 1-D-L-IDN
attribute_code: "1·Div·None·None·Touch·Instantaneous"
incantation: "Silix"
tier: 1
school: Divination
affinity: D
grade: L
pz_total: 7.1
pz_quantum: 350.0
t_e: -2.89
updated: 2026-11-16
---

**Identify** (`1-D-L-IDN`) is a 1st Tier working of the [[Divination]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **7.1 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -2.89 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Divination]]
        - **Identify** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-D-L-IDN` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Div·None·None·Touch·Instantaneous` |
| Incantation | *Silix* |
| Affinity | D (Divination) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Divination]] |
| Casting time | 1 minute |
| Range | Touch |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A pearl worth at least 100gp and an owl feather |
| Ritual | yes |
| Practitioner lineages | Bard, Wizard |

### Mechanism

A minute of sustained contact lets the field read the active patterns bound into an object or resting on a creature. The result is a direct informational readout with negligible physical work.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Item or creature readout (instant info) | `instant info = 1 Pz` | 1.0 |
| Pattern cost | `0.01 × Q1 × (1 + 0.75)` | 6.1 |

| Quantity | Value |
|---|---|
| Effect energy | 1.0 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **7.1 Pz** (10.7 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.0204 |
| Energy-equivalent tier T_E | -2.89 |
| Handling points | 0.75 |
| Grade score | -0.25 → L |

**Handling flags:** ritual, costly material, long cast.

**Assumptions:** Single readout treated as instant information; 1 minute contact casting.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Identify (1-D-L-IDN) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Divination | 2 | `0000000000101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Silix** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisilix* · T3: *Lisilix* · T4: *Visilix* · T5: *Tisilix* · T6: *Risilix* · T7: *Misilix* · T8: *Nisilix* · T9: *Xyisilix*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 2→0 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#dd5c3d`.

![[Identify (1-D-L-IDN) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Divination | 0.250 | 0.989 | `#cdff00` (625 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.995 | `#ff0028` (700 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.736 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.19): swatch `#e3725a`, measured lines at 0.004, 0.101, 0.251, 0.883. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 0.85. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·D·None`; the k4 to k6 lines (None, Touch, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·D·None` |
| Standard spectrometer detection range | 0.27 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.0 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Light, 2x Extraspection. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 2c 1d 1F 2g 1J` (Beyond, 2x Light, Life, Potential, 2x Extraspection, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1.2 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (2.0% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Divination school with aspect lean Beyond, Light, 2x Extraspection. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Divination]] |
| Affinity | [[Divination]] (D) |
| Function | [[Divination and Sensing]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Comprehend Languages (1-D-L-CL)|Comprehend Languages]] (1) · [[Detect Evil and Good (1-D-L-DEG)|Detect Evil and Good]] (1) · [[Detect Habitat (1-D-L-DH)|Detect Habitat]] (1) · [[Detect Magic (1-D-L-DMT)|Detect Magic]] (1) · [[Detect Poison and Disease (1-D-L-DPD)|Detect Poison and Disease]] (1) · [[Expectation Values (1-D-L-EV)|Expectation Values]] (1) · [[Hunter's Mark (1-D-L-HSM)|Hunter's Mark]] (1) · [[Magic Antenna (1-D-L-MAG)|Magic Antenna]] (1).


---

## Tactical Assessment

Used by logistics and intelligence staff to triage captured enchanted materiel and check personnel for hostile workings. Its value is analytic, with no battlefield effect.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Divination]] · [[Spell Breakdown Procedure]] · [[Parzival]]
