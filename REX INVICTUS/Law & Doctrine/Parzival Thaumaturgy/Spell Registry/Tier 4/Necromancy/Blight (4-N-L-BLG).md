---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/necromancy
  - source/srd
aliases:
  - "4th Tier Spell: Blight"
  - "Blight"
  - "4-N-L-BLG"
registry_id: 4-N-L-BLG
attribute_code: "4·Nec·Necrotic·None·30 feet·Instantaneous"
incantation: "Vourho-’usin"
tier: 4
school: Necromancy
affinity: N
grade: L
pz_total: 77.5
pz_quantum: 7029.9
t_e: -0.51
updated: 2026-11-16
---

**Blight** (`4-N-L-BLG`) is a 4th Tier working of the [[Necromancy (School)|Necromancy]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **77.5 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E -0.51 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Necromancy (School)|Necromancy]]
        - **Blight** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-N-L-BLG` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Nec·Necrotic·None·30 feet·Instantaneous` |
| Incantation | *Vourho-’usin* |
| Affinity | N (Necromancy) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Necromancy (School)\|Necromancy]] |
| Casting time | 1 action |
| Range | 30 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 8d8 necrotic (mean 36) |
| Injury by tier | T4: 8d8, T5: 9d8, T6: 10d8, T7: 11d8, T8: 12d8, T9: 13d8 |
| Resistance check | constitution; on success: half injury |
| Practitioner lineages | Druid, Sorcerer, Warlock, Wizard |

### Mechanism

Necrotic flux washes over one target and draws out water and vitality, killing ordinary plants outright.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| vitality drain | `36 HP * 0.2 Pz/HP (necrotic) * F 1.0 * 1 target(s)/hit(s)` | 7.2 |
| Pattern cost | `0.01 × Q4 × (1 + 0.00)` | 70.3 |

| Quantity | Value |
|---|---|
| Effect energy | 7.2 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **77.5 Pz** (116.2 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 0.011 |
| Energy-equivalent tier T_E | -0.51 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Average 36 injury points; whole-body delivery factor 1.0.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Blight (4-N-L-BLG) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 4 | 4 | `0000000001001` |
| k2 School | Necromancy | 6 | `0000000001101` |
| k3 Damage | Necrotic | 6 | `0000000001101` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Vourho-’usin** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T5: *Tivourho-’usin* · T6: *Rivourho-’usin* · T7: *Mivourho-’usin* · T8: *Nivourho-’usin* · T9: *Xyivourho-’usin*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 3→2 | 2 |
| k2 School | 0→11 2→0 3→1 | 3 |
| k3 Damage | 0→10 2→12 3→0 | 3 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#4ea155`.

![[Blight (4-N-L-BLG) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| Damage | Necrotic | 0.500 | 0.995 | `#00ff8b` (550 nm eq.) | source grid |
| School | Necromancy | 0.750 | 0.941 | `#0017ff` (475 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.923 | `#ff0028` (700 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.994 | `#91ff00` (612 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.14): swatch `#7fc9a6`, measured lines at 0.004, 0.295, 0.401, 0.501, 0.751. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.89. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·N·Necrotic`; the k4 to k6 lines (None, 30 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·N·Necrotic` |
| Standard spectrometer detection range | 0.88 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 703 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is 2x Death, 2x Diminutive and the school lean is Within, Dark, 2x Death. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1C 4D 2E` (Within, Dark, 4x Death, 2x Diminutive).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 12.9 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 4th Tier quantum of 7,030 Pz (1.1% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 4th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Necromancy school with aspect lean Within, Dark, 2x Death. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 4 Workings]] |
| School | [[Necromancy (School)\|Necromancy]] |
| Affinity | [[Necromancy (School)\|Necromancy]] (N) |
| Function | [[Light and Radiance]], [[Necromantic and Soul Workings]], [[Precision Strikes]] |
| Element | [[Necrotic Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Vampiric Touch (3-N-L-VT)|Vampiric Touch]] (3) · [[Harm (6-N-L-HRM)|Harm]] (6) · [[Finger of Death (7-N-L-FDN)|Finger of Death]] (7) · [[Inflict Wounds (1-N-L-IW)|Inflict Wounds]] (1) · [[Chill Touch (0-N-L-CT)|Chill Touch]] (0) · [[Circle of Death (6-N-L-CD)|Circle of Death]] (6) · [[Chain Lightning (6-V-L-CLA)|Chain Lightning]] (6) · [[Animate Dead (3-N-M-AD)|Animate Dead]] (3).


---

## Tactical Assessment

Single-target attrition against heavy infantry and defoliation of cover.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Necromancy (School)|Necromancy]] · [[Spell Breakdown Procedure]] · [[Parzival]]
