---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-0
  - spell/enchantment
  - source/srd
aliases:
  - "Cantrip Spell: Vicious Mockery"
  - "Vicious Mockery"
  - "0-E-L-VM"
registry_id: 0-E-L-VM
attribute_code: "0·Enc·Psychic·None·60 feet·Instantaneous"
incantation: "Cochar-’wyn"
tier: 0
school: Enchantment
affinity: E
grade: L
pz_total: 1.3
pz_quantum: 128.8
t_e: -4.56
updated: 2026-11-16
---

**Vicious Mockery** (`0-E-L-VM`) is a Cantrip (Tier 0) working of the [[Enchantment]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **1.3 Pz** against a slot quantum of 129 Pz, which puts its energy-equivalent tier at T_E -4.56 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 0 Workings]]
      - [[Enchantment]]
        - **Vicious Mockery** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `0-E-L-VM` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `0·Enc·Psychic·None·60 feet·Instantaneous` |
| Incantation | *Cochar-’wyn* |
| Affinity | E (Enchantment) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | Cantrip (Tier 0) |
| School | [[Enchantment]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation) |
| Ritual | no |
| Injury | 1d4 psychic (mean 2.5) |
| Injury by caster maturity bands | T1: 1d4, T5: 2d4, T11: 3d4, T17: 4d4 |
| Resistance check | will; on success: no effect |
| Practitioner lineages | Bard |

### Mechanism

Spoken taunts carry a psychic impulse that causes a small injury and spoils the target's next attack.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Psychic sting | `2.5 HP * 0.02 * 0.5` | 0.025 |
| Distraction | `0.005 Pz/s * 6 s` | 0.03 |
| Pattern cost | `0.01 × Q0 × (1 + 0.00)` | 1.3 |

| Quantity | Value |
|---|---|
| Effect energy | 0.055 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **1.3 Pz** (2.0 kJ) |
| Slot quantum Q0 | 129 Pz |
| Field gain (draw / quantum) | 0.0104 |
| Energy-equivalent tier T_E | -4.56 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** 1d4 = 2.5 at base caster level.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Vicious Mockery (0-E-L-VM) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 0 | 0 | `0000000000001` |
| k2 School | Enchantment | 3 | `0000000000111` |
| k3 Damage | Psychic | 10 | `0000000010101` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Cochar-’wyn** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T1: *Sicochar-’wyn* · T2: *Hicochar-’wyn* · T3: *Licochar-’wyn* · T4: *Vicochar-’wyn* · T5: *Ticochar-’wyn* · T6: *Ricochar-’wyn* · T7: *Micochar-’wyn* · T8: *Nicochar-’wyn* · T9: *Xyicochar-’wyn*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 | 1 |
| k2 School | 0→11 1→12 2→0 | 3 |
| k3 Damage | 0→10 2→12 4→1 | 3 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#766f6c`.

![[Vicious Mockery (0-E-L-VM) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 0 | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| Damage | Psychic | 0.714 | 0.775 | `#004dff` (486 nm eq.) | source grid |
| School | Enchantment | 0.375 | 0.932 | `#20ff00` (588 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.841 | `#00fbff` (524 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 0.13. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `0·E·Psychic`; the k4 to k6 lines (None, 60 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `0·E·Psychic` |
| Standard spectrometer detection range | 0.12 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 6.4 Pz (0.05 × Q0) |
| Counter drawn cold (all six layers) | 12.9 Pz (0.10 × Q0) |
| Unravel after completion | 12.9 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Dark, Potential, Introspection, Hopelessness and the school lean is Within, Introspection, Flexibility, Hope. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1C 1F 2G 1h` (Within, Dark, Potential, 2x Introspection, Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 0.224 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the Cantrip (Tier 0) quantum of 129 Pz (1.0% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at Cantrip (Tier 0) up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Enchantment school with aspect lean Within, Introspection, Flexibility, Hope. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 0 Workings]] |
| School | [[Enchantment]] |
| Affinity | [[Enchantment]] (E) |
| Function | [[Mind and Will]], [[Precision Strikes]] |
| Element | [[Psychic Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Phantasmal Killer (4-I-L-PK)|Phantasmal Killer]] (4) · [[Dream (5-I-L-DRM)|Dream]] (5) · [[Feeblemind (8-E-L-FBL)|Feeblemind]] (8) · [[Animal Friendship (1-E-M-AF)|Animal Friendship]] (1) · [[Bane (1-E-L-BAN)|Bane]] (1) · [[Charm Person (1-E-L-CP)|Charm Person]] (1) · [[Command (1-E-L-CMM)|Command]] (1) · [[Heroism (1-E-L-HRS)|Heroism]] (1).


---

## Tactical Assessment

Cheap harassment at 18 m that reduces enemy accuracy for one exchange.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 0 Workings]] · [[Enchantment]] · [[Spell Breakdown Procedure]] · [[Parzival]]
