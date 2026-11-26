---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/enchantment
  - source/srd
aliases:
  - "1st Tier Spell: Charm Person"
  - "Charm Person"
  - "1-E-L-CP"
registry_id: 1-E-L-CP
attribute_code: "1·Enc·None·None·30 feet·1 hour"
incantation: "Sousina"
tier: 1
school: Enchantment
affinity: E
grade: L
pz_total: 26.0
pz_quantum: 350.0
t_e: -1.60
updated: 2026-11-16
---

**Charm Person** (`1-E-L-CP`) is a 1st Tier working of the [[Enchantment]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **26.0 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -1.60 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Enchantment]]
        - **Charm Person** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-E-L-CP` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Enc·None·None·30 feet·1 hour` |
| Incantation | *Sousina* |
| Affinity | E (Enchantment) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Enchantment]] |
| Casting time | 1 action |
| Range | 30 feet |
| Area | single point or target |
| Duration | 1 hour |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Resistance check | will; on success: no effect |
| Practitioner lineages | Bard, Druid, Sorcerer, Warlock, Wizard |

### Mechanism

A person comes to regard the caster as a friendly acquaintance for an hour, and remembers it afterward.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| instant information | `1 * 1 Pz` | 1.0 |
| enchantment upkeep | `0.005 Pz/s * 1 creature(s) * 3600 s` | 18.0 |
| Pattern cost | `0.01 × Q1 × (1 + 1.00)` | 7.0 |

| Quantity | Value |
|---|---|
| Effect energy | 1.0 Pz |
| Upkeep energy | 18.0 Pz (0.005 Pz/s) |
| **Total draw** | **26.0 Pz** (39.0 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.0743 |
| Energy-equivalent tier T_E | -1.60 |
| Handling points | 1.00 |
| Grade score | 0.00 → L |

**Handling flags:** fragile.

**Assumptions:** 1 target for 1 h.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Charm Person (1-E-L-CP) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Enchantment | 3 | `0000000000111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | 1 hour | 0 | `0000000000001` |

### Incantation

Spoken as **Sousina** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisousina* · T3: *Lisousina* · T4: *Visousina* · T5: *Tisousina* · T6: *Risousina* · T7: *Misousina* · T8: *Nisousina* · T9: *Xyisousina*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 1→12 2→0 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 | 1 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#ad9c00`.

![[Charm Person (1-E-L-CP) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Enchantment | 0.375 | 0.963 | `#20ff00` (588 nm eq.) | source grid |
| Duration | 1 hour | 0.053 | 0.999 | `#ff1c00` (684 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.981 | `#91ff00` (612 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.14): swatch `#e49757`, measured lines at 0.053, 0.101, 0.295, 0.376. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.41. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·E·None`; the k4 to k6 lines (None, 30 feet, 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·E·None` |
| Standard spectrometer detection range | 0.51 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 38.6 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Introspection, Flexibility, Hope. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1G 1h 1i 1J` (Within, Light, Life, Potential, Introspection, Flexibility, Hope, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 4.3 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (7.4% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Enchantment school with aspect lean Within, Introspection, Flexibility, Hope. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Enchantment]] |
| Affinity | [[Enchantment]] (E) |
| Function | [[Mind and Will]], [[Necromantic and Soul Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Animal Friendship (1-E-M-AF)|Animal Friendship]] (1) · [[Bane (1-E-L-BAN)|Bane]] (1) · [[Beacon of Hope (3-A-L-BHA)|Beacon of Hope]] (3) · [[Command (1-E-L-CMM)|Command]] (1) · [[Heroism (1-E-L-HRS)|Heroism]] (1) · [[Hideous Laughter (1-E-L-HL)|Hideous Laughter]] (1) · [[Sleep (1-E-L-SLP)|Sleep]] (1) · [[Calm Emotions (2-E-L-CE)|Calm Emotions]] (2).


---

## Tactical Assessment

Social engineering at checkpoints; the target's later awareness is an intelligence risk.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Enchantment]] · [[Spell Breakdown Procedure]] · [[Parzival]]
