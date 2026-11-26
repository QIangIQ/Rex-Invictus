---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/evocation
  - source/srd
aliases:
  - "1st Tier Spell: Divine Favor"
  - "Divine Favor"
  - "1-V-L-DF"
registry_id: 1-V-L-DF
attribute_code: "1·Evo·Radiant·None·Self·Up to 1 minute"
incantation: "Sunat-’porse"
tier: 1
school: Evocation
affinity: V
grade: L
pz_total: 5.0
pz_quantum: 350.0
t_e: -3.24
updated: 2026-11-16
---

**Divine Favor** (`1-V-L-DF`) is a 1st Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **5.0 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -3.24 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Evocation]]
        - **Divine Favor** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-V-L-DF` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Evo·Radiant·None·Self·Up to 1 minute` |
| Incantation | *Sunat-’porse* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Evocation]] |
| Casting time | 1 bonus action |
| Range | Self |
| Area | single point or target |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 1d4 radiant (mean 2.5) |
| Injury by tier | T1: 1d4 |
| Practitioner lineages | Paladin |

### Mechanism

The caster weapon strikes carry an extra radiant charge for a minute.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| 1d4 radiant rider on 6.5 strikes | `2.5*0.50*0.08*6.5` | 0.65 |
| Pattern cost | `0.01 × Q1 × (1 + 0.25)` | 4.4 |

| Quantity | Value |
|---|---|
| Effect energy | 0.65 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **5.0 Pz** (7.5 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.0144 |
| Energy-equivalent tier T_E | -3.24 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** concentration.

**Assumptions:** 6.5 hits over 10 rounds; focused delivery F=0.08.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Divine Favor (1-V-L-DF) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Radiant | 11 | `0000000010111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Sunat-’porse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisunat-’porse* · T3: *Lisunat-’porse* · T4: *Visunat-’porse* · T5: *Tisunat-’porse* · T6: *Risunat-’porse* · T7: *Misunat-’porse* · T8: *Nisunat-’porse* · T9: *Xyisunat-’porse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 4→1 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#3e71ac`.

![[Divine Favor (1-V-L-DF) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| Damage | Radiant | 0.786 | 0.790 | `#1900ff` (464 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.923 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.843 | `#0074ff` (495 nm eq.) | source grid |
| Range | Self | 0.706 | 0.832 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.16): swatch `#78b4a3`, measured lines at 0.101, 0.501, 0.685, 0.706, 0.786. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 0.70. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·V·Radiant`; the k4 to k6 lines (None, Self, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·V·Radiant` |
| Standard spectrometer detection range | 0.22 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.0 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Life, Hope and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `2b 1c 1d 2f 1i 1j` (2x Heat, Light, Life, 2x Energy, Hope, Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 0.838 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (1.4% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Precision Strikes]] |
| Element | [[Radiant Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Guiding Bolt (1-V-L-GB)|Guiding Bolt]] (1) · [[Branding Smite (2-V-L-BS)|Branding Smite]] (2) · [[Sacred Flame (0-V-L-SF)|Sacred Flame]] (0) · [[Electrify (1-V-L-ELC)|Electrify]] (1) · [[Focusing Lens (1-V-L-FLC)|Focusing Lens]] (1) · [[Hellish Rebuke (1-V-L-HR)|Hellish Rebuke]] (1) · [[Magic Missile (1-P-L-MM)|Magic Missile]] (1) · [[Acid Arrow (2-V-L-AA)|Acid Arrow]] (2).


---

## Tactical Assessment

Modest damage boost for close combatants.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
