---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/illusion
  - source/srd
aliases:
  - "1st Tier Spell: Disguise Self"
  - "Disguise Self"
  - "1-I-L-DS"
registry_id: 1-I-L-DS
attribute_code: "1·Ill·None·None·Self·1 hour"
incantation: "Saipora"
tier: 1
school: Illusion
affinity: I
grade: L
pz_total: 3.6
pz_quantum: 350.0
t_e: -3.59
updated: 2026-11-16
---

**Disguise Self** (`1-I-L-DS`) is a 1st Tier working of the [[Illusion]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **3.6 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -3.59 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Illusion]]
        - **Disguise Self** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-I-L-DS` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Ill·None·None·Self·1 hour` |
| Incantation | *Saipora* |
| Affinity | I (Illusion) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Illusion]] |
| Casting time | 1 action |
| Range | Self |
| Area | single point or target |
| Duration | 1 hour |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Bard, Sorcerer, Wizard |

### Mechanism

The field overlays the caster and their gear with a new visual appearance within the same body plan. Touch passes through the false parts.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| appearance overlay | `0.05` | 0.05 |
| upkeep: illusion envelope 0.15 m3 for 1 h | `0.002*(0.15/1000)*3600` | 0.0011 |
| Pattern cost | `0.01 × Q1 × (1 + 0.00)` | 3.5 |

| Quantity | Value |
|---|---|
| Effect energy | 0.05 Pz |
| Upkeep energy | 0.0011 Pz (0 Pz/s) |
| **Total draw** | **3.6 Pz** (5.3 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.0101 |
| Energy-equivalent tier T_E | -3.59 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Illusion volume 0.15 m3.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Disguise Self (1-I-L-DS) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Illusion | 5 | `0000000001011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | 1 hour | 0 | `0000000000001` |

### Incantation

Spoken as **Saipora** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisaipora* · T3: *Lisaipora* · T4: *Visaipora* · T5: *Tisaipora* · T6: *Risaipora* · T7: *Misaipora* · T8: *Nisaipora* · T9: *Xyisaipora*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 1→12 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 | 1 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#896275`.

![[Disguise Self (1-I-L-DS) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Illusion | 0.625 | 0.871 | `#00c5ff` (512 nm eq.) | source grid |
| Duration | 1 hour | 0.053 | 0.999 | `#ff1c00` (684 nm eq.) | source grid |
| Range | Self | 0.706 | 0.832 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.16): swatch `#97937f`, measured lines at 0.053, 0.101, 0.626, 0.706. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 0.55. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·I·None`; the k4 to k6 lines (None, Self, 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·I·None` |
| Standard spectrometer detection range | 0.19 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.0 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Light, Introspection, 2x Flexibility. The working vector used by [[Recast Tension and Combination Affinity]] is `2c 1d 1F 1G 2h 1J` (2x Light, Life, Potential, Introspection, 2x Flexibility, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 0.592 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (1.0% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Illusion school with aspect lean Light, Introspection, 2x Flexibility. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Illusion]] |
| Affinity | [[Illusion]] (I) |
| Function | [[Concealment and Illusion]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Alter Difraction Pattern (1-I-L-ADP)|Alter Difraction Pattern]] (1) · [[Illusory Script (1-I-L-IS)|Illusory Script]] (1) · [[Moe's Sensory Illusion (1-I-L-MSSI)|Moe's Sensory Illusion]] (1) · [[One Way Mirror (1-I-L-OWM)|One Way Mirror]] (1) · [[Silent Image (1-I-L-SI)|Silent Image]] (1) · [[Arcanist's Magic Aura (2-I-L-ASMA)|Arcanist's Magic Aura]] (2) · [[Blur (2-I-L-BLR)|Blur]] (2) · [[Cloak (2-I-L-CLK)|Cloak]] (2).


---

## Tactical Assessment

Infiltration and evasion of visual identification; physical inspection defeats it.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Illusion]] · [[Spell Breakdown Procedure]] · [[Parzival]]
