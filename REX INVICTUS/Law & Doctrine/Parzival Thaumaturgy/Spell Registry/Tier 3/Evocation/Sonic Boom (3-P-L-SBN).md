---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/evocation
  - source/science-spellbook
aliases:
  - "3rd Tier Spell: Sonic Boom"
  - "3-P-L-SBN"
  - "Sonic Boom (Science)"
registry_id: 3-P-L-SBN
attribute_code: "3·Evo·Force·sphere (20)·Self·Instantaneous"
incantation: "Luton-Sopor"
tier: 3
school: Evocation
affinity: P
grade: L
pz_total: 4430.4
pz_quantum: 2586.2
t_e: 3.54
updated: 2026-11-16
---

**Sonic Boom** (`3-P-L-SBN`) is a 3rd Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **4,430 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E 3.54 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Evocation]]
        - **Sonic Boom** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-P-L-SBN` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Evo·Force·sphere (20)·Self·Instantaneous` |
| Incantation | *Luton-Sopor* |
| Affinity | P (Pure field construct) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Evocation]] |
| Casting time | 1 Action |
| Range | Self |
| Area | sphere (20) |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A small set of finger cymbals |
| Ritual | no |
| Injury | 3d10 force (mean 16.5) |
| Injury by tier | T3: 3d10, T4: 3d10, T5: 3d10, T6: 3d10, T7: 3d10, T8: 3d10, T9: 3d10 |
| Resistance check | agility; on success: half injury |
| Practitioner lineages | Wizard, Sorcerer |

### Mechanism

The caster drives a shock front outward through the air, striking everything within 20 ft and shoving it back.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Shock front | `16.5 HP x 0.4 (force) x S/A_c, S = sphere r=6.096 m = 467.0 m^2` | 4,403 |
| Push-back | `4 x 0.5 x 80 kg x 9.81 x 1.524 m = 2392 J / 1500` | 1.6 |
| Pattern cost | `0.01 × Q3 × (1 + 0.00)` | 25.9 |

| Quantity | Value |
|---|---|
| Effect energy | 4,405 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **4,430 Pz** (6,645.6 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 1.71 |
| Energy-equivalent tier T_E | 3.54 |
| Handling points | 0.00 |
| Grade score | 0.27 → L |

**Handling flags:** none.

**Assumptions:** Force 3d10 = 16.5 over a 20 ft sphere; 4 creatures pushed 1.524 m against friction.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Sonic Boom (3-P-L-SBN) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Force | 4 | `0000000001001` |
| k4 Area | sphere (20) | 30 | `0000000111101` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Luton-Sopor** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Viluton-Sopor* · T5: *Tiluton-Sopor* · T6: *Riluton-Sopor* · T7: *Miluton-Sopor* · T8: *Niluton-Sopor* · T9: *Xyiluton-Sopor*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 3→0 | 2 |
| k4 Area | 0→9 2→11 3→12 4→0 5→1 | 5 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#5a926e`.

![[Sonic Boom (3-P-L-SBN) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| Damage | Force | 0.357 | 0.998 | `#3bff00` (593 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.980 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.956 | `#ff0028` (700 nm eq.) | source grid |
| Area | sphere (20) | 0.833 | 0.867 | `#5a00ff` (450 nm eq.) | source grid |
| Range | Self | 0.706 | 0.921 | `#0058ff` (488 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 3.65. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·V·Force`; the k4 to k6 lines (sphere (20), Self, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·V·Force` |
| Standard spectrometer detection range | 6.66 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 259 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Beyond, Introspection, 2x Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1b 2f 1G 3j` (Beyond, Heat, 2x Energy, Introspection, 3x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 738 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 1.71 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 3rd Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Pure]] (P) |
| Function | [[Area Destruction]] |
| Element | [[Force Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Bohr's Model (2-P-L-BSM)|Bohr's Model]] (2) · [[Turbulent Gas (3-P-L-TG)|Turbulent Gas]] (3) · [[Planetary Rings (4-P-L-PR)|Planetary Rings]] (4) · [[Fireball (3-V-M-FRB)|Fireball]] (3) · [[Lightning Bolt (3-V-L-LB)|Lightning Bolt]] (3) · [[Wind Wall (3-V-L-WWN)|Wind Wall]] (3) · [[Disintegrate (6-P-L-DSN)|Disintegrate]] (6) · [[Fire Shield (4-V-L-FSR)|Fire Shield]] (4).


---

## Tactical Assessment

Clears boarders and close attackers from a caster.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
