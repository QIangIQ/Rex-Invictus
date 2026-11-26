---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-8
  - spell/evocation
  - source/srd
aliases:
  - "8th Tier Spell: Earthquake"
  - "Earthquake"
  - "8-V-M-ERT"
registry_id: 8-V-M-ERT
attribute_code: "8·Evo·None·sphere (100)·500 feet·Up to 1 minute"
incantation: "Nu’-Sasinse"
tier: 8
school: Evocation
affinity: V
grade: M
pz_total: 641690.0
pz_quantum: 383821.6
t_e: 8.51
updated: 2026-11-16
---

**Earthquake** (`8-V-M-ERT`) is a 8th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **641,690 Pz** against a slot quantum of 383,822 Pz, which puts its energy-equivalent tier at T_E 8.51 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 8 Workings]]
      - [[Evocation]]
        - **Earthquake** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `8-V-M-ERT` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `8·Evo·None·sphere (100)·500 feet·Up to 1 minute` |
| Incantation | *Nu’-Sasinse* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 8th Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 500 feet |
| Area | sphere (100) |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A pinch of dirt, a piece of rock, and a lump of clay |
| Ritual | no |
| Practitioner lineages | Cleric, Druid, Sorcerer |

### Mechanism

The field drives an intense ground tremor through a 100 ft radius, knocking people down, breaking concentration, opening fissures and collapsing structures.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| open 3.5 fissures, 55 ft deep, 200 ft long, against lateral earth pressure | `3.5*2*(0.5*1800*g*(55*ft)/2)*(55*ft)*(200*ft)*(5*ft)/J` | 537,865 |
| upkeep: shake 3 m soil in 100 ft radius at 0.5 m/s, 2 Hz, Q=10, 1 min | `(2*pi*2*0.5*(pi*(100*ft)**2*3*1800)*0.5**2/10)*60/J` | 99,027 |
| Pattern cost | `0.01 × Q8 × (1 + 0.25)` | 4,798 |

| Quantity | Value |
|---|---|
| Effect energy | 537,865 Pz |
| Upkeep energy | 99,027 Pz (1,650 Pz/s) |
| **Total draw** | **641,690 Pz** (962,535.0 kJ) |
| Slot quantum Q8 | 383,822 Pz |
| Field gain (draw / quantum) | 1.67 |
| Energy-equivalent tier T_E | 8.51 |
| Handling points | 0.25 |
| Grade score | 0.51 → M |

**Handling flags:** concentration.

**Assumptions:** Soil 1800 kg/m3, lateral earth pressure coefficient 0.5, each wall pushed 5 ft; ground oscillation energy replenished per cycle with Q=10.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Earthquake (8-V-M-ERT) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 8 | 8 | `0000000010001` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (100) | 28 | `0000000111001` |
| k5 Range | 500 feet | 8 | `0000000010001` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Nu’-Sasinse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T9: *Xyinu’-Sasinse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 4→3 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 3→12 4→0 5→1 | 4 |
| k5 Range | 0→8 4→12 | 2 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#0b7ac9`.

![[Earthquake (8-V-M-ERT) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 8 | 0.800 | 1.000 | `#2900ff` (460 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.956 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.993 | `#0074ff` (495 nm eq.) | source grid |
| Area | sphere (100) | 0.778 | 1.000 | `#0e00ff` (467 nm eq.) | source grid |
| Range | 500 feet | 0.471 | 0.947 | `#00ff60` (559 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.16): swatch `#4ed3d0`, measured lines at 0.471, 0.501, 0.685, 0.778, 0.801. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 5.81. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `8·V·None`; the k4 to k6 lines (sphere (100), 500 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `8·V·None` |
| Standard spectrometer detection range | 80.11 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 19,191 Pz (0.05 × Q8) |
| Counter drawn cold (all six layers) | 38,382 Pz (0.10 × Q8) |
| Unravel after completion | 58,188 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1b 1c 1d 1f` (Heat, Light, Life, Energy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 106,948 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 1.67 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 8th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 8th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 8 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Terrain and Matter Shaping]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Control Weather (8-T-H-CWT)|Control Weather]] (8) · [[Alter Biome (9-T-X-AB)|Alter Biome]] (9) · [[Wall of Stone (5-V-M-WS)|Wall of Stone]] (5) · [[Gravitational Wave (8-V-L-GWV)|Gravitational Wave]] (8) · [[Ice Storm (4-V-L-ISE)|Ice Storm]] (4) · [[Lance of Longinus (8-V-L-LL)|Lance of Longinus]] (8) · [[Move Earth (6-T-M-ME)|Move Earth]] (6) · [[Sunburst (8-V-L-SNBB)|Sunburst]] (8).


---

## Tactical Assessment

Destroys fortifications and buried positions and halts movement in the zone; collateral risk to friendly structures is high.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 8 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
