---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/abjuration
  - source/science-spellbook
aliases:
  - "3rd Tier Spell: Turbulent Gas"
  - "3-P-L-TG"
  - "Turbulent Gas (Science)"
registry_id: 3-P-L-TG
attribute_code: "3·Abj·Force·cone (30)·150 feet·Instantaneous"
incantation: "Laton-Nenosin"
tier: 3
school: Abjuration
affinity: P
grade: L
pz_total: 375.9
pz_quantum: 2586.2
t_e: 1.07
updated: 2026-11-16
---

**Turbulent Gas** (`3-P-L-TG`) is a 3rd Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **376 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E 1.07 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Abjuration]]
        - **Turbulent Gas** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-P-L-TG` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Abj·Force·cone (30)·150 feet·Instantaneous` |
| Incantation | *Laton-Nenosin* |
| Affinity | P (Pure field construct) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Abjuration]] |
| Casting time | 1 Action |
| Range | 150 feet |
| Area | cone (30) |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 2d10 force (mean 11) |
| Injury by tier | T3: 2d10, T4: 3d10, T5: 4d10, T6: 5d10, T7: 6d10, T8: 7d10, T9: 8d10 |
| Resistance check | strength; on success: half injury |
| Practitioner lineages | Wizard |

### Mechanism

A violent turbulent air jet sweeps a 30 ft cone, battering and knocking down those in it.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Turbulent jet | `11 HP x 0.4 (force) x S/A_c, S = cone l=9.144 m = 55.7 m^2` | 350 |
| Pattern cost | `0.01 × Q3 × (1 + 0.00)` | 25.9 |

| Quantity | Value |
|---|---|
| Effect energy | 350 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **376 Pz** (563.8 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 0.145 |
| Energy-equivalent tier T_E | 1.07 |
| Handling points | 0.00 |
| Grade score | -0.96 → L |

**Handling flags:** none.

**Assumptions:** Force 2d10 = 11 over a 30 ft cone.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Turbulent Gas (3-P-L-TG) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | Force | 4 | `0000000001001` |
| k4 Area | cone (30) | 2 | `0000000000101` |
| k5 Range | 150 feet | 4 | `0000000001001` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Laton-Nenosin** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vilaton-Nenosin* · T5: *Tilaton-Nenosin* · T6: *Rilaton-Nenosin* · T7: *Milaton-Nenosin* · T8: *Nilaton-Nenosin* · T9: *Xyilaton-Nenosin*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 3→0 | 2 |
| k4 Area | 0→9 2→11 | 2 |
| k5 Range | 0→8 3→11 | 2 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#c5870d`.

![[Turbulent Gas (3-P-L-TG) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| Damage | Force | 0.357 | 0.998 | `#3bff00` (593 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.956 | `#ff0028` (700 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.956 | `#ff0028` (700 nm eq.) | source grid |
| Area | cone (30) | 0.056 | 0.971 | `#ff2200` (683 nm eq.) | source grid |
| Range | 150 feet | 0.235 | 0.998 | `#e3ff00` (629 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 2.58. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·A·Force`; the k4 to k6 lines (cone (30), 150 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·A·Force` |
| Standard spectrometer detection range | 1.94 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 259 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Beyond, Introspection, 2x Movement and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1G 1H 1i 1j` (Introspection, Rigidity, Hope, Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 62.6 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 3rd Tier quantum of 2,586 Pz (14.5% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Pure]] (P) |
| Function | [[Area Destruction]] |
| Element | [[Force Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Sonic Boom (3-P-L-SBN)|Sonic Boom]] (3) · [[Bohr's Model (2-P-L-BSM)|Bohr's Model]] (2) · [[Planetary Rings (4-P-L-PR)|Planetary Rings]] (4) · [[Disintegrate (6-P-L-DSN)|Disintegrate]] (6) · [[Call Lightning (3-C-L-CLL)|Call Lightning]] (3) · [[Fireball (3-V-M-FRB)|Fireball]] (3) · [[Lightning Bolt (3-V-L-LB)|Lightning Bolt]] (3) · [[Outflows (5-A-L-OTF)|Outflows]] (5).


---

## Tactical Assessment

Knocks down an advancing line.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
