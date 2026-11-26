---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-7
  - spell/illusion
  - source/srd
aliases:
  - "7th Tier Spell: Mirage Arcane"
  - "Mirage Arcane"
  - "7-I-M-MAR"
registry_id: 7-I-M-MAR
attribute_code: "7·Ill·None·cube (5280)·Sight·10 days"
incantation: "Mai’-Baetory"
tier: 7
school: Illusion
affinity: I
grade: M
pz_total: 449318.0
pz_quantum: 141200.1
t_e: 8.16
updated: 2026-11-16
---

**Mirage Arcane** (`7-I-M-MAR`) is a 7th Tier working of the [[Illusion]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **449,318 Pz** against a slot quantum of 141,200 Pz, which puts its energy-equivalent tier at T_E 8.16 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 7 Workings]]
      - [[Illusion]]
        - **Mirage Arcane** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `7-I-M-MAR` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `7·Ill·None·cube (5280)·Sight·10 days` |
| Incantation | *Mai’-Baetory* |
| Affinity | I (Illusion) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 7th Tier |
| School | [[Illusion]] |
| Casting time | 10 minutes |
| Range | Sight |
| Area | cube (5280) |
| Duration | 10 days |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Bard, Druid, Wizard |

### Mechanism

The field overlays up to a square mile of land with a convincing false terrain that can be seen, heard, smelled and touched, persisting for 10 days. Creatures are neither hidden nor added.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Terrain overlay construction (instant info) | `instant info = 1 Pz` | 1.0 |
| Terrain illusion skin, 1 square mile x 2 m (upkeep) | `0.002*(2.59e6 m^2*0.1 m/1000)*864000 s  [C6]` | 447,552 |
| Pattern cost | `0.01 × Q7 × (1 + 0.25)` | 1,765 |

| Quantity | Value |
|---|---|
| Effect energy | 1.0 Pz |
| Upkeep energy | 447,552 Pz (10.4 Pz/s) |
| **Total draw** | **449,318 Pz** (673,977.0 kJ) |
| Slot quantum Q7 | 141,200 Pz |
| Field gain (draw / quantum) | 3.18 |
| Energy-equivalent tier T_E | 8.16 |
| Handling points | 0.25 |
| Grade score | 0.83 → M |

Calibration applied: C6 (Illusion skin), see [[Parzival Energy Budget#Registry calibration rules]].

**Handling flags:** long cast.

**Assumptions:** Overlay modelled as a 2 m deep skin over 1 square mile for 10 days; the volume constant gives a cost far above the tier return, so treat as an upper bound.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Mirage Arcane (7-I-M-MAR) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 7 | 7 | `0000000001111` |
| k2 School | Illusion | 5 | `0000000001011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | cube (5280) | 16 | `0000000100001` |
| k5 Range | Sight | 13 | `0000000011011` |
| k6 Duration | 10 days | 3 | `0000000000111` |

### Incantation

Spoken as **Mai’-Baetory** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T8: *Nimai’-Baetory* · T9: *Xyimai’-Baetory*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 3→2 | 4 |
| k2 School | 0→11 1→12 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 5→1 | 2 |
| k5 Range | 0→8 1→9 3→11 4→12 | 4 |
| k6 Duration | 0→7 1→8 2→9 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#2e9da9`.

![[Mirage Arcane (7-I-M-MAR) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 7 | 0.700 | 1.000 | `#005eff` (490 nm eq.) | source grid |
| School | Illusion | 0.625 | 0.997 | `#00c5ff` (512 nm eq.) | source grid |
| Duration | 10 days | 0.211 | 0.887 | `#fff500` (637 nm eq.) | source grid |
| Area | cube (5280) | 0.444 | 0.968 | `#00ff3b` (567 nm eq.) | source grid |
| Range | Sight | 0.765 | 0.998 | `#0007ff` (471 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.20): swatch `#4bcfc9`, measured lines at 0.211, 0.445, 0.626, 0.701, 0.765. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 5.65. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `7·I·None`; the k4 to k6 lines (cube (5280), Sight, 10 days) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `7·I·None` |
| Standard spectrometer detection range | 67.03 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 7,060 Pz (0.05 × Q7) |
| Counter drawn cold (all six layers) | 14,120 Pz (0.10 × Q7) |
| Unravel after completion | 103,630 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Light, Introspection, 2x Flexibility. The working vector used by [[Recast Tension and Combination Affinity]] is `2c 1d 1F 1G 2h 1J` (2x Light, Life, Potential, Introspection, 2x Flexibility, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 74,886 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 3.18 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 7th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Endures independently once set, which places it under the decay clause of ULMTU-XIII. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIII]] | Lex Impermanentiae | Long-lived patterns drift toward reversion unless refreshed from a source that satisfies ULMTU-I. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 7th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Illusion school with aspect lean Light, Introspection, 2x Flexibility. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 7 Workings]] |
| School | [[Illusion]] |
| Affinity | [[Illusion]] (I) |
| Function | [[Concealment and Illusion]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Project Image (7-I-L-PIO)|Project Image]] (7) · [[Programmed Illusion (6-I-L-PI)|Programmed Illusion]] (6) · [[Dream of the Blue Veil (7-C-M-DBV)|Dream of the Blue Veil]] (7) · [[Mislead (5-I-L-MSL)|Mislead]] (5) · [[Seeming (5-I-L-SMN)|Seeming]] (5) · [[Sequester (7-T-L-SQS)|Sequester]] (7) · [[Greater Invisibility (4-I-L-GIE)|Greater Invisibility]] (4) · [[Hallucinatory Terrain (4-I-M-HT)|Hallucinatory Terrain]] (4).


---

## Tactical Assessment

Disguises airfields, roads and fortifications, or makes open ground impassable to troops, over a whole sector for days. Imaging from orbit or by non-optical sensors may still reveal the real terrain.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 7 Workings]] · [[Illusion]] · [[Spell Breakdown Procedure]] · [[Parzival]]
