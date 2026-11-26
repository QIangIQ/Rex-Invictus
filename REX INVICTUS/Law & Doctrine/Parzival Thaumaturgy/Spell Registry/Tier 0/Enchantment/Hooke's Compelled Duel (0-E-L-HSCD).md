---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-0
  - spell/enchantment
  - source/science-spellbook
aliases:
  - "Cantrip Spell: Hooke's Compelled Duel"
  - "0-E-L-HSCD"
  - "Hooke's Compelled Duel (Science)"
registry_id: 0-E-L-HSCD
attribute_code: "0·Enc·None·None·30 feet·Up to 1 minute"
incantation: "Cousinse"
tier: 0
school: Enchantment
affinity: E
grade: L
pz_total: 26.9
pz_quantum: 128.8
t_e: -1.57
updated: 2026-11-16
---

**Hooke's Compelled Duel** (`0-E-L-HSCD`) is a Cantrip (Tier 0) working of the [[Enchantment]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **26.9 Pz** against a slot quantum of 129 Pz, which puts its energy-equivalent tier at T_E -1.57 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 0 Workings]]
      - [[Enchantment]]
        - **Hooke's Compelled Duel** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `0-E-L-HSCD` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `0·Enc·None·None·30 feet·Up to 1 minute` |
| Incantation | *Cousinse* |
| Affinity | E (Enchantment) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | Cantrip (Tier 0) |
| School | [[Enchantment]] |
| Casting time | 1 Bonus Action |
| Range | 30 feet |
| Area | single point or target |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A spring |
| Ritual | no |
| Resistance check | strength; on success: no effect |
| Practitioner lineages | Wizard, Sorcerer, Warlock, Ranger, Bard, Cleric, Paladin |

### Mechanism

Ties caster and target with an elastic field whose restoring force grows with separation and snaps beyond 30 ft.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Spring restoring work (upkeep) | `400 N x 9 m x 10 rounds = 3.6e+04 J / 1500` | 24.0 |
| Pattern cost | `0.01 × Q0 × (1 + 1.25)` | 2.9 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 24.0 Pz (0.4 Pz/s) |
| **Total draw** | **26.9 Pz** (40.3 kJ) |
| Slot quantum Q0 | 129 Pz |
| Field gain (draw / quantum) | 0.209 |
| Energy-equivalent tier T_E | -1.57 |
| Handling points | 1.25 |
| Grade score | 0.47 → L |

**Handling flags:** concentration, fragile.

**Assumptions:** Restoring force about 400 N worked over 9 m per round for 10 rounds.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Hooke's Compelled Duel (0-E-L-HSCD) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 0 | 0 | `0000000000001` |
| k2 School | Enchantment | 3 | `0000000000111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Cousinse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T1: *Sicousinse* · T2: *Hicousinse* · T3: *Licousinse* · T4: *Vicousinse* · T5: *Ticousinse* · T6: *Ricousinse* · T7: *Micousinse* · T8: *Nicousinse* · T9: *Xyicousinse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 | 1 |
| k2 School | 0→11 1→12 2→0 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#739b41`.

![[Hooke's Compelled Duel (0-E-L-HSCD) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 0 | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| School | Enchantment | 0.375 | 0.932 | `#20ff00` (588 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.791 | `#0074ff` (495 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.958 | `#91ff00` (612 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 1.43. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `0·E·None`; the k4 to k6 lines (None, 30 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `0·E·None` |
| Standard spectrometer detection range | 0.52 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 6.4 Pz (0.05 × Q0) |
| Counter drawn cold (all six layers) | 12.9 Pz (0.10 × Q0) |
| Unravel after completion | 17.7 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Introspection, Flexibility, Hope. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1G 1h 1i 1J` (Within, Light, Life, Potential, Introspection, Flexibility, Hope, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 4.5 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the Cantrip (Tier 0) quantum of 129 Pz (20.9% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at Cantrip (Tier 0) up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Enchantment school with aspect lean Within, Introspection, Flexibility, Hope. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 0 Workings]] |
| School | [[Enchantment]] |
| Affinity | [[Enchantment]] (E) |
| Function | [[Divination and Sensing]], [[Negation and Counterspell]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Animal Messenger (2-E-L-AM)|Animal Messenger]] (2) · [[Hunter's Mark (1-D-L-HSM)|Hunter's Mark]] (1) · [[Blindness-Deafness (2-N-L-BD)|Blindness/Deafness]] (2) · [[Knock (2-T-L-KNC)|Knock]] (2) · [[Nondetection (3-A-L-NND)|Nondetection]] (3) · [[Arcane Die (0-C-L-ADC)|Arcane Die]] (0) · [[Arcane Gravitational Lens (0-D-L-AGL)|Arcane Gravitational Lens]] (0) · [[Guidance (0-D-L-GDN)|Guidance]] (0).


---

## Tactical Assessment

Keeps a fleeing officer or runner from breaking contact; pins an enemy champion into a duel.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 0 Workings]] · [[Enchantment]] · [[Spell Breakdown Procedure]] · [[Parzival]]
