---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/evocation
  - source/srd
aliases:
  - "5th Tier Spell: Wall of Stone"
  - "Wall of Stone"
  - "5-V-M-WS"
registry_id: 5-V-M-WS
attribute_code: "5·Evo·None·None·120 feet·Up to 10 minutes"
incantation: "Tumully"
tier: 5
school: Evocation
affinity: V
grade: M
pz_total: 111038.9
pz_quantum: 19109.4
t_e: 6.76
updated: 2026-11-16
---

**Wall of Stone** (`5-V-M-WS`) is a 5th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **111,039 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 6.76 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Evocation]]
        - **Wall of Stone** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-V-M-WS` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Evo·None·None·120 feet·Up to 10 minutes` |
| Incantation | *Tumully* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 120 feet |
| Area | single point or target |
| Duration | Up to 10 minutes (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A small block of granite |
| Ritual | no |
| Practitioner lineages | Druid, Sorcerer, Wizard |

### Mechanism

Ten panels of real stone, 15 cm thick, form where the caster directs, merging with existing rock; held for ten minutes they become permanent.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Conjured stone | `3 Pz/kg * 36812 kg (14.16 m^3 * 2600)` | 110,400 |
| Raising centre of mass 1.5 m | `36812 kg * 9.81 * 1.524 / 1500` | 367 |
| Pattern cost | `0.01 × Q5 × (1 + 0.25)` | 239 |

| Quantity | Value |
|---|---|
| Effect energy | 110,800 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **111,039 Pz** (166,558.3 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 5.81 |
| Energy-equivalent tier T_E | 6.76 |
| Handling points | 0.25 |
| Grade score | 1.13 → M |

**Handling flags:** concentration.

**Assumptions:** 6 in panel option; granite density 2600 kg/m^3.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Wall of Stone (5-V-M-WS) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 120 feet | 3 | `0000000000111` |
| k6 Duration | Up to 10 minutes | 15 | `0000000011111` |

### Incantation

Spoken as **Tumully** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Ritumully* · T7: *Mitumully* · T8: *Nitumully* · T9: *Xyitumully*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]]. This attribute set is shared with other workings, so the glyph carries 1 centre dot(s) to tell it apart.

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 | 3 |
| k6 Duration | 0→7 1→8 2→9 3→10 4→11 | 5 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#45b385`.

![[Wall of Stone (5-V-M-WS) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| School | Evocation | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Up to 10 minutes | 0.789 | 0.959 | `#1e00ff` (463 nm eq.) | source grid |
| Range | 120 feet | 0.176 | 0.949 | `#ffc900` (647 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 5.05. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·V·None`; the k4 to k6 lines (None, 120 feet, Up to 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·V·None` |
| Standard spectrometer detection range | 33.32 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 1,911 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1b 1c 1d 1f` (Heat, Light, Life, Energy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 18,506 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 5.81 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 5th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 5th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 5 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Walls and Barriers]], [[Terrain and Matter Shaping]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Passwall (5-T-L-PSS)|Passwall]] (5) · [[Wall of Force (5-P-L-WFL)|Wall of Force]] (5) · [[Blade Barrier (6-V-L-BB)|Blade Barrier]] (6) · [[Ice Storm (4-V-L-ISE)|Ice Storm]] (4) · [[Wall of Fire (4-V-M-WF)|Wall of Fire]] (4) · [[Wall of Ice (6-V-M-WI)|Wall of Ice]] (6) · [[Creation (5-I-L-CRT)|Creation]] (5) · [[Forcecage (7-P-L-FRC)|Forcecage]] (7).


---

## Tactical Assessment

Rapid permanent fortification, bridges and ramps; a standard field-engineering working.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
