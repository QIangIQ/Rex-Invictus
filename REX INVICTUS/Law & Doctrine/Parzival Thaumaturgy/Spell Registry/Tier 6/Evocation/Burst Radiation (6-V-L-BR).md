---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-6
  - spell/evocation
  - source/science-spellbook
aliases:
  - "6th Tier Spell: Burst Radiation"
  - "6-V-L-BR"
  - "Burst Radiation (Science)"
registry_id: 6-V-L-BR
attribute_code: "6·Evo·Radiant·sphere (30)·150 feet·Up to 1 minute"
incantation: "Runat-Sornosinse"
tier: 6
school: Evocation
affinity: V
grade: L
pz_total: 20638.9
pz_quantum: 51944.6
t_e: 5.08
updated: 2026-11-16
---

**Burst Radiation** (`6-V-L-BR`) is a 6th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **20,639 Pz** against a slot quantum of 51,945 Pz, which puts its energy-equivalent tier at T_E 5.08 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 6 Workings]]
      - [[Evocation]]
        - **Burst Radiation** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `6-V-L-BR` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `6·Evo·Radiant·sphere (30)·150 feet·Up to 1 minute` |
| Incantation | *Runat-Sornosinse* |
| Affinity | V (Evocation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 6th Tier |
| School | [[Evocation]] |
| Casting time | 1 Action |
| Range | 150 feet |
| Area | sphere (30) |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A small platinum star |
| Ritual | no |
| Injury | 4d6 radiant (mean 14) |
| Injury by tier | T6: 4d6, T7: 5d6, T8: 6d6, T9: 7d6 |
| Resistance check | constitution; on success: half injury |
| Practitioner lineages | Wizard, Paladin, Sorcerer, Cleric |

### Mechanism

A star-bright ball flashes radiant and thermal energy over a 30 ft radius and then hangs as an intense heat source that burns anything passing through it.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Radiant burst | `14 HP x 0.5 (radiant) x S/A_c, S = sphere r=9.144 m = 1050.7 m^2` | 10,507 |
| Thermal burst | `9 HP x 0.7 (fire) x S/A_c, S = sphere r=9.144 m = 1050.7 m^2` | 9,456 |
| Contact burn in ball | `24.5 HP x 0.7 (fire) x F 1.0` | 17.1 |
| Bright light, 30 ft (upkeep) | `225 W x 60 s = 1.35e+04 J / 1500` | 9.0 |
| Pattern cost | `0.01 × Q6 × (1 + 0.25)` | 649 |

| Quantity | Value |
|---|---|
| Effect energy | 19,981 Pz |
| Upkeep energy | 9.0 Pz (0.15 Pz/s) |
| **Total draw** | **20,639 Pz** (30,958.4 kJ) |
| Slot quantum Q6 | 51,945 Pz |
| Field gain (draw / quantum) | 0.397 |
| Energy-equivalent tier T_E | 5.08 |
| Handling points | 0.25 |
| Grade score | -0.21 → L |

**Handling flags:** concentration.

**Assumptions:** Radiant 4d6 = 14 and fire 2d8 = 9 over a 30 ft sphere; one creature crossing the ball for 7d6 = 24.5 fire whole-body; light 225 W (30 ft bright radius) for 1 minute.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Burst Radiation (6-V-L-BR) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 6 | 6 | `0000000001101` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Radiant | 11 | `0000000010111` |
| k4 Area | sphere (30) | 31 | `0000000111111` |
| k5 Range | 150 feet | 4 | `0000000001001` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Runat-Sornosinse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T7: *Mirunat-Sornosinse* · T8: *Nirunat-Sornosinse* · T9: *Xyirunat-Sornosinse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 3→2 | 3 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 4→1 | 4 |
| k4 Area | 0→9 1→10 2→11 3→12 4→0 5→1 | 6 |
| k5 Range | 0→8 3→11 | 2 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#3d8fc2`.

![[Burst Radiation (6-V-L-BR) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 6 | 0.600 | 1.000 | `#00ebff` (520 nm eq.) | source grid |
| Damage | Radiant | 0.786 | 0.983 | `#1900ff` (464 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.995 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.996 | `#0074ff` (495 nm eq.) | source grid |
| Area | sphere (30) | 0.861 | 0.966 | `#8000ff` (442 nm eq.) | source grid |
| Range | 150 feet | 0.235 | 0.936 | `#e3ff00` (629 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 4.31. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `6·V·Radiant`; the k4 to k6 lines (sphere (30), 150 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `6·V·Radiant` |
| Standard spectrometer detection range | 14.37 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 2,597 Pz (0.05 × Q6) |
| Counter drawn cold (all six layers) | 5,194 Pz (0.10 × Q6) |
| Unravel after completion | 5,196 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Life, Hope and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `2b 1c 1d 2f 1i 1j` (2x Heat, Light, Life, 2x Energy, Hope, Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 3,440 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 6th Tier quantum of 51,945 Pz (39.7% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 6th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 6 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Area Destruction]] |
| Element | [[Radiant Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Sunbeam (6-V-L-SNB)|Sunbeam]] (6) · [[Summon Demon Core (6-A-M-SDC)|Summon Demon Core]] (6) · [[Sunburst (8-V-L-SNBB)|Sunburst]] (8) · [[Absolute Zero (6-V-L-AZ)|Absolute Zero]] (6) · [[Blade Barrier (6-V-L-BB)|Blade Barrier]] (6) · [[Freezing Sphere (6-V-M-FSZ)|Freezing Sphere]] (6) · [[Guardian of Faith (4-C-L-GFA)|Guardian of Faith]] (4) · [[Moonbeam (2-V-M-MNB)|Moonbeam]] (2).


---

## Tactical Assessment

Opening strike against massed infantry plus a lingering hot point that blocks a doorway or corridor.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 6 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
