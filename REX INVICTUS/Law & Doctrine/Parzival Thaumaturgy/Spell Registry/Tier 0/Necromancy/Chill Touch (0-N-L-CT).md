---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-0
  - spell/necromancy
  - source/srd
aliases:
  - "Cantrip Spell: Chill Touch"
  - "Chill Touch"
  - "0-N-L-CT"
registry_id: 0-N-L-CT
attribute_code: "0·Nec·Necrotic·None·120 feet·1 round"
incantation: "Courho-’muli"
tier: 0
school: Necromancy
affinity: N
grade: L
pz_total: 1.8
pz_quantum: 128.8
t_e: -4.29
updated: 2026-11-16
---

**Chill Touch** (`0-N-L-CT`) is a Cantrip (Tier 0) working of the [[Necromancy (School)|Necromancy]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **1.8 Pz** against a slot quantum of 129 Pz, which puts its energy-equivalent tier at T_E -4.29 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 0 Workings]]
      - [[Necromancy (School)|Necromancy]]
        - **Chill Touch** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `0-N-L-CT` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `0·Nec·Necrotic·None·120 feet·1 round` |
| Incantation | *Courho-’muli* |
| Affinity | N (Necromancy) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | Cantrip (Tier 0) |
| School | [[Necromancy (School)\|Necromancy]] |
| Casting time | 1 action |
| Range | 120 feet |
| Area | single point or target |
| Duration | 1 round |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 1d8 necrotic (mean 4.5) |
| Injury by caster maturity bands | T1: 1d8, T5: 2d8, T11: 3d8, T17: 4d8 |
| Delivery | aimed ranged working |
| Practitioner lineages | Sorcerer, Warlock, Wizard |

### Mechanism

A spectral hand forms on the target, draining vitality and blocking healing until the caster's next turn.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| necrotic grip | `4.5 HP * 0.2 Pz/HP (necrotic) * F 0.5 * 1 target(s)/hit(s)` | 0.45 |
| healing block hold | `0.005 Pz/s * 1 creature(s) * 6 s` | 0.03 |
| Pattern cost | `0.01 × Q0 × (1 + 0.00)` | 1.3 |

| Quantity | Value |
|---|---|
| Effect energy | 0.45 Pz |
| Upkeep energy | 0.03 Pz (0.005 Pz/s) |
| **Total draw** | **1.8 Pz** (2.7 kJ) |
| Slot quantum Q0 | 129 Pz |
| Field gain (draw / quantum) | 0.0137 |
| Energy-equivalent tier T_E | -4.29 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Average 4.5 injury; ray factor 0.5; 6 s hold.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Chill Touch (0-N-L-CT) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 0 | 0 | `0000000000001` |
| k2 School | Necromancy | 6 | `0000000001101` |
| k3 Damage | Necrotic | 6 | `0000000001101` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 120 feet | 3 | `0000000000111` |
| k6 Duration | 1 round | 2 | `0000000000101` |

### Incantation

Spoken as **Courho-’muli** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T1: *Sicourho-’muli* · T2: *Hicourho-’muli* · T3: *Licourho-’muli* · T4: *Vicourho-’muli* · T5: *Ticourho-’muli* · T6: *Ricourho-’muli* · T7: *Micourho-’muli* · T8: *Nicourho-’muli* · T9: *Xyicourho-’muli*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 | 1 |
| k2 School | 0→11 2→0 3→1 | 3 |
| k3 Damage | 0→10 2→12 3→0 | 3 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 | 3 |
| k6 Duration | 0→7 2→9 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#a4844d`.

![[Chill Touch (0-N-L-CT) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 0 | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| Damage | Necrotic | 0.500 | 0.882 | `#00ff8b` (550 nm eq.) | source grid |
| School | Necromancy | 0.750 | 0.755 | `#0017ff` (475 nm eq.) | source grid |
| Duration | 1 round | 0.158 | 0.988 | `#ffae00` (653 nm eq.) | source grid |
| Range | 120 feet | 0.176 | 0.985 | `#ffc900` (647 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.14): swatch `#9c927f`, measured lines at 0.006, 0.159, 0.177, 0.501, 0.751. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 0.25. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `0·N·Necrotic`; the k4 to k6 lines (None, 120 feet, 1 round) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `0·N·Necrotic` |
| Standard spectrometer detection range | 0.13 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 6.4 Pz (0.05 × Q0) |
| Counter drawn cold (all six layers) | 12.9 Pz (0.10 × Q0) |
| Unravel after completion | 12.9 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is 2x Death, 2x Diminutive and the school lean is Within, Dark, 2x Death. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1C 4D 2E` (Within, Dark, 4x Death, 2x Diminutive).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 0.295 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the Cantrip (Tier 0) quantum of 129 Pz (1.4% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at Cantrip (Tier 0) up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Necromancy school with aspect lean Within, Dark, 2x Death. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 0 Workings]] |
| School | [[Necromancy (School)\|Necromancy]] |
| Affinity | [[Necromancy (School)\|Necromancy]] (N) |
| Function | [[Necromantic and Soul Workings]], [[Precision Strikes]] |
| Element | [[Necrotic Workings]], [[Cold and Ice Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Inflict Wounds (1-N-L-IW)|Inflict Wounds]] (1) · [[Vampiric Touch (3-N-L-VT)|Vampiric Touch]] (3) · [[Blight (4-N-L-BLG)|Blight]] (4) · [[Harm (6-N-L-HRM)|Harm]] (6) · [[Ray of Frost (0-V-L-RF)|Ray of Frost]] (0) · [[Finger of Death (7-N-L-FDN)|Finger of Death]] (7) · [[Cool Metal (2-T-L-CM)|Cool Metal]] (2) · [[Acid Splash (0-C-L-AS)|Acid Splash]] (0).


---

## Tactical Assessment

Denies field medicine to a high-value target for a round.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 0 Workings]] · [[Necromancy (School)|Necromancy]] · [[Spell Breakdown Procedure]] · [[Parzival]]
