---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-8
  - spell/evocation
  - source/srd
aliases:
  - "8th Tier Spell: Sunburst"
  - "Sunburst"
  - "8-V-L-SNBB"
registry_id: 8-V-L-SNBB
attribute_code: "8·Evo·Radiant·cylinder (60)·150 feet·Instantaneous"
incantation: "Nunat-Xanosin"
tier: 8
school: Evocation
affinity: V
grade: L
pz_total: 129938.2
pz_quantum: 383821.6
t_e: 6.92
updated: 2026-11-16
---

**Sunburst** (`8-V-L-SNBB`) is a 8th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **129,938 Pz** against a slot quantum of 383,822 Pz, which puts its energy-equivalent tier at T_E 6.92 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 8 Workings]]
      - [[Evocation]]
        - **Sunburst** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `8-V-L-SNBB` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `8·Evo·Radiant·cylinder (60)·150 feet·Instantaneous` |
| Incantation | *Nunat-Xanosin* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 8th Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 150 feet |
| Area | cylinder (60) |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Fire and a piece of sunstone |
| Ritual | no |
| Injury | 12d6 radiant (mean 42) |
| Injury by tier | T8: 12d6 |
| Resistance check | constitution; on success: half injury |
| Practitioner lineages | Druid, Sorcerer, Wizard |

### Mechanism

A sudden burst of sunlight-grade radiation fills an 18 m radius, burning and blinding those exposed and stripping away any field-made darkness.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Radiant flash, 60 ft radius | `42 HP * 0.50 * 4203 m^2 / 0.7` | 126,100 |
| Pattern cost | `0.01 × Q8 × (1 + 0.00)` | 3,838 |

| Quantity | Value |
|---|---|
| Effect energy | 126,100 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **129,938 Pz** (194,907.3 kJ) |
| Slot quantum Q8 | 383,822 Pz |
| Field gain (draw / quantum) | 0.339 |
| Energy-equivalent tier T_E | 6.92 |
| Handling points | 0.00 |
| Grade score | -0.54 → L |

**Handling flags:** none.

**Assumptions:** 12d6 = 42; area treated as sphere of radius 60 ft.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Sunburst (8-V-L-SNBB) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 8 | 8 | `0000000010001` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Radiant | 11 | `0000000010111` |
| k4 Area | cylinder (60) | 22 | `0000000101101` |
| k5 Range | 150 feet | 4 | `0000000001001` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Nunat-Xanosin** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T9: *Xyinunat-Xanosin*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 4→3 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 4→1 | 4 |
| k4 Area | 0→9 2→11 3→12 5→1 | 4 |
| k5 Range | 0→8 3→11 | 2 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#507aa7`.

![[Sunburst (8-V-L-SNBB) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 8 | 0.800 | 1.000 | `#2900ff` (460 nm eq.) | source grid |
| Damage | Radiant | 0.786 | 1.000 | `#1900ff` (464 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.956 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.726 | `#ff0028` (700 nm eq.) | source grid |
| Area | cylinder (60) | 0.611 | 0.982 | `#00dbff` (517 nm eq.) | source grid |
| Range | 150 feet | 0.235 | 0.853 | `#e3ff00` (629 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.23): swatch `#64b8bd`, measured lines at 0.004, 0.236, 0.501, 0.612, 0.787, 0.802. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 5.11. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `8·V·Radiant`; the k4 to k6 lines (cylinder (60), 150 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `8·V·Radiant` |
| Standard spectrometer detection range | 36.05 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 19,191 Pz (0.05 × Q8) |
| Counter drawn cold (all six layers) | 38,382 Pz (0.10 × Q8) |
| Unravel after completion | 38,382 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Life, Hope and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `2b 1c 1d 2f 1i 1j` (2x Heat, Light, Life, 2x Energy, Hope, Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 21,656 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 8th Tier quantum of 383,822 Pz (33.9% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 8th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 8 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Light and Radiance]], [[Area Destruction]] |
| Element | [[Radiant Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Sunbeam (6-V-L-SNB)|Sunbeam]] (6) · [[Burst Radiation (6-V-L-BR)|Burst Radiation]] (6) · [[Moonbeam (2-V-M-MNB)|Moonbeam]] (2) · [[Lance of Longinus (8-V-L-LL)|Lance of Longinus]] (8) · [[Summon Demon Core (6-A-M-SDC)|Summon Demon Core]] (6) · [[Supernova (8-V-L-SPR)|Supernova]] (8) · [[Delayed Blast Fireball (7-V-M-DBF)|Delayed Blast Fireball]] (7) · [[Eruption (9-V-M-ERP)|Eruption]] (9).


---

## Tactical Assessment

A single-pulse area weapon against massed infantry and undead, also used to blind sensors across a compound.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 8 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
