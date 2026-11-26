---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/illusion
  - source/srd
aliases:
  - "5th Tier Spell: Creation"
  - "Creation"
  - "5-I-L-CRT"
registry_id: 5-I-L-CRT
attribute_code: "5·Ill·None·cube (5)·30 feet·Special"
incantation: "Tai’-Buusinyl"
tier: 5
school: Illusion
affinity: I
grade: L
pz_total: 27847.8
pz_quantum: 19109.4
t_e: 5.38
updated: 2026-11-16
---

**Creation** (`5-I-L-CRT`) is a 5th Tier working of the [[Illusion]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **27,848 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 5.38 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Illusion]]
        - **Creation** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-I-L-CRT` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Ill·None·cube (5)·30 feet·Special` |
| Incantation | *Tai’-Buusinyl* |
| Affinity | I (Illusion) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Illusion]] |
| Casting time | 1 minute |
| Range | 30 feet |
| Area | cube (5) |
| Duration | Special |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A tiny piece of matter of the same type of the item you plan to create |
| Ritual | no |
| Practitioner lineages | Sorcerer, Wizard |

### Mechanism

The field draws shadow substance and sets it into a nonliving object up to a 5 ft cube, of a material the caster has seen. Harder and rarer materials hold for shorter times before dissolving.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| 5 ft cube of stone (2600 kg/m3) as structured solid | `3*2600*(5*ft)**3` | 27,609 |
| Pattern cost | `0.01 × Q5 × (1 + 0.25)` | 239 |

| Quantity | Value |
|---|---|
| Effect energy | 27,609 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **27,848 Pz** (41,771.7 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 1.46 |
| Energy-equivalent tier T_E | 5.38 |
| Handling points | 0.25 |
| Grade score | 0.44 → L |

**Handling flags:** long cast.

**Assumptions:** Stone cube filled solid (9200 kg) as reference; a solid iron cube would be about 83600 Pz; no upkeep, the material dissolves at lease end.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Creation (5-I-L-CRT) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Illusion | 5 | `0000000001011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | cube (5) | 15 | `0000000011111` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Special | 10 | `0000000010101` |

### Incantation

Spoken as **Tai’-Buusinyl** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Ritai’-Buusinyl* · T7: *Mitai’-Buusinyl* · T8: *Nitai’-Buusinyl* · T9: *Xyitai’-Buusinyl*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 1→12 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 2→11 3→12 4→0 | 5 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 2→9 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#1cf375`.

![[Creation (5-I-L-CRT) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| School | Illusion | 0.625 | 0.992 | `#00c5ff` (512 nm eq.) | source grid |
| Duration | Special | 0.526 | 1.000 | `#00ffac` (542 nm eq.) | source grid |
| Area | cube (5) | 0.417 | 0.997 | `#00ff15` (575 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.979 | `#91ff00` (612 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.15): swatch `#7befb4`, measured lines at 0.295, 0.417, 0.501, 0.527, 0.626. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.44. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·I·None`; the k4 to k6 lines (cube (5), 30 feet, Special) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·I·None` |
| Standard spectrometer detection range | 16.69 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 1,911 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Light, Introspection, 2x Flexibility. The working vector used by [[Recast Tension and Combination Affinity]] is `2c 1d 1F 1G 2h 1J` (2x Light, Life, Potential, Introspection, 2x Flexibility, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 4,641 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 1.46 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 5th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Endures independently once set, which places it under the decay clause of ULMTU-XIII. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIII]] | Lex Impermanentiae | Long-lived patterns drift toward reversion unless refreshed from a source that satisfies ULMTU-I. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 5th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Illusion school with aspect lean Light, Introspection, 2x Flexibility. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 5 Workings]] |
| School | [[Illusion]] |
| Affinity | [[Illusion]] (I) |
| Function | [[Terrain and Matter Shaping]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Passwall (5-T-L-PSS)|Passwall]] (5) · [[Wall of Stone (5-V-M-WS)|Wall of Stone]] (5) · [[Control Water (4-T-H-CWN)|Control Water]] (4) · [[Fabricate (4-T-L-FBR)|Fabricate]] (4) · [[Freefall (4-T-L-FRF)|Freefall]] (4) · [[Ice Storm (4-V-L-ISE)|Ice Storm]] (4) · [[Move Earth (6-T-M-ME)|Move Earth]] (6) · [[Stone Shape (4-T-M-SSO)|Stone Shape]] (4).


---

## Tactical Assessment

Temporary fortifications, tools or bridging material; short lease times on metals limit it to emergency use.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Illusion]] · [[Spell Breakdown Procedure]] · [[Parzival]]
