---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/abjuration
  - source/srd
aliases:
  - "4th Tier Spell: Stoneskin"
  - "Stoneskin"
  - "4-A-L-STN"
registry_id: 4-A-L-STN
attribute_code: "4·Abj·None·None·Touch·Up to 1 hour"
incantation: "Valixsi"
tier: 4
school: Abjuration
affinity: A
grade: L
pz_total: 150.0
pz_quantum: 7029.9
t_e: 0.15
updated: 2026-11-16
---

**Stoneskin** (`4-A-L-STN`) is a 4th Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **150 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E 0.15 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Abjuration]]
        - **Stoneskin** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-A-L-STN` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Abj·None·None·Touch·Up to 1 hour` |
| Incantation | *Valixsi* |
| Affinity | A (Abjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Abjuration]] |
| Casting time | 1 action |
| Range | Touch |
| Area | single point or target |
| Duration | Up to 1 hour (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Diamond dust worth 100 gp, which the spell consumes |
| Ritual | no |
| Practitioner lineages | Druid, Ranger, Sorcerer, Wizard |

### Mechanism

The subject's skin takes on the hardness of stone, halving injury from ordinary blunt, piercing and cutting weapons.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Skin hardening | `3 Pz/kg * 4 kg dermis` | 12.0 |
| Upkeep: Physical-injury absorption over 1 h | `0.20 * 75 HP (10 rounds * 15 HP, halved)` | 15.0 |
| Pattern cost | `0.01 × Q4 × (1 + 0.75)` | 123 |

| Quantity | Value |
|---|---|
| Effect energy | 12.0 Pz |
| Upkeep energy | 15.0 Pz (0.00417 Pz/s) |
| **Total draw** | **150 Pz** (225.0 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 0.0213 |
| Energy-equivalent tier T_E | 0.15 |
| Handling points | 0.75 |
| Grade score | -0.25 → L |

**Handling flags:** concentration, costly material, consumed material.

**Assumptions:** 4 kg skin restructured; 10 rounds of 15 HP/round physical incoming; resistance halves it.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Stoneskin (4-A-L-STN) glyph.svg]]

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

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

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

![[Stoneskin (4-A-L-STN) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.923 | `#ff0028` (700 nm eq.) | source grid |
| Duration | Up to 1 hour | 0.632 | 0.974 | `#00c0ff` (511 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.890 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.23): swatch `#979b94`, measured lines at 0.007, 0.401, 0.632, 0.883. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.18. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·A·None`; the k4 to k6 lines (None, Touch, Up to 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·A·None` |
| Standard spectrometer detection range | 1.22 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 706 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 25.0 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 4th Tier quantum of 7,030 Pz (2.1% of it). |
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
| Function | [[Wards and Shields]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Death Ward (4-A-L-DW)|Death Ward]] (4) · [[Bulwark (3-A-L-BLW)|Bulwark]] (3) · [[Glyph of Warding (3-A-H-GWY)|Glyph of Warding]] (3) · [[Nondetection (3-A-L-NND)|Nondetection]] (3) · [[Protection From Energy (3-A-L-PE)|Protection From Energy]] (3) · [[Aid (2-A-L-AID)|Aid]] (2) · [[Fire Shield (4-V-L-FSR)|Fire Shield]] (4) · [[Globe of Invulnerability (6-A-L-GIO)|Globe of Invulnerability]] (6).


---

## Tactical Assessment

Protects a key operator against small-arms fragments and blades; offers nothing against energy weapons or enchanted munitions.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
