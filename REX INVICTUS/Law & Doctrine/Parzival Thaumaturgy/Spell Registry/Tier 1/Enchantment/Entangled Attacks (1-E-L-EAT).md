---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/enchantment
  - source/science-spellbook
aliases:
  - "1st Tier Spell: Entangled Attacks"
  - "1-E-L-EAT"
  - "Entangled Attacks (Science)"
registry_id: 1-E-L-EAT
attribute_code: "1·Enc·None·None·150 feet·1 minute"
incantation: "Sonosine"
tier: 1
school: Enchantment
affinity: E
grade: L
pz_total: 3.8
pz_quantum: 350.0
t_e: -3.52
updated: 2026-11-16
---

**Entangled Attacks** (`1-E-L-EAT`) is a 1st Tier working of the [[Enchantment]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **3.8 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -3.52 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Enchantment]]
        - **Entangled Attacks** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-E-L-EAT` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Enc·None·None·150 feet·1 minute` |
| Incantation | *Sonosine* |
| Affinity | E (Enchantment) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Enchantment]] |
| Casting time | 1 Bonus Action |
| Range | 150 feet |
| Area | single point or target |
| Duration | 1 minute |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Resistance check | will; on success: no effect |
| Practitioner lineages | Wizard, Sorcerer, Warlock, Druid |

### Mechanism

Links the aim of caster and target so one strike can borrow or impose the other side's last result.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Aim link (upkeep) | `enchantment rate: 0.005 Pz/s x 60 s` | 0.3 |
| Pattern cost | `0.01 × Q1 × (1 + 0.00)` | 3.5 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 0.3 Pz (0.005 Pz/s) |
| **Total draw** | **3.8 Pz** (5.7 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.0109 |
| Energy-equivalent tier T_E | -3.52 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Enchantment rate on one creature for 1 minute.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Entangled Attacks (1-E-L-EAT) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Enchantment | 3 | `0000000000111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 150 feet | 4 | `0000000001001` |
| k6 Duration | 1 minute | 1 | `0000000000011` |

### Incantation

Spoken as **Sonosine** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisonosine* · T3: *Lisonosine* · T4: *Visonosine* · T5: *Tisonosine* · T6: *Risonosine* · T7: *Misonosine* · T8: *Nisonosine* · T9: *Xyisonosine*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 1→12 2→0 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 | 2 |
| k6 Duration | 0→7 1→8 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#c1ae00`.

![[Entangled Attacks (1-E-L-EAT) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Enchantment | 0.375 | 0.963 | `#20ff00` (588 nm eq.) | source grid |
| Duration | 1 minute | 0.105 | 1.000 | `#ff6300` (668 nm eq.) | source grid |
| Range | 150 feet | 0.235 | 0.991 | `#e3ff00` (629 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 0.58. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·E·None`; the k4 to k6 lines (None, 150 feet, 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·E·None` |
| Standard spectrometer detection range | 0.19 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.1 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Introspection, Flexibility, Hope. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1G 1h 1i 1J` (Within, Light, Life, Potential, Introspection, Flexibility, Hope, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 0.633 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (1.1% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Enchantment school with aspect lean Within, Introspection, Flexibility, Hope. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Enchantment]] |
| Affinity | [[Enchantment]] (E) |
| Function | [[Terrain and Matter Shaping]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Create or Destroy Water (1-T-L-CDW)|Create or Destroy Water]] (1) · [[Entangle (1-C-M-ENT)|Entangle]] (1) · [[Entangle Spell Slots (3-E-L-ESS)|Entangle Spell Slots]] (3) · [[Glue (1-T-L-GLU)|Glue]] (1) · [[Grease (1-C-L-GRS)|Grease]] (1) · [[Purify Food and Drink (1-T-L-PFD)|Purify Food and Drink]] (1) · [[Summon Liquid (1-C-L-SL)|Summon Liquid]] (1) · [[Summon Metal (1-C-L-SM)|Summon Metal]] (1).


---

## Tactical Assessment

Spoils an elite marksman's aim or borrows it for one shot.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Enchantment]] · [[Spell Breakdown Procedure]] · [[Parzival]]
