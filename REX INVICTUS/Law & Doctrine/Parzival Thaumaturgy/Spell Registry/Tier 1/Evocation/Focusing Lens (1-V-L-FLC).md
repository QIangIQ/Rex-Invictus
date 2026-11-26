---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/evocation
  - source/science-spellbook
aliases:
  - "1st Tier Spell: Focusing Lens"
  - "1-V-L-FLC"
  - "Focusing Lens (Science)"
registry_id: 1-V-L-FLC
attribute_code: "1·Evo·Fire·None·15 feet·Instantaneous"
incantation: "Suire-’bal"
tier: 1
school: Evocation
affinity: V
grade: L
pz_total: 3.9
pz_quantum: 350.0
t_e: -3.49
updated: 2026-11-16
---

**Focusing Lens** (`1-V-L-FLC`) is a 1st Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **3.9 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -3.49 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Evocation]]
        - **Focusing Lens** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-V-L-FLC` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Evo·Fire·None·15 feet·Instantaneous` |
| Incantation | *Suire-’bal* |
| Affinity | V (Evocation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Evocation]] |
| Casting time | 1 Action |
| Range | 15 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A lens |
| Ritual | no |
| Injury | 2d4 fire (mean 5) |
| Injury by tier | T1: 2d4, T2: 3d4, T3: 4d4, T4: 5d4, T5: 6d4, T6: 7d4, T7: 8d4, T8: 9d4, T9: 10d4 |
| Practitioner lineages | Wizard, Sorcerer, Ranger, Druid, Warlock |

### Mechanism

Conjures a lens that concentrates ambient light onto a point within 15 ft; power depends on available light.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Lens conjured | `0.05 kg x 3 Pz/kg` | 0.15 |
| Focused sunlight | `5 HP x 0.7 (fire) x F 0.08` | 0.28 |
| Pattern cost | `0.01 × Q1 × (1 + 0.00)` | 3.5 |

| Quantity | Value |
|---|---|
| Effect energy | 0.43 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **3.9 Pz** (5.9 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.0112 |
| Energy-equivalent tier T_E | -3.49 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Broad daylight 2d4 = 5 fire at a focused point F 0.08; lens 0.05 kg glass at 3 Pz/kg.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Focusing Lens (1-V-L-FLC) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Fire | 3 | `0000000000111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 15 feet | 18 | `0000000100101` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Suire-’bal** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisuire-’bal* · T3: *Lisuire-’bal* · T4: *Visuire-’bal* · T5: *Tisuire-’bal* · T6: *Risuire-’bal* · T7: *Misuire-’bal* · T8: *Nisuire-’bal* · T9: *Xyisuire-’bal*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 | 3 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 5→0 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#bba622`.

![[Focusing Lens (1-V-L-FLC) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| Damage | Fire | 0.286 | 0.983 | `#9cff00` (614 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.923 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.995 | `#ff0028` (700 nm eq.) | source grid |
| Range | 15 feet | 0.206 | 0.994 | `#ffef00` (638 nm eq.) | RI half-step |

Relative luminosity scales with initial energy: log10(E) = 0.59. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·V·Fire`; the k4 to k6 lines (None, 15 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·V·Fire` |
| Standard spectrometer detection range | 0.20 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.0 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Energy, Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `2b 1c 3f 2j` (2x Heat, Light, 3x Energy, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 0.655 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (1.1% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Divination and Sensing]], [[Precision Strikes]] |
| Element | [[Fire Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Hellish Rebuke (1-V-L-HR)|Hellish Rebuke]] (1) · [[Fire Bolt (0-V-L-FB)|Fire Bolt]] (0) · [[Flame Blade (2-V-L-FBA)|Flame Blade]] (2) · [[Sacred Flame (0-V-L-SF)|Sacred Flame]] (0) · [[Scorching Ray (2-V-L-SR)|Scorching Ray]] (2) · [[Flaming Sphere (2-C-L-FSA)|Flaming Sphere]] (2) · [[Heat Metal (2-T-M-HM)|Heat Metal]] (2) · [[Produce Flame (0-C-L-PF)|Produce Flame]] (0).


---

## Tactical Assessment

Silent fire starting and a weak burning point in daylight.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
