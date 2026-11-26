---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/necromancy
  - source/srd
aliases:
  - "3rd Tier Spell: Bestow Curse"
  - "Bestow Curse"
  - "3-N-L-BC"
registry_id: 3-N-L-BC
attribute_code: "3·Nec·None·None·Touch·Up to 1 minute"
incantation: "Loulixse"
tier: 3
school: Necromancy
affinity: N
grade: L
pz_total: 35.9
pz_quantum: 2586.2
t_e: -1.28
updated: 2026-11-16
---

**Bestow Curse** (`3-N-L-BC`) is a 3rd Tier working of the [[Necromancy (School)|Necromancy]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **35.9 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E -1.28 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Necromancy (School)|Necromancy]]
        - **Bestow Curse** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-N-L-BC` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Nec·None·None·Touch·Up to 1 minute` |
| Incantation | *Loulixse* |
| Affinity | N (Necromancy) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Necromancy (School)\|Necromancy]] |
| Casting time | 1 action |
| Range | Touch |
| Area | single point or target |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Resistance check | will; on success: no effect |
| Practitioner lineages | Bard, Cleric, Wizard |

### Mechanism

A touched creature is marked with a persistent interference pattern that weakens one capacity, wastes its actions or makes it vulnerable to the caster.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| necrotic rider | `4.5 HP * 0.2 Pz/HP (necrotic) * F 0.5 * 5 target(s)/hit(s)` | 2.2 |
| instant information | `1 * 1 Pz` | 1.0 |
| enchantment upkeep | `0.005 Pz/s * 1 creature(s) * 60 s` | 0.3 |
| Pattern cost | `0.01 × Q3 × (1 + 0.25)` | 32.3 |

| Quantity | Value |
|---|---|
| Effect energy | 3.2 Pz |
| Upkeep energy | 0.3 Pz (0.005 Pz/s) |
| **Total draw** | **35.9 Pz** (53.8 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 0.0139 |
| Energy-equivalent tier T_E | -1.28 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** concentration.

**Assumptions:** Necrotic option; 5 follow-up hits at 4.5 average injury, touch factor 0.5.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Bestow Curse (3-N-L-BC) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Necromancy | 6 | `0000000001101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Loulixse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Viloulixse* · T5: *Tiloulixse* · T6: *Riloulixse* · T7: *Miloulixse* · T8: *Niloulixse* · T9: *Xyiloulixse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 2→0 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#4968b9`.

![[Bestow Curse (3-N-L-BC) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| School | Necromancy | 0.750 | 0.904 | `#0017ff` (475 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.929 | `#0074ff` (495 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.844 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.13): swatch `#5ab3c6`, measured lines at 0.300, 0.685, 0.751, 0.883. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.55. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·N·None`; the k4 to k6 lines (None, Touch, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·N·None` |
| Standard spectrometer detection range | 0.60 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 259 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Dark, 2x Death. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1D 1F 1J` (Within, Death, Potential, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 6.0 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 3rd Tier quantum of 2,586 Pz (1.4% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
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
| Function | [[Mind and Will]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Beacon of Hope (3-A-L-BHA)|Beacon of Hope]] (3) · [[Fear (3-I-L-FEA)|Fear]] (3) · [[Hypnotic Pattern (3-I-L-HPP)|Hypnotic Pattern]] (3) · [[Spirit Guardians (3-C-M-SGR)|Spirit Guardians]] (3) · [[Calm Emotions (2-E-L-CE)|Calm Emotions]] (2) · [[Compulsion (4-E-L-CMP)|Compulsion]] (4) · [[Confusion (4-E-L-CNF)|Confusion]] (4) · [[Dominate Beast (4-E-L-DB)|Dominate Beast]] (4).


---

## Tactical Assessment

Neutralizes an enemy officer or specialist over a minute-long engagement.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Necromancy (School)|Necromancy]] · [[Spell Breakdown Procedure]] · [[Parzival]]
