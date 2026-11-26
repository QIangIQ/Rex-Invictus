---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-0
  - spell/evocation
  - source/science-spellbook
aliases:
  - "Cantrip Spell: Radiation Poisoning"
  - "0-V-L-RP"
  - "Radiation Poisoning (Science)"
registry_id: 0-V-L-RP
attribute_code: "0·Evo·Poison·None·30 feet·1 minute"
incantation: "Cunis-’usine"
tier: 0
school: Evocation
affinity: V
grade: L
pz_total: 1.9
pz_quantum: 128.8
t_e: -4.20
updated: 2026-11-16
---

**Radiation Poisoning** (`0-V-L-RP`) is a Cantrip (Tier 0) working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **1.9 Pz** against a slot quantum of 129 Pz, which puts its energy-equivalent tier at T_E -4.20 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 0 Workings]]
      - [[Evocation]]
        - **Radiation Poisoning** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `0-V-L-RP` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `0·Evo·Poison·None·30 feet·1 minute` |
| Incantation | *Cunis-’usine* |
| Affinity | V (Evocation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | Cantrip (Tier 0) |
| School | [[Evocation]] |
| Casting time | 1 Action |
| Range | 30 feet |
| Area | single point or target |
| Duration | 1 minute |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Any object made of rare metal worth at least 50GP |
| Ritual | no |
| Injury | 2d6 poison (mean 7) |
| Injury by caster maturity bands | T1: 2d6, T5: 2d8, T11: 2d12, T17: 3d12 |
| Resistance check | constitution; on success: half injury |
| Delivery | aimed ranged working |
| Practitioner lineages | Wizard, Sorcerer |

### Mechanism

An ionising dose that injures at once and keeps doing smaller harm over the next rounds.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Radiation dose | `13 HP x 0.05 (poison) x F 0.5` | 0.325 |
| Pattern cost | `0.01 × Q0 × (1 + 0.25)` | 1.6 |

| Quantity | Value |
|---|---|
| Effect energy | 0.325 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **1.9 Pz** (2.9 kJ) |
| Slot quantum Q0 | 129 Pz |
| Field gain (draw / quantum) | 0.015 |
| Energy-equivalent tier T_E | -4.20 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** costly material.

**Assumptions:** Dose 2d6 + 1d6 + 1d4 = 13 at the poison rate, ray F 0.5; a real acute dose of 5 Gy to 80 kg is 400 J (0.27 Pz), which agrees.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Radiation Poisoning (0-V-L-RP) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 0 | 0 | `0000000000001` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Poison | 9 | `0000000010011` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | 1 minute | 1 | `0000000000011` |

### Incantation

Spoken as **Cunis-’usine** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T1: *Sicunis-’usine* · T2: *Hicunis-’usine* · T3: *Licunis-’usine* · T4: *Vicunis-’usine* · T5: *Ticunis-’usine* · T6: *Ricunis-’usine* · T7: *Micunis-’usine* · T8: *Nicunis-’usine* · T9: *Xyicunis-’usine*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 | 1 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 4→1 | 3 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#8b984f`.

![[Radiation Poisoning (0-V-L-RP) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 0 | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| Damage | Poison | 0.643 | 0.813 | `#00afff` (507 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.882 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | 1 minute | 0.105 | 0.994 | `#ff6300` (668 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.958 | `#91ff00` (612 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 0.29. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `0·V·Poison`; the k4 to k6 lines (None, 30 feet, 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `0·V·Poison` |
| Standard spectrometer detection range | 0.14 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 6.4 Pz (0.05 × Q0) |
| Counter drawn cold (all six layers) | 12.9 Pz (0.10 × Q0) |
| Unravel after completion | 12.9 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Within, Cold, Death, Diminutive and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1D 1E 2f 1j` (Within, Death, Diminutive, 2x Energy, Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 0.322 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the Cantrip (Tier 0) quantum of 129 Pz (1.5% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at Cantrip (Tier 0) up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 0 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Precision Strikes]] |
| Element | [[Poison Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Poison Spray (0-C-L-PS)|Poison Spray]] (0) · [[Eldritch Blast (0-P-L-EB)|Eldritch Blast]] (0) · [[Fire Bolt (0-V-L-FB)|Fire Bolt]] (0) · [[Ray of Frost (0-V-L-RF)|Ray of Frost]] (0) · [[Sacred Flame (0-V-L-SF)|Sacred Flame]] (0) · [[Shocking Grasp (0-V-L-SG)|Shocking Grasp]] (0) · [[Divine Favor (1-V-L-DF)|Divine Favor]] (1) · [[Electrify (1-V-L-ELC)|Electrify]] (1).


---

## Tactical Assessment

Sustained harassment of a single target.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 0 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
