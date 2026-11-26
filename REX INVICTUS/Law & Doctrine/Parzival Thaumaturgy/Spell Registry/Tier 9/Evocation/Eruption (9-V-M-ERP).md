---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-9
  - spell/evocation
  - source/science-spellbook
aliases:
  - "9th Tier Spell: Eruption"
  - "9-V-M-ERP"
  - "Eruption (Science)"
registry_id: 9-V-M-ERP
attribute_code: "9·Evo·Fire·sphere (40)·1 mile·Instantaneous"
incantation: "Xyuire-Soeyp"
tier: 9
school: Evocation
affinity: V
grade: M
pz_total: 1764963.2
pz_quantum: 1043335.3
t_e: 9.53
updated: 2026-11-16
---

**Eruption** (`9-V-M-ERP`) is a 9th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **1.76 MPz Pz** against a slot quantum of 1.04 MPz Pz, which puts its energy-equivalent tier at T_E 9.53 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 9 Workings]]
      - [[Evocation]]
        - **Eruption** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `9-V-M-ERP` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `9·Evo·Fire·sphere (40)·1 mile·Instantaneous` |
| Incantation | *Xyuire-Soeyp* |
| Affinity | V (Evocation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 9th Tier |
| School | [[Evocation]] |
| Casting time | 1 Action |
| Range | 1 mile |
| Area | sphere (40) |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 9d8 fire (mean 40.5) |
| Injury by tier | T9: 9d8 |
| Resistance check | agility; on success: half injury |
| Practitioner lineages | Wizard, Sorcerer, Druid |

### Mechanism

Triggers a mountain peak within a mile to erupt, sending pyroclasts and lava onto five chosen points; lava lingers for ten minutes.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Pyroclast heat, 5 points | `40.5 HP x 0.7 (fire) x S/A_c, S = sphere r=12.19 m = 1867.9 m^2 x 5` | 378,255 |
| Pyroclast impact, 5 points | `38.5 HP x 0.46 (bludgeoning) x S/A_c, S = sphere r=12.19 m = 1867.9 m^2 x 5` | 236,293 |
| Lingering lava, 5 points | `40.5 HP x 0.7 (fire) x S/A_c, S = sphere r=12.19 m = 1867.9 m^2 x 15` | 1.13 MPz |
| Pattern cost | `0.01 × Q9 × (1 + 0.50)` | 15,650 |

| Quantity | Value |
|---|---|
| Effect energy | 1.75 MPz Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **1.76 MPz Pz** (2,647,444.7 kJ) |
| Slot quantum Q9 | 1.04 MPz Pz |
| Field gain (draw / quantum) | 1.69 |
| Energy-equivalent tier T_E | 9.53 |
| Handling points | 0.50 |
| Grade score | 0.76 → M |

**Handling flags:** multi target control.

**Assumptions:** Fire 9d8 = 40.5 and bludgeoning 11d6 = 38.5 over five 40 ft spheres; lingering lava fire 9d8 at 3 triggers on the same areas; the mountain supplies the bulk heat of the magma (real thermal content ~1e9 Pz), which is not charged to the working.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Eruption (9-V-M-ERP) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 9 | 9 | `0000000010011` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Fire | 3 | `0000000000111` |
| k4 Area | sphere (40) | 33 | `0000001000011` |
| k5 Range | 1 mile | 0 | `0000000000001` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Xyuire-Soeyp** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]]. This attribute set is shared with other workings, so the glyph carries 1 centre dot(s) to tell it apart.

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 4→3 | 3 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 | 3 |
| k4 Area | 0→9 1→10 6→2 | 3 |
| k5 Range | 0→8 | 1 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#a85788`.

![[Eruption (9-V-M-ERP) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 9 | 0.900 | 1.000 | `#b600ff` (430 nm eq.) | source grid |
| Damage | Fire | 0.286 | 0.828 | `#9cff00` (614 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.923 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.667 | `#ff0028` (700 nm eq.) | source grid |
| Area | sphere (40) | 0.917 | 1.000 | `#cc00ff` (425 nm eq.) | source grid |
| Range | 1 mile | 0.000 | 0.667 | `#ff0028` (700 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 6.25. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `9·V·Fire`; the k4 to k6 lines (sphere (40), 1 mile, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `9·V·Fire` |
| Standard spectrometer detection range | 132.85 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 52,167 Pz (0.05 × Q9) |
| Counter drawn cold (all six layers) | 104,334 Pz (0.10 × Q9) |
| Unravel after completion | 104,334 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Energy, Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `2b 1c 3f 2j` (2x Heat, Light, 3x Energy, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 294,161 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 1.69 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 9th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 9th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 9 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Area Destruction]] |
| Element | [[Fire Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Meteor Swarm (9-V-L-MST)|Meteor Swarm]] (9) · [[Thermonuclear Fireball (9-P-L-TFE)|Thermonuclear Fireball]] (9) · [[Supernova (8-V-L-SPR)|Supernova]] (8) · [[Delayed Blast Fireball (7-V-M-DBF)|Delayed Blast Fireball]] (7) · [[Fire Storm (7-V-L-FSS)|Fire Storm]] (7) · [[Starburst (9-A-L-STR)|Starburst]] (9) · [[Incendiary Cloud (8-C-M-IC)|Incendiary Cloud]] (8) · [[Flame Strike (5-V-L-FSM)|Flame Strike]] (5).


---

## Tactical Assessment

Strategic area denial against forces in mountain terrain; destroys infantry and light vehicles.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 9 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
