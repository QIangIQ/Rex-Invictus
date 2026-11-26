---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/enchantment
  - source/srd
aliases:
  - "1st Tier Spell: Sleep"
  - "Sleep"
  - "1-E-L-SLP"
registry_id: 1-E-L-SLP
attribute_code: "1·Enc·None·sphere (20)·90 feet·1 minute"
incantation: "So’-Soylare"
tier: 1
school: Enchantment
affinity: E
grade: L
pz_total: 11.8
pz_quantum: 350.0
t_e: -2.39
updated: 2026-11-16
---

**Sleep** (`1-E-L-SLP`) is a 1st Tier working of the [[Enchantment]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **11.8 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -2.39 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Enchantment]]
        - **Sleep** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-E-L-SLP` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Enc·None·sphere (20)·90 feet·1 minute` |
| Incantation | *So’-Soylare* |
| Affinity | E (Enchantment) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Enchantment]] |
| Casting time | 1 action |
| Range | 90 feet |
| Area | sphere (20) |
| Duration | 1 minute |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A pinch of fine sand, rose petals, or a cricket |
| Ritual | no |
| Injury | 5d8 untyped (mean 22.5) |
| Injury by tier | T1: 5d8 |
| Practitioner lineages | Bard, Sorcerer, Wizard |

### Mechanism

A neural damping field drops the weakest creatures in an area into sleep.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| sleep induction, 3 creatures, instant information | `3*1` | 3.0 |
| [upkeep] sleep hold, 3 creatures, 1 min | `0.005*3*60` | 0.9 |
| Pattern cost | `0.01 × Q1 × (1 + 1.25)` | 7.9 |

| Quantity | Value |
|---|---|
| Effect energy | 3.0 Pz |
| Upkeep energy | 0.9 Pz (0.015 Pz/s) |
| **Total draw** | **11.8 Pz** (17.7 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.0336 |
| Energy-equivalent tier T_E | -2.39 |
| Handling points | 1.25 |
| Grade score | 0.25 → L |

**Handling flags:** fragile, save or suck.

**Assumptions:** 5d8 pool (22.5) covers about 3 light targets.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Sleep (1-E-L-SLP) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Enchantment | 3 | `0000000000111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (20) | 30 | `0000000111101` |
| k5 Range | 90 feet | 11 | `0000000010111` |
| k6 Duration | 1 minute | 1 | `0000000000011` |

### Incantation

Spoken as **So’-Soylare** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hiso’-Soylare* · T3: *Liso’-Soylare* · T4: *Viso’-Soylare* · T5: *Tiso’-Soylare* · T6: *Riso’-Soylare* · T7: *Miso’-Soylare* · T8: *Niso’-Soylare* · T9: *Xyiso’-Soylare*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 1→12 2→0 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 2→11 3→12 4→0 5→1 | 5 |
| k5 Range | 0→8 1→9 2→10 4→12 | 4 |
| k6 Duration | 0→7 1→8 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#847f5a`.

![[Sleep (1-E-L-SLP) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Enchantment | 0.375 | 0.963 | `#20ff00` (588 nm eq.) | source grid |
| Duration | 1 minute | 0.105 | 1.000 | `#ff6300` (668 nm eq.) | source grid |
| Area | sphere (20) | 0.833 | 0.764 | `#5a00ff` (450 nm eq.) | source grid |
| Range | 90 feet | 0.647 | 0.861 | `#00aaff` (506 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.22): swatch `#be9f72`, measured lines at 0.102, 0.376, 0.648, 0.834. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.07. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·E·None`; the k4 to k6 lines (sphere (20), 90 feet, 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·E·None` |
| Standard spectrometer detection range | 0.34 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.2 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Introspection, Flexibility, Hope. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1G 1h 1i 1J` (Within, Light, Life, Potential, Introspection, Flexibility, Hope, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 2.0 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (3.4% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Enchantment school with aspect lean Within, Introspection, Flexibility, Hope. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Enchantment]] |
| Affinity | [[Enchantment]] (E) |
| Function | [[Mind and Will]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Animal Friendship (1-E-M-AF)|Animal Friendship]] (1) · [[Bane (1-E-L-BAN)|Bane]] (1) · [[Charm Person (1-E-L-CP)|Charm Person]] (1) · [[Command (1-E-L-CMM)|Command]] (1) · [[Heroism (1-E-L-HRS)|Heroism]] (1) · [[Hideous Laughter (1-E-L-HL)|Hideous Laughter]] (1) · [[Calm Emotions (2-E-L-CE)|Calm Emotions]] (2) · [[Enthrall (2-E-L-ENTH)|Enthrall]] (2).


---

## Tactical Assessment

Silent removal of sentries and light troops.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Enchantment]] · [[Spell Breakdown Procedure]] · [[Parzival]]
