---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/enchantment
  - source/science-spellbook
aliases:
  - "3rd Tier Spell: Entangle Spell Slots"
  - "3-E-L-ESS"
  - "Entangle Spell Slots (Science)"
registry_id: 3-E-L-ESS
attribute_code: "3·Enc·None·None·30 feet·Up to 10 minutes"
incantation: "Lousinly"
tier: 3
school: Enchantment
affinity: E
grade: L
pz_total: 64.2
pz_quantum: 2586.2
t_e: -0.70
updated: 2026-11-16
---

**Entangle Spell Slots** (`3-E-L-ESS`) is a 3rd Tier working of the [[Enchantment]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **64.2 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E -0.70 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Enchantment]]
        - **Entangle Spell Slots** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-E-L-ESS` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Enc·None·None·30 feet·Up to 10 minutes` |
| Incantation | *Lousinly* |
| Affinity | E (Enchantment) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Enchantment]] |
| Casting time | 1 Action |
| Range | 30 feet |
| Area | single point or target |
| Duration | Up to 10 minutes (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A piece of string |
| Ritual | no |
| Resistance check | presence; on success: no effect |
| Practitioner lineages | Wizard, Sorcerer, Warlock, Bard |

### Mechanism

Couples the field access of caster and target so each working by one drains a working of matching tier from the other.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Linked field access, 2 creatures (upkeep) | `enchantment 0.005 x 2: 0.01 Pz/s x 600 s` | 6.0 |
| Pattern cost | `0.01 × Q3 × (1 + 1.25)` | 58.2 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 6.0 Pz (0.01 Pz/s) |
| **Total draw** | **64.2 Pz** (96.3 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 0.0248 |
| Energy-equivalent tier T_E | -0.70 |
| Handling points | 1.25 |
| Grade score | 0.25 → L |

**Handling flags:** concentration, fragile.

**Assumptions:** Enchantment rate on two linked creatures for 10 minutes.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Entangle Spell Slots (3-E-L-ESS) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Enchantment | 3 | `0000000000111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Up to 10 minutes | 15 | `0000000011111` |

### Incantation

Spoken as **Lousinly** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vilousinly* · T5: *Tilousinly* · T6: *Rilousinly* · T7: *Milousinly* · T8: *Nilousinly* · T9: *Xyilousinly*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 1→12 2→0 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 2→9 3→10 4→11 | 5 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#58c43a`.

![[Entangle Spell Slots (3-E-L-ESS) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| School | Enchantment | 0.375 | 0.997 | `#20ff00` (588 nm eq.) | source grid |
| Duration | Up to 10 minutes | 0.789 | 0.887 | `#1e00ff` (463 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 1.000 | `#91ff00` (612 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 1.81. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·E·None`; the k4 to k6 lines (None, 30 feet, Up to 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·E·None` |
| Standard spectrometer detection range | 0.80 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 260 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Introspection, Flexibility, Hope. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1G 1h 1i 1J` (Within, Light, Life, Potential, Introspection, Flexibility, Hope, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 10.7 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 3rd Tier quantum of 2,586 Pz (2.5% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Enchantment school with aspect lean Within, Introspection, Flexibility, Hope. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Enchantment]] |
| Affinity | [[Enchantment]] (E) |
| Function | [[Terrain and Matter Shaping]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Arcane Redirection (3-A-L-AR)|Arcane Redirection]] (3) · [[Create Food and Water (3-C-L-CFW)|Create Food and Water]] (3) · [[Entangled Attacks (1-E-L-EAT)|Entangled Attacks]] (1) · [[Meld Into Stone (3-T-M-MIS)|Meld Into Stone]] (3) · [[Plant Growth (3-T-M-PG)|Plant Growth]] (3) · [[Sleet Storm (3-C-L-SS)|Sleet Storm]] (3) · [[Control Water (4-T-H-CWN)|Control Water]] (4) · [[Fabricate (4-T-L-FBR)|Fabricate]] (4).


---

## Tactical Assessment

Counter-caster duel tool; can strip an enemy caster, at equal cost to oneself.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Enchantment]] · [[Spell Breakdown Procedure]] · [[Parzival]]
