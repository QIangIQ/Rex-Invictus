---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-9
  - spell/divination
  - source/science-spellbook
aliases:
  - "9th Tier Spell: Multiverse Exploration"
  - "9-D-L-MEL"
  - "Multiverse Exploration (Science)"
registry_id: 9-D-L-MEL
attribute_code: "9·Div·None·None·Self·Instantaneous"
incantation: "Xyipor"
tier: 9
school: Divination
affinity: D
grade: L
pz_total: 60434.4
pz_quantum: 1043335.3
t_e: 6.15
updated: 2026-11-16
---

**Multiverse Exploration** (`9-D-L-MEL`) is a 9th Tier working of the [[Divination]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **60,434 Pz** against a slot quantum of 1.04 MPz Pz, which puts its energy-equivalent tier at T_E 6.15 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 9 Workings]]
      - [[Divination]]
        - **Multiverse Exploration** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `9-D-L-MEL` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `9·Div·None·None·Self·Instantaneous` |
| Incantation | *Xyipor* |
| Affinity | D (Divination) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 9th Tier |
| School | [[Divination]] |
| Casting time | 1 Bonus Action |
| Range | Self |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A kaleidoscope |
| Ritual | no |
| Practitioner lineages | Wizard |

### Mechanism

The caster lives several alternative versions of the same moment and then commits one of them as real.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Branch reversal | `2.5 discarded turns x 2e4 Pz` | 50,000 |
| Branch selection | `instant info` | 1.0 |
| Pattern cost | `0.01 × Q9 × (1 + 0.00)` | 10,433 |

| Quantity | Value |
|---|---|
| Effect energy | 50,001 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **60,434 Pz** (90,651.5 kJ) |
| Slot quantum Q9 | 1.04 MPz Pz |
| Field gain (draw / quantum) | 0.0579 |
| Energy-equivalent tier T_E | 6.15 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Reasoned order of magnitude: each discarded branch reverses about 2e4 Pz of local activity in the engagement area; 1d4+1 = 3.5 branches, 2.5 discarded.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Multiverse Exploration (9-D-L-MEL) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 9 | 9 | `0000000010011` |
| k2 School | Divination | 2 | `0000000000101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Xyipor** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 4→3 | 3 |
| k2 School | 0→11 2→0 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#955499`.

![[Multiverse Exploration (9-D-L-MEL) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 9 | 0.900 | 1.000 | `#b600ff` (430 nm eq.) | source grid |
| School | Divination | 0.250 | 0.810 | `#cdff00` (625 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.667 | `#ff0028` (700 nm eq.) | source grid |
| Range | Self | 0.706 | 0.981 | `#0058ff` (488 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 4.78. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `9·D·None`; the k4 to k6 lines (None, Self, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `9·D·None` |
| Standard spectrometer detection range | 24.58 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 52,167 Pz (0.05 × Q9) |
| Counter drawn cold (all six layers) | 104,334 Pz (0.10 × Q9) |
| Unravel after completion | 104,334 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Light, 2x Extraspection. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 2c 1d 1F 2g 1J` (Beyond, 2x Light, Life, Potential, 2x Extraspection, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 10,072 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 9th Tier quantum of 1.04 MPz Pz (5.8% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 9th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Divination school with aspect lean Beyond, Light, 2x Extraspection. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 9 Workings]] |
| School | [[Divination]] |
| Affinity | [[Divination]] (D) |
| Function | [[Utility Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Weave Warp (9-T-L-WWA)|Weave Warp]] (9) · [[Foresight (9-D-L-FRS)|Foresight]] (9) · [[Create Chimera (6-T-L-CCE)|Create Chimera]] (6) · [[Alter Biome (9-T-X-AB)|Alter Biome]] (9) · [[Astral Projection (9-N-M-AP)|Astral Projection]] (9) · [[Enhance Potion (5-T-L-EP)|Enhance Potion]] (5) · [[Eruption (9-V-M-ERP)|Eruption]] (9) · [[Gate (9-C-L-GAT)|Gate]] (9).


---

## Tactical Assessment

Decisive-moment insurance for commanders and assault leads.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 9 Workings]] · [[Divination]] · [[Spell Breakdown Procedure]] · [[Parzival]]
