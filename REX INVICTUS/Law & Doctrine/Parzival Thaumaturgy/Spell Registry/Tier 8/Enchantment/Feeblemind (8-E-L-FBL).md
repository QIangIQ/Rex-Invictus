---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-8
  - spell/enchantment
  - source/srd
aliases:
  - "8th Tier Spell: Feeblemind"
  - "Feeblemind"
  - "8-E-L-FBL"
registry_id: 8-E-L-FBL
attribute_code: "8·Enc·Psychic·None·150 feet·Instantaneous"
incantation: "Nochar-’nosin"
tier: 8
school: Enchantment
affinity: E
grade: L
pz_total: 16798.3
pz_quantum: 383821.6
t_e: 4.87
updated: 2026-11-16
---

**Feeblemind** (`8-E-L-FBL`) is a 8th Tier working of the [[Enchantment]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **16,798 Pz** against a slot quantum of 383,822 Pz, which puts its energy-equivalent tier at T_E 4.87 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 8 Workings]]
      - [[Enchantment]]
        - **Feeblemind** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `8-E-L-FBL` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `8·Enc·Psychic·None·150 feet·Instantaneous` |
| Incantation | *Nochar-’nosin* |
| Affinity | E (Enchantment) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 8th Tier |
| School | [[Enchantment]] |
| Casting time | 1 action |
| Range | 150 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A handful of clay, crystal, glass, or mineral spheres |
| Ritual | no |
| Injury | 4d6 psychic (mean 14) |
| Injury by tier | T8: 4d6 |
| Resistance check | intellect; on success: other |
| Practitioner lineages | Bard, Druid, Warlock, Wizard |

### Mechanism

A directed psychic pulse injures the target and then locks its higher reasoning and language centres into a degraded stable state that persists until the subject's own resistance breaks it at a 30-day check or another working repairs it.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| psychic shock, 4d6=14 | `14 HP * kappa_psychic 0.02 * F 0.5 * 1 target(s) * 1 trigger(s)` | 0.14 |
| persistent cognitive imprint | `0.005 Pz/s * 2,592,000 s (one 30-day relapse interval, booked at casting)` | 12,960 |
| Pattern cost | `0.01 × Q8 × (1 + 0.00)` | 3,838 |

| Quantity | Value |
|---|---|
| Effect energy | 12,960 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **16,798 Pz** (25,197.5 kJ) |
| Slot quantum Q8 | 383,822 Pz |
| Field gain (draw / quantum) | 0.0438 |
| Energy-equivalent tier T_E | 4.87 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** 4d6 avg 14 psychic, ray delivery; the lasting imprint costed as enchantment power 0.005 Pz/s over one 30-day interval, paid up front since the working is instantaneous.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Feeblemind (8-E-L-FBL) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 8 | 8 | `0000000010001` |
| k2 School | Enchantment | 3 | `0000000000111` |
| k3 Damage | Psychic | 10 | `0000000010101` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 150 feet | 4 | `0000000001001` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Nochar-’nosin** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T9: *Xyinochar-’nosin*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 4→3 | 2 |
| k2 School | 0→11 1→12 2→0 | 3 |
| k3 Damage | 0→10 2→12 4→1 | 3 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 | 2 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#647577`.

![[Feeblemind (8-E-L-FBL) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 8 | 0.800 | 1.000 | `#2900ff` (460 nm eq.) | source grid |
| Damage | Psychic | 0.714 | 0.996 | `#004dff` (486 nm eq.) | source grid |
| School | Enchantment | 0.375 | 0.914 | `#20ff00` (588 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.726 | `#ff0028` (700 nm eq.) | source grid |
| Range | 150 feet | 0.235 | 0.853 | `#e3ff00` (629 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.17): swatch `#7ab4ad`, measured lines at 0.004, 0.236, 0.376, 0.715, 0.801. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.23. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `8·E·Psychic`; the k4 to k6 lines (None, 150 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `8·E·Psychic` |
| Standard spectrometer detection range | 12.96 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 19,191 Pz (0.05 × Q8) |
| Counter drawn cold (all six layers) | 38,382 Pz (0.10 × Q8) |
| Unravel after completion | 38,382 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Dark, Potential, Introspection, Hopelessness and the school lean is Within, Introspection, Flexibility, Hope. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1C 1F 2G 1h` (Within, Dark, Potential, 2x Introspection, Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 2,800 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 8th Tier quantum of 383,822 Pz (4.4% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 8th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Enchantment school with aspect lean Within, Introspection, Flexibility, Hope. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 8 Workings]] |
| School | [[Enchantment]] |
| Affinity | [[Enchantment]] (E) |
| Function | [[Mind and Will]], [[Precision Strikes]] |
| Element | [[Psychic Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Dream (5-I-L-DRM)|Dream]] (5) · [[Phantasmal Killer (4-I-L-PK)|Phantasmal Killer]] (4) · [[Antipathy-Sympathy (8-E-L-ASP)|Antipathy/Sympathy]] (8) · [[Dominate Monster (8-E-L-DMM)|Dominate Monster]] (8) · [[Power Word Stun (8-E-L-PWS)|Power Word Stun]] (8) · [[Vicious Mockery (0-E-L-VM)|Vicious Mockery]] (0) · [[Power Word Kill (9-E-L-PWK)|Power Word Kill]] (9) · [[Gravitational Wave (8-V-L-GWV)|Gravitational Wave]] (8).


---

## Tactical Assessment

Removes an enemy commander, psion or field-caster from the fight permanently while leaving a docile body that still recognises allies; valuable for decapitation strikes where a killing would create a martyr.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 8 Workings]] · [[Enchantment]] · [[Spell Breakdown Procedure]] · [[Parzival]]
