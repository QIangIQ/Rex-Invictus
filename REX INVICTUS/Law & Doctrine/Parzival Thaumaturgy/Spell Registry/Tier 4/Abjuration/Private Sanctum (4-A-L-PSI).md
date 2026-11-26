---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/abjuration
  - source/srd
aliases:
  - "4th Tier Spell: Private Sanctum"
  - "Private Sanctum"
  - "4-A-L-PSI"
registry_id: 4-A-L-PSI
attribute_code: "4·Abj·None·cube (100)·120 feet·24 hours"
incantation: "Va’-Bimull"
tier: 4
school: Abjuration
affinity: A
grade: L
pz_total: 5565.4
pz_quantum: 7029.9
t_e: 3.77
updated: 2026-11-16
---

**Private Sanctum** (`4-A-L-PSI`) is a 4th Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **5,565 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E 3.77 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Abjuration]]
        - **Private Sanctum** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-A-L-PSI` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Abj·None·cube (100)·120 feet·24 hours` |
| Incantation | *Va’-Bimull* |
| Affinity | A (Abjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Abjuration]] |
| Casting time | 10 minutes |
| Range | 120 feet |
| Area | cube (100) |
| Duration | 24 hours |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A thin sheet of lead, a piece of opaque glass, a wad of cotton or cloth, and powdered chrysolite |
| Ritual | no |
| Practitioner lineages | Wizard |

### Mechanism

A cubic boundary field scatters light, blocks sound, and denies remote sensing, teleportation and planar transit across it for a day.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| [upkeep] vision screen, illusion rate over 100 ft cube volume, 24 h | `0.002*((100*ft)**3/1000)*86400` | 4,893 |
| [upkeep] sound blocking, 90 dB flux 1e-3 W/m^2 on 6 faces, 24 h | `1e-3*6*(100*ft)**2*86400/1500` | 321 |
| [upkeep] anti-divination and anti-teleport screen, 24 h | `0.001*((100*ft)/10)*86400` | 263 |
| Pattern cost | `0.01 × Q4 × (1 + 0.25)` | 87.9 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 5,478 Pz (0.0634 Pz/s) |
| **Total draw** | **5,565 Pz** (8,348.2 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 0.792 |
| Energy-equivalent tier T_E | 3.77 |
| Handling points | 0.25 |
| Grade score | 0.13 → L |

**Handling flags:** long cast.

**Assumptions:** Maximum 100 ft cube with all options; scattering treated as lossless; ward rate taken from the divination formula over the cube edge.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Private Sanctum (4-A-L-PSI) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 4 | 4 | `0000000001001` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | cube (100) | 6 | `0000000001101` |
| k5 Range | 120 feet | 3 | `0000000000111` |
| k6 Duration | 24 hours | 5 | `0000000001011` |

### Incantation

Spoken as **Va’-Bimull** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T5: *Tiva’-Bimull* · T6: *Riva’-Bimull* · T7: *Miva’-Bimull* · T8: *Niva’-Bimull* · T9: *Xyiva’-Bimull*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 3→2 | 2 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 2→11 3→12 | 3 |
| k5 Range | 0→8 1→9 2→10 | 3 |
| k6 Duration | 0→7 1→8 3→10 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#aeb507`.

![[Private Sanctum (4-A-L-PSI) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.923 | `#ff0028` (700 nm eq.) | source grid |
| Duration | 24 hours | 0.316 | 0.996 | `#76ff00` (605 nm eq.) | source grid |
| Area | cube (100) | 0.167 | 0.973 | `#ffb900` (650 nm eq.) | source grid |
| Range | 120 feet | 0.176 | 0.975 | `#ffc900` (647 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.21): swatch `#e09c5b`, measured lines at 0.007, 0.173, 0.316, 0.401. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.75. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·A·None`; the k4 to k6 lines (cube (100), 120 feet, 24 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·A·None` |
| Standard spectrometer detection range | 7.46 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 1,799 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 928 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 4th Tier quantum of 7,030 Pz (79.2% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
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

Similar workings: [[Arcane Insulation (4-A-L-AI)|Arcane Insulation]] (4) · [[Banishment (4-A-M-BNS)|Banishment]] (4) · [[Antilife Shell (5-A-L-ASI)|Antilife Shell]] (5) · [[Counterspell (3-A-L-CNT)|Counterspell]] (3) · [[Dispel Evil and Good (5-A-L-DEGP)|Dispel Evil and Good]] (5) · [[Dispel Magic (3-A-L-DM)|Dispel Magic]] (3) · [[Nondetection (3-A-L-NND)|Nondetection]] (3) · [[Remove Curse (3-A-L-RC)|Remove Curse]] (3).


---

## Tactical Assessment

A secure command post or briefing room in contested territory, closed to remote observation and translocated raids.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
