---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/evocation
  - source/srd
aliases:
  - "4th Tier Spell: Fire Shield"
  - "Fire Shield"
  - "4-V-L-FSR"
registry_id: 4-V-L-FSR
attribute_code: "4·Evo·Fire·sphere (5)·Self·10 minutes"
incantation: "Vuire-Supors"
tier: 4
school: Evocation
affinity: V
grade: L
pz_total: 92.7
pz_quantum: 7029.9
t_e: -0.33
updated: 2026-11-16
---

**Fire Shield** (`4-V-L-FSR`) is a 4th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **92.7 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E -0.33 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Evocation]]
        - **Fire Shield** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-V-L-FSR` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Evo·Fire·sphere (5)·Self·10 minutes` |
| Incantation | *Vuire-Supors* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | Self |
| Area | sphere (5) |
| Duration | 10 minutes |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A little phosphorus or a firefly |
| Ritual | no |
| Injury | 2d8 fire (mean 9) |
| Injury by tier | T4: 2d8 |
| Practitioner lineages | Wizard |

### Mechanism

A thin shell of flame or frost-vapour around the body halves incoming injury of the opposite thermal kind and lashes any adjacent attacker who strikes the bearer.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| elemental resistance absorption | `0.20 Pz * (15 HP/round * 10 rounds * 20% elemental * 50% blocked = 15 HP)` | 3.0 |
| retaliation flames, 2d8=9 | `9 HP * kappa_fire 0.7 * F 0.5 * 1 target(s) * 3 trigger(s)` | 9.4 |
| field light (10 ft bright) | `25 W / 1500 = 0.0166667 Pz/s * 600 s` | 10.0 |
| Pattern cost | `0.01 × Q4 × (1 + 0.00)` | 70.3 |

| Quantity | Value |
|---|---|
| Effect energy | 12.4 Pz |
| Upkeep energy | 10.0 Pz (0.0167 Pz/s) |
| **Total draw** | **92.7 Pz** (139.1 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 0.0132 |
| Energy-equivalent tier T_E | -0.33 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** One combat of 10 rounds, 15 injury points per round incoming, 20% of it fire or cold and halved; 3 retaliation triggers at F 0.5; light 25 W for 10 minutes.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Fire Shield (4-V-L-FSR) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 4 | 4 | `0000000001001` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Fire | 3 | `0000000000111` |
| k4 Area | sphere (5) | 34 | `0000001000101` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | 10 minutes | 4 | `0000000001001` |

### Incantation

Spoken as **Vuire-Supors** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T5: *Tivuire-Supors* · T6: *Rivuire-Supors* · T7: *Mivuire-Supors* · T8: *Nivuire-Supors* · T9: *Xyivuire-Supors*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 3→2 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 | 3 |
| k4 Area | 0→9 2→11 6→2 | 3 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 3→10 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#5fbd67`.

![[Fire Shield (4-V-L-FSR) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| Damage | Fire | 0.286 | 0.993 | `#9cff00` (614 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.995 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | 10 minutes | 0.263 | 0.991 | `#bdff00` (621 nm eq.) | source grid |
| Area | sphere (5) | 0.944 | 0.862 | `#f200ff` (417 nm eq.) | source grid |
| Range | Self | 0.706 | 0.954 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.17): swatch `#9dd8a3`, measured lines at 0.264, 0.286, 0.401, 0.501, 0.706, 0.945. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.97. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·V·Fire`; the k4 to k6 lines (sphere (5), Self, 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·V·Fire` |
| Standard spectrometer detection range | 0.96 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 705 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Energy, Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `2b 1c 3f 2j` (2x Heat, Light, 3x Energy, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 15.5 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 4th Tier quantum of 7,030 Pz (1.3% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 4th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 4 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Wards and Shields]], [[Area Destruction]] |
| Element | [[Fire Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Wall of Fire (4-V-M-WF)|Wall of Fire]] (4) · [[Fireball (3-V-M-FRB)|Fireball]] (3) · [[Flame Strike (5-V-L-FSM)|Flame Strike]] (5) · [[Galaxy Whirl (2-V-L-GWL)|Galaxy Whirl]] (2) · [[Burning Hands (1-V-L-BH)|Burning Hands]] (1) · [[Delayed Blast Fireball (7-V-M-DBF)|Delayed Blast Fireball]] (7) · [[Fire Storm (7-V-L-FSS)|Fire Storm]] (7) · [[Kilonova (1-V-M-KLN)|Kilonova]] (1).


---

## Tactical Assessment

A close-defence aura for casters who expect melee; it punishes boarding actions and hand-to-hand assault and offers protection against thermal weapons.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
