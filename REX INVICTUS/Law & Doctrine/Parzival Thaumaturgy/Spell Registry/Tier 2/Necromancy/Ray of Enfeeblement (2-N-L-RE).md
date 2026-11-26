---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/necromancy
  - source/srd
aliases:
  - "2nd Tier Spell: Ray of Enfeeblement"
  - "Ray of Enfeeblement"
  - "2-N-L-RE"
registry_id: 2-N-L-RE
attribute_code: "2·Nec·None·None·60 feet·Up to 1 minute"
incantation: "Houwynse"
tier: 2
school: Necromancy
affinity: N
grade: L
pz_total: 19.2
pz_quantum: 951.4
t_e: -1.90
updated: 2026-11-16
---

**Ray of Enfeeblement** (`2-N-L-RE`) is a 2nd Tier working of the [[Necromancy (School)|Necromancy]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **19.2 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E -1.90 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Necromancy (School)|Necromancy]]
        - **Ray of Enfeeblement** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-N-L-RE` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Nec·None·None·60 feet·Up to 1 minute` |
| Incantation | *Houwynse* |
| Affinity | N (Necromancy) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Necromancy (School)\|Necromancy]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | single point or target |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Resistance check | constitution; on success: no effect |
| Delivery | aimed ranged working |
| Practitioner lineages | Warlock, Wizard |

### Mechanism

A beam couples a power sink to the target's muscles and halves the force of its physical strikes.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| absorbed strike output, half of 7 points x 10 strikes | `0.20*0.5*7*10` | 7.0 |
| [upkeep] muscular suppression hold, 1 creature, 1 min | `0.005*60` | 0.3 |
| Pattern cost | `0.01 × Q2 × (1 + 0.25)` | 11.9 |

| Quantity | Value |
|---|---|
| Effect energy | 7.0 Pz |
| Upkeep energy | 0.3 Pz (0.005 Pz/s) |
| **Total draw** | **19.2 Pz** (28.8 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.0202 |
| Energy-equivalent tier T_E | -1.90 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** concentration.

**Assumptions:** Ten strikes averaging 7 points over the minute; half absorbed.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Ray of Enfeeblement (2-N-L-RE) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Necromancy | 6 | `0000000001101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Houwynse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihouwynse* · T4: *Vihouwynse* · T5: *Tihouwynse* · T6: *Rihouwynse* · T7: *Mihouwynse* · T8: *Nihouwynse* · T9: *Xyihouwynse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 2→0 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#45a0b9`.

![[Ray of Enfeeblement (2-N-L-RE) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Necromancy | 0.750 | 0.860 | `#0017ff` (475 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.889 | `#0074ff` (495 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.927 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.21): swatch `#66bbb2`, measured lines at 0.201, 0.589, 0.685, 0.751. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.28. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·N·None`; the k4 to k6 lines (None, 60 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·N·None` |
| Standard spectrometer detection range | 0.44 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 95.2 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Dark, 2x Death. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1D 1F 1J` (Within, Death, Potential, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 3.2 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (2.0% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Necromancy school with aspect lean Within, Dark, 2x Death. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Necromancy (School)\|Necromancy]] |
| Affinity | [[Necromancy (School)\|Necromancy]] (N) |
| Function | [[Negation and Counterspell]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Blindness-Deafness (2-N-L-BD)|Blindness/Deafness]] (2) · [[Hawking's Mark (1-N-L-HSMK)|Hawking's Mark]] (1) · [[Animal Messenger (2-E-L-AM)|Animal Messenger]] (2) · [[Arcane Lock (2-A-L-AL)|Arcane Lock]] (2) · [[Gust of Wind (2-V-M-GW)|Gust of Wind]] (2) · [[Knock (2-T-L-KNC)|Knock]] (2) · [[Magic Weapon (2-T-L-MW)|Magic Weapon]] (2) · [[Oscillate (2-C-L-OSC)|Oscillate]] (2).


---

## Tactical Assessment

Neutralises a heavy melee threat, such as a powered brute, for the length of an engagement.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Necromancy (School)|Necromancy]] · [[Spell Breakdown Procedure]] · [[Parzival]]
