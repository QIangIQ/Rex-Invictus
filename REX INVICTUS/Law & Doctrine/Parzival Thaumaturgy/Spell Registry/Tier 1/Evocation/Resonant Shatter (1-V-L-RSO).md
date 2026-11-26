---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/evocation
  - source/science-spellbook
aliases:
  - "1st Tier Spell: Resonant Shatter"
  - "1-V-L-RSO"
  - "Resonant Shatter (Science)"
registry_id: 1-V-L-RSO
attribute_code: "1·Evo·Piercing·sphere (10)·60 feet·Instantaneous"
incantation: "Suix-Sewyn"
tier: 1
school: Evocation
affinity: V
grade: L
pz_total: 528.9
pz_quantum: 350.0
t_e: 1.41
updated: 2026-11-16
---

**Resonant Shatter** (`1-V-L-RSO`) is a 1st Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **529 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E 1.41 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Evocation]]
        - **Resonant Shatter** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-V-L-RSO` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Evo·Piercing·sphere (10)·60 feet·Instantaneous` |
| Incantation | *Suix-Sewyn* |
| Affinity | V (Evocation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Evocation]] |
| Casting time | 1 Action |
| Range | 60 feet |
| Area | sphere (10) |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A drinking glass |
| Ritual | no |
| Injury | 2d8 piercing (mean 9) |
| Injury by tier | T1: 2d8, T2: 3d8, T3: 4d8, T4: 5d8, T5: 6d8, T6: 7d8, T7: 8d8, T8: 9d8, T9: 10d8 |
| Resistance check | constitution; on success: half injury |
| Practitioner lineages | Wizard, Sorcerer, Warlock, Bard |

### Mechanism

Finds the resonant mode of an inorganic object and drives it until the object bursts into shrapnel over 10 ft.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Shrapnel | `9 HP x 0.35 (piercing) x S/A_c, S = sphere r=3.048 m = 116.7 m^2` | 525 |
| Resonant drive | `fracture energy = 50 J / 1500` | 0.0333 |
| Pattern cost | `0.01 × Q1 × (1 + 0.00)` | 3.5 |

| Quantity | Value |
|---|---|
| Effect energy | 525 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **529 Pz** (793.3 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 1.51 |
| Energy-equivalent tier T_E | 1.41 |
| Handling points | 0.00 |
| Grade score | 0.21 → L |

**Handling flags:** none.

**Assumptions:** Shrapnel 2d8 = 9 piercing over a 10 ft sphere; resonant drive to fracture 50 J.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Resonant Shatter (1-V-L-RSO) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Piercing | 8 | `0000000010001` |
| k4 Area | sphere (10) | 27 | `0000000110111` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Suix-Sewyn** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisuix-Sewyn* · T3: *Lisuix-Sewyn* · T4: *Visuix-Sewyn* · T5: *Tisuix-Sewyn* · T6: *Risuix-Sewyn* · T7: *Misuix-Sewyn* · T8: *Nisuix-Sewyn* · T9: *Xyisuix-Sewyn*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 4→1 | 2 |
| k4 Area | 0→9 1→10 2→11 4→0 5→1 | 5 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#5c9093`.

![[Resonant Shatter (1-V-L-RSO) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| Damage | Piercing | 0.571 | 0.895 | `#00ffec` (529 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.923 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.995 | `#ff0028` (700 nm eq.) | source grid |
| Area | sphere (10) | 0.750 | 0.810 | `#0017ff` (475 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.888 | `#00fbff` (524 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 2.72. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·V·Piercing`; the k4 to k6 lines (sphere (10), 60 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·V·Piercing` |
| Standard spectrometer detection range | 2.30 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.0 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Beyond, Cold, Hopelessness, Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 2f 1I 2j` (Beyond, 2x Energy, Hopelessness, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 88.1 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 1.51 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 1st Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Area Destruction]] |
| Element | [[Piercing Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Blast (1-V-L-BLS)|Blast]] (1) · [[Burning Hands (1-V-L-BH)|Burning Hands]] (1) · [[Kilonova (1-V-M-KLN)|Kilonova]] (1) · [[Thunderwave (1-V-L-THN)|Thunderwave]] (1) · [[Bohr's Model (2-P-L-BSM)|Bohr's Model]] (2) · [[Galaxy Whirl (2-V-L-GWL)|Galaxy Whirl]] (2) · [[Geyser (2-V-L-GYS)|Geyser]] (2) · [[Moonbeam (2-V-M-MNB)|Moonbeam]] (2).


---

## Tactical Assessment

Turns windows, stone facing or vehicle glass into fragmentation charges.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
