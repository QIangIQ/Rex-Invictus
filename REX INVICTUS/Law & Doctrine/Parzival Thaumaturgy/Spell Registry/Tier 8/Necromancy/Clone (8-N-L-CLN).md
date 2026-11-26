---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-8
  - spell/necromancy
  - source/srd
aliases:
  - "8th Tier Spell: Clone"
  - "Clone"
  - "8-N-L-CLN"
registry_id: 8-N-L-CLN
attribute_code: "8·Nec·None·None·Touch·Instantaneous"
incantation: "Noulix"
tier: 8
school: Necromancy
affinity: N
grade: L
pz_total: 57416.9
pz_quantum: 383821.6
t_e: 6.10
updated: 2026-11-16
---

**Clone** (`8-N-L-CLN`) is a 8th Tier working of the [[Necromancy (School)|Necromancy]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **57,417 Pz** against a slot quantum of 383,822 Pz, which puts its energy-equivalent tier at T_E 6.10 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 8 Workings]]
      - [[Necromancy (School)|Necromancy]]
        - **Clone** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `8-N-L-CLN` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `8·Nec·None·None·Touch·Instantaneous` |
| Incantation | *Noulix* |
| Affinity | N (Necromancy) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 8th Tier |
| School | [[Necromancy (School)\|Necromancy]] |
| Casting time | 1 hour |
| Range | Touch |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A diamond worth at least 1,000 gp and at least 1 cubic inch of flesh of the creature that is to be cloned, which the spell consumes, and a vessel worth at least 2,000 gp that has a sealable lid and is large enough to hold a Medium creature, such as a huge urn, coffin, mud-filled cyst in the ground, or crystal container filled with salt water |
| Ritual | no |
| Practitioner lineages | Wizard |

### Mechanism

An inert duplicate body grows in a sealed vessel over 120 days, and receives the original's soul on its death.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| body growth | `70 kg * 10 Pz/kg` | 700 |
| soul anchoring | `1e4 Pz * (8 - 3)` | 50,000 |
| Pattern cost | `0.01 × Q8 × (1 + 0.75)` | 6,717 |

| Quantity | Value |
|---|---|
| Effect energy | 50,700 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **57,417 Pz** (86,125.3 kJ) |
| Slot quantum Q8 | 383,822 Pz |
| Field gain (draw / quantum) | 0.15 |
| Energy-equivalent tier T_E | 6.10 |
| Handling points | 0.75 |
| Grade score | -0.20 → L |

**Handling flags:** costly material, consumed material, long cast.

**Assumptions:** Body 70 kg without gear; soul anchoring at tier 8; growth period covered by the matter term.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Clone (8-N-L-CLN) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 8 | 8 | `0000000010001` |
| k2 School | Necromancy | 6 | `0000000001101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Noulix** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T9: *Xyinoulix*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 4→3 | 2 |
| k2 School | 0→11 2→0 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#6606d5`.

![[Clone (8-N-L-CLN) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 8 | 0.800 | 1.000 | `#2900ff` (460 nm eq.) | source grid |
| School | Necromancy | 0.750 | 0.999 | `#0017ff` (475 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.726 | `#ff0028` (700 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.997 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.14): swatch `#288ce1`, measured lines at 0.004, 0.751, 0.801, 0.883. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.76. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `8·N·None`; the k4 to k6 lines (None, Touch, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `8·N·None` |
| Standard spectrometer detection range | 23.96 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 19,191 Pz (0.05 × Q8) |
| Counter drawn cold (all six layers) | 38,382 Pz (0.10 × Q8) |
| Unravel after completion | 38,382 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Dark, 2x Death. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1D 1F 1J` (Within, Death, Potential, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 9,569 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 8th Tier quantum of 383,822 Pz (15.0% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 8th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Necromancy school with aspect lean Within, Dark, 2x Death. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 8 Workings]] |
| School | [[Necromancy (School)\|Necromancy]] |
| Affinity | [[Necromancy (School)\|Necromancy]] (N) |
| Function | [[Summoning and Conjured Creatures]], [[Necromantic and Soul Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Create Undead (6-N-L-CU)|Create Undead]] (6) · [[Animate Dead (3-N-M-AD)|Animate Dead]] (3) · [[Finger of Death (7-N-L-FDN)|Finger of Death]] (7) · [[Resurrection (7-N-L-RSR)|Resurrection]] (7) · [[True Resurrection (9-N-L-TR)|True Resurrection]] (9) · [[Circle of Death (6-N-L-CD)|Circle of Death]] (6) · [[Glibness (8-T-L-GLB)|Glibness]] (8) · [[Gravitational Wave (8-V-L-GWV)|Gravitational Wave]] (8).


---

## Tactical Assessment

Insurance for critical leaders and specialists against assassination.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 8 Workings]] · [[Necromancy (School)|Necromancy]] · [[Spell Breakdown Procedure]] · [[Parzival]]
