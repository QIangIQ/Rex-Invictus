---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/necromancy
  - source/srd
aliases:
  - "3rd Tier Spell: Vampiric Touch"
  - "Vampiric Touch"
  - "3-N-L-VT"
registry_id: 3-N-L-VT
attribute_code: "3·Nec·Necrotic·None·Self·Up to 1 minute"
incantation: "Lourho-’porse"
tier: 3
school: Necromancy
affinity: N
grade: L
pz_total: 58.6
pz_quantum: 2586.2
t_e: -0.79
updated: 2026-11-16
---

**Vampiric Touch** (`3-N-L-VT`) is a 3rd Tier working of the [[Necromancy (School)|Necromancy]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **58.6 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E -0.79 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Necromancy (School)|Necromancy]]
        - **Vampiric Touch** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-N-L-VT` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Nec·Necrotic·None·Self·Up to 1 minute` |
| Incantation | *Lourho-’porse* |
| Affinity | N (Necromancy) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Necromancy (School)\|Necromancy]] |
| Casting time | 1 action |
| Range | Self |
| Area | single point or target |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 3d6 necrotic (mean 10.5) |
| Injury by tier | T3: 3d6, T4: 4d6, T5: 5d6, T6: 6d6, T7: 7d6, T8: 8d6, T9: 9d6 |
| Delivery | aimed melee working |
| Practitioner lineages | Warlock, Wizard |

### Mechanism

A shadowed hand drains vitality from a touched creature and returns half of it to the caster, repeatable each round for a minute.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Necrotic draining touches, 10 | `10.5 HP * 0.20 * 0.5 * 10` | 10.5 |
| Caster healing, half of drained | `5.25 HP * 0.30 * 10` | 15.8 |
| Pattern cost | `0.01 × Q3 × (1 + 0.25)` | 32.3 |

| Quantity | Value |
|---|---|
| Effect energy | 26.2 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **58.6 Pz** (87.9 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 0.0227 |
| Energy-equivalent tier T_E | -0.79 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** concentration.

**Assumptions:** 3d6 = 10.5; all 10 touches land.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Vampiric Touch (3-N-L-VT) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Necromancy | 6 | `0000000001101` |
| k3 Damage | Necrotic | 6 | `0000000001101` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Lourho-’porse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vilourho-’porse* · T5: *Tilourho-’porse* · T6: *Rilourho-’porse* · T7: *Milourho-’porse* · T8: *Nilourho-’porse* · T9: *Xyilourho-’porse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 2→0 3→1 | 3 |
| k3 Damage | 0→10 2→12 3→0 | 3 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#1d96b1`.

![[Vampiric Touch (3-N-L-VT) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| Damage | Necrotic | 0.500 | 0.980 | `#00ff8b` (550 nm eq.) | source grid |
| School | Necromancy | 0.750 | 0.904 | `#0017ff` (475 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.929 | `#0074ff` (495 nm eq.) | source grid |
| Range | Self | 0.706 | 0.921 | `#0058ff` (488 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 1.77. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·N·Necrotic`; the k4 to k6 lines (None, Self, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·N·Necrotic` |
| Standard spectrometer detection range | 0.77 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 259 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is 2x Death, 2x Diminutive and the school lean is Within, Dark, 2x Death. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1C 4D 2E` (Within, Dark, 4x Death, 2x Diminutive).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 9.8 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 3rd Tier quantum of 2,586 Pz (2.3% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Necromancy school with aspect lean Within, Dark, 2x Death. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Necromancy (School)\|Necromancy]] |
| Affinity | [[Necromancy (School)\|Necromancy]] (N) |
| Function | [[Necromantic and Soul Workings]], [[Precision Strikes]] |
| Element | [[Necrotic Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Blight (4-N-L-BLG)|Blight]] (4) · [[Inflict Wounds (1-N-L-IW)|Inflict Wounds]] (1) · [[Chill Touch (0-N-L-CT)|Chill Touch]] (0) · [[Harm (6-N-L-HRM)|Harm]] (6) · [[Finger of Death (7-N-L-FDN)|Finger of Death]] (7) · [[Circle of Death (6-N-L-CD)|Circle of Death]] (6) · [[Animate Dead (3-N-M-AD)|Animate Dead]] (3) · [[Speak with Dead (3-N-L-SDE)|Speak with Dead]] (3).


---

## Tactical Assessment

Close-quarters sustain for a caster forced into melee.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Necromancy (School)|Necromancy]] · [[Spell Breakdown Procedure]] · [[Parzival]]
