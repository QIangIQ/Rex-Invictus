---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/necromancy
  - source/srd
aliases:
  - "3rd Tier Spell: Speak with Dead"
  - "Speak with Dead"
  - "3-N-L-SDE"
registry_id: 3-N-L-SDE
attribute_code: "3·Nec·None·None·10 feet·10 minutes"
incantation: "Louspuls"
tier: 3
school: Necromancy
affinity: N
grade: L
pz_total: 34.2
pz_quantum: 2586.2
t_e: -1.33
updated: 2026-11-16
---

**Speak with Dead** (`3-N-L-SDE`) is a 3rd Tier working of the [[Necromancy (School)|Necromancy]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **34.2 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E -1.33 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Necromancy (School)|Necromancy]]
        - **Speak with Dead** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-N-L-SDE` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Nec·None·None·10 feet·10 minutes` |
| Incantation | *Louspuls* |
| Affinity | N (Necromancy) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Necromancy (School)\|Necromancy]] |
| Casting time | 1 action |
| Range | 10 feet |
| Area | single point or target |
| Duration | 10 minutes |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Burning incense |
| Ritual | no |
| Practitioner lineages | Bard, Cleric |

### Mechanism

The field drives the residual animating pattern of a corpse, actuating jaw and larynx so it can answer up to five questions from memory.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Animating impulse and speech actuation | `10 W * 50 s / 1500` | 0.333 |
| Five answers retrieved | `5 * 1 Pz instant info` | 5.0 |
| Upkeep: Animating spirit held in corpse | `0.005 Pz/s * 600 s` | 3.0 |
| Pattern cost | `0.01 × Q3 × (1 + 0.00)` | 25.9 |

| Quantity | Value |
|---|---|
| Effect energy | 5.3 Pz |
| Upkeep energy | 3.0 Pz (0.005 Pz/s) |
| **Total draw** | **34.2 Pz** (51.3 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 0.0132 |
| Energy-equivalent tier T_E | -1.33 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** 5 answers of ~10 s at 10 W mechanical; no soul return, so no re-anchoring term.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Speak with Dead (3-N-L-SDE) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Necromancy | 6 | `0000000001101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 10 feet | 1 | `0000000000011` |
| k6 Duration | 10 minutes | 4 | `0000000001001` |

### Incantation

Spoken as **Louspuls** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vilouspuls* · T5: *Tilouspuls* · T6: *Rilouspuls* · T7: *Milouspuls* · T8: *Nilouspuls* · T9: *Xyilouspuls*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 2→0 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 | 2 |
| k6 Duration | 0→7 3→10 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#94923b`.

![[Speak with Dead (3-N-L-SDE) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| School | Necromancy | 0.750 | 0.904 | `#0017ff` (475 nm eq.) | source grid |
| Duration | 10 minutes | 0.263 | 0.999 | `#bdff00` (621 nm eq.) | source grid |
| Range | 10 feet | 0.059 | 0.971 | `#ff2700` (682 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.23): swatch `#9da68c`, measured lines at 0.059, 0.264, 0.300, 0.751. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.53. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·N·None`; the k4 to k6 lines (None, 10 feet, 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·N·None` |
| Standard spectrometer detection range | 0.58 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 259 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Dark, 2x Death. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1D 1F 1J` (Within, Death, Potential, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 5.7 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 3rd Tier quantum of 2,586 Pz (1.3% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Necromancy school with aspect lean Within, Dark, 2x Death. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Necromancy (School)\|Necromancy]] |
| Affinity | [[Necromancy (School)\|Necromancy]] (N) |
| Function | [[Divination and Sensing]], [[Necromantic and Soul Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Animate Dead (3-N-M-AD)|Animate Dead]] (3) · [[Vampiric Touch (3-N-L-VT)|Vampiric Touch]] (3) · [[Blight (4-N-L-BLG)|Blight]] (4) · [[Blindness-Deafness (2-N-L-BD)|Blindness/Deafness]] (2) · [[Gentle Repose (2-N-H-GR)|Gentle Repose]] (2) · [[Arcane Singularity (3-C-L-ASA)|Arcane Singularity]] (3) · [[Beacon of Hope (3-A-L-BHA)|Beacon of Hope]] (3) · [[Clairvoyance (3-D-L-CLR)|Clairvoyance]] (3).


---

## Tactical Assessment

An interrogation tool for fallen enemy personnel, limited by the corpse's goodwill and by a 10-day refractory period.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Necromancy (School)|Necromancy]] · [[Spell Breakdown Procedure]] · [[Parzival]]
