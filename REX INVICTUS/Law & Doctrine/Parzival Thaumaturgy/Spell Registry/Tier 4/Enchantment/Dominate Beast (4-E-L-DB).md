---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/enchantment
  - source/srd
aliases:
  - "4th Tier Spell: Dominate Beast"
  - "Dominate Beast"
  - "4-E-L-DB"
registry_id: 4-E-L-DB
attribute_code: "4·Enc·None·None·60 feet·Up to 1 minute"
incantation: "Vowynse"
tier: 4
school: Enchantment
affinity: E
grade: L
pz_total: 177.0
pz_quantum: 7029.9
t_e: 0.32
updated: 2026-11-16
---

**Dominate Beast** (`4-E-L-DB`) is a 4th Tier working of the [[Enchantment]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **177 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E 0.32 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Enchantment]]
        - **Dominate Beast** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-E-L-DB` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Enc·None·None·60 feet·Up to 1 minute` |
| Incantation | *Vowynse* |
| Affinity | E (Enchantment) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Enchantment]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | single point or target |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Resistance check | will; on success: no effect |
| Practitioner lineages | Druid, Sorcerer |

### Mechanism

The field binds a beast to the caster will through a telepathic link that carries commands and allows direct control. Injury to the beast may break the hold.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| initial capture | `1` | 1.0 |
| upkeep: control coupling, 1 creature, 1 min | `0.005*1*60` | 0.3 |
| Pattern cost | `0.01 × Q4 × (1 + 1.50)` | 176 |

| Quantity | Value |
|---|---|
| Effect energy | 1.0 Pz |
| Upkeep energy | 0.3 Pz (0.005 Pz/s) |
| **Total draw** | **177 Pz** (265.6 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 0.0252 |
| Energy-equivalent tier T_E | 0.32 |
| Handling points | 1.50 |
| Grade score | 0.50 → L |

**Handling flags:** concentration, fragile, save or suck.

**Assumptions:** Enchantment rate for 60 s.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Dominate Beast (4-E-L-DB) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 4 | 4 | `0000000001001` |
| k2 School | Enchantment | 3 | `0000000000111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Vowynse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T5: *Tivowynse* · T6: *Rivowynse* · T7: *Mivowynse* · T8: *Nivowynse* · T9: *Xyivowynse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 3→2 | 2 |
| k2 School | 0→11 1→12 2→0 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#08dc7d`.

![[Dominate Beast (4-E-L-DB) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| School | Enchantment | 0.375 | 1.000 | `#20ff00` (588 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.960 | `#0074ff` (495 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.982 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.16): swatch `#90eca7`, measured lines at 0.376, 0.400, 0.589, 0.685. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.25. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·E·None`; the k4 to k6 lines (None, 60 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·E·None` |
| Standard spectrometer detection range | 1.33 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 703 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Introspection, Flexibility, Hope. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1G 1h 1i 1J` (Within, Light, Life, Potential, Introspection, Flexibility, Hope, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 29.5 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 4th Tier quantum of 7,030 Pz (2.5% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 4th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Enchantment school with aspect lean Within, Introspection, Flexibility, Hope. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 4 Workings]] |
| School | [[Enchantment]] |
| Affinity | [[Enchantment]] (E) |
| Function | [[Mind and Will]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Compulsion (4-E-L-CMP)|Compulsion]] (4) · [[Confusion (4-E-L-CNF)|Confusion]] (4) · [[Plagarise (4-E-L-PLG)|Plagarise]] (4) · [[Dominate Person (5-E-L-DP)|Dominate Person]] (5) · [[Geas (5-E-M-GEA)|Geas]] (5) · [[Hold Monster (5-E-L-HML)|Hold Monster]] (5) · [[Modify Memory (5-E-L-MMD)|Modify Memory]] (5) · [[Calm Emotions (2-E-L-CE)|Calm Emotions]] (2).


---

## Tactical Assessment

Turning enemy war animals or local fauna against their handlers.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Enchantment]] · [[Spell Breakdown Procedure]] · [[Parzival]]
