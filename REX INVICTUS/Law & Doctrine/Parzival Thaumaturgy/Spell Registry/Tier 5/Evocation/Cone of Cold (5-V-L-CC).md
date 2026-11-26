---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/evocation
  - source/srd
aliases:
  - "5th Tier Spell: Cone of Cold"
  - "Cone of Cold"
  - "5-V-L-CC"
registry_id: 5-V-L-CC
attribute_code: "5·Evo·Cold·cone (60)·Self·Instantaneous"
incantation: "Tulod-Nopor"
tier: 5
school: Evocation
affinity: V
grade: L
pz_total: 10501.0
pz_quantum: 19109.4
t_e: 4.40
updated: 2026-11-16
---

**Cone of Cold** (`5-V-L-CC`) is a 5th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **10,501 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 4.40 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Evocation]]
        - **Cone of Cold** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-V-L-CC` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Evo·Cold·cone (60)·Self·Instantaneous` |
| Incantation | *Tulod-Nopor* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | Self |
| Area | cone (60) |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A small crystal or glass cone |
| Ritual | no |
| Injury | 8d8 cold (mean 36) |
| Injury by tier | T5: 8d8, T6: 9d8, T7: 10d8, T8: 11d8, T9: 12d8 |
| Resistance check | constitution; on success: half injury |
| Practitioner lineages | Sorcerer, Wizard |

### Mechanism

A blast of supercooled air sweeps an 18 m cone, freezing anyone it kills.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| cold blast | `36 HP * 0.9 Pz/HP (cold) * (cone 60 ft: 0.666*18.288^2 = 222.744 m^2 / 0.7 m^2)` | 10,310 |
| Pattern cost | `0.01 × Q5 × (1 + 0.00)` | 191 |

| Quantity | Value |
|---|---|
| Effect energy | 10,310 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **10,501 Pz** (15,751.5 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 0.55 |
| Energy-equivalent tier T_E | 4.40 |
| Handling points | 0.00 |
| Grade score | -0.30 → L |

**Handling flags:** none.

**Assumptions:** Average 36 injury.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Cone of Cold (5-V-L-CC) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Cold | 2 | `0000000000101` |
| k4 Area | cone (60) | 4 | `0000000001001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Tulod-Nopor** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Ritulod-Nopor* · T7: *Mitulod-Nopor* · T8: *Nitulod-Nopor* · T9: *Xyitulod-Nopor*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 2→12 | 2 |
| k4 Area | 0→9 3→12 | 2 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#7aa361`.

![[Cone of Cold (5-V-L-CC) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| Damage | Cold | 0.214 | 0.960 | `#fffa00` (636 nm eq.) | source grid |
| School | Evocation | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.882 | `#ff0028` (700 nm eq.) | source grid |
| Area | cone (60) | 0.111 | 0.927 | `#ff6e00` (667 nm eq.) | source grid |
| Range | Self | 0.706 | 0.979 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.14): swatch `#96cc97`, measured lines at 0.004, 0.112, 0.215, 0.501, 0.706. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.02. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·V·Cold`; the k4 to k6 lines (cone (60), Self, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·V·Cold` |
| Standard spectrometer detection range | 10.25 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 1,911 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is 2x Cold, 2x Death and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1B 2D 2f 1j` (Cold, 2x Death, 2x Energy, Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1,750 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 5th Tier quantum of 19,109 Pz (55.0% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 5th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 5 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Area Destruction]] |
| Element | [[Cold and Ice Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Absolute Zero (6-V-L-AZ)|Absolute Zero]] (6) · [[Freezing Sphere (6-V-M-FSZ)|Freezing Sphere]] (6) · [[Ice Storm (4-V-L-ISE)|Ice Storm]] (4) · [[Wall of Ice (6-V-M-WI)|Wall of Ice]] (6) · [[Flame Strike (5-V-L-FSM)|Flame Strike]] (5) · [[Voltaic Arc (5-V-L-VA)|Voltaic Arc]] (5) · [[Blade Barrier (6-V-L-BB)|Blade Barrier]] (6) · [[Burst Radiation (6-V-L-BR)|Burst Radiation]] (6).


---

## Tactical Assessment

Wide-area attack against infantry.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
