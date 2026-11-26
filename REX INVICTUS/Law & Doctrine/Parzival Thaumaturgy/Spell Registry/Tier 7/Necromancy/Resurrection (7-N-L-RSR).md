---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-7
  - spell/necromancy
  - source/srd
aliases:
  - "7th Tier Spell: Resurrection"
  - "Resurrection"
  - "7-N-L-RSR"
registry_id: 7-N-L-RSR
attribute_code: "7·Nec·None·None·Touch·Instantaneous"
incantation: "Moulix"
tier: 7
school: Necromancy
affinity: N
grade: L
pz_total: 42590.0
pz_quantum: 141200.1
t_e: 5.80
updated: 2026-11-16
---

**Resurrection** (`7-N-L-RSR`) is a 7th Tier working of the [[Necromancy (School)|Necromancy]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **42,590 Pz** against a slot quantum of 141,200 Pz, which puts its energy-equivalent tier at T_E 5.80 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 7 Workings]]
      - [[Necromancy (School)|Necromancy]]
        - **Resurrection** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `7-N-L-RSR` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `7·Nec·None·None·Touch·Instantaneous` |
| Incantation | *Moulix* |
| Affinity | N (Necromancy) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 7th Tier |
| School | [[Necromancy (School)\|Necromancy]] |
| Casting time | 1 hour |
| Range | Touch |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A diamond worth at least 1,000gp, which the spell consumes |
| Ritual | no |
| Practitioner lineages | Bard, Cleric |

### Mechanism

A soul dead up to a century is recalled into its restored body, with missing parts regrown and injuries fully cleared.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| soul re-anchoring, 4 tiers above 3 | `1e4*(7-3)` | 40,000 |
| full healing, 60 points | `0.30*60` | 18.0 |
| regrow missing parts, 10 kg living tissue | `10*10` | 100 |
| neutralise poisons and disease | `1` | 1.0 |
| Pattern cost | `0.01 × Q7 × (1 + 0.75)` | 2,471 |

| Quantity | Value |
|---|---|
| Effect energy | 40,119 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **42,590 Pz** (63,885.0 kJ) |
| Slot quantum Q7 | 141,200 Pz |
| Field gain (draw / quantum) | 0.302 |
| Energy-equivalent tier T_E | 5.80 |
| Handling points | 0.75 |
| Grade score | 0.15 → L |

**Handling flags:** costly material, consumed material, long cast.

**Assumptions:** Full condition 60 points; 10 kg of missing tissue; soul constant 1e4 Pz per tier above 3.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Resurrection (7-N-L-RSR) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 7 | 7 | `0000000001111` |
| k2 School | Necromancy | 6 | `0000000001101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Moulix** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T8: *Nimoulix* · T9: *Xyimoulix*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 3→2 | 4 |
| k2 School | 0→11 2→0 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#5d1fd2`.

![[Resurrection (7-N-L-RSR) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 7 | 0.700 | 1.000 | `#005eff` (490 nm eq.) | source grid |
| School | Necromancy | 0.750 | 0.999 | `#0017ff` (475 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.783 | `#ff0028` (700 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.984 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.22): swatch `#299eda`, measured lines at 0.004, 0.701, 0.751, 0.883. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.63. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `7·N·None`; the k4 to k6 lines (None, Touch, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `7·N·None` |
| Standard spectrometer detection range | 20.64 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 7,060 Pz (0.05 × Q7) |
| Counter drawn cold (all six layers) | 14,120 Pz (0.10 × Q7) |
| Unravel after completion | 14,120 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Dark, 2x Death. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1D 1F 1J` (Within, Death, Potential, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 7,098 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 7th Tier quantum of 141,200 Pz (30.2% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
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
| Function | [[Healing and Restoration]], [[Necromantic and Soul Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Raise Dead (5-N-M-RD)|Raise Dead]] (5) · [[True Resurrection (9-N-L-TR)|True Resurrection]] (9) · [[Finger of Death (7-N-L-FDN)|Finger of Death]] (7) · [[Circle of Death (6-N-L-CD)|Circle of Death]] (6) · [[Clone (8-N-L-CLN)|Clone]] (8) · [[Create Undead (6-N-L-CU)|Create Undead]] (6) · [[Harm (6-N-L-HRM)|Harm]] (6) · [[Magic Jar (6-N-H-MJ)|Magic Jar]] (6).


---

## Tactical Assessment

Strategic recovery of irreplaceable leaders long after death; casting on the long-dead exhausts the caster.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 7 Workings]] · [[Necromancy (School)|Necromancy]] · [[Spell Breakdown Procedure]] · [[Parzival]]
