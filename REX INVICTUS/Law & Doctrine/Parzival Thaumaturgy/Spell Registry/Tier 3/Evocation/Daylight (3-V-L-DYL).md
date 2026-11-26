---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/evocation
  - source/srd
aliases:
  - "3rd Tier Spell: Daylight"
  - "Daylight"
  - "3-V-L-DYL"
registry_id: 3-V-L-DYL
attribute_code: "3·Evo·None·sphere (60)·60 feet·1 hour"
incantation: "Lu’-Siwyna"
tier: 3
school: Evocation
affinity: V
grade: L
pz_total: 5426.4
pz_quantum: 2586.2
t_e: 3.74
updated: 2026-11-16
---

**Daylight** (`3-V-L-DYL`) is a 3rd Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **5,426 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E 3.74 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Evocation]]
        - **Daylight** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-V-L-DYL` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Evo·None·sphere (60)·60 feet·1 hour` |
| Incantation | *Lu’-Siwyna* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | sphere (60) |
| Duration | 1 hour |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Cleric, Druid, Paladin, Ranger, Sorcerer |

### Mechanism

The field lights a 60 ft sphere to daylight intensity with a further 60 ft of dim light, optionally carried on an object. It cancels weaker darkness workings it overlaps.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| light ignition | `0.5` | 0.5 |
| upkeep: 60 ft bright + 60 ft dim light, 2250 W for 1 h | `((60/20)**2*100+((120**2-60**2)/20**2)*0.5*100)*3600/J` | 5,400 |
| Pattern cost | `0.01 × Q3 × (1 + 0.00)` | 25.9 |

| Quantity | Value |
|---|---|
| Effect energy | 0.5 Pz |
| Upkeep energy | 5,400 Pz (1.5 Pz/s) |
| **Total draw** | **5,426 Pz** (8,139.5 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 2.1 |
| Energy-equivalent tier T_E | 3.74 |
| Handling points | 0.00 |
| Grade score | 0.37 → L |

**Handling flags:** none.

**Assumptions:** Torch reference 100 W per 20 ft bright radius scaled by area; dim annulus at half intensity.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Daylight (3-V-L-DYL) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (60) | 35 | `0000001000111` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | 1 hour | 0 | `0000000000001` |

### Incantation

Spoken as **Lu’-Siwyna** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vilu’-Siwyna* · T5: *Tilu’-Siwyna* · T6: *Rilu’-Siwyna* · T7: *Milu’-Siwyna* · T8: *Nilu’-Siwyna* · T9: *Xyilu’-Siwyna*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 2→11 6→2 | 4 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 | 1 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#7da477`.

![[Daylight (3-V-L-DYL) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.980 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | 1 hour | 0.053 | 0.970 | `#ff1c00` (684 nm eq.) | source grid |
| Area | sphere (60) | 0.972 | 0.798 | `#ff00e5` (408 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.959 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.15): swatch `#a7c294`, measured lines at 0.053, 0.300, 0.501, 0.589, 0.973. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.73. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·V·None`; the k4 to k6 lines (sphere (60), 60 feet, 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·V·None` |
| Standard spectrometer detection range | 7.37 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 1,339 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1b 1c 1d 1f` (Heat, Light, Life, Energy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 904 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 2.10 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 3rd Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Light and Radiance]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Lightning Bolt (3-V-L-LB)|Lightning Bolt]] (3) · [[Continual Flame (2-V-M-CF)|Continual Flame]] (2) · [[Moonbeam (2-V-M-MNB)|Moonbeam]] (2) · [[Call Lightning (3-C-L-CLL)|Call Lightning]] (3) · [[Faerie Fire (1-V-L-FF)|Faerie Fire]] (1) · [[Guiding Bolt (1-V-L-GB)|Guiding Bolt]] (1) · [[Blight (4-N-L-BLG)|Blight]] (4) · [[Chain Lightning (6-V-L-CLA)|Chain Lightning]] (6).


---

## Tactical Assessment

Lights an assault area or landing zone, and strips cover from troops using field-made darkness.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
