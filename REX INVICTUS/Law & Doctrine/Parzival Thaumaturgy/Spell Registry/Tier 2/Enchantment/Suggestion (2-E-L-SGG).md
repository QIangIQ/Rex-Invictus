---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/enchantment
  - source/srd
aliases:
  - "2nd Tier Spell: Suggestion"
  - "Suggestion"
  - "2-E-L-SGG"
registry_id: 2-E-L-SGG
attribute_code: "2·Enc·None·None·30 feet·Up to 8 hours"
incantation: "Housinos"
tier: 2
school: Enchantment
affinity: E
grade: L
pz_total: 166.4
pz_quantum: 951.4
t_e: 0.26
updated: 2026-11-16
---

**Suggestion** (`2-E-L-SGG`) is a 2nd Tier working of the [[Enchantment]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **166 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E 0.26 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Enchantment]]
        - **Suggestion** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-E-L-SGG` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Enc·None·None·30 feet·Up to 8 hours` |
| Incantation | *Housinos* |
| Affinity | E (Enchantment) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Enchantment]] |
| Casting time | 1 action |
| Range | 30 feet |
| Area | single point or target |
| Duration | Up to 8 hours (concentration) |
| Components | spoken (incantation), material focus. Material: A snake's tongue and either a bit of honeycomb or a drop of sweet oil |
| Ritual | no |
| Resistance check | will; on success: no effect |
| Practitioner lineages | Bard, Sorcerer, Warlock, Wizard |

### Mechanism

A short spoken directive is anchored in the listener's motivation so it pursues a reasonable-sounding course of action for up to eight hours.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Implanting the directive | `instant info = 1 Pz` | 1.0 |
| Upkeep: Compulsion held on 1 creature for 8 h | `0.005 Pz/s * 28800 s` | 144 |
| Pattern cost | `0.01 × Q2 × (1 + 1.25)` | 21.4 |

| Quantity | Value |
|---|---|
| Effect energy | 1.0 Pz |
| Upkeep energy | 144 Pz (0.005 Pz/s) |
| **Total draw** | **166 Pz** (249.6 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.175 |
| Energy-equivalent tier T_E | 0.26 |
| Handling points | 1.25 |
| Grade score | 0.38 → L |

**Handling flags:** concentration, fragile.

**Assumptions:** 1 target, full 8 h duration.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Suggestion (2-E-L-SGG) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Enchantment | 3 | `0000000000111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Up to 8 hours | 18 | `0000000100101` |

### Incantation

Spoken as **Housinos** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihousinos* · T4: *Vihousinos* · T5: *Tihousinos* · T6: *Rihousinos* · T7: *Mihousinos* · T8: *Nihousinos* · T9: *Xyihousinos*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 1→12 2→0 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 2→9 5→12 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#a5c533`.

![[Suggestion (2-E-L-SGG) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Enchantment | 0.375 | 0.985 | `#20ff00` (588 nm eq.) | source grid |
| Duration | Up to 8 hours | 0.947 | 0.756 | `#f800ff` (416 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.996 | `#91ff00` (612 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.23): swatch `#cfb283`, measured lines at 0.201, 0.295, 0.376, 0.948. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.22. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·E·None`; the k4 to k6 lines (None, 30 feet, Up to 8 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·E·None` |
| Standard spectrometer detection range | 1.29 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 124 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Introspection, Flexibility, Hope. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1G 1h 1i 1J` (Within, Light, Life, Potential, Introspection, Flexibility, Hope, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 27.7 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (17.5% of it). |
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

Similar workings: [[Calm Emotions (2-E-L-CE)|Calm Emotions]] (2) · [[Enthrall (2-E-L-ENTH)|Enthrall]] (2) · [[Hold Person (2-E-L-HP)|Hold Person]] (2) · [[Zone of Truth (2-E-L-ZT)|Zone of Truth]] (2) · [[Animal Friendship (1-E-M-AF)|Animal Friendship]] (1) · [[Bane (1-E-L-BAN)|Bane]] (1) · [[Charm Person (1-E-L-CP)|Charm Person]] (1) · [[Command (1-E-L-CMM)|Command]] (1).


---

## Tactical Assessment

Used to redirect sentries, delay couriers or plant triggered actions; harming the subject breaks it.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Enchantment]] · [[Spell Breakdown Procedure]] · [[Parzival]]
