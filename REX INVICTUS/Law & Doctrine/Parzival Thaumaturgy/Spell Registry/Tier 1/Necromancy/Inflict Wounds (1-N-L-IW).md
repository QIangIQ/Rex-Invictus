---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/necromancy
  - source/srd
aliases:
  - "1st Tier Spell: Inflict Wounds"
  - "Inflict Wounds"
  - "1-N-L-IW"
registry_id: 1-N-L-IW
attribute_code: "1·Nec·Necrotic·None·Touch·Instantaneous"
incantation: "Sourho-’lix"
tier: 1
school: Necromancy
affinity: N
grade: L
pz_total: 5.2
pz_quantum: 350.0
t_e: -3.22
updated: 2026-11-16
---

**Inflict Wounds** (`1-N-L-IW`) is a 1st Tier working of the [[Necromancy (School)|Necromancy]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **5.2 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -3.22 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Necromancy (School)|Necromancy]]
        - **Inflict Wounds** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-N-L-IW` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Nec·Necrotic·None·Touch·Instantaneous` |
| Incantation | *Sourho-’lix* |
| Affinity | N (Necromancy) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Necromancy (School)\|Necromancy]] |
| Casting time | 1 action |
| Range | Touch |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 3d10 necrotic (mean 16.5) |
| Injury by tier | T1: 3d10, T2: 4d10, T3: 5d10, T4: 6d10, T5: 7d10, T6: 8d10, T7: 9d10, T8: 10d10, T9: 11d10 |
| Delivery | aimed melee working |
| Practitioner lineages | Cleric |

### Mechanism

A touch discharges a necrotizing pulse into one creature's tissue. Energy cost is low because necrotic injury disrupts living structure instead of doing bulk mechanical work.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Necrotic touch | `16.5 HP * 0.20 * 0.5 (touch)` | 1.6 |
| Pattern cost | `0.01 × Q1 × (1 + 0.00)` | 3.5 |

| Quantity | Value |
|---|---|
| Effect energy | 1.6 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **5.2 Pz** (7.7 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.0147 |
| Energy-equivalent tier T_E | -3.22 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** 3d10 = 16.5 average, full value, single touched target.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Inflict Wounds (1-N-L-IW) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Necromancy | 6 | `0000000001101` |
| k3 Damage | Necrotic | 6 | `0000000001101` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Sourho-’lix** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisourho-’lix* · T3: *Lisourho-’lix* · T4: *Visourho-’lix* · T5: *Tisourho-’lix* · T6: *Risourho-’lix* · T7: *Misourho-’lix* · T8: *Nisourho-’lix* · T9: *Xyisourho-’lix*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 2→0 3→1 | 3 |
| k3 Damage | 0→10 2→12 3→0 | 3 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#8b4d7d`.

![[Inflict Wounds (1-N-L-IW) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| Damage | Necrotic | 0.500 | 0.923 | `#00ff8b` (550 nm eq.) | source grid |
| School | Necromancy | 0.750 | 0.810 | `#0017ff` (475 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.995 | `#ff0028` (700 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.736 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.19): swatch `#838994`, measured lines at 0.004, 0.101, 0.501, 0.751, 0.883. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 0.71. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·N·Necrotic`; the k4 to k6 lines (None, Touch, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·N·Necrotic` |
| Standard spectrometer detection range | 0.23 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.0 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is 2x Death, 2x Diminutive and the school lean is Within, Dark, 2x Death. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1C 4D 2E` (Within, Dark, 4x Death, 2x Diminutive).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 0.858 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (1.5% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Necromancy school with aspect lean Within, Dark, 2x Death. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Necromancy (School)\|Necromancy]] |
| Affinity | [[Necromancy (School)\|Necromancy]] (N) |
| Function | [[Necromantic and Soul Workings]], [[Precision Strikes]] |
| Element | [[Necrotic Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Chill Touch (0-N-L-CT)|Chill Touch]] (0) · [[Vampiric Touch (3-N-L-VT)|Vampiric Touch]] (3) · [[Blight (4-N-L-BLG)|Blight]] (4) · [[Harm (6-N-L-HRM)|Harm]] (6) · [[Finger of Death (7-N-L-FDN)|Finger of Death]] (7) · [[Circle of Death (6-N-L-CD)|Circle of Death]] (6) · [[Gentle Repose (2-N-H-GR)|Gentle Repose]] (2) · [[Animate Dead (3-N-M-AD)|Animate Dead]] (3).


---

## Tactical Assessment

A close-quarters option for boarding actions and room clearing when firearms are impractical. Its reach limits it to melee range.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Necromancy (School)|Necromancy]] · [[Spell Breakdown Procedure]] · [[Parzival]]
