---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/illusion
  - source/srd
aliases:
  - "2nd Tier Spell: Blur"
  - "Blur"
  - "2-I-L-BLR"
registry_id: 2-I-L-BLR
attribute_code: "2·Ill·None·None·Self·Up to 1 minute"
incantation: "Haiporse"
tier: 2
school: Illusion
affinity: I
grade: L
pz_total: 19.4
pz_quantum: 951.4
t_e: -1.89
updated: 2026-11-16
---

**Blur** (`2-I-L-BLR`) is a 2nd Tier working of the [[Illusion]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **19.4 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E -1.89 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Illusion]]
        - **Blur** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-I-L-BLR` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Ill·None·None·Self·Up to 1 minute` |
| Incantation | *Haiporse* |
| Affinity | I (Illusion) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Illusion]] |
| Casting time | 1 action |
| Range | Self |
| Area | single point or target |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation) |
| Ritual | no |
| Practitioner lineages | Sorcerer, Wizard |

### Mechanism

The caster's outline is visually smeared, spoiling aimed attacks that rely on sight.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| evasion absorption | `25% of 15 points/round * 10 rounds * 0.20` | 7.5 |
| illusion upkeep | `0.002 Pz/s/1000 m^3 * 1 m^3 * 60 s` | 0.0001 |
| Pattern cost | `0.01 × Q2 × (1 + 0.25)` | 11.9 |

| Quantity | Value |
|---|---|
| Effect energy | 7.5 Pz |
| Upkeep energy | 0.0001 Pz (0 Pz/s) |
| **Total draw** | **19.4 Pz** (29.1 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.0204 |
| Energy-equivalent tier T_E | -1.89 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** concentration.

**Assumptions:** Hits reduced by 25% over 10 rounds of 15 points per round.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Blur (2-I-L-BLR) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Illusion | 5 | `0000000001011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Haiporse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihaiporse* · T4: *Vihaiporse* · T5: *Tihaiporse* · T6: *Rihaiporse* · T7: *Mihaiporse* · T8: *Nihaiporse* · T9: *Xyihaiporse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 1→12 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#45a1b9`.

![[Blur (2-I-L-BLR) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Illusion | 0.625 | 0.914 | `#00c5ff` (512 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.889 | `#0074ff` (495 nm eq.) | source grid |
| Range | Self | 0.706 | 0.880 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.14): swatch `#71c7ae`, measured lines at 0.201, 0.626, 0.685, 0.706. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.29. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·I·None`; the k4 to k6 lines (None, Self, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·I·None` |
| Standard spectrometer detection range | 0.44 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 95.1 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Light, Introspection, 2x Flexibility. The working vector used by [[Recast Tension and Combination Affinity]] is `2c 1d 1F 1G 2h 1J` (2x Light, Life, Potential, Introspection, 2x Flexibility, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 3.2 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (2.0% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Illusion school with aspect lean Light, Introspection, 2x Flexibility. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Illusion]] |
| Affinity | [[Illusion]] (I) |
| Function | [[Concealment and Illusion]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Arcanist's Magic Aura (2-I-L-ASMA)|Arcanist's Magic Aura]] (2) · [[Cloak (2-I-L-CLK)|Cloak]] (2) · [[Invisibility (2-I-L-INV)|Invisibility]] (2) · [[Mirror Image (2-I-L-MIR)|Mirror Image]] (2) · [[Silence (2-I-L-SLN)|Silence]] (2) · [[Alter Difraction Pattern (1-I-L-ADP)|Alter Difraction Pattern]] (1) · [[Disguise Self (1-I-L-DS)|Disguise Self]] (1) · [[Illusory Geodesic Curve (3-I-L-IGC)|Illusory Geodesic Curve]] (3).


---

## Tactical Assessment

Defensive measure against optically aimed fire; useless against thermal or non-visual targeting.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Illusion]] · [[Spell Breakdown Procedure]] · [[Parzival]]
