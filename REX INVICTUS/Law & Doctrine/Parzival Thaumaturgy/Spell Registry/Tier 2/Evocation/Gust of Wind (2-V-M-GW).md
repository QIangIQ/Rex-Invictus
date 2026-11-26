---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/evocation
  - source/srd
aliases:
  - "2nd Tier Spell: Gust of Wind"
  - "Gust of Wind"
  - "2-V-M-GW"
registry_id: 2-V-M-GW
attribute_code: "2·Evo·None·line (60)·Self·Up to 1 minute"
incantation: "Hu’-Leporse"
tier: 2
school: Evocation
affinity: V
grade: M
pz_total: 1836.4
pz_quantum: 951.4
t_e: 2.66
updated: 2026-11-16
---

**Gust of Wind** (`2-V-M-GW`) is a 2nd Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **1,836 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E 2.66 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Evocation]]
        - **Gust of Wind** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-V-M-GW` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Evo·None·line (60)·Self·Up to 1 minute` |
| Incantation | *Hu’-Leporse* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | Self |
| Area | line (60) |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A legume seed |
| Ritual | no |
| Resistance check | strength; on success: no effect |
| Practitioner lineages | Druid, Sorcerer, Wizard |

### Mechanism

Drives a sustained 20 m/s air stream along an 18 m by 3 m line, shoving creatures back, dispersing gas and putting out open flames.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| pushing creatures 15 ft | `3 triggers * 0.5 * 80 kg * 9.81 * 4.57 m / 1500` | 3.6 |
| wind stream power | `0.5 * 1.225 kg/m^3 * 9.29 m^2 * (20 m/s)^3 / 1500 = 30.3483 Pz/s * 60 s` | 1,821 |
| Pattern cost | `0.01 × Q2 × (1 + 0.25)` | 11.9 |

| Quantity | Value |
|---|---|
| Effect energy | 3.6 Pz |
| Upkeep energy | 1,821 Pz (30.3 Pz/s) |
| **Total draw** | **1,836 Pz** (2,754.6 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 1.93 |
| Energy-equivalent tier T_E | 2.66 |
| Handling points | 0.25 |
| Grade score | 0.58 → M |

**Handling flags:** concentration.

**Assumptions:** Wind 20 m/s across a 10 ft x 10 ft cross-section for 1 minute; 3 pushes of 80 kg with friction coefficient 0.5.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Gust of Wind (2-V-M-GW) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | line (60) | 25 | `0000000110011` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Hu’-Leporse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihu’-Leporse* · T4: *Vihu’-Leporse* · T5: *Tihu’-Leporse* · T6: *Rihu’-Leporse* · T7: *Mihu’-Leporse* · T8: *Nihu’-Leporse* · T9: *Xyihu’-Leporse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 4→0 5→1 | 4 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#37a2af`.

![[Gust of Wind (2-V-M-GW) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.956 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.889 | `#0074ff` (495 nm eq.) | source grid |
| Area | line (60) | 0.694 | 0.885 | `#0069ff` (492 nm eq.) | source grid |
| Range | Self | 0.706 | 0.880 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.18): swatch `#80cfa7`, measured lines at 0.201, 0.501, 0.687, 0.705. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.26. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·V·None`; the k4 to k6 lines (line (60), Self, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·V·None` |
| Standard spectrometer detection range | 4.29 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 459 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1b 1c 1d 1f` (Heat, Light, Life, Energy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 306 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 1.93 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 2nd Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Negation and Counterspell]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Animal Messenger (2-E-L-AM)|Animal Messenger]] (2) · [[Arcane Lock (2-A-L-AL)|Arcane Lock]] (2) · [[Blindness-Deafness (2-N-L-BD)|Blindness/Deafness]] (2) · [[Knock (2-T-L-KNC)|Knock]] (2) · [[Magic Weapon (2-T-L-MW)|Magic Weapon]] (2) · [[Oscillate (2-C-L-OSC)|Oscillate]] (2) · [[Ray of Enfeeblement (2-N-L-RE)|Ray of Enfeeblement]] (2) · [[Counterspell (3-A-L-CNT)|Counterspell]] (3).


---

## Tactical Assessment

Clears gas and smoke from a position, holds a corridor against advancing infantry and grounds small drones.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
