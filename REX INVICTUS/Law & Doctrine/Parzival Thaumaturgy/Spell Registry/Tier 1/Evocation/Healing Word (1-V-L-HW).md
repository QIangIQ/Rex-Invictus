---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/evocation
  - source/srd
aliases:
  - "1st Tier Spell: Healing Word"
  - "Healing Word"
  - "1-V-L-HW"
registry_id: 1-V-L-HW
attribute_code: "1·Evo·None·None·60 feet·Instantaneous"
incantation: "Suwyn"
tier: 1
school: Evocation
affinity: V
grade: L
pz_total: 5.2
pz_quantum: 350.0
t_e: -3.22
updated: 2026-11-16
---

**Healing Word** (`1-V-L-HW`) is a 1st Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **5.2 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -3.22 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Evocation]]
        - **Healing Word** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-V-L-HW` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Evo·None·None·60 feet·Instantaneous` |
| Incantation | *Suwyn* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Evocation]] |
| Casting time | 1 bonus action |
| Range | 60 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation) |
| Ritual | no |
| Restoration | 1d4 + MOD restored (mean 5.5, modifier taken as +3) |
| Practitioner lineages | Bard, Cleric, Druid |

### Mechanism

A brief spoken pulse delivers a small amount of positive energy to a visible creature at range.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| healing 1d4+3 | `0.30 Pz * 5.5 HP` | 1.6 |
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

**Assumptions:** Average 2.5 plus a caster aptitude bonus of 3.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Healing Word (1-V-L-HW) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Suwyn** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisuwyn* · T3: *Lisuwyn* · T4: *Visuwyn* · T5: *Tisuwyn* · T6: *Risuwyn* · T7: *Misuwyn* · T8: *Nisuwyn* · T9: *Xyisuwyn*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#859067`.

![[Healing Word (1-V-L-HW) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.923 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.995 | `#ff0028` (700 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.888 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.18): swatch `#afa877`, measured lines at 0.004, 0.101, 0.501, 0.589. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 0.71. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·V·None`; the k4 to k6 lines (None, 60 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·V·None` |
| Standard spectrometer detection range | 0.23 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.0 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1b 1c 1d 1f` (Heat, Light, Life, Energy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 0.858 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (1.5% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Healing and Restoration]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Cure Wounds (1-V-L-CW)|Cure Wounds]] (1) · [[Prayer of Healing (2-V-L-PH)|Prayer of Healing]] (2) · [[Goodberry (1-T-L-GDB)|Goodberry]] (1) · [[Mass Healing Word (3-V-L-MHW)|Mass Healing Word]] (3) · [[Lesser Restoration (2-A-L-LR)|Lesser Restoration]] (2) · [[Reverse Entropy (0-T-L-REV)|Reverse Entropy]] (0) · [[Spare the Dying (0-N-L-SD)|Spare the Dying]] (0) · [[Thomson's Plum Pudding (2-T-L-TSPP)|Thomson's Plum Pudding]] (2).


---

## Tactical Assessment

A quick emergency stabiliser that can be used while doing something else, keeping a downed comrade in the fight.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
