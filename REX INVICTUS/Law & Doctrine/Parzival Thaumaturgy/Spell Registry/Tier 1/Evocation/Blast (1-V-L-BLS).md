---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/evocation
  - source/rex-invictus
aliases:
  - "1st Tier Spell: Blast"
  - "Blast"
  - "1-V-L-BLS"
registry_id: 1-V-L-BLS
attribute_code: "1·Evo·Thunder·sphere (10)·60 feet·Instantaneous"
incantation: "Suder-Sewyn"
tier: 1
school: Evocation
affinity: V
grade: L
pz_total: 904.1
pz_quantum: 350.0
t_e: 1.95
updated: 2026-11-16
---

**Blast** (`1-V-L-BLS`) is a 1st Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Rex Invictus original working. Its modelled draw is **904 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E 1.95 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Evocation]]
        - **Blast** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-V-L-BLS` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Evo·Thunder·sphere (10)·60 feet·Instantaneous` |
| Incantation | *Suder-Sewyn* |
| Affinity | V (Evocation) |
| Source | Rex Invictus |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | sphere (10) |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 2d8 thunder (mean 9) |
| Injury by tier | T1: 2d8, T2: 3d8 |
| Resistance check | constitution; on success: half injury |
| Practitioner lineages | Wizard, Sorcerer, Sorcerer |

### Effect

A sharp concussive burst at a point, 10 feet in radius. Creatures inside take 2d8 thunder injury, halved by a constitution check.

### Mechanism

Releases field return as an overpressure front. When it is sealed inside a casing or a bound fluid the front is directed and becomes the driver of a shaped jet.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| burst 9 injury, 10 ft sphere | `9*0.6*4*pi*3.048^2/0.7` | 901 |
| Pattern cost | `0.01 × Q1 × (1 + 0.00)` | 3.5 |

| Quantity | Value |
|---|---|
| Effect energy | 901 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **904 Pz** (1,356.2 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 2.58 |
| Energy-equivalent tier T_E | 1.95 |
| Handling points | 0.00 |
| Grade score | 0.47 → L |

**Handling flags:** none.

**Assumptions:** 2d8 = 9 average; sphere fluence model.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Blast (1-V-L-BLS) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Thunder | 13 | `0000000011011` |
| k4 Area | sphere (10) | 27 | `0000000110111` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Suder-Sewyn** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisuder-Sewyn* · T3: *Lisuder-Sewyn* · T4: *Visuder-Sewyn* · T5: *Tisuder-Sewyn* · T6: *Risuder-Sewyn* · T7: *Misuder-Sewyn* · T8: *Nisuder-Sewyn* · T9: *Xyisuder-Sewyn*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 3→0 4→1 | 4 |
| k4 Area | 0→9 1→10 2→11 4→0 5→1 | 5 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#7c6b92`.

![[Blast (1-V-L-BLS) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| Damage | Thunder | 0.929 | 0.709 | `#dc00ff` (421 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.923 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.995 | `#ff0028` (700 nm eq.) | source grid |
| Area | sphere (10) | 0.750 | 0.810 | `#0017ff` (475 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.888 | `#00fbff` (524 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 2.96. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·V·Thunder`; the k4 to k6 lines (sphere (10), 60 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·V·Thunder` |
| Standard spectrometer detection range | 3.01 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.0 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is 2x Heat, Dark, Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `3b 1C 2f 2j` (3x Heat, Dark, 2x Energy, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 151 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 2.58 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 1st Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Area Destruction]] |
| Element | [[Thunder and Concussion Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Thunderwave (1-V-L-THN)|Thunderwave]] (1) · [[Shatter (2-V-L-SHT)|Shatter]] (2) · [[Burning Hands (1-V-L-BH)|Burning Hands]] (1) · [[Kilonova (1-V-M-KLN)|Kilonova]] (1) · [[Resonant Shatter (1-V-L-RSO)|Resonant Shatter]] (1) · [[Bohr's Model (2-P-L-BSM)|Bohr's Model]] (2) · [[Galaxy Whirl (2-V-L-GWL)|Galaxy Whirl]] (2) · [[Geyser (2-V-L-GYS)|Geyser]] (2).


---

## Tactical Assessment

A grenade substitute, and the fuze charge of airburst bolts and anti-ward primers.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
