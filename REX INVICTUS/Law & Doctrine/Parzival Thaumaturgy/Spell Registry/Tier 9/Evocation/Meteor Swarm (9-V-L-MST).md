---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-9
  - spell/evocation
  - source/srd
aliases:
  - "9th Tier Spell: Meteor Swarm"
  - "Meteor Swarm"
  - "9-V-L-MST"
registry_id: 9-V-L-MST
attribute_code: "9·Evo·Fire·sphere (40)·1 mile·Instantaneous"
incantation: "Xyuire-Soeyp"
tier: 9
school: Evocation
affinity: V
grade: L
pz_total: 877133.4
pz_quantum: 1043335.3
t_e: 8.83
updated: 2026-11-16
---

**Meteor Swarm** (`9-V-L-MST`) is a 9th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **877,133 Pz** against a slot quantum of 1.04 MPz Pz, which puts its energy-equivalent tier at T_E 8.83 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 9 Workings]]
      - [[Evocation]]
        - **Meteor Swarm** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `9-V-L-MST` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `9·Evo·Fire·sphere (40)·1 mile·Instantaneous` |
| Incantation | *Xyuire-Soeyp* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 9th Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 1 mile |
| Area | sphere (40) |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 20d6 fire (mean 70) |
| Injury by tier | T9: 20d6 |
| Resistance check | agility; on success: half injury |
| Practitioner lineages | Sorcerer, Wizard |

### Mechanism

The field drives four blazing masses down onto points up to a mile away, each bursting across a 40 ft radius with fire and blast that wrap around cover. Structures in the zone are damaged and set alight.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Fire injury, 4 bursts | `4 * 70 HP * 0.70 * (1867.9 m^2 / 0.7)` | 523,000 |
| Impact injury, 4 bursts | `4 * 70 HP * 0.46 * (1867.9 m^2 / 0.7)` | 343,700 |
| Pattern cost | `0.01 × Q9 × (1 + 0.00)` | 10,433 |

| Quantity | Value |
|---|---|
| Effect energy | 866,700 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **877,133 Pz** (1,315,700.0 kJ) |
| Slot quantum Q9 | 1.04 MPz Pz |
| Field gain (draw / quantum) | 0.841 |
| Energy-equivalent tier T_E | 8.83 |
| Handling points | 0.00 |
| Grade score | -0.09 → L |

**Handling flags:** none.

**Assumptions:** Four 40 ft radius spheres without overlap; 20d6 = 70 fire and 70 impact, full value.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Meteor Swarm (9-V-L-MST) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 9 | 9 | `0000000010011` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Fire | 3 | `0000000000111` |
| k4 Area | sphere (40) | 33 | `0000001000011` |
| k5 Range | 1 mile | 0 | `0000000000001` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Xyuire-Soeyp** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 4→3 | 3 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 | 3 |
| k4 Area | 0→9 1→10 6→2 | 3 |
| k5 Range | 0→8 | 1 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#a85788`.

![[Meteor Swarm (9-V-L-MST) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 9 | 0.900 | 1.000 | `#b600ff` (430 nm eq.) | source grid |
| Damage | Fire | 0.286 | 0.828 | `#9cff00` (614 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.923 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.667 | `#ff0028` (700 nm eq.) | source grid |
| Area | sphere (40) | 0.917 | 1.000 | `#cc00ff` (425 nm eq.) | source grid |
| Range | 1 mile | 0.000 | 0.667 | `#ff0028` (700 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.20): swatch `#8e92af`, measured lines at 0.004, 0.286, 0.501, 0.900, 0.917. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 5.94. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `9·V·Fire`; the k4 to k6 lines (sphere (40), 1 mile, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `9·V·Fire` |
| Standard spectrometer detection range | 93.66 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 52,167 Pz (0.05 × Q9) |
| Counter drawn cold (all six layers) | 104,334 Pz (0.10 × Q9) |
| Unravel after completion | 104,334 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Energy, Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `2b 1c 3f 2j` (2x Heat, Light, 3x Energy, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 146,189 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 9th Tier quantum of 1.04 MPz Pz (84.1% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 9th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 9 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Area Destruction]] |
| Element | [[Fire Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Eruption (9-V-M-ERP)|Eruption]] (9) · [[Thermonuclear Fireball (9-P-L-TFE)|Thermonuclear Fireball]] (9) · [[Supernova (8-V-L-SPR)|Supernova]] (8) · [[Delayed Blast Fireball (7-V-M-DBF)|Delayed Blast Fireball]] (7) · [[Fire Storm (7-V-L-FSS)|Fire Storm]] (7) · [[Starburst (9-A-L-STR)|Starburst]] (9) · [[Incendiary Cloud (8-C-M-IC)|Incendiary Cloud]] (8) · [[Flame Strike (5-V-L-FSM)|Flame Strike]] (5).


---

## Tactical Assessment

Comparable to a heavy artillery barrage delivered in a single action, able to destroy an entire position. The one-mile range keeps the caster outside most direct fire.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 9 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
