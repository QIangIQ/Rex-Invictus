---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/evocation
  - source/srd
aliases:
  - "3rd Tier Spell: Tiny Hut"
  - "Tiny Hut"
  - "3-V-H-TH"
registry_id: 3-V-H-TH
attribute_code: "3·Evo·None·sphere (10)·Self·8 hours"
incantation: "Lu’-Seporiy"
tier: 3
school: Evocation
affinity: V
grade: H
pz_total: 3447.7
pz_quantum: 2586.2
t_e: 3.29
updated: 2026-11-16
---

**Tiny Hut** (`3-V-H-TH`) is a 3rd Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **3,448 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E 3.29 and its handling grade at **High**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Evocation]]
        - **Tiny Hut** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-V-H-TH` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Evo·None·sphere (10)·Self·8 hours` |
| Incantation | *Lu’-Seporiy* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Evocation]] |
| Casting time | 1 minute |
| Range | Self |
| Area | sphere (10) |
| Duration | 8 hours |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A small crystal bead |
| Ritual | yes |
| Practitioner lineages | Bard, Wizard |

### Mechanism

An opaque hemispherical force dome of 3 m radius blocks entry and field effects, holds a dry, comfortable interior and stays as long as the caster remains inside.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Dome formation | `instant set-up = 1 Pz` | 1.0 |
| Upkeep: Interior climate control | `0.3 W/m^2K * 58.4 m^2 * 10 K * 28800 s / 1500` | 3,362 |
| Upkeep: Barrier absorption | `0.20 * 100 HP over 8 h` | 20.0 |
| Pattern cost | `0.01 × Q3 × (1 + 1.50)` | 64.7 |

| Quantity | Value |
|---|---|
| Effect energy | 1.0 Pz |
| Upkeep energy | 3,382 Pz (0.117 Pz/s) |
| **Total draw** | **3,448 Pz** (5,171.5 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 1.33 |
| Energy-equivalent tier T_E | 3.29 |
| Handling points | 1.50 |
| Grade score | 1.64 → H |

**Handling flags:** ritual, fragile, long cast.

**Assumptions:** Dome U = 0.3 W/m^2K, 10 K differential; 100 HP absorbed over 8 h.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Tiny Hut (3-V-H-TH) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (10) | 27 | `0000000110111` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | 8 hours | 8 | `0000000010001` |

### Incantation

Spoken as **Lu’-Seporiy** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vilu’-Seporiy* · T5: *Tilu’-Seporiy* · T6: *Rilu’-Seporiy* · T7: *Milu’-Seporiy* · T8: *Nilu’-Seporiy* · T9: *Xyilu’-Seporiy*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 2→11 4→0 5→1 | 5 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 4→11 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#1db392`.

![[Tiny Hut (3-V-H-TH) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.980 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | 8 hours | 0.474 | 0.985 | `#00ff66` (558 nm eq.) | source grid |
| Area | sphere (10) | 0.750 | 0.904 | `#0017ff` (475 nm eq.) | source grid |
| Range | Self | 0.706 | 0.921 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.23): swatch `#85e4ac`, measured lines at 0.300, 0.474, 0.501, 0.706, 0.751. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.54. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·V·None`; the k4 to k6 lines (sphere (10), Self, 8 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·V·None` |
| Standard spectrometer detection range | 5.87 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 935 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1b 1c 1d 1f` (Heat, Light, Life, Energy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 575 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 1.33 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 3rd Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Walls and Barriers]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|High]] |

Similar workings: [[Wind Wall (3-V-L-WWN)|Wind Wall]] (3) · [[Wall of Fire (4-V-M-WF)|Wall of Fire]] (4) · [[Wall of Force (5-P-L-WFL)|Wall of Force]] (5) · [[Wall of Stone (5-V-M-WS)|Wall of Stone]] (5) · [[Blade Barrier (6-V-L-BB)|Blade Barrier]] (6) · [[Magic Polarising Filter (4-C-L-MPF)|Magic Polarising Filter]] (4) · [[Wall of Ice (6-V-M-WI)|Wall of Ice]] (6) · [[Daylight (3-V-L-DYL)|Daylight]] (3).


---

## Tactical Assessment

A rapid shelter for a squad of ten, proof against weather, scouts and field effects for a full rest period.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
