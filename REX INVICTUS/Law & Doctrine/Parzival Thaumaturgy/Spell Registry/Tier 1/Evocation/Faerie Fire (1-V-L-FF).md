---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/evocation
  - source/srd
aliases:
  - "1st Tier Spell: Faerie Fire"
  - "Faerie Fire"
  - "1-V-L-FF"
registry_id: 1-V-L-FF
attribute_code: "1·Evo·None·cube (20)·60 feet·Up to 1 minute"
incantation: "Su’-Bowynse"
tier: 1
school: Evocation
affinity: V
grade: L
pz_total: 7.5
pz_quantum: 350.0
t_e: -2.85
updated: 2026-11-16
---

**Faerie Fire** (`1-V-L-FF`) is a 1st Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **7.5 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -2.85 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Evocation]]
        - **Faerie Fire** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-V-L-FF` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Evo·None·cube (20)·60 feet·Up to 1 minute` |
| Incantation | *Su’-Bowynse* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | cube (20) |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation) |
| Ritual | no |
| Resistance check | agility; on success: no effect |
| Practitioner lineages | Druid |

### Mechanism

Objects and creatures in a 20 ft cube are outlined in coloured light that makes them easier to hit and cancels their invisibility.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| outline ignition | `0.1` | 0.1 |
| upkeep: 6 dim outlines at 12.5 W for 1 min | `6*12.5*60/J` | 3.0 |
| Pattern cost | `0.01 × Q1 × (1 + 0.25)` | 4.4 |

| Quantity | Value |
|---|---|
| Effect energy | 0.1 Pz |
| Upkeep energy | 3.0 Pz (0.05 Pz/s) |
| **Total draw** | **7.5 Pz** (11.2 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.0214 |
| Energy-equivalent tier T_E | -2.85 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** concentration.

**Assumptions:** Six outlined objects or creatures; dim light 12.5 W each.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Faerie Fire (1-V-L-FF) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | cube (20) | 9 | `0000000010011` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Su’-Bowynse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisu’-Bowynse* · T3: *Lisu’-Bowynse* · T4: *Visu’-Bowynse* · T5: *Tisu’-Bowynse* · T6: *Risu’-Bowynse* · T7: *Misu’-Bowynse* · T8: *Nisu’-Bowynse* · T9: *Xyisu’-Bowynse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 4→0 | 3 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#62c27a`.

![[Faerie Fire (1-V-L-FF) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.923 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.843 | `#0074ff` (495 nm eq.) | source grid |
| Area | cube (20) | 0.250 | 0.989 | `#cdff00` (625 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.888 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.16): swatch `#9cbe8e`, measured lines at 0.101, 0.251, 0.501, 0.589, 0.685. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 0.87. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·V·None`; the k4 to k6 lines (cube (20), 60 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·V·None` |
| Standard spectrometer detection range | 0.27 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.6 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1b 1c 1d 1f` (Heat, Light, Life, Energy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1.2 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (2.1% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Light and Radiance]] |
| Element | [[Fire Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Continual Flame (2-V-M-CF)|Continual Flame]] (2) · [[Sacred Flame (0-V-L-SF)|Sacred Flame]] (0) · [[Burning Hands (1-V-L-BH)|Burning Hands]] (1) · [[Focusing Lens (1-V-L-FLC)|Focusing Lens]] (1) · [[Guiding Bolt (1-V-L-GB)|Guiding Bolt]] (1) · [[Hellish Rebuke (1-V-L-HR)|Hellish Rebuke]] (1) · [[Kilonova (1-V-M-KLN)|Kilonova]] (1) · [[Dancing Lights (0-V-L-DL)|Dancing Lights]] (0).


---

## Tactical Assessment

Marks camouflaged or invisible targets for fire.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
