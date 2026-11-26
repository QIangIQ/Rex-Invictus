---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-9
  - spell/evocation
  - source/science-spellbook
aliases:
  - "9th Tier Spell: Thermonuclear Fireball"
  - "9-P-L-TFE"
  - "Thermonuclear Fireball (Science)"
registry_id: 9-P-L-TFE
attribute_code: "9·Evo·Force·sphere (150)·300 feet·1 hour"
incantation: "Xyuton-Siesphina"
tier: 9
school: Evocation
affinity: P
grade: L
pz_total: 553029.9
pz_quantum: 1043335.3
t_e: 8.37
updated: 2026-11-16
---

**Thermonuclear Fireball** (`9-P-L-TFE`) is a 9th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **553,030 Pz** against a slot quantum of 1.04 MPz Pz, which puts its energy-equivalent tier at T_E 8.37 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 9 Workings]]
      - [[Evocation]]
        - **Thermonuclear Fireball** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `9-P-L-TFE` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `9·Evo·Force·sphere (150)·300 feet·1 hour` |
| Incantation | *Xyuton-Siesphina* |
| Affinity | P (Pure field construct) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 9th Tier |
| School | [[Evocation]] |
| Casting time | 1 Action |
| Range | 300 feet |
| Area | sphere (150) |
| Duration | 1 hour |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Two containers of light gas like Hydrogen or helium, which are consumed by the spell |
| Ritual | no |
| Injury | 6d6 force (mean 21) |
| Injury by tier | T9: 6d6 |
| Resistance check | agility; on success: no effect |
| Practitioner lineages | Wizard, Warlock, Sorcerer |

### Mechanism

A flash, then a 150 ft blast wave, then a 50 ft fireball, leaving a radiant glow that injures anyone who stays inside 50 ft for an hour.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Blast wave | `21 HP x 0.4 (force) x S/A_c, S = sphere r=45.72 m = 26267.7 m^2` | 315,213 |
| Fireball | `16.5 HP x 0.7 (fire) x S/A_c, S = sphere r=15.24 m = 2918.6 m^2` | 48,157 |
| Radiant afterglow | `28 HP x 0.5 (radiant) x S/A_c, S = sphere r=15.24 m = 2918.6 m^2 x 3` | 175,118 |
| Glow (upkeep) | `625 W x 3600 s = 2.25e+06 J / 1500` | 1,500 |
| Pattern cost | `0.01 × Q9 × (1 + 0.25)` | 13,042 |

| Quantity | Value |
|---|---|
| Effect energy | 538,488 Pz |
| Upkeep energy | 1,500 Pz (0.417 Pz/s) |
| **Total draw** | **553,030 Pz** (829,544.8 kJ) |
| Slot quantum Q9 | 1.04 MPz Pz |
| Field gain (draw / quantum) | 0.53 |
| Energy-equivalent tier T_E | 8.37 |
| Handling points | 0.25 |
| Grade score | -0.07 → L |

**Handling flags:** consumed material.

**Assumptions:** Force 6d6 = 21 over 150 ft, fire 3d10 = 16.5 over 50 ft, radiant 8d6 = 28 over 50 ft at 3 triggers; glow 625 W for 1 hour; the consumed gas would yield kilotons if fully fused, so the field caps the release to the described effects.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Thermonuclear Fireball (9-P-L-TFE) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 9 | 9 | `0000000010011` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Force | 4 | `0000000001001` |
| k4 Area | sphere (150) | 40 | `0000001010001` |
| k5 Range | 300 feet | 6 | `0000000001101` |
| k6 Duration | 1 hour | 0 | `0000000000001` |

### Incantation

Spoken as **Xyuton-Siesphina** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 4→3 | 3 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 3→0 | 2 |
| k4 Area | 0→9 4→0 6→2 | 3 |
| k5 Range | 0→8 2→10 3→11 | 3 |
| k6 Duration | 0→7 | 1 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#638277`.

![[Thermonuclear Fireball (9-P-L-TFE) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 9 | 0.900 | 1.000 | `#b600ff` (430 nm eq.) | source grid |
| Damage | Force | 0.357 | 0.863 | `#3bff00` (593 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.923 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | 1 hour | 0.053 | 0.698 | `#ff1c00` (684 nm eq.) | source grid |
| Area | sphere (150) | 0.819 | 0.997 | `#4400ff` (454 nm eq.) | RI half-step |
| Range | 300 feet | 0.353 | 0.861 | `#40ff00` (594 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 5.74. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `9·V·Force`; the k4 to k6 lines (sphere (150), 300 feet, 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `9·V·Force` |
| Standard spectrometer detection range | 74.37 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 52,167 Pz (0.05 × Q9) |
| Counter drawn cold (all six layers) | 104,334 Pz (0.10 × Q9) |
| Unravel after completion | 104,634 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Beyond, Introspection, 2x Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1b 2f 1G 3j` (Beyond, Heat, 2x Energy, Introspection, 3x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 92,172 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 9th Tier quantum of 1.04 MPz Pz (53.0% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 9th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 9 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Pure]] (P) |
| Function | [[Area Destruction]] |
| Element | [[Force Workings]], [[Fire Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Eruption (9-V-M-ERP)|Eruption]] (9) · [[Meteor Swarm (9-V-L-MST)|Meteor Swarm]] (9) · [[Supernova (8-V-L-SPR)|Supernova]] (8) · [[Delayed Blast Fireball (7-V-M-DBF)|Delayed Blast Fireball]] (7) · [[Fire Storm (7-V-L-FSS)|Fire Storm]] (7) · [[Starburst (9-A-L-STR)|Starburst]] (9) · [[Wormhole (9-P-L-WRM)|Wormhole]] (9) · [[Incendiary Cloud (8-C-M-IC)|Incendiary Cloud]] (8).


---

## Tactical Assessment

Strategic strike on a fortified position, with lingering contamination that denies the area.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 9 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
