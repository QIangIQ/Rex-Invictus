---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-8
  - spell/evocation
  - source/science-spellbook
aliases:
  - "8th Tier Spell: Supernova"
  - "8-V-L-SPR"
  - "Supernova (Science)"
registry_id: 8-V-L-SPR
attribute_code: "8·Evo·Fire·sphere (60)·150 feet·1 minute"
incantation: "Nuire-Sinosine"
tier: 8
school: Evocation
affinity: V
grade: L
pz_total: 239861.1
pz_quantum: 383821.6
t_e: 7.53
updated: 2026-11-16
---

**Supernova** (`8-V-L-SPR`) is a 8th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **239,861 Pz** against a slot quantum of 383,822 Pz, which puts its energy-equivalent tier at T_E 7.53 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 8 Workings]]
      - [[Evocation]]
        - **Supernova** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `8-V-L-SPR` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `8·Evo·Fire·sphere (60)·150 feet·1 minute` |
| Incantation | *Nuire-Sinosine* |
| Affinity | V (Evocation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 8th Tier |
| School | [[Evocation]] |
| Casting time | 1 Action |
| Range | 150 feet |
| Area | sphere (60) |
| Duration | 1 minute |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A small platinum model of a star or artistic representation of a star worth over 500GP |
| Ritual | no |
| Injury | 10d10 fire (mean 55) |
| Injury by tier | T8: 10d10, T9: 10d10 |
| Resistance check | agility; on success: no effect |
| Practitioner lineages | Wizard, Sorcerer |

### Mechanism

A hot, bright gas explosion fills a 60 ft radius with daylight-level light, then leaves a coloured cloud that blinds those inside.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Explosion heat | `55 HP x 0.7 (fire) x S/A_c, S = sphere r=18.29 m = 4202.8 m^2` | 231,156 |
| Daylight illumination (upkeep) | `90 kW x 60 s = 5.4e+06 J / 1500` | 3,600 |
| Coloured gas | `0.01 x 30745 kg x 1 Pz/kg` | 307 |
| Pattern cost | `0.01 × Q8 × (1 + 0.25)` | 4,798 |

| Quantity | Value |
|---|---|
| Effect energy | 231,463 Pz |
| Upkeep energy | 3,600 Pz (60.0 Pz/s) |
| **Total draw** | **239,861 Pz** (359,791.7 kJ) |
| Slot quantum Q8 | 383,822 Pz |
| Field gain (draw / quantum) | 0.625 |
| Energy-equivalent tier T_E | 7.53 |
| Handling points | 0.25 |
| Grade score | 0.01 → L |

**Handling flags:** costly material.

**Assumptions:** Fire 10d10 = 55 over a 60 ft sphere; daylight illumination 90 kW for 1 minute; coloured gas at 1% of the 30.8 t of air in the sphere at 1 Pz/kg.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Supernova (8-V-L-SPR) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 8 | 8 | `0000000010001` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Fire | 3 | `0000000000111` |
| k4 Area | sphere (60) | 35 | `0000001000111` |
| k5 Range | 150 feet | 4 | `0000000001001` |
| k6 Duration | 1 minute | 1 | `0000000000011` |

### Incantation

Spoken as **Nuire-Sinosine** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T9: *Xyinuire-Sinosine*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 4→3 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 | 3 |
| k4 Area | 0→9 1→10 2→11 6→2 | 4 |
| k5 Range | 0→8 3→11 | 2 |
| k6 Duration | 0→7 1→8 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#968b70`.

![[Supernova (8-V-L-SPR) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 8 | 0.800 | 1.000 | `#2900ff` (460 nm eq.) | source grid |
| Damage | Fire | 0.286 | 0.876 | `#9cff00` (614 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.956 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | 1 minute | 0.105 | 0.786 | `#ff6300` (668 nm eq.) | source grid |
| Area | sphere (60) | 0.972 | 0.985 | `#ff00e5` (408 nm eq.) | source grid |
| Range | 150 feet | 0.235 | 0.853 | `#e3ff00` (629 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 5.38. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `8·V·Fire`; the k4 to k6 lines (sphere (60), 150 feet, 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `8·V·Fire` |
| Standard spectrometer detection range | 48.98 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 19,191 Pz (0.05 × Q8) |
| Counter drawn cold (all six layers) | 38,382 Pz (0.10 × Q8) |
| Unravel after completion | 39,102 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Energy, Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `2b 1c 3f 2j` (2x Heat, Light, 3x Energy, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 39,977 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 8th Tier quantum of 383,822 Pz (62.5% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 8th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 8 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Area Destruction]] |
| Element | [[Fire Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Delayed Blast Fireball (7-V-M-DBF)|Delayed Blast Fireball]] (7) · [[Eruption (9-V-M-ERP)|Eruption]] (9) · [[Fire Storm (7-V-L-FSS)|Fire Storm]] (7) · [[Meteor Swarm (9-V-L-MST)|Meteor Swarm]] (9) · [[Thermonuclear Fireball (9-P-L-TFE)|Thermonuclear Fireball]] (9) · [[Incendiary Cloud (8-C-M-IC)|Incendiary Cloud]] (8) · [[Flame Strike (5-V-L-FSM)|Flame Strike]] (5) · [[Starburst (9-A-L-STR)|Starburst]] (9).


---

## Tactical Assessment

Large-area strike against infantry and light vehicles with a blinding aftermath that covers a withdrawal.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 8 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
