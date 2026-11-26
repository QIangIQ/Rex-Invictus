---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-6
  - spell/necromancy
  - source/srd
aliases:
  - "6th Tier Spell: Harm"
  - "Harm"
  - "6-N-L-HRM"
registry_id: 6-N-L-HRM
attribute_code: "6·Nec·Necrotic·None·60 feet·Instantaneous"
incantation: "Rourho-’wyn"
tier: 6
school: Necromancy
affinity: N
grade: L
pz_total: 542.3
pz_quantum: 51944.6
t_e: 1.44
updated: 2026-11-16
---

**Harm** (`6-N-L-HRM`) is a 6th Tier working of the [[Necromancy (School)|Necromancy]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **542 Pz** against a slot quantum of 51,945 Pz, which puts its energy-equivalent tier at T_E 1.44 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 6 Workings]]
      - [[Necromancy (School)|Necromancy]]
        - **Harm** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `6-N-L-HRM` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `6·Nec·Necrotic·None·60 feet·Instantaneous` |
| Incantation | *Rourho-’wyn* |
| Affinity | N (Necromancy) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 6th Tier |
| School | [[Necromancy (School)\|Necromancy]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 14d6 necrotic (mean 49) |
| Injury by tier | T6: 14d6 |
| Resistance check | constitution; on success: half injury |
| Practitioner lineages | Cleric |

### Mechanism

Seeds a fast virulent disease that injures the target severely but non-lethally and caps its recovery for an hour.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| necrotic disease surge, 14d6=49 | `49 HP * kappa_necrotic 0.2 * F 0.5 * 1 target(s) * 1 trigger(s)` | 4.9 |
| capacity reduction for 1 h | `0.005 Pz/s * 3600 s` | 18.0 |
| Pattern cost | `0.01 × Q6 × (1 + 0.00)` | 519 |

| Quantity | Value |
|---|---|
| Effect energy | 22.9 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **542 Pz** (813.5 kJ) |
| Slot quantum Q6 | 51,945 Pz |
| Field gain (draw / quantum) | 0.0104 |
| Energy-equivalent tier T_E | 1.44 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** 14d6 avg 49 necrotic, ray delivery; capacity reduction costed at enchantment rate for 1 h, paid at casting.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Harm (6-N-L-HRM) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 6 | 6 | `0000000001101` |
| k2 School | Necromancy | 6 | `0000000001101` |
| k3 Damage | Necrotic | 6 | `0000000001101` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Rourho-’wyn** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T7: *Mirourho-’wyn* · T8: *Nirourho-’wyn* · T9: *Xyirourho-’wyn*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 3→2 | 3 |
| k2 School | 0→11 2→0 3→1 | 3 |
| k3 Damage | 0→10 2→12 3→0 | 3 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#2c9ec1`.

![[Harm (6-N-L-HRM) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 6 | 0.600 | 1.000 | `#00ebff` (520 nm eq.) | source grid |
| Damage | Necrotic | 0.500 | 0.995 | `#00ff8b` (550 nm eq.) | source grid |
| School | Necromancy | 0.750 | 0.989 | `#0017ff` (475 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.835 | `#ff0028` (700 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 1.000 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.18): swatch `#4ad1c5`, measured lines at 0.004, 0.501, 0.596, 0.751. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.73. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `6·N·Necrotic`; the k4 to k6 lines (None, 60 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `6·N·Necrotic` |
| Standard spectrometer detection range | 2.33 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 2,597 Pz (0.05 × Q6) |
| Counter drawn cold (all six layers) | 5,194 Pz (0.10 × Q6) |
| Unravel after completion | 5,194 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is 2x Death, 2x Diminutive and the school lean is Within, Dark, 2x Death. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1C 4D 2E` (Within, Dark, 4x Death, 2x Diminutive).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 90.4 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 6th Tier quantum of 51,945 Pz (1.0% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 6th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Necromancy school with aspect lean Within, Dark, 2x Death. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 6 Workings]] |
| School | [[Necromancy (School)\|Necromancy]] |
| Affinity | [[Necromancy (School)\|Necromancy]] (N) |
| Function | [[Necromantic and Soul Workings]], [[Precision Strikes]] |
| Element | [[Necrotic Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Finger of Death (7-N-L-FDN)|Finger of Death]] (7) · [[Blight (4-N-L-BLG)|Blight]] (4) · [[Vampiric Touch (3-N-L-VT)|Vampiric Touch]] (3) · [[Circle of Death (6-N-L-CD)|Circle of Death]] (6) · [[Inflict Wounds (1-N-L-IW)|Inflict Wounds]] (1) · [[Chill Touch (0-N-L-CT)|Chill Touch]] (0) · [[Create Undead (6-N-L-CU)|Create Undead]] (6) · [[Magic Jar (6-N-H-MJ)|Magic Jar]] (6).


---

## Tactical Assessment

Cripples a key enemy without killing, useful for capture missions and for draining enemy medical resources.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 6 Workings]] · [[Necromancy (School)|Necromancy]] · [[Spell Breakdown Procedure]] · [[Parzival]]
