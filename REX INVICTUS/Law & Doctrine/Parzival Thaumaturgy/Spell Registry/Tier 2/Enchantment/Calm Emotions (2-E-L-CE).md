---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/enchantment
  - source/srd
aliases:
  - "2nd Tier Spell: Calm Emotions"
  - "Calm Emotions"
  - "2-E-L-CE"
registry_id: 2-E-L-CE
attribute_code: "2·Enc·None·sphere (20)·60 feet·Up to 1 minute"
incantation: "Ho’-Sowynse"
tier: 2
school: Enchantment
affinity: E
grade: L
pz_total: 24.8
pz_quantum: 951.4
t_e: -1.65
updated: 2026-11-16
---

**Calm Emotions** (`2-E-L-CE`) is a 2nd Tier working of the [[Enchantment]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **24.8 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E -1.65 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Enchantment]]
        - **Calm Emotions** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-E-L-CE` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Enc·None·sphere (20)·60 feet·Up to 1 minute` |
| Incantation | *Ho’-Sowynse* |
| Affinity | E (Enchantment) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Enchantment]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | sphere (20) |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Resistance check | presence; on success: no effect |
| Practitioner lineages | Bard, Cleric |

### Mechanism

Strong emotions in a 6 m radius are suppressed, cancelling fear or charm effects or rendering targets indifferent to chosen foes.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| instant information | `1 * 1 Pz` | 1.0 |
| enchantment upkeep | `0.005 Pz/s * 8 creature(s) * 60 s` | 2.4 |
| Pattern cost | `0.01 × Q2 × (1 + 1.25)` | 21.4 |

| Quantity | Value |
|---|---|
| Effect energy | 1.0 Pz |
| Upkeep energy | 2.4 Pz (0.04 Pz/s) |
| **Total draw** | **24.8 Pz** (37.2 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.0261 |
| Energy-equivalent tier T_E | -1.65 |
| Handling points | 1.25 |
| Grade score | 0.25 → L |

**Handling flags:** concentration, fragile.

**Assumptions:** 8 people affected for 1 min.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Calm Emotions (2-E-L-CE) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Enchantment | 3 | `0000000000111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (20) | 30 | `0000000111101` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Ho’-Sowynse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Liho’-Sowynse* · T4: *Viho’-Sowynse* · T5: *Tiho’-Sowynse* · T6: *Riho’-Sowynse* · T7: *Miho’-Sowynse* · T8: *Niho’-Sowynse* · T9: *Xyiho’-Sowynse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 1→12 2→0 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 2→11 3→12 4→0 5→1 | 5 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#4db191`.

![[Calm Emotions (2-E-L-CE) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Enchantment | 0.375 | 0.985 | `#20ff00` (588 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.889 | `#0074ff` (495 nm eq.) | source grid |
| Area | sphere (20) | 0.833 | 0.818 | `#5a00ff` (450 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.927 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.14): swatch `#a1ca97`, measured lines at 0.201, 0.376, 0.589, 0.685, 0.834. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.39. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·E·None`; the k4 to k6 lines (sphere (20), 60 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·E·None` |
| Standard spectrometer detection range | 0.50 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 95.6 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Introspection, Flexibility, Hope. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1G 1h 1i 1J` (Within, Light, Life, Potential, Introspection, Flexibility, Hope, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 4.1 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (2.6% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Enchantment school with aspect lean Within, Introspection, Flexibility, Hope. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Enchantment]] |
| Affinity | [[Enchantment]] (E) |
| Function | [[Mind and Will]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Enthrall (2-E-L-ENTH)|Enthrall]] (2) · [[Hold Person (2-E-L-HP)|Hold Person]] (2) · [[Suggestion (2-E-L-SGG)|Suggestion]] (2) · [[Zone of Truth (2-E-L-ZT)|Zone of Truth]] (2) · [[Animal Friendship (1-E-M-AF)|Animal Friendship]] (1) · [[Bane (1-E-L-BAN)|Bane]] (1) · [[Charm Person (1-E-L-CP)|Charm Person]] (1) · [[Command (1-E-L-CMM)|Command]] (1).


---

## Tactical Assessment

Crowd control and de-escalation at checkpoints or riots.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Enchantment]] · [[Spell Breakdown Procedure]] · [[Parzival]]
