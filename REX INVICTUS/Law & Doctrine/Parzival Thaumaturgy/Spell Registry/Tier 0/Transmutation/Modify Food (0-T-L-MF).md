---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-0
  - spell/transmutation
  - source/science-spellbook
aliases:
  - "Cantrip Spell: Modify Food"
  - "0-T-L-MF"
  - "Modify Food (Science)"
registry_id: 0-T-L-MF
attribute_code: "0·Tra·None·None·5 feet·Instantaneous"
incantation: "Ciewosin"
tier: 0
school: Transmutation
affinity: T
grade: L
pz_total: 43.6
pz_quantum: 128.8
t_e: -1.08
updated: 2026-11-16
---

**Modify Food** (`0-T-L-MF`) is a Cantrip (Tier 0) working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **43.6 Pz** against a slot quantum of 129 Pz, which puts its energy-equivalent tier at T_E -1.08 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 0 Workings]]
      - [[Transmutation]]
        - **Modify Food** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `0-T-L-MF` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `0·Tra·None·None·5 feet·Instantaneous` |
| Incantation | *Ciewosin* |
| Affinity | T (Transmutation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | Cantrip (Tier 0) |
| School | [[Transmutation]] |
| Casting time | 1 Action |
| Range | 5 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Food dye |
| Ritual | no |
| Practitioner lineages | Wizard, Sorcerer, Druid, Bard, Warlock |

### Mechanism

Changes the colour, texture, flavour, temperature or density of one item of food without changing its nutrition.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Food heated | `food item: 0.3 kg x 3500 J/kgK x 60 K / 1500` | 42.0 |
| Texture and flavour rework | `0.3 kg x 1 Pz/kg` | 0.3 |
| Pattern cost | `0.01 × Q0 × (1 + 0.00)` | 1.3 |

| Quantity | Value |
|---|---|
| Effect energy | 42.3 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **43.6 Pz** (65.4 kJ) |
| Slot quantum Q0 | 129 Pz |
| Field gain (draw / quantum) | 0.339 |
| Energy-equivalent tier T_E | -1.08 |
| Handling points | 0.00 |
| Grade score | -0.54 → L |

**Handling flags:** none.

**Assumptions:** Food item 0.3 kg heated by 60 K (c = 3500 J/kgK) plus texture rework at 1 Pz/kg.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Modify Food (0-T-L-MF) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 0 | 0 | `0000000000001` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 5 feet | 7 | `0000000001111` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Ciewosin** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T1: *Siciewosin* · T2: *Hiciewosin* · T3: *Liciewosin* · T4: *Viciewosin* · T5: *Ticiewosin* · T6: *Riciewosin* · T7: *Miciewosin* · T8: *Niciewosin* · T9: *Xyiciewosin*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 | 1 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 | 4 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#aa414a`.

![[Modify Food (0-T-L-MF) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 0 | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.682 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| Range | 5 feet | 0.412 | 0.919 | `#00ff10` (576 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 1.64. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `0·T·None`; the k4 to k6 lines (None, 5 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `0·T·None` |
| Standard spectrometer detection range | 0.66 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 6.4 Pz (0.05 × Q0) |
| Counter drawn cold (all six layers) | 12.9 Pz (0.10 × Q0) |
| Unravel after completion | 12.9 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 7.3 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the Cantrip (Tier 0) quantum of 129 Pz (33.9% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at Cantrip (Tier 0) up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 0 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Divination and Sensing]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Message (0-T-L-MSS)|Message]] (0) · [[Reflective Coating (0-T-L-RCF)|Reflective Coating]] (0) · [[Stress (Non-Battle) (0-T-L-SNBE)|Stress (Non-Battle)]] (0) · [[Alter Projectile Velocity (2-T-L-APV)|Alter Projectile Velocity]] (2) · [[Arcane Gravitational Lens (0-D-L-AGL)|Arcane Gravitational Lens]] (0) · [[Darkvision (2-T-L-DRKK)|Darkvision]] (2) · [[Guidance (0-D-L-GDN)|Guidance]] (0) · [[Hooke's Compelled Duel (0-E-L-HSCD)|Hooke's Compelled Duel]] (0).


---

## Tactical Assessment

Morale and field cooking; hot meals without fire signatures.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 0 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
