---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-8
  - spell/evocation
  - source/science-spellbook
aliases:
  - "8th Tier Spell: Gravitational Wave"
  - "8-V-L-GWV"
  - "Gravitational Wave (Science)"
registry_id: 8-V-L-GWV
attribute_code: "8·Evo·None·cone (60)·Self·Up to 1 minute"
incantation: "Nu’-Noporse"
tier: 8
school: Evocation
affinity: V
grade: L
pz_total: 6877.9
pz_quantum: 383821.6
t_e: 3.98
updated: 2026-11-16
---

**Gravitational Wave** (`8-V-L-GWV`) is a 8th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **6,878 Pz** against a slot quantum of 383,822 Pz, which puts its energy-equivalent tier at T_E 3.98 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 8 Workings]]
      - [[Evocation]]
        - **Gravitational Wave** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `8-V-L-GWV` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `8·Evo·None·cone (60)·Self·Up to 1 minute` |
| Incantation | *Nu’-Noporse* |
| Affinity | V (Evocation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 8th Tier |
| School | [[Evocation]] |
| Casting time | 1 Action |
| Range | Self |
| Area | cone (60) |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Two dense metal stars (or star symbols) worth at least 500GP each |
| Ritual | no |
| Practitioner lineages | Wizard |

### Mechanism

Two conjured micro-holes inspiral and their focused wave advances 10 ft each round along a 60 ft cone, freezing anything it passes in slowed time.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Time-hold on creatures in band (upkeep) | `4 x 1 kW x 60 s = 2.4e+05 J / 1500` | 160 |
| Micro-hole pair formed | `instant info-scale pattern` | 1.0 |
| Pattern cost | `0.01 × Q8 × (1 + 0.75)` | 6,717 |

| Quantity | Value |
|---|---|
| Effect energy | 1.0 Pz |
| Upkeep energy | 160 Pz (2.7 Pz/s) |
| **Total draw** | **6,878 Pz** (10,316.8 kJ) |
| Slot quantum Q8 | 383,822 Pz |
| Field gain (draw / quantum) | 0.0179 |
| Energy-equivalent tier T_E | 3.98 |
| Handling points | 0.75 |
| Grade score | -0.25 → L |

**Handling flags:** concentration, costly material, save or suck.

**Assumptions:** Reasoned order of magnitude: the wave suppresses kinetic and metabolic output of about 4 creatures in its band (1 kW each) for 60 s; a literal gravitational wave strong enough to slow time would need on the order of 1e20 Pz, so the effect is modelled as a time-hold field on the creatures in the band.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Gravitational Wave (8-V-L-GWV) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 8 | 8 | `0000000010001` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | cone (60) | 4 | `0000000001001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Nu’-Noporse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T9: *Xyinu’-Noporse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 4→3 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 3→12 | 2 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#3370bd`.

![[Gravitational Wave (8-V-L-GWV) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 8 | 0.800 | 1.000 | `#2900ff` (460 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.956 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.993 | `#0074ff` (495 nm eq.) | source grid |
| Area | cone (60) | 0.111 | 0.789 | `#ff6e00` (667 nm eq.) | source grid |
| Range | Self | 0.706 | 0.996 | `#0058ff` (488 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 3.84. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `8·V·None`; the k4 to k6 lines (cone (60), Self, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `8·V·None` |
| Standard spectrometer detection range | 8.29 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 19,191 Pz (0.05 × Q8) |
| Counter drawn cold (all six layers) | 38,382 Pz (0.10 × Q8) |
| Unravel after completion | 38,414 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1b 1c 1d 1f` (Heat, Light, Life, Energy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1,146 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 8th Tier quantum of 383,822 Pz (1.8% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 8th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 8 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Summoning and Conjured Creatures]], [[Mind and Will]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Arcane Sword (7-P-L-ASC)|Arcane Sword]] (7) · [[Divine Word (7-V-L-DWV)|Divine Word]] (7) · [[Antipathy-Sympathy (8-E-L-ASP)|Antipathy/Sympathy]] (8) · [[Clone (8-N-L-CLN)|Clone]] (8) · [[Dominate Monster (8-E-L-DMM)|Dominate Monster]] (8) · [[Feeblemind (8-E-L-FBL)|Feeblemind]] (8) · [[Power Word Stun (8-E-L-PWS)|Power Word Stun]] (8) · [[Arcane Hand (5-P-L-AH)|Arcane Hand]] (5).


---

## Tactical Assessment

Holds a breach point or bridge for a minute against everything in the cone.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 8 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
