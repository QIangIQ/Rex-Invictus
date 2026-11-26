---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/abjuration
  - source/rex-invictus
aliases:
  - "3rd Tier Spell: Bulwark"
  - "Bulwark"
  - "3-A-L-BLW"
registry_id: 3-A-L-BLW
attribute_code: "3·Abj·None·None·Self·Up to 1 minute"
incantation: "Laporse"
tier: 3
school: Abjuration
affinity: A
grade: L
pz_total: 61.3
pz_quantum: 2586.2
t_e: -0.74
updated: 2026-11-16
---

**Bulwark** (`3-A-L-BLW`) is a 3rd Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Rex Invictus original working. Its modelled draw is **61.3 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E -0.74 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Abjuration]]
        - **Bulwark** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-A-L-BLW` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Abj·None·None·Self·Up to 1 minute` |
| Incantation | *Laporse* |
| Affinity | A (Abjuration) |
| Source | Rex Invictus |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Abjuration]] |
| Casting time | 1 reaction |
| Range | Self |
| Area | single point or target |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: a steel rivet |
| Ritual | no |
| Practitioner lineages | Wizard, Cleric, Paladin |

### Effect

Raises a curved ward plate 3 m wide in front of the caster that absorbs up to 60 points of injury from the front arc. The plate can be braced against a single blow to absorb double for that hit.

### Mechanism

A rigid ward plate that spreads incoming injury across its whole area before it reaches the caster.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| absorption capacity, 60 injury points | `0.20*60` | 12.0 |
| plate formation, 3 m^2 at 2.5 Pz/m^2 | `2.5*3` | 7.5 |
| [upkeep] plate hold, 60 s | `0.05*60` | 3.0 |
| Pattern cost | `0.01 × Q3 × (1 + 0.50)` | 38.8 |

| Quantity | Value |
|---|---|
| Effect energy | 19.5 Pz |
| Upkeep energy | 3.0 Pz (0.05 Pz/s) |
| **Total draw** | **61.3 Pz** (91.9 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 0.0237 |
| Energy-equivalent tier T_E | -0.74 |
| Handling points | 0.50 |
| Grade score | -0.50 → L |

**Handling flags:** concentration, reaction cast.

**Assumptions:** Ward areal strength 2.5 Pz/m^2; capacity 60 points.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Bulwark (3-A-L-BLW) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Laporse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vilaporse* · T5: *Tilaporse* · T6: *Rilaporse* · T7: *Milaporse* · T8: *Nilaporse* · T9: *Xyilaporse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#647485`.

![[Bulwark (3-A-L-BLW) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.956 | `#ff0028` (700 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.929 | `#0074ff` (495 nm eq.) | source grid |
| Range | Self | 0.706 | 0.921 | `#0058ff` (488 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 1.79. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·A·None`; the k4 to k6 lines (None, Self, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·A·None` |
| Standard spectrometer detection range | 0.78 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 259 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 10.2 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 3rd Tier quantum of 2,586 Pz (2.4% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Wards and Shields]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Glyph of Warding (3-A-H-GWY)|Glyph of Warding]] (3) · [[Nondetection (3-A-L-NND)|Nondetection]] (3) · [[Protection From Energy (3-A-L-PE)|Protection From Energy]] (3) · [[Aid (2-A-L-AID)|Aid]] (2) · [[Death Ward (4-A-L-DW)|Death Ward]] (4) · [[Leadskin (2-A-L-LDS)|Leadskin]] (2) · [[Protection from Poison (2-A-L-PP)|Protection from Poison]] (2) · [[Stoneskin (4-A-L-STN)|Stoneskin]] (4).


---

## Tactical Assessment

A battlefield caster's frontal armour. It stops a burst of small-arms fire or a light evocation, and is the outer layer that anti-mage primers are built to punch.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
