---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-9
  - spell/divination
  - source/srd
aliases:
  - "9th Tier Spell: Foresight"
  - "Foresight"
  - "9-D-L-FRS"
registry_id: 9-D-L-FRS
attribute_code: "9·Div·None·None·Touch·8 hours"
incantation: "Xyilixiy"
tier: 9
school: Divination
affinity: D
grade: L
pz_total: 13164.1
pz_quantum: 1043335.3
t_e: 4.63
updated: 2026-11-16
---

**Foresight** (`9-D-L-FRS`) is a 9th Tier working of the [[Divination]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **13,164 Pz** against a slot quantum of 1.04 MPz Pz, which puts its energy-equivalent tier at T_E 4.63 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 9 Workings]]
      - [[Divination]]
        - **Foresight** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `9-D-L-FRS` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `9·Div·None·None·Touch·8 hours` |
| Incantation | *Xyilixiy* |
| Affinity | D (Divination) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 9th Tier |
| School | [[Divination]] |
| Casting time | 1 minute |
| Range | Touch |
| Area | single point or target |
| Duration | 8 hours |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A hummingbird feather |
| Ritual | no |
| Practitioner lineages | Bard, Druid, Warlock, Wizard |

### Mechanism

Gives a touched creature continuous precognition a few seconds ahead, so it cannot be surprised and its actions and defences anticipate events.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| evasion absorption | `0.20 Pz * (3 engagements * 10 rounds * 15 HP/round * 40% avoided = 180 HP)` | 36.0 |
| short-horizon precognition | `0.001 Pz/s * (30 m / 10) = 0.003 Pz/s * 28800 s` | 86.4 |
| Pattern cost | `0.01 × Q9 × (1 + 0.25)` | 13,042 |

| Quantity | Value |
|---|---|
| Effect energy | 36.0 Pz |
| Upkeep energy | 86.4 Pz (0.003 Pz/s) |
| **Total draw** | **13,164 Pz** (19,746.1 kJ) |
| Slot quantum Q9 | 1.04 MPz Pz |
| Field gain (draw / quantum) | 0.0126 |
| Energy-equivalent tier T_E | 4.63 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** long cast.

**Assumptions:** Order-of-magnitude only: precognition is a time-class effect; divination radius 30 m; three engagements with 40% of incoming injury avoided.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Foresight (9-D-L-FRS) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 9 | 9 | `0000000010011` |
| k2 School | Divination | 2 | `0000000000101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | 8 hours | 8 | `0000000010001` |

### Incantation

Spoken as **Xyilixiy** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 4→3 | 3 |
| k2 School | 0→11 2→0 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 4→11 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#8776a2`.

![[Foresight (9-D-L-FRS) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 9 | 0.900 | 1.000 | `#b600ff` (430 nm eq.) | source grid |
| School | Divination | 0.250 | 0.810 | `#cdff00` (625 nm eq.) | source grid |
| Duration | 8 hours | 0.474 | 0.913 | `#00ff66` (558 nm eq.) | source grid |
| Range | Touch | 0.882 | 1.000 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.17): swatch `#8d8cbf`, measured lines at 0.251, 0.474, 0.883, 0.901. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.12. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `9·D·None`; the k4 to k6 lines (None, Touch, 8 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `9·D·None` |
| Standard spectrometer detection range | 11.47 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 52,167 Pz (0.05 × Q9) |
| Counter drawn cold (all six layers) | 104,334 Pz (0.10 × Q9) |
| Unravel after completion | 104,351 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Light, 2x Extraspection. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 2c 1d 1F 2g 1J` (Beyond, 2x Light, Life, Potential, 2x Extraspection, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 2,194 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 9th Tier quantum of 1.04 MPz Pz (1.3% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 9th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Divination school with aspect lean Beyond, Light, 2x Extraspection. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 9 Workings]] |
| School | [[Divination]] |
| Affinity | [[Divination]] (D) |
| Function | [[Divination and Sensing]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Find the Path (6-D-L-FP)|Find the Path]] (6) · [[Medic's Tent (8-A-L-MSTI)|Medic's Tent]] (8) · [[True Seeing (6-D-L-TSU)|True Seeing]] (6) · [[Commune (5-D-L-CMMM)|Commune]] (5) · [[Commune With Nature (5-D-L-CN)|Commune With Nature]] (5) · [[Contact Other Plane (5-D-L-COP)|Contact Other Plane]] (5) · [[Divine Word (7-V-L-DWV)|Divine Word]] (7) · [[Legend Lore (5-D-L-LLG)|Legend Lore]] (5).


---

## Tactical Assessment

Turns a single operative into a near-untouchable point soldier or pilot for 8 hours; precognition counters ambush and stealth tactics.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 9 Workings]] · [[Divination]] · [[Spell Breakdown Procedure]] · [[Parzival]]
