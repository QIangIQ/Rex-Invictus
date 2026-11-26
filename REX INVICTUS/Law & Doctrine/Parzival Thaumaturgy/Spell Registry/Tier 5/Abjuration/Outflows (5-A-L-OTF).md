---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/abjuration
  - source/science-spellbook
aliases:
  - "5th Tier Spell: Outflows"
  - "5-A-L-OTF"
  - "Outflows (Science)"
registry_id: 5-A-L-OTF
attribute_code: "5·Abj·Fire·cone (15)·Self·Up to 1 minute"
incantation: "Taire-Nuporse"
tier: 5
school: Abjuration
affinity: A
grade: L
pz_total: 1993.0
pz_quantum: 19109.4
t_e: 2.74
updated: 2026-11-16
---

**Outflows** (`5-A-L-OTF`) is a 5th Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **1,993 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 2.74 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Abjuration]]
        - **Outflows** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-A-L-OTF` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Abj·Fire·cone (15)·Self·Up to 1 minute` |
| Incantation | *Taire-Nuporse* |
| Affinity | A (Abjuration) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Abjuration]] |
| Casting time | 1 Action |
| Range | Self |
| Area | cone (15) |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 6d6 fire (mean 21) |
| Injury by tier | T5: 6d6, T6: 6d6, T7: 6d6, T8: 6d6, T9: 6d6 |
| Resistance check | constitution; on success: half injury |
| Practitioner lineages | Wizard, Sorcerer |

### Mechanism

Two opposed cones of superheated gas jet 15 ft from the caster, like the bipolar outflows of a forming star.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Hot gas jets | `21 HP x 0.7 (fire) x S/A_c, S = cone l=4.572 m = 13.9 m^2 x 6` | 1,754 |
| Pattern cost | `0.01 × Q5 × (1 + 0.25)` | 239 |

| Quantity | Value |
|---|---|
| Effect energy | 1,754 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **1,993 Pz** (2,989.5 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 0.104 |
| Energy-equivalent tier T_E | 2.74 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** concentration.

**Assumptions:** Fire 6d6 = 21 over two 15 ft cones, 3 triggers.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Outflows (5-A-L-OTF) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | Fire | 3 | `0000000000111` |
| k4 Area | cone (15) | 1 | `0000000000011` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Taire-Nuporse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Ritaire-Nuporse* · T7: *Mitaire-Nuporse* · T8: *Nitaire-Nuporse* · T9: *Xyitaire-Nuporse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 | 3 |
| k4 Area | 0→9 1→10 | 2 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#697b76`.

![[Outflows (5-A-L-OTF) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| Damage | Fire | 0.286 | 0.977 | `#9cff00` (614 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.882 | `#ff0028` (700 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.983 | `#0074ff` (495 nm eq.) | source grid |
| Area | cone (15) | 0.028 | 0.894 | `#ff0003` (692 nm eq.) | source grid |
| Range | Self | 0.706 | 0.979 | `#0058ff` (488 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 3.30. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·A·Fire`; the k4 to k6 lines (cone (15), Self, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·A·Fire` |
| Standard spectrometer detection range | 4.46 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 1,911 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Energy, Movement and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1b 1c 1f 1H 1i` (Within, Heat, Light, Energy, Rigidity, Hope).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 332 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 5th Tier quantum of 19,109 Pz (10.4% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 5th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 5 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Area Destruction]] |
| Element | [[Fire Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Flame Strike (5-V-L-FSM)|Flame Strike]] (5) · [[Fire Shield (4-V-L-FSR)|Fire Shield]] (4) · [[Wall of Fire (4-V-M-WF)|Wall of Fire]] (4) · [[Delayed Blast Fireball (7-V-M-DBF)|Delayed Blast Fireball]] (7) · [[Fire Storm (7-V-L-FSS)|Fire Storm]] (7) · [[Fireball (3-V-M-FRB)|Fireball]] (3) · [[Starburst (9-A-L-STR)|Starburst]] (9) · [[Galaxy Whirl (2-V-L-GWL)|Galaxy Whirl]] (2).


---

## Tactical Assessment

Holds a corridor in two directions at once.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
