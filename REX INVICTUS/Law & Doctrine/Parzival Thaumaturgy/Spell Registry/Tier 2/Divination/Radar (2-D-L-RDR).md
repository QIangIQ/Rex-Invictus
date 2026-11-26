---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/divination
  - source/science-spellbook
aliases:
  - "2nd Tier Spell: Radar"
  - "2-D-L-RDR"
  - "Radar (Science)"
registry_id: 2-D-L-RDR
attribute_code: "2·Div·None·sphere (120)·30 feet·Instantaneous"
incantation: "Hi’-Seiusin"
tier: 2
school: Divination
affinity: D
grade: L
pz_total: 10.5
pz_quantum: 951.4
t_e: -2.51
updated: 2026-11-16
---

**Radar** (`2-D-L-RDR`) is a 2nd Tier working of the [[Divination]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **10.5 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E -2.51 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Divination]]
        - **Radar** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-D-L-RDR` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Div·None·sphere (120)·30 feet·Instantaneous` |
| Incantation | *Hi’-Seiusin* |
| Affinity | D (Divination) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Divination]] |
| Casting time | 1 Action |
| Range | 30 feet |
| Area | sphere (120) |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A parabolic surface |
| Ritual | no |
| Practitioner lineages | Wizard, Sorcerer, Bard |

### Mechanism

A pulse of unseen waves reflects through openings and returns a snapshot of creature positions within 120 ft.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Position snapshot | `instant info` | 1.0 |
| Pattern cost | `0.01 × Q2 × (1 + 0.00)` | 9.5 |

| Quantity | Value |
|---|---|
| Effect energy | 1.0 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **10.5 Pz** (15.8 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.0111 |
| Energy-equivalent tier T_E | -2.51 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Instant information, 1 Pz; a real radar pulse at this range would need far less.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Radar (2-D-L-RDR) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Divination | 2 | `0000000000101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (120) | 39 | `0000001001111` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Hi’-Seiusin** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihi’-Seiusin* · T4: *Vihi’-Seiusin* · T5: *Tihi’-Seiusin* · T6: *Rihi’-Seiusin* · T7: *Mihi’-Seiusin* · T8: *Nihi’-Seiusin* · T9: *Xyihi’-Seiusin*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 2→0 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 2→11 3→12 6→2 | 5 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#b69a34`.

![[Radar (2-D-L-RDR) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Divination | 0.250 | 0.999 | `#cdff00` (625 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.980 | `#ff0028` (700 nm eq.) | source grid |
| Area | sphere (120) | 0.792 | 0.839 | `#1e00ff` (462 nm eq.) | RI half-step |
| Range | 30 feet | 0.294 | 0.996 | `#91ff00` (612 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 1.02. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·D·None`; the k4 to k6 lines (sphere (120), 30 feet, Instantaneous) refine it to a registry match.

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
| Function | [[Concealment and Illusion]], [[Divination and Sensing]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[See Invisibility (2-D-L-SIE)|See Invisibility]] (2) · [[Osteonum (1-D-L-OST)|Osteonum]] (1) · [[Arcanist's Magic Aura (2-I-L-ASMA)|Arcanist's Magic Aura]] (2) · [[Illusory Script (1-I-L-IS)|Illusory Script]] (1) · [[Nondetection (3-A-L-NND)|Nondetection]] (3) · [[Augury (2-D-L-AGR)|Augury]] (2) · [[Detect Thoughts (2-D-L-DT)|Detect Thoughts]] (2) · [[Find Traps (2-D-L-FT)|Find Traps]] (2).


---

## Tactical Assessment

Room and building clearing; locates hidden enemies through doorways.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Divination]] · [[Spell Breakdown Procedure]] · [[Parzival]]
