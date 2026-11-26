---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-6
  - spell/evocation
  - source/srd
aliases:
  - "6th Tier Spell: Wall of Ice"
  - "Wall of Ice"
  - "6-V-M-WI"
registry_id: 6-V-M-WI
attribute_code: "6·Evo·Cold·sphere (10)·120 feet·Up to 10 minutes"
incantation: "Rulod-Semully"
tier: 6
school: Evocation
affinity: V
grade: M
pz_total: 88169.3
pz_quantum: 51944.6
t_e: 6.53
updated: 2026-11-16
---

**Wall of Ice** (`6-V-M-WI`) is a 6th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **88,169 Pz** against a slot quantum of 51,945 Pz, which puts its energy-equivalent tier at T_E 6.53 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 6 Workings]]
      - [[Evocation]]
        - **Wall of Ice** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `6-V-M-WI` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `6·Evo·Cold·sphere (10)·120 feet·Up to 10 minutes` |
| Incantation | *Rulod-Semully* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 6th Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 120 feet |
| Area | sphere (10) |
| Duration | Up to 10 minutes (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A small piece of quartz |
| Ritual | no |
| Injury | 10d6 cold (mean 35) |
| Injury by tier | T6: 10d6, T7: 12d6, T8: 14d6, T9: 16d6 |
| Resistance check | agility; on success: half injury |
| Practitioner lineages | Wizard |

### Mechanism

A 30 cm thick wall or dome of ice forms, injuring those it cuts through; broken sections leave a sheet of freezing air.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Conjured ice | `3 Pz/kg * 25967 kg (28.32 m^3 * 917)` | 77,900 |
| Cold injury on formation | `35 HP * 0.90 * 186 m^2 / 0.7` | 8,361 |
| Frigid sheet, 1 breached section, 3 triggers | `17.5 * 0.90 * 18.6 / 0.7 * 3` | 1,254 |
| Pattern cost | `0.01 × Q6 × (1 + 0.25)` | 649 |

| Quantity | Value |
|---|---|
| Effect energy | 87,520 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **88,169 Pz** (132,254.0 kJ) |
| Slot quantum Q6 | 51,945 Pz |
| Field gain (draw / quantum) | 1.7 |
| Energy-equivalent tier T_E | 6.53 |
| Handling points | 0.25 |
| Grade score | 0.51 → M |

**Handling flags:** concentration.

**Assumptions:** Ten 10x10 ft panels 1 ft thick; ice holds itself for 10 min without upkeep.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Wall of Ice (6-V-M-WI) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 6 | 6 | `0000000001101` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Cold | 2 | `0000000000101` |
| k4 Area | sphere (10) | 27 | `0000000110111` |
| k5 Range | 120 feet | 3 | `0000000000111` |
| k6 Duration | Up to 10 minutes | 15 | `0000000011111` |

### Incantation

Spoken as **Rulod-Semully** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T7: *Mirulod-Semully* · T8: *Nirulod-Semully* · T9: *Xyirulod-Semully*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 3→2 | 3 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 2→12 | 2 |
| k4 Area | 0→9 1→10 2→11 4→0 5→1 | 5 |
| k5 Range | 0→8 1→9 2→10 | 3 |
| k6 Duration | 0→7 1→8 2→9 3→10 4→11 | 5 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#559f9a`.

![[Wall of Ice (6-V-M-WI) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 6 | 0.600 | 1.000 | `#00ebff` (520 nm eq.) | source grid |
| Damage | Cold | 0.214 | 0.928 | `#fffa00` (636 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.995 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Up to 10 minutes | 0.789 | 0.982 | `#1e00ff` (463 nm eq.) | source grid |
| Area | sphere (10) | 0.750 | 0.989 | `#0017ff` (475 nm eq.) | source grid |
| Range | 120 feet | 0.176 | 0.914 | `#ffc900` (647 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 4.95. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `6·V·Cold`; the k4 to k6 lines (sphere (10), 120 feet, Up to 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `6·V·Cold` |
| Standard spectrometer detection range | 29.69 km (r = 1 km × √(E/100 Pz)) |
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
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 14,695 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 1.70 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 6th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
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
| Function | [[Walls and Barriers]], [[Area Destruction]] |
| Element | [[Cold and Ice Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Absolute Zero (6-V-L-AZ)|Absolute Zero]] (6) · [[Blade Barrier (6-V-L-BB)|Blade Barrier]] (6) · [[Freezing Sphere (6-V-M-FSZ)|Freezing Sphere]] (6) · [[Cone of Cold (5-V-L-CC)|Cone of Cold]] (5) · [[Ice Storm (4-V-L-ISE)|Ice Storm]] (4) · [[Wall of Fire (4-V-M-WF)|Wall of Fire]] (4) · [[Wall of Thorns (6-C-L-WT)|Wall of Thorns]] (6) · [[Wind Wall (3-V-L-WWN)|Wind Wall]] (3).


---

## Tactical Assessment

Fast fortification and isolation; vulnerable to incendiaries and high-explosive.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 6 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
