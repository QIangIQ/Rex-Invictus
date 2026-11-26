---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/transmutation
  - source/science-spellbook
aliases:
  - "1st Tier Spell: Reduce Relative Velocity"
  - "1-T-L-RRV"
  - "Reduce Relative Velocity (Science)"
registry_id: 1-T-L-RRV
attribute_code: "1·Tra·None·None·30 feet·1 round"
incantation: "Sieusini"
tier: 1
school: Transmutation
affinity: T
grade: L
pz_total: 9.7
pz_quantum: 350.0
t_e: -2.58
updated: 2026-11-16
---

**Reduce Relative Velocity** (`1-T-L-RRV`) is a 1st Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **9.7 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -2.58 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Transmutation]]
        - **Reduce Relative Velocity** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-T-L-RRV` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Tra·None·None·30 feet·1 round` |
| Incantation | *Sieusini* |
| Affinity | T (Transmutation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Transmutation]] |
| Casting time | 1 reaction, which you take when you see an object within 30 feet of you moves or when you move or are within 30 feet of an object |
| Range | 30 feet |
| Area | single point or target |
| Duration | 1 round |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Wizard, Sorcerer, Warlock, Bard, Druid |

### Mechanism

Locks the caster and an object to the same velocity for one round, then halts both.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Velocity matched | `0.5 x 80 kg x (10 m/s)^2 = 4000 J / 1500` | 2.7 |
| Both halted | `0.5 x 80 kg x (10 m/s)^2 = 4000 J / 1500` | 2.7 |
| Pattern cost | `0.01 × Q1 × (1 + 0.25)` | 4.4 |

| Quantity | Value |
|---|---|
| Effect energy | 5.3 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **9.7 Pz** (14.6 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.0277 |
| Energy-equivalent tier T_E | -2.58 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** reaction cast.

**Assumptions:** Object and caster 80 kg each; matching then stopping at 10 m/s.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Reduce Relative Velocity (1-T-L-RRV) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | 1 round | 2 | `0000000000101` |

### Incantation

Spoken as **Sieusini** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisieusini* · T3: *Lisieusini* · T4: *Visieusini* · T5: *Tisieusini* · T6: *Risieusini* · T7: *Misieusini* · T8: *Nisieusini* · T9: *Xyisieusini*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 2→9 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#cd8a32`.

![[Reduce Relative Velocity (1-T-L-RRV) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.741 | `#9600ff` (438 nm eq.) | source grid |
| Duration | 1 round | 0.158 | 0.998 | `#ffae00` (653 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.981 | `#91ff00` (612 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 0.99. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·T·None`; the k4 to k6 lines (None, 30 feet, 1 round) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·T·None` |
| Standard spectrometer detection range | 0.31 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.0 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1.6 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (2.8% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Transformation]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Crystalise (1-T-L-CRY)|Crystalise]] (1) · [[Alter Self (2-T-L-AST)|Alter Self]] (2) · [[Enlarge-Reduce (2-T-M-ERL)|Enlarge/Reduce]] (2) · [[Chemical Transition (3-T-L-CTE)|Chemical Transition]] (3) · [[Gaseous Form (3-T-M-GF)|Gaseous Form]] (3) · [[Polymorph (4-T-L-PLY)|Polymorph]] (4) · [[Temporary Magic Prism (2-C-L-TMP)|Temporary Magic Prism]] (2) · [[Alter Weight (1-T-L-AWT)|Alter Weight]] (1).


---

## Tactical Assessment

Boarding moving vehicles, matching a falling object, or stopping a rolling load.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
