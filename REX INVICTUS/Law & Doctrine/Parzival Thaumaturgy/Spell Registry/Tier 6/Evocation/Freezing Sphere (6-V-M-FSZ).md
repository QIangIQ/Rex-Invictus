---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-6
  - spell/evocation
  - source/srd
aliases:
  - "6th Tier Spell: Freezing Sphere"
  - "Freezing Sphere"
  - "6-V-M-FSZ"
registry_id: 6-V-M-FSZ
attribute_code: "6·Evo·Cold·sphere (60)·300 feet·Instantaneous"
incantation: "Rulod-Sisphin"
tier: 6
school: Evocation
affinity: V
grade: M
pz_total: 189647.4
pz_quantum: 51944.6
t_e: 7.29
updated: 2026-11-16
---

**Freezing Sphere** (`6-V-M-FSZ`) is a 6th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **189,647 Pz** against a slot quantum of 51,945 Pz, which puts its energy-equivalent tier at T_E 7.29 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 6 Workings]]
      - [[Evocation]]
        - **Freezing Sphere** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `6-V-M-FSZ` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `6·Evo·Cold·sphere (60)·300 feet·Instantaneous` |
| Incantation | *Rulod-Sisphin* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 6th Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 300 feet |
| Area | sphere (60) |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A small crystal sphere |
| Ritual | no |
| Injury | 10d6 cold (mean 35) |
| Injury by tier | T6: 10d6 |
| Resistance check | constitution; on success: half injury |
| Practitioner lineages | Wizard |

### Mechanism

A globe of extreme cold detonates over an 18 m radius, freezing creatures inside and capable of freezing open water to 15 cm depth; it can also be held as a thrown charge for up to a minute.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| cold burst, 10d6=35 | `35 HP * kappa_cold 0.9 * S/A_c (1 x 4*pi*(60 ft*0.3048)^2 = 4202.8 m^2 / 0.7)` | 189,128 |
| Pattern cost | `0.01 × Q6 × (1 + 0.00)` | 519 |

| Quantity | Value |
|---|---|
| Effect energy | 189,128 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **189,647 Pz** (284,471.2 kJ) |
| Slot quantum Q6 | 51,945 Pz |
| Field gain (draw / quantum) | 3.65 |
| Energy-equivalent tier T_E | 7.29 |
| Handling points | 0.00 |
| Grade score | 0.65 → M |

**Handling flags:** none.

**Assumptions:** 10d6 avg 35 cold, 60 ft sphere. Excluded conditional term: freezing 30 ft x 30 ft x 6 in of water (12,740 kg, cooled 10 K and frozen, 376 kJ/kg) would add about 3.19e6 Pz.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Freezing Sphere (6-V-M-FSZ) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 6 | 6 | `0000000001101` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Cold | 2 | `0000000000101` |
| k4 Area | sphere (60) | 35 | `0000001000111` |
| k5 Range | 300 feet | 6 | `0000000001101` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Rulod-Sisphin** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T7: *Mirulod-Sisphin* · T8: *Nirulod-Sisphin* · T9: *Xyirulod-Sisphin*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 3→2 | 3 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 2→12 | 2 |
| k4 Area | 0→9 1→10 2→11 6→2 | 4 |
| k5 Range | 0→8 2→10 3→11 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#84ab71`.

![[Freezing Sphere (6-V-M-FSZ) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 6 | 0.600 | 1.000 | `#00ebff` (520 nm eq.) | source grid |
| Damage | Cold | 0.214 | 0.928 | `#fffa00` (636 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.995 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.835 | `#ff0028` (700 nm eq.) | source grid |
| Area | sphere (60) | 0.972 | 0.933 | `#ff00e5` (408 nm eq.) | source grid |
| Range | 300 feet | 0.353 | 0.970 | `#40ff00` (594 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.17): swatch `#99c89e`, measured lines at 0.004, 0.215, 0.354, 0.501, 0.601, 0.973. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 5.28. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `6·V·Cold`; the k4 to k6 lines (sphere (60), 300 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `6·V·Cold` |
| Standard spectrometer detection range | 43.55 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 2,597 Pz (0.05 × Q6) |
| Counter drawn cold (all six layers) | 5,194 Pz (0.10 × Q6) |
| Unravel after completion | 5,194 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is 2x Cold, 2x Death and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1B 2D 2f 1j` (Cold, 2x Death, 2x Energy, Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 31,608 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 3.65 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 6th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 6th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 6 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Area Destruction]] |
| Element | [[Cold and Ice Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Absolute Zero (6-V-L-AZ)|Absolute Zero]] (6) · [[Wall of Ice (6-V-M-WI)|Wall of Ice]] (6) · [[Cone of Cold (5-V-L-CC)|Cone of Cold]] (5) · [[Ice Storm (4-V-L-ISE)|Ice Storm]] (4) · [[Blade Barrier (6-V-L-BB)|Blade Barrier]] (6) · [[Burst Radiation (6-V-L-BR)|Burst Radiation]] (6) · [[Sunbeam (6-V-L-SNB)|Sunbeam]] (6) · [[Delayed Blast Fireball (7-V-M-DBF)|Delayed Blast Fireball]] (7).


---

## Tactical Assessment

A large-area cryo munition that can be handed to non-casters as a grenade or sling round; freezing a river crossing or harbour surface creates temporary bridges or traps swimmers.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 6 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
