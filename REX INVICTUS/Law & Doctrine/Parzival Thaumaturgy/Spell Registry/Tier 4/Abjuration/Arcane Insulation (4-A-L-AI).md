---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/abjuration
  - source/science-spellbook
aliases:
  - "4th Tier Spell: Arcane Insulation"
  - "4-A-L-AI"
  - "Arcane Insulation (Science)"
registry_id: 4-A-L-AI
attribute_code: "4·Abj·None·None·Touch·Up to 1 hour"
incantation: "Valixsi"
tier: 4
school: Abjuration
affinity: A
grade: L
pz_total: 99.9
pz_quantum: 7029.9
t_e: -0.25
updated: 2026-11-16
---

**Arcane Insulation** (`4-A-L-AI`) is a 4th Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **99.9 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E -0.25 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Abjuration]]
        - **Arcane Insulation** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-A-L-AI` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Abj·None·None·Touch·Up to 1 hour` |
| Incantation | *Valixsi* |
| Affinity | A (Abjuration) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Abjuration]] |
| Casting time | 1 Action |
| Range | Touch |
| Area | single point or target |
| Duration | Up to 1 hour (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: At least 10 feathers |
| Ritual | no |
| Practitioner lineages | Wizard, Sorcerer, Warlock, Cleric |

### Mechanism

Wraps one creature in a thermal barrier that halves heat and cold injury for an hour.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Thermal barrier absorption | `0.20 Pz x 60 absorbed` | 12.0 |
| Pattern cost | `0.01 × Q4 × (1 + 0.25)` | 87.9 |

| Quantity | Value |
|---|---|
| Effect energy | 12.0 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **99.9 Pz** (149.8 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 0.0142 |
| Energy-equivalent tier T_E | -0.25 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** concentration.

**Assumptions:** Expected incoming heat and cold injury over the hour 120, halved by the barrier, so 60 absorbed at 0.20 Pz each.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Arcane Insulation (4-A-L-AI) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 4 | 4 | `0000000001001` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Up to 1 hour | 12 | `0000000011001` |

### Incantation

Spoken as **Valixsi** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T5: *Tivalixsi* · T6: *Rivalixsi* · T7: *Mivalixsi* · T8: *Nivalixsi* · T9: *Xyivalixsi*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]]. This attribute set is shared with other workings, so the glyph carries 1 centre dot(s) to tell it apart.

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 3→2 | 2 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 3→10 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#627487`.

![[Arcane Insulation (4-A-L-AI) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.923 | `#ff0028` (700 nm eq.) | source grid |
| Duration | Up to 1 hour | 0.632 | 0.974 | `#00c0ff` (511 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.890 | `#9b00ff` (435 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 2.00. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·A·None`; the k4 to k6 lines (None, Touch, Up to 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·A·None` |
| Standard spectrometer detection range | 1.00 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 703 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 16.6 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 4th Tier quantum of 7,030 Pz (1.4% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 4th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 4 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Negation and Counterspell]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Banishment (4-A-M-BNS)|Banishment]] (4) · [[Private Sanctum (4-A-L-PSI)|Private Sanctum]] (4) · [[Antilife Shell (5-A-L-ASI)|Antilife Shell]] (5) · [[Counterspell (3-A-L-CNT)|Counterspell]] (3) · [[Dispel Evil and Good (5-A-L-DEGP)|Dispel Evil and Good]] (5) · [[Dispel Magic (3-A-L-DM)|Dispel Magic]] (3) · [[Nondetection (3-A-L-NND)|Nondetection]] (3) · [[Remove Curse (3-A-L-RC)|Remove Curse]] (3).


---

## Tactical Assessment

Lets assault teams cross burning or cryogenic zones and resist incendiary weapons.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
