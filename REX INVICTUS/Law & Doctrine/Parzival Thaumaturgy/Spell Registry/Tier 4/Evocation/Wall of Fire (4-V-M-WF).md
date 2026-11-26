---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/evocation
  - source/srd
aliases:
  - "4th Tier Spell: Wall of Fire"
  - "Wall of Fire"
  - "4-V-M-WF"
registry_id: 4-V-M-WF
attribute_code: "4·Evo·Fire·line (60)·120 feet·Up to 1 minute"
incantation: "Vuire-Lemulse"
tier: 4
school: Evocation
affinity: V
grade: M
pz_total: 20157.9
pz_quantum: 7029.9
t_e: 5.05
updated: 2026-11-16
---

**Wall of Fire** (`4-V-M-WF`) is a 4th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **20,158 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E 5.05 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Evocation]]
        - **Wall of Fire** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-V-M-WF` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Evo·Fire·line (60)·120 feet·Up to 1 minute` |
| Incantation | *Vuire-Lemulse* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 120 feet |
| Area | line (60) |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A small piece of phosphorus |
| Ritual | no |
| Injury | 5d8 fire (mean 22.5) |
| Injury by tier | T4: 5d8 |
| Resistance check | agility; on success: half injury |
| Practitioner lineages | Druid, Sorcerer, Wizard |

### Mechanism

An opaque wall of flame up to 18 m long and 6 m high stands for a minute, burning those it forms on and anyone near its active face.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Fire injury, 1 initial + 3 ongoing | `22.5 HP * 0.70 * 223 m^2 / 0.7 * 4` | 20,070 |
| Pattern cost | `0.01 × Q4 × (1 + 0.25)` | 87.9 |

| Quantity | Value |
|---|---|
| Effect energy | 20,070 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **20,158 Pz** (30,236.8 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 2.87 |
| Energy-equivalent tier T_E | 5.05 |
| Handling points | 0.25 |
| Grade score | 0.78 → M |

**Handling flags:** concentration.

**Assumptions:** 5d8 = 22.5; line exposure l=60 ft, h=20 ft; 3 ongoing triggers.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Wall of Fire (4-V-M-WF) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 4 | 4 | `0000000001001` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Fire | 3 | `0000000000111` |
| k4 Area | line (60) | 25 | `0000000110011` |
| k5 Range | 120 feet | 3 | `0000000000111` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Vuire-Lemulse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T5: *Tivuire-Lemulse* · T6: *Rivuire-Lemulse* · T7: *Mivuire-Lemulse* · T8: *Nivuire-Lemulse* · T9: *Xyivuire-Lemulse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 3→2 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 | 3 |
| k4 Area | 0→9 1→10 4→0 5→1 | 4 |
| k5 Range | 0→8 1→9 2→10 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#44c66a`.

![[Wall of Fire (4-V-M-WF) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| Damage | Fire | 0.286 | 0.993 | `#9cff00` (614 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.995 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.960 | `#0074ff` (495 nm eq.) | source grid |
| Area | line (60) | 0.694 | 0.958 | `#0069ff` (492 nm eq.) | source grid |
| Range | 120 feet | 0.176 | 0.975 | `#ffc900` (647 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 4.30. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·V·Fire`; the k4 to k6 lines (line (60), 120 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·V·Fire` |
| Standard spectrometer detection range | 14.20 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 703 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Energy, Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `2b 1c 3f 2j` (2x Heat, Light, 3x Energy, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 3,360 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 2.87 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 4th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 4th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 4 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Walls and Barriers]], [[Area Destruction]] |
| Element | [[Fire Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Fire Shield (4-V-L-FSR)|Fire Shield]] (4) · [[Fireball (3-V-M-FRB)|Fireball]] (3) · [[Flame Strike (5-V-L-FSM)|Flame Strike]] (5) · [[Wind Wall (3-V-L-WWN)|Wind Wall]] (3) · [[Blade Barrier (6-V-L-BB)|Blade Barrier]] (6) · [[Galaxy Whirl (2-V-L-GWL)|Galaxy Whirl]] (2) · [[Wall of Ice (6-V-M-WI)|Wall of Ice]] (6) · [[Burning Hands (1-V-L-BH)|Burning Hands]] (1).


---

## Tactical Assessment

Blocks sight lines and channels infantry movement; a ring form can protect a landing zone.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
