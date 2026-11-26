---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/evocation
  - source/srd
aliases:
  - "1st Tier Spell: Hellish Rebuke"
  - "Hellish Rebuke"
  - "1-V-L-HR"
registry_id: 1-V-L-HR
attribute_code: "1·Evo·Fire·None·60 feet·Instantaneous"
incantation: "Suire-’wyn"
tier: 1
school: Evocation
affinity: V
grade: L
pz_total: 12.1
pz_quantum: 350.0
t_e: -2.37
updated: 2026-11-16
---

**Hellish Rebuke** (`1-V-L-HR`) is a 1st Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **12.1 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -2.37 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Evocation]]
        - **Hellish Rebuke** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-V-L-HR` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Evo·Fire·None·60 feet·Instantaneous` |
| Incantation | *Suire-’wyn* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Evocation]] |
| Casting time | 1 reaction |
| Range | 60 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 2d10 fire (mean 11) |
| Injury by tier | T1: 2d10, T2: 3d10, T3: 4d10, T4: 5d10, T5: 6d10, T6: 7d10, T7: 8d10, T8: 9d10, T9: 10d10 |
| Resistance check | agility; on success: half injury |
| Practitioner lineages | Warlock |

### Mechanism

A reflexive retaliation that wraps the creature that just injured the caster in flame.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| enveloping flames, 2d10=11 | `11 HP * kappa_fire 0.7 * F 1.0 * 1 target(s) * 1 trigger(s)` | 7.7 |
| Pattern cost | `0.01 × Q1 × (1 + 0.25)` | 4.4 |

| Quantity | Value |
|---|---|
| Effect energy | 7.7 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **12.1 Pz** (18.1 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.0345 |
| Energy-equivalent tier T_E | -2.37 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** reaction cast.

**Assumptions:** 2d10 avg 11 fire, whole-body delivery on one target.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Hellish Rebuke (1-V-L-HR) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Fire | 3 | `0000000000111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Suire-’wyn** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisuire-’wyn* · T3: *Lisuire-’wyn* · T4: *Visuire-’wyn* · T5: *Tisuire-’wyn* · T6: *Risuire-’wyn* · T7: *Misuire-’wyn* · T8: *Nisuire-’wyn* · T9: *Xyisuire-’wyn*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 | 3 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#8aa752`.

![[Hellish Rebuke (1-V-L-HR) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| Damage | Fire | 0.286 | 0.983 | `#9cff00` (614 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.923 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.995 | `#ff0028` (700 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.888 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.18): swatch `#bbae75`, measured lines at 0.004, 0.101, 0.286, 0.501, 0.589. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.08. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·V·Fire`; the k4 to k6 lines (None, 60 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·V·Fire` |
| Standard spectrometer detection range | 0.35 km (r = 1 km × √(E/100 Pz)) |
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
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 2.0 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (3.4% of it). |
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
| Element | [[Fire Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Focusing Lens (1-V-L-FLC)|Focusing Lens]] (1) · [[Fire Bolt (0-V-L-FB)|Fire Bolt]] (0) · [[Flame Blade (2-V-L-FBA)|Flame Blade]] (2) · [[Sacred Flame (0-V-L-SF)|Sacred Flame]] (0) · [[Scorching Ray (2-V-L-SR)|Scorching Ray]] (2) · [[Flaming Sphere (2-C-L-FSA)|Flaming Sphere]] (2) · [[Heat Metal (2-T-M-HM)|Heat Metal]] (2) · [[Produce Flame (0-C-L-PF)|Produce Flame]] (0).


---

## Tactical Assessment

Makes close assault on a caster costly and punishes the first enemy to land a hit.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
