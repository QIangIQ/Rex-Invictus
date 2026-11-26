---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-6
  - spell/enchantment
  - source/srd
aliases:
  - "6th Tier Spell: Mass Suggestion"
  - "Mass Suggestion"
  - "6-E-L-MSU"
registry_id: 6-E-L-MSU
attribute_code: "6·Enc·None·None·60 feet·24 hours"
incantation: "Rowynl"
tier: 6
school: Enchantment
affinity: E
grade: L
pz_total: 6223.9
pz_quantum: 51944.6
t_e: 3.88
updated: 2026-11-16
---

**Mass Suggestion** (`6-E-L-MSU`) is a 6th Tier working of the [[Enchantment]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **6,224 Pz** against a slot quantum of 51,945 Pz, which puts its energy-equivalent tier at T_E 3.88 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 6 Workings]]
      - [[Enchantment]]
        - **Mass Suggestion** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `6-E-L-MSU` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `6·Enc·None·None·60 feet·24 hours` |
| Incantation | *Rowynl* |
| Affinity | E (Enchantment) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 6th Tier |
| School | [[Enchantment]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | single point or target |
| Duration | 24 hours |
| Components | spoken (incantation), material focus. Material: A snake's tongue and either a bit of honeycomb or a drop of sweet oil |
| Ritual | no |
| Resistance check | will; on success: no effect |
| Practitioner lineages | Bard, Sorcerer, Warlock, Wizard |

### Mechanism

The field plants one reasonable-sounding course of action in up to twelve listeners and keeps them pursuing it for up to a day, or until they finish or are harmed by the caster's side. Obviously self-destructive orders fail.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Suggestion imprint, 12 subjects (instant info) | `instant info = 1 Pz` | 1.0 |
| Compulsion hold, 12 subjects (upkeep) | `0.005 Pz/s * 12 * 86400 s` | 5,184 |
| Pattern cost | `0.01 × Q6 × (1 + 1.00)` | 1,039 |

| Quantity | Value |
|---|---|
| Effect energy | 1.0 Pz |
| Upkeep energy | 5,184 Pz (0.06 Pz/s) |
| **Total draw** | **6,224 Pz** (9,335.8 kJ) |
| Slot quantum Q6 | 51,945 Pz |
| Field gain (draw / quantum) | 0.12 |
| Energy-equivalent tier T_E | 3.88 |
| Handling points | 1.00 |
| Grade score | 0.00 → L |

**Handling flags:** fragile.

**Assumptions:** Twelve subjects held for 24 hours.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Mass Suggestion (6-E-L-MSU) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 6 | 6 | `0000000001101` |
| k2 School | Enchantment | 3 | `0000000000111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | 24 hours | 5 | `0000000001011` |

### Incantation

Spoken as **Rowynl** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T7: *Mirowynl* · T8: *Nirowynl* · T9: *Xyirowynl*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 3→2 | 3 |
| k2 School | 0→11 1→12 2→0 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 3→10 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#24f881`.

![[Mass Suggestion (6-E-L-MSU) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 6 | 0.600 | 1.000 | `#00ebff` (520 nm eq.) | source grid |
| School | Enchantment | 0.375 | 0.975 | `#20ff00` (588 nm eq.) | source grid |
| Duration | 24 hours | 0.316 | 0.960 | `#76ff00` (605 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 1.000 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.20): swatch `#8deca9`, measured lines at 0.316, 0.376, 0.596. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.79. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `6·E·None`; the k4 to k6 lines (None, 60 feet, 24 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `6·E·None` |
| Standard spectrometer detection range | 7.89 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 2,597 Pz (0.05 × Q6) |
| Counter drawn cold (all six layers) | 5,194 Pz (0.10 × Q6) |
| Unravel after completion | 6,231 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Introspection, Flexibility, Hope. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1G 1h 1i 1J` (Within, Light, Life, Potential, Introspection, Flexibility, Hope, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1,037 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 6th Tier quantum of 51,945 Pz (12.0% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 6th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Enchantment school with aspect lean Within, Introspection, Flexibility, Hope. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 6 Workings]] |
| School | [[Enchantment]] |
| Affinity | [[Enchantment]] (E) |
| Function | [[Mind and Will]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Irresistible Dance (6-E-L-ID)|Irresistible Dance]] (6) · [[Dominate Person (5-E-L-DP)|Dominate Person]] (5) · [[Geas (5-E-M-GEA)|Geas]] (5) · [[Hold Monster (5-E-L-HML)|Hold Monster]] (5) · [[Modify Memory (5-E-L-MMD)|Modify Memory]] (5) · [[Antipathy-Sympathy (8-E-L-ASP)|Antipathy/Sympathy]] (8) · [[Compulsion (4-E-L-CMP)|Compulsion]] (4) · [[Confusion (4-E-L-CNF)|Confusion]] (4).


---

## Tactical Assessment

Turns patrols, checkpoints or crowds to new tasks without a fight, such as abandoning a post or escorting someone. Harming the subjects ends it for them.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 6 Workings]] · [[Enchantment]] · [[Spell Breakdown Procedure]] · [[Parzival]]
