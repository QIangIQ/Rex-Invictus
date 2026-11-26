---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-7
  - spell/illusion
  - source/srd
aliases:
  - "7th Tier Spell: Simulacrum"
  - "Simulacrum"
  - "7-I-M-SML"
registry_id: 7-I-M-SML
attribute_code: "7·Ill·None·None·Touch·Until dispelled"
incantation: "Mailixis"
tier: 7
school: Illusion
affinity: I
grade: M
pz_total: 132871.0
pz_quantum: 141200.1
t_e: 6.94
updated: 2026-11-16
---

**Simulacrum** (`7-I-M-SML`) is a 7th Tier working of the [[Illusion]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **132,871 Pz** against a slot quantum of 141,200 Pz, which puts its energy-equivalent tier at T_E 6.94 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 7 Workings]]
      - [[Illusion]]
        - **Simulacrum** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `7-I-M-SML` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `7·Ill·None·None·Touch·Until dispelled` |
| Incantation | *Mailixis* |
| Affinity | I (Illusion) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 7th Tier |
| School | [[Illusion]] |
| Casting time | 12 hours |
| Range | Touch |
| Area | single point or target |
| Duration | Until dispelled |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Snow or ice in quantities sufficient to made a life-size copy of the duplicated creature; some hair, fingernail clippings, or other piece of that creature's body placed inside the snow or ice; and powdered ruby worth 1,500 gp, sprinkled over the duplicate and consumed by the spell |
| Ritual | no |
| Practitioner lineages | Wizard |

### Mechanism

A partially real copy of a creature is built from ice and loaded with the original's abilities.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| animated ice body, 80 kg semi-living at 10 Pz/kg | `10*80` | 800 |
| [upkeep] autonomy upkeep, 30-day reference | `0.05*30*86400` | 129,600 |
| Pattern cost | `0.01 × Q7 × (1 + 0.75)` | 2,471 |

| Quantity | Value |
|---|---|
| Effect energy | 800 Pz |
| Upkeep energy | 129,600 Pz (0.05 Pz/s) |
| **Total draw** | **132,871 Pz** (199,306.5 kJ) |
| Slot quantum Q7 | 141,200 Pz |
| Field gain (draw / quantum) | 0.941 |
| Energy-equivalent tier T_E | 6.94 |
| Handling points | 0.75 |
| Grade score | 0.72 → M |

**Handling flags:** costly material, consumed material, long cast.

**Assumptions:** Body 80 kg; open-ended duration counted over 30 days.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Simulacrum (7-I-M-SML) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 7 | 7 | `0000000001111` |
| k2 School | Illusion | 5 | `0000000001011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Until dispelled | 11 | `0000000010111` |

### Incantation

Spoken as **Mailixis** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T8: *Nimailixis* · T9: *Xyimailixis*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 3→2 | 4 |
| k2 School | 0→11 1→12 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 2→9 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#2688fd`.

![[Simulacrum (7-I-M-SML) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 7 | 0.700 | 1.000 | `#005eff` (490 nm eq.) | source grid |
| School | Illusion | 0.625 | 0.997 | `#00c5ff` (512 nm eq.) | source grid |
| Duration | Until dispelled | 0.579 | 0.993 | `#00fff7` (526 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.984 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.22): swatch `#39cbde`, measured lines at 0.579, 0.626, 0.701, 0.883. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 5.12. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `7·I·None`; the k4 to k6 lines (None, Touch, Until dispelled) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `7·I·None` |
| Standard spectrometer detection range | 36.45 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 7,060 Pz (0.05 × Q7) |
| Counter drawn cold (all six layers) | 14,120 Pz (0.10 × Q7) |
| Unravel after completion | 40,040 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Light, Introspection, 2x Flexibility. The working vector used by [[Recast Tension and Combination Affinity]] is `2c 1d 1F 1G 2h 1J` (2x Light, Life, Potential, Introspection, 2x Flexibility, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 22,145 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 7th Tier quantum of 141,200 Pz (94.1% of it). |
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
| Function | [[Summoning and Conjured Creatures]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Arcane Sword (7-P-L-ASC)|Arcane Sword]] (7) · [[Conjure Celestial (7-C-L-CCN)|Conjure Celestial]] (7) · [[Clone (8-N-L-CLN)|Clone]] (8) · [[Conjure Fey (6-C-L-CFN)|Conjure Fey]] (6) · [[Create Undead (6-N-L-CU)|Create Undead]] (6) · [[Gravitational Wave (8-V-L-GWV)|Gravitational Wave]] (8) · [[Instant Summons (6-C-L-ISS)|Instant Summons]] (6) · [[Planar Ally (6-C-L-PA)|Planar Ally]] (6).


---

## Tactical Assessment

Doubles a key specialist, including a caster, for long-term service.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 7 Workings]] · [[Illusion]] · [[Spell Breakdown Procedure]] · [[Parzival]]
