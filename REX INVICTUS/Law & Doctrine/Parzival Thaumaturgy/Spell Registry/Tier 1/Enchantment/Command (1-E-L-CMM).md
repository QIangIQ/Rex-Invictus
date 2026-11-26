---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/enchantment
  - source/srd
aliases:
  - "1st Tier Spell: Command"
  - "Command"
  - "1-E-L-CMM"
registry_id: 1-E-L-CMM
attribute_code: "1·Enc·None·None·60 feet·1 round"
incantation: "Sowyni"
tier: 1
school: Enchantment
affinity: E
grade: L
pz_total: 8.9
pz_quantum: 350.0
t_e: -2.67
updated: 2026-11-16
---

**Command** (`1-E-L-CMM`) is a 1st Tier working of the [[Enchantment]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **8.9 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -2.67 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Enchantment]]
        - **Command** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-E-L-CMM` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Enc·None·None·60 feet·1 round` |
| Incantation | *Sowyni* |
| Affinity | E (Enchantment) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Enchantment]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | single point or target |
| Duration | 1 round |
| Components | spoken (incantation) |
| Ritual | no |
| Resistance check | will; on success: no effect |
| Practitioner lineages | Cleric, Paladin |

### Mechanism

A one-word order is imposed on a creature which carries it out on its next action.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| instant information | `1 * 1 Pz` | 1.0 |
| enchantment upkeep | `0.005 Pz/s * 1 creature(s) * 6 s` | 0.03 |
| Pattern cost | `0.01 × Q1 × (1 + 1.25)` | 7.9 |

| Quantity | Value |
|---|---|
| Effect energy | 1.0 Pz |
| Upkeep energy | 0.03 Pz (0.005 Pz/s) |
| **Total draw** | **8.9 Pz** (13.4 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.0254 |
| Energy-equivalent tier T_E | -2.67 |
| Handling points | 1.25 |
| Grade score | 0.25 → L |

**Handling flags:** fragile, save or suck.

**Assumptions:** 1 target for 6 s.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Command (1-E-L-CMM) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Enchantment | 3 | `0000000000111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | 1 round | 2 | `0000000000101` |

### Incantation

Spoken as **Sowyni** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisowyni* · T3: *Lisowyni* · T4: *Visowyni* · T5: *Tisowyni* · T6: *Risowyni* · T7: *Misowyni* · T8: *Nisowyni* · T9: *Xyisowyni*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 1→12 2→0 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 2→9 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#8cbe3a`.

![[Command (1-E-L-CMM) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Enchantment | 0.375 | 0.963 | `#20ff00` (588 nm eq.) | source grid |
| Duration | 1 round | 0.158 | 0.998 | `#ffae00` (653 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.888 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.14): swatch `#ccaa6b`, measured lines at 0.101, 0.159, 0.376, 0.589. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 0.95. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·E·None`; the k4 to k6 lines (None, 60 feet, 1 round) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·E·None` |
| Standard spectrometer detection range | 0.30 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.0 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Introspection, Flexibility, Hope. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1G 1h 1i 1J` (Within, Light, Life, Potential, Introspection, Flexibility, Hope, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1.5 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (2.5% of it). |
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

Similar workings: [[Animal Friendship (1-E-M-AF)|Animal Friendship]] (1) · [[Bane (1-E-L-BAN)|Bane]] (1) · [[Charm Person (1-E-L-CP)|Charm Person]] (1) · [[Heroism (1-E-L-HRS)|Heroism]] (1) · [[Hideous Laughter (1-E-L-HL)|Hideous Laughter]] (1) · [[Sleep (1-E-L-SLP)|Sleep]] (1) · [[Calm Emotions (2-E-L-CE)|Calm Emotions]] (2) · [[Enthrall (2-E-L-ENTH)|Enthrall]] (2).


---

## Tactical Assessment

Forces a sentry to drop a weapon or halt.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Enchantment]] · [[Spell Breakdown Procedure]] · [[Parzival]]
