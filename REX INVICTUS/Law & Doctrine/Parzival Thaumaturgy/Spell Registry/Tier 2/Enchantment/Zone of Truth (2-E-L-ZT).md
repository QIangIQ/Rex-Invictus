---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/enchantment
  - source/srd
aliases:
  - "2nd Tier Spell: Zone of Truth"
  - "Zone of Truth"
  - "2-E-L-ZT"
registry_id: 2-E-L-ZT
attribute_code: "2·Enc·None·sphere (15)·60 feet·10 minutes"
incantation: "Ho’-Séwyns"
tier: 2
school: Enchantment
affinity: E
grade: L
pz_total: 25.5
pz_quantum: 951.4
t_e: -1.62
updated: 2026-11-16
---

**Zone of Truth** (`2-E-L-ZT`) is a 2nd Tier working of the [[Enchantment]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **25.5 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E -1.62 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Enchantment]]
        - **Zone of Truth** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-E-L-ZT` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Enc·None·sphere (15)·60 feet·10 minutes` |
| Incantation | *Ho’-Séwyns* |
| Affinity | E (Enchantment) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Enchantment]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | sphere (15) |
| Duration | 10 minutes |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Bard, Cleric, Paladin |

### Mechanism

Within a 4.6 m sphere, affected creatures cannot speak deliberate falsehoods for ten minutes, and the caster knows who is affected.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Reporting each creature result | `4 * 1 Pz instant info` | 4.0 |
| Upkeep: Lie suppression, 4 creatures | `0.005 * 4 * 600 s` | 12.0 |
| Pattern cost | `0.01 × Q2 × (1 + 0.00)` | 9.5 |

| Quantity | Value |
|---|---|
| Effect energy | 4.0 Pz |
| Upkeep energy | 12.0 Pz (0.02 Pz/s) |
| **Total draw** | **25.5 Pz** (38.3 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.0268 |
| Energy-equivalent tier T_E | -1.62 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** 4 creatures for 10 min.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Zone of Truth (2-E-L-ZT) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Enchantment | 3 | `0000000000111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (15) | 29 | `0000000111011` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | 10 minutes | 4 | `0000000001001` |

### Incantation

Spoken as **Ho’-Séwyns** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Liho’-Séwyns* · T4: *Viho’-Séwyns* · T5: *Tiho’-Séwyns* · T6: *Riho’-Séwyns* · T7: *Miho’-Séwyns* · T8: *Niho’-Séwyns* · T9: *Xyiho’-Séwyns*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 1→12 2→0 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 3→12 4→0 5→1 | 5 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 3→10 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#6dcd5e`.

![[Zone of Truth (2-E-L-ZT) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Enchantment | 0.375 | 0.985 | `#20ff00` (588 nm eq.) | source grid |
| Duration | 10 minutes | 0.263 | 0.998 | `#bdff00` (621 nm eq.) | source grid |
| Area | sphere (15) | 0.806 | 0.832 | `#3400ff` (458 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.927 | `#00fbff` (524 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 1.41. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·E·None`; the k4 to k6 lines (sphere (15), 60 feet, 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·E·None` |
| Standard spectrometer detection range | 0.51 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 97.5 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Introspection, Flexibility, Hope. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1G 1h 1i 1J` (Within, Light, Life, Potential, Introspection, Flexibility, Hope, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 4.3 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (2.7% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
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

Similar workings: [[Calm Emotions (2-E-L-CE)|Calm Emotions]] (2) · [[Enthrall (2-E-L-ENTH)|Enthrall]] (2) · [[Hold Person (2-E-L-HP)|Hold Person]] (2) · [[Suggestion (2-E-L-SGG)|Suggestion]] (2) · [[Animal Friendship (1-E-M-AF)|Animal Friendship]] (1) · [[Bane (1-E-L-BAN)|Bane]] (1) · [[Charm Person (1-E-L-CP)|Charm Person]] (1) · [[Command (1-E-L-CMM)|Command]] (1).


---

## Tactical Assessment

Interrogation and negotiation aid; subjects can still stay silent or evade.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Enchantment]] · [[Spell Breakdown Procedure]] · [[Parzival]]
