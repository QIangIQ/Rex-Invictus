---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-7
  - spell/necromancy
  - source/srd
aliases:
  - "7th Tier Spell: Finger of Death"
  - "Finger of Death"
  - "7-N-L-FDN"
registry_id: 7-N-L-FDN
attribute_code: "7·Nec·Necrotic·None·60 feet·Instantaneous"
incantation: "Mourho-’wyn"
tier: 7
school: Necromancy
affinity: N
grade: L
pz_total: 1598.2
pz_quantum: 141200.1
t_e: 2.52
updated: 2026-11-16
---

**Finger of Death** (`7-N-L-FDN`) is a 7th Tier working of the [[Necromancy (School)|Necromancy]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **1,598 Pz** against a slot quantum of 141,200 Pz, which puts its energy-equivalent tier at T_E 2.52 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 7 Workings]]
      - [[Necromancy (School)|Necromancy]]
        - **Finger of Death** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `7-N-L-FDN` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `7·Nec·Necrotic·None·60 feet·Instantaneous` |
| Incantation | *Mourho-’wyn* |
| Affinity | N (Necromancy) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 7th Tier |
| School | [[Necromancy (School)\|Necromancy]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 7d8 + 30 necrotic (mean 61.5) |
| Injury by tier | T7: 7d8 + 30 |
| Resistance check | constitution; on success: half injury |
| Practitioner lineages | Sorcerer, Warlock, Wizard |

### Mechanism

A directed necrotic current disrupts the target's tissue and, if the target dies, leaves a binding pattern that raises the body as a commanded corpse servant.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| necrotic surge, 7d8+30=61.5 | `61.5 HP * kappa_necrotic 0.2 * F 0.5 * 1 target(s) * 1 trigger(s)` | 6.2 |
| reanimation and command bond (if target dies) | `0.05 Pz/s * 3600 s (1 h reference)` | 180 |
| Pattern cost | `0.01 × Q7 × (1 + 0.00)` | 1,412 |

| Quantity | Value |
|---|---|
| Effect energy | 186 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **1,598 Pz** (2,397.2 kJ) |
| Slot quantum Q7 | 141,200 Pz |
| Field gain (draw / quantum) | 0.0113 |
| Energy-equivalent tier T_E | 2.52 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** 7d8+30 avg 61.5 necrotic, ray delivery; reanimation booked as autonomy endowment 0.05 Pz/s over 1 h, assuming the target dies.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Finger of Death (7-N-L-FDN) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 7 | 7 | `0000000001111` |
| k2 School | Necromancy | 6 | `0000000001101` |
| k3 Damage | Necrotic | 6 | `0000000001101` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Mourho-’wyn** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T8: *Nimourho-’wyn* · T9: *Xyimourho-’wyn*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 3→2 | 4 |
| k2 School | 0→11 2→0 3→1 | 3 |
| k3 Damage | 0→10 2→12 3→0 | 3 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#2981c3`.

![[Finger of Death (7-N-L-FDN) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 7 | 0.700 | 1.000 | `#005eff` (490 nm eq.) | source grid |
| Damage | Necrotic | 0.500 | 0.980 | `#00ff8b` (550 nm eq.) | source grid |
| School | Necromancy | 0.750 | 0.999 | `#0017ff` (475 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.783 | `#ff0028` (700 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.994 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.17): swatch `#3bc8cc`, measured lines at 0.004, 0.501, 0.589, 0.701, 0.751. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.20. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `7·N·Necrotic`; the k4 to k6 lines (None, 60 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `7·N·Necrotic` |
| Standard spectrometer detection range | 4.00 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 7,060 Pz (0.05 × Q7) |
| Counter drawn cold (all six layers) | 14,120 Pz (0.10 × Q7) |
| Unravel after completion | 14,120 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is 2x Death, 2x Diminutive and the school lean is Within, Dark, 2x Death. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1C 4D 2E` (Within, Dark, 4x Death, 2x Diminutive).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 266 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 7th Tier quantum of 141,200 Pz (1.1% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 7th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Necromancy school with aspect lean Within, Dark, 2x Death. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 7 Workings]] |
| School | [[Necromancy (School)\|Necromancy]] |
| Affinity | [[Necromancy (School)\|Necromancy]] (N) |
| Function | [[Necromantic and Soul Workings]], [[Precision Strikes]] |
| Element | [[Necrotic Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Harm (6-N-L-HRM)|Harm]] (6) · [[Blight (4-N-L-BLG)|Blight]] (4) · [[Vampiric Touch (3-N-L-VT)|Vampiric Touch]] (3) · [[Circle of Death (6-N-L-CD)|Circle of Death]] (6) · [[Inflict Wounds (1-N-L-IW)|Inflict Wounds]] (1) · [[Chill Touch (0-N-L-CT)|Chill Touch]] (0) · [[Resurrection (7-N-L-RSR)|Resurrection]] (7) · [[Clone (8-N-L-CLN)|Clone]] (8).


---

## Tactical Assessment

A heavy single-target kill with a strategic side effect: each fallen enemy soldier becomes a permanent obedient unit, which makes it a weapon of attrition and terror.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 7 Workings]] · [[Necromancy (School)|Necromancy]] · [[Spell Breakdown Procedure]] · [[Parzival]]
