---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/evocation
  - source/srd
aliases:
  - "3rd Tier Spell: Fireball"
  - "Fireball"
  - "3-V-M-FRB"
registry_id: 3-V-M-FRB
attribute_code: "3·Evo·Fire·sphere (20)·150 feet·Instantaneous"
incantation: "Luire-Sonosin"
tier: 3
school: Evocation
affinity: V
grade: M
pz_total: 13101.4
pz_quantum: 2586.2
t_e: 4.62
updated: 2026-11-16
---

**Fireball** (`3-V-M-FRB`) is a 3rd Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **13,101 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E 4.62 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Evocation]]
        - **Fireball** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-V-M-FRB` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Evo·Fire·sphere (20)·150 feet·Instantaneous` |
| Incantation | *Luire-Sonosin* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 150 feet |
| Area | sphere (20) |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A tiny ball of bat guano and sulfur |
| Ritual | no |
| Injury | 8d6 fire (mean 28) |
| Injury by tier | T3: 8d6, T4: 9d6, T5: 10d6, T6: 11d6, T7: 12d6, T8: 13d6, T9: 14d6 |
| Resistance check | agility; on success: half injury |
| Practitioner lineages | Sorcerer, Wizard |

### Mechanism

A guided streak carries a charge to a chosen point where it releases as a 6 m radius flame burst that wraps around corners and ignites loose fuel.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| fire burst, 8d6=28 | `28 HP * kappa_fire 0.7 * S/A_c (1 x 4*pi*(20 ft*0.3048)^2 = 467.0 m^2 / 0.7)` | 13,076 |
| Pattern cost | `0.01 × Q3 × (1 + 0.00)` | 25.9 |

| Quantity | Value |
|---|---|
| Effect energy | 13,076 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **13,101 Pz** (19,652.0 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 5.07 |
| Energy-equivalent tier T_E | 4.62 |
| Handling points | 0.00 |
| Grade score | 0.81 → M |

**Handling flags:** none.

**Assumptions:** 8d6 avg 28 fire; 20 ft radius sphere fluence model.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Fireball (3-V-M-FRB) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Fire | 3 | `0000000000111` |
| k4 Area | sphere (20) | 30 | `0000000111101` |
| k5 Range | 150 feet | 4 | `0000000001001` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Luire-Sonosin** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Viluire-Sonosin* · T5: *Tiluire-Sonosin* · T6: *Riluire-Sonosin* · T7: *Miluire-Sonosin* · T8: *Niluire-Sonosin* · T9: *Xyiluire-Sonosin*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 | 3 |
| k4 Area | 0→9 2→11 3→12 4→0 5→1 | 5 |
| k5 Range | 0→8 3→11 | 2 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#91ae44`.

![[Fireball (3-V-M-FRB) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| Damage | Fire | 0.286 | 1.000 | `#9cff00` (614 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.980 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.956 | `#ff0028` (700 nm eq.) | source grid |
| Area | sphere (20) | 0.833 | 0.867 | `#5a00ff` (450 nm eq.) | source grid |
| Range | 150 feet | 0.235 | 0.998 | `#e3ff00` (629 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.17): swatch `#c2c382`, measured lines at 0.004, 0.236, 0.285, 0.301, 0.501, 0.834. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.12. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·V·Fire`; the k4 to k6 lines (sphere (20), 150 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·V·Fire` |
| Standard spectrometer detection range | 11.45 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 259 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Energy, Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `2b 1c 3f 2j` (2x Heat, Light, 3x Energy, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 2,184 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 5.07 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 3rd Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Area Destruction]] |
| Element | [[Fire Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Fire Shield (4-V-L-FSR)|Fire Shield]] (4) · [[Galaxy Whirl (2-V-L-GWL)|Galaxy Whirl]] (2) · [[Wall of Fire (4-V-M-WF)|Wall of Fire]] (4) · [[Burning Hands (1-V-L-BH)|Burning Hands]] (1) · [[Flame Strike (5-V-L-FSM)|Flame Strike]] (5) · [[Kilonova (1-V-M-KLN)|Kilonova]] (1) · [[Delayed Blast Fireball (7-V-M-DBF)|Delayed Blast Fireball]] (7) · [[Fire Storm (7-V-L-FSS)|Fire Storm]] (7).


---

## Tactical Assessment

The standard artillery round of a field-caster, comparable to a heavy grenade or light mortar shell; effective against massed infantry and soft-skinned vehicles.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
