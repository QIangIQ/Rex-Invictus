---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/evocation
  - source/science-spellbook
aliases:
  - "2nd Tier Spell: Bohr's Model"
  - "2-P-L-BSM"
  - "Bohr's Model (Science)"
registry_id: 2-P-L-BSM
attribute_code: "2·Evo·Force·sphere (10)·Self·Up to 10 minutes"
incantation: "Huton-Seporly"
tier: 2
school: Evocation
affinity: P
grade: L
pz_total: 21.7
pz_quantum: 951.4
t_e: -1.78
updated: 2026-11-16
---

**Bohr's Model** (`2-P-L-BSM`) is a 2nd Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **21.7 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E -1.78 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Evocation]]
        - **Bohr's Model** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-P-L-BSM` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Evo·Force·sphere (10)·Self·Up to 10 minutes` |
| Incantation | *Huton-Seporly* |
| Affinity | P (Pure field construct) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Evocation]] |
| Casting time | 1 Action |
| Range | Self |
| Area | sphere (10) |
| Duration | Up to 10 minutes (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Two balls of different size |
| Ritual | no |
| Injury | 1d4+1 force (mean 3.5) |
| Injury by tier | T2: 1d4+1, T3: 1d4+1, T4: 1d4+1, T5: 1d4+1, T6: 1d4+1, T7: 1d4+1, T8: 1d4+1, T9: 1d4+1 |
| Practitioner lineages | Wizard, Sorcerer |

### Mechanism

Three force darts orbit the caster and strike automatically at creatures closing within 10 ft.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Force darts | `3.5 HP x 0.4 (force) x F 0.5 x 3 targets/projectiles` | 2.1 |
| Orbit held (upkeep) | `enchantment rate: 0.005 Pz/s x 600 s` | 3.0 |
| Pattern cost | `0.01 × Q2 × (1 + 0.75)` | 16.6 |

| Quantity | Value |
|---|---|
| Effect energy | 2.1 Pz |
| Upkeep energy | 3.0 Pz (0.005 Pz/s) |
| **Total draw** | **21.7 Pz** (32.6 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.0229 |
| Energy-equivalent tier T_E | -1.78 |
| Handling points | 0.75 |
| Grade score | -0.25 → L |

**Handling flags:** concentration, multi target control.

**Assumptions:** Darts 1d4+1 = 3.5 force each, directed bolt F 0.5, 3 darts at base; orbit held 10 minutes at the enchantment rate.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Bohr's Model (2-P-L-BSM) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Force | 4 | `0000000001001` |
| k4 Area | sphere (10) | 27 | `0000000110111` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Up to 10 minutes | 15 | `0000000011111` |

### Incantation

Spoken as **Huton-Seporly** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihuton-Seporly* · T4: *Vihuton-Seporly* · T5: *Tihuton-Seporly* · T6: *Rihuton-Seporly* · T7: *Mihuton-Seporly* · T8: *Nihuton-Seporly* · T9: *Xyihuton-Seporly*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 3→0 | 2 |
| k4 Area | 0→9 1→10 2→11 4→0 5→1 | 5 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 2→9 3→10 4→11 | 5 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#3d958f`.

![[Bohr's Model (2-P-L-BSM) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| Damage | Force | 0.357 | 0.988 | `#3bff00` (593 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.956 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Up to 10 minutes | 0.789 | 0.841 | `#1e00ff` (463 nm eq.) | source grid |
| Area | sphere (10) | 0.750 | 0.860 | `#0017ff` (475 nm eq.) | source grid |
| Range | Self | 0.706 | 0.880 | `#0058ff` (488 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 1.34. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·V·Force`; the k4 to k6 lines (sphere (10), Self, Up to 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·V·Force` |
| Standard spectrometer detection range | 0.47 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 95.7 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Beyond, Introspection, 2x Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1b 2f 1G 3j` (Beyond, Heat, 2x Energy, Introspection, 3x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 3.6 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (2.3% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Pure]] (P) |
| Function | [[Area Destruction]] |
| Element | [[Force Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Sonic Boom (3-P-L-SBN)|Sonic Boom]] (3) · [[Turbulent Gas (3-P-L-TG)|Turbulent Gas]] (3) · [[Galaxy Whirl (2-V-L-GWL)|Galaxy Whirl]] (2) · [[Geyser (2-V-L-GYS)|Geyser]] (2) · [[Moonbeam (2-V-M-MNB)|Moonbeam]] (2) · [[Planetary Rings (4-P-L-PR)|Planetary Rings]] (4) · [[Shatter (2-V-L-SHT)|Shatter]] (2) · [[Spiritual Weapon (2-P-L-SW)|Spiritual Weapon]] (2).


---

## Tactical Assessment

Close protection against rushes and ambush, useful for officers and couriers.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
