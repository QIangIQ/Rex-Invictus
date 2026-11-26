---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/illusion
  - source/srd
aliases:
  - "5th Tier Spell: Mislead"
  - "Mislead"
  - "5-I-L-MSL"
registry_id: 5-I-L-MSL
attribute_code: "5·Ill·None·None·Self·Up to 1 hour"
incantation: "Taiporsi"
tier: 5
school: Illusion
affinity: I
grade: L
pz_total: 646.0
pz_quantum: 19109.4
t_e: 1.61
updated: 2026-11-16
---

**Mislead** (`5-I-L-MSL`) is a 5th Tier working of the [[Illusion]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **646 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 1.61 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Illusion]]
        - **Mislead** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-I-L-MSL` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Ill·None·None·Self·Up to 1 hour` |
| Incantation | *Taiporsi* |
| Affinity | I (Illusion) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Illusion]] |
| Casting time | 1 action |
| Range | Self |
| Area | single point or target |
| Duration | Up to 1 hour (concentration) |
| Components | somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Bard, Wizard |

### Mechanism

The caster turns invisible while an illusory double appears in their place; the double can be moved and speaks, and the caster can see and hear through it. Attacking or channelling ends the invisibility.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Optical redirection around caster (upkeep) | `1000 W/m^2 * 0.7 m^2 * 10% / 1500 * 3600 s` | 168 |
| Illusory double light (upkeep) | `5 W / 1500 * 3600 s` | 12.0 |
| Remote senses via the double, 100 m (upkeep) | `0.001 Pz/s * (100 m / 10) * 3600 s` | 36.0 |
| Pattern cost | `0.01 × Q5 × (1 + 1.25)` | 430 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 216 Pz (0.06 Pz/s) |
| **Total draw** | **646 Pz** (968.9 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 0.0338 |
| Energy-equivalent tier T_E | 1.61 |
| Handling points | 1.25 |
| Grade score | 0.25 → L |

**Handling flags:** concentration, fragile.

**Assumptions:** Invisibility costed as for a single subject in daylight; double kept within 100 m; 1 hour.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Mislead (5-I-L-MSL) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Illusion | 5 | `0000000001011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Up to 1 hour | 12 | `0000000011001` |

### Incantation

Spoken as **Taiporsi** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Ritaiporsi* · T7: *Mitaiporsi* · T8: *Nitaiporsi* · T9: *Xyitaiporsi*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 1→12 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 3→10 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#00b7e1`.

![[Mislead (5-I-L-MSL) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| School | Illusion | 0.625 | 0.992 | `#00c5ff` (512 nm eq.) | source grid |
| Duration | Up to 1 hour | 0.632 | 0.991 | `#00c0ff` (511 nm eq.) | source grid |
| Range | Self | 0.706 | 0.979 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.20): swatch `#4bebce`, measured lines at 0.501, 0.627, 0.706. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.81. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·I·None`; the k4 to k6 lines (None, Self, Up to 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·I·None` |
| Standard spectrometer detection range | 2.54 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 1,954 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Light, Introspection, 2x Flexibility. The working vector used by [[Recast Tension and Combination Affinity]] is `2c 1d 1F 1G 2h 1J` (2x Light, Life, Potential, Introspection, 2x Flexibility, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 108 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 5th Tier quantum of 19,109 Pz (3.4% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 5th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Illusion school with aspect lean Light, Introspection, 2x Flexibility. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 5 Workings]] |
| School | [[Illusion]] |
| Affinity | [[Illusion]] (I) |
| Function | [[Concealment and Illusion]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Seeming (5-I-L-SMN)|Seeming]] (5) · [[Greater Invisibility (4-I-L-GIE)|Greater Invisibility]] (4) · [[Hallucinatory Terrain (4-I-M-HT)|Hallucinatory Terrain]] (4) · [[Programmed Illusion (6-I-L-PI)|Programmed Illusion]] (6) · [[Illusory Geodesic Curve (3-I-L-IGC)|Illusory Geodesic Curve]] (3) · [[Major Image (3-I-L-MIJ)|Major Image]] (3) · [[Mirage Arcane (7-I-M-MAR)|Mirage Arcane]] (7) · [[Project Image (7-I-L-PIO)|Project Image]] (7).


---

## Tactical Assessment

Lets a commander or agent slip away while a decoy keeps talking, or scout a building through the double's senses. The real body is vulnerable while using the double's senses.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Illusion]] · [[Spell Breakdown Procedure]] · [[Parzival]]
