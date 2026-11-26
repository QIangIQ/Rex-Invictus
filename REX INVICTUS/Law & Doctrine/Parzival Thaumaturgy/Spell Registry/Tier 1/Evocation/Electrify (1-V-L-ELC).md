---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/evocation
  - source/science-spellbook
aliases:
  - "1st Tier Spell: Electrify"
  - "1-V-L-ELC"
  - "Electrify (Science)"
registry_id: 1-V-L-ELC
attribute_code: "1·Evo·Lightning·None·Touch·Up to 10 minutes"
incantation: "Sunin-’lixly"
tier: 1
school: Evocation
affinity: V
grade: L
pz_total: 6.8
pz_quantum: 350.0
t_e: -2.94
updated: 2026-11-16
---

**Electrify** (`1-V-L-ELC`) is a 1st Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **6.8 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -2.94 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Evocation]]
        - **Electrify** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-V-L-ELC` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Evo·Lightning·None·Touch·Up to 10 minutes` |
| Incantation | *Sunin-’lixly* |
| Affinity | V (Evocation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Evocation]] |
| Casting time | 1 Action |
| Range | Touch |
| Area | single point or target |
| Duration | Up to 10 minutes (concentration) |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 3d8 lightning (mean 13.5) |
| Injury by tier | T1: 3d8, T2: 4d8, T3: 5d8, T4: 6d8, T5: 7d8, T6: 8d8, T7: 9d8, T8: 10d8, T9: 11d8 |
| Resistance check | constitution; on success: half injury |
| Practitioner lineages | Wizard, Sorcerer, Warlock |

### Mechanism

Charges a conductive object up to 30 ft across so the first creature to touch it takes the discharge.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Stored discharge | `13.5 HP x 0.3 (lightning) x F 0.5` | 2.0 |
| Charge leakage (upkeep) | `1 W x 600 s = 600 J / 1500` | 0.4 |
| Pattern cost | `0.01 × Q1 × (1 + 0.25)` | 4.4 |

| Quantity | Value |
|---|---|
| Effect energy | 2.0 Pz |
| Upkeep energy | 0.4 Pz (0.000667 Pz/s) |
| **Total draw** | **6.8 Pz** (10.2 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.0194 |
| Energy-equivalent tier T_E | -2.94 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** concentration.

**Assumptions:** Discharge 3d8 = 13.5 lightning into one creature, touch F 0.5; charge leakage 1 W for 10 minutes.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Electrify (1-V-L-ELC) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Lightning | 5 | `0000000001011` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Up to 10 minutes | 15 | `0000000011111` |

### Incantation

Spoken as **Sunin-’lixly** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisunin-’lixly* · T3: *Lisunin-’lixly* · T4: *Visunin-’lixly* · T5: *Tisunin-’lixly* · T6: *Risunin-’lixly* · T7: *Misunin-’lixly* · T8: *Nisunin-’lixly* · T9: *Xyisunin-’lixly*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 3→0 | 3 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 2→9 3→10 4→11 | 5 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#59817d`.

![[Electrify (1-V-L-ELC) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| Damage | Lightning | 0.429 | 0.947 | `#00ff25` (571 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.923 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Up to 10 minutes | 0.789 | 0.788 | `#1e00ff` (463 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.736 | `#9b00ff` (435 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 0.83. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·V·Lightning`; the k4 to k6 lines (None, Touch, Up to 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·V·Lightning` |
| Standard spectrometer detection range | 0.26 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.1 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is 2x Heat, Light, Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `3b 1c 2f 2j` (3x Heat, Light, 2x Energy, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1.1 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (1.9% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
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
| Function | [[Precision Strikes]] |
| Element | [[Lightning Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Shocking Grasp (0-V-L-SG)|Shocking Grasp]] (0) · [[Divine Favor (1-V-L-DF)|Divine Favor]] (1) · [[Focusing Lens (1-V-L-FLC)|Focusing Lens]] (1) · [[Guiding Bolt (1-V-L-GB)|Guiding Bolt]] (1) · [[Hellish Rebuke (1-V-L-HR)|Hellish Rebuke]] (1) · [[Magic Missile (1-P-L-MM)|Magic Missile]] (1) · [[Acid Arrow (2-V-L-AA)|Acid Arrow]] (2) · [[Branding Smite (2-V-L-BS)|Branding Smite]] (2).


---

## Tactical Assessment

Booby traps on doors, rails and vehicle hulls.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
