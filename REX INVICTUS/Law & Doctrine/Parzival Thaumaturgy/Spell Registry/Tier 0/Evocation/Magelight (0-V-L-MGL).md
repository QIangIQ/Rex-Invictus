---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-0
  - spell/evocation
  - source/rex-invictus
aliases:
  - "Cantrip Spell: Magelight"
  - "Magelight"
  - "0-V-L-MGL"
registry_id: 0-V-L-MGL
attribute_code: "0·Evo·None·sphere (20)·60 feet·10 minutes"
incantation: "Cu’-Sowyns"
tier: 0
school: Evocation
affinity: V
grade: L
pz_total: 42.3
pz_quantum: 128.8
t_e: -1.11
updated: 2026-11-16
---

**Magelight** (`0-V-L-MGL`) is a Cantrip (Tier 0) working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Rex Invictus original working. Its modelled draw is **42.3 Pz** against a slot quantum of 129 Pz, which puts its energy-equivalent tier at T_E -1.11 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 0 Workings]]
      - [[Evocation]]
        - **Magelight** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `0-V-L-MGL` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `0·Evo·None·sphere (20)·60 feet·10 minutes` |
| Incantation | *Cu’-Sowyns* |
| Affinity | V (Evocation) |
| Source | Rex Invictus |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | Cantrip (Tier 0) |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | sphere (20) |
| Duration | 10 minutes |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Wizard, Sorcerer, Cleric, Bard |

### Effect

Kindles a mote of field light that sheds bright light in a 20 foot radius and dim light 20 feet beyond. The mote can be fixed in place, carried, or left to drift.

### Mechanism

Converts field return directly to visible light at high efficiency. The luminous output follows the spectroscopic rule that a stationary low-tier working is dim in its own arcane band.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| ignition | `instant info` | 1.0 |
| [upkeep] 100 W field light, 600 s | `100*600/1500` | 40.0 |
| Pattern cost | `0.01 × Q0 × (1 + 0.00)` | 1.3 |

| Quantity | Value |
|---|---|
| Effect energy | 1.0 Pz |
| Upkeep energy | 40.0 Pz (0.0667 Pz/s) |
| **Total draw** | **42.3 Pz** (63.4 kJ) |
| Slot quantum Q0 | 129 Pz |
| Field gain (draw / quantum) | 0.328 |
| Energy-equivalent tier T_E | -1.11 |
| Handling points | 0.00 |
| Grade score | -0.56 → L |

**Handling flags:** none.

**Assumptions:** Torch-equivalent 100 W of field light for 10 minutes.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Magelight (0-V-L-MGL) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 0 | 0 | `0000000000001` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (20) | 30 | `0000000111101` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | 10 minutes | 4 | `0000000001001` |

### Incantation

Spoken as **Cu’-Sowyns** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T1: *Sicu’-Sowyns* · T2: *Hicu’-Sowyns* · T3: *Licu’-Sowyns* · T4: *Vicu’-Sowyns* · T5: *Ticu’-Sowyns* · T6: *Ricu’-Sowyns* · T7: *Micu’-Sowyns* · T8: *Nicu’-Sowyns* · T9: *Xyicu’-Sowyns*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 | 1 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 2→11 3→12 4→0 5→1 | 5 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 3→10 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#719b7e`.

![[Magelight (0-V-L-MGL) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 0 | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.882 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | 10 minutes | 0.263 | 0.966 | `#bdff00` (621 nm eq.) | source grid |
| Area | sphere (20) | 0.833 | 0.707 | `#5a00ff` (450 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.841 | `#00fbff` (524 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 1.63. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `0·V·None`; the k4 to k6 lines (sphere (20), 60 feet, 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `0·V·None` |
| Standard spectrometer detection range | 0.65 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 6.4 Pz (0.05 × Q0) |
| Counter drawn cold (all six layers) | 12.9 Pz (0.10 × Q0) |
| Unravel after completion | 20.9 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1b 1c 1d 1f` (Heat, Light, Life, Energy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 7.0 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the Cantrip (Tier 0) quantum of 129 Pz (32.8% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at Cantrip (Tier 0) up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 0 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Light and Radiance]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Dancing Lights (0-V-L-DL)|Dancing Lights]] (0) · [[Light (0-V-L-LGH)|Light]] (0) · [[Sacred Flame (0-V-L-SF)|Sacred Flame]] (0) · [[Faerie Fire (1-V-L-FF)|Faerie Fire]] (1) · [[Guiding Bolt (1-V-L-GB)|Guiding Bolt]] (1) · [[Continual Flame (2-V-M-CF)|Continual Flame]] (2) · [[Moonbeam (2-V-M-MNB)|Moonbeam]] (2) · [[Color Spray (1-I-L-CS)|Color Spray]] (1).


---

## Tactical Assessment

Illumination and marking. It is the payload of the marker flare combination.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 0 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
