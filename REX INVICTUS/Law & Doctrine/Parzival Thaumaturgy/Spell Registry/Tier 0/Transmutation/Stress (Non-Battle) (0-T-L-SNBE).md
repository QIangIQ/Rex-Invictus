---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-0
  - spell/transmutation
  - source/science-spellbook
aliases:
  - "Cantrip Spell: Stress (Non-Battle)"
  - "0-T-L-SNBE"
  - "Stress (Non-Battle) (Science)"
registry_id: 0-T-L-SNBE
attribute_code: "0·Tra·None·None·15 feet·Instantaneous"
incantation: "Ciebal"
tier: 0
school: Transmutation
affinity: T
grade: L
pz_total: 1.4
pz_quantum: 128.8
t_e: -4.55
updated: 2026-11-16
---

**Stress (Non-Battle)** (`0-T-L-SNBE`) is a Cantrip (Tier 0) working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **1.4 Pz** against a slot quantum of 129 Pz, which puts its energy-equivalent tier at T_E -4.55 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 0 Workings]]
      - [[Transmutation]]
        - **Stress (Non-Battle)** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `0-T-L-SNBE` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `0·Tra·None·None·15 feet·Instantaneous` |
| Incantation | *Ciebal* |
| Affinity | T (Transmutation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | Cantrip (Tier 0) |
| School | [[Transmutation]] |
| Casting time | 1 Action |
| Range | 15 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A copy of "Theory of Magic" |
| Ritual | no |
| Practitioner lineages | Druid, Sorcerer, Warlock, Wizard |

### Mechanism

Applies a controlled stress to an object up to 5 ft across to bend, shear or break it.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Plastic work | `bend 1 mm sheet steel = 100 J / 1500` | 0.0667 |
| Pattern cost | `0.01 × Q0 × (1 + 0.00)` | 1.3 |

| Quantity | Value |
|---|---|
| Effect energy | 0.0667 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **1.4 Pz** (2.0 kJ) |
| Slot quantum Q0 | 129 Pz |
| Field gain (draw / quantum) | 0.0105 |
| Energy-equivalent tier T_E | -4.55 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Plastic bending of 1 mm sheet steel taken as 100 J.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Stress (Non-Battle) (0-T-L-SNBE) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 0 | 0 | `0000000000001` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 15 feet | 18 | `0000000100101` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Ciebal** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T1: *Siciebal* · T2: *Hiciebal* · T3: *Liciebal* · T4: *Viciebal* · T5: *Ticiebal* · T6: *Riciebal* · T7: *Miciebal* · T8: *Niciebal* · T9: *Xyiciebal*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 | 1 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 5→0 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#eb3f45`.

![[Stress (Non-Battle) (0-T-L-SNBE) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 0 | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.682 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| Range | 15 feet | 0.206 | 0.979 | `#ffef00` (638 nm eq.) | RI half-step |

Relative luminosity scales with initial energy: log10(E) = 0.13. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `0·T·None`; the k4 to k6 lines (None, 15 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `0·T·None` |
| Standard spectrometer detection range | 0.12 km (r = 1 km × √(E/100 Pz)) |
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
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 0.226 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the Cantrip (Tier 0) quantum of 129 Pz (1.1% of it). |
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
| Function | [[Divination and Sensing]], [[Terrain and Matter Shaping]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Reflective Coating (0-T-L-RCF)|Reflective Coating]] (0) · [[Druidcraft (0-T-L-DRD)|Druidcraft]] (0) · [[Mending (0-T-L-MND)|Mending]] (0) · [[Message (0-T-L-MSS)|Message]] (0) · [[Modify Food (0-T-L-MF)|Modify Food]] (0) · [[Prestidigitation (0-T-L-PRS)|Prestidigitation]] (0) · [[Sharpen (0-T-L-SHR)|Sharpen]] (0) · [[Thaumaturgy (0-T-L-THM)|Thaumaturgy]] (0).


---

## Tactical Assessment

Silent breaking of windows, locks and thin sheet metal.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 0 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
