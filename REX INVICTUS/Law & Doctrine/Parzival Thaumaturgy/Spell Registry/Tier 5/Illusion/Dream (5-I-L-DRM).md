---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/illusion
  - source/srd
aliases:
  - "5th Tier Spell: Dream"
  - "Dream"
  - "5-I-L-DRM"
registry_id: 5-I-L-DRM
attribute_code: "5·Ill·Psychic·None·Special·8 hours"
incantation: "Taichar-’intixiy"
tier: 5
school: Illusion
affinity: I
grade: L
pz_total: 527.0
pz_quantum: 19109.4
t_e: 1.41
updated: 2026-11-16
---

**Dream** (`5-I-L-DRM`) is a 5th Tier working of the [[Illusion]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **527 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 1.41 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Illusion]]
        - **Dream** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-I-L-DRM` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Ill·Psychic·None·Special·8 hours` |
| Incantation | *Taichar-’intixiy* |
| Affinity | I (Illusion) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Illusion]] |
| Casting time | 1 minute |
| Range | Special |
| Area | single point or target |
| Duration | 8 hours |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A handful of sand, a dab of ink, and a writing quill plucked from a sleeping bird |
| Ritual | no |
| Injury | 3d6 psychic (mean 10.5) |
| Injury by tier | T5: 3d6 |
| Resistance check | will; on success: no effect |
| Practitioner lineages | Bard, Warlock, Wizard |

### Mechanism

A messenger in trance enters a sleeping target dreams anywhere on the same plane to talk or shape the dream, and can turn it into a nightmare that ruins rest.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| 3d6 = 10.5 psychic on waking | `10.5*0.02*0.5` | 0.105 |
| upkeep: dream contact: target and messenger coupling for 8 h | `0.005*2*8*3600` | 288 |
| Pattern cost | `0.01 × Q5 × (1 + 0.25)` | 239 |

| Quantity | Value |
|---|---|
| Effect energy | 0.105 Pz |
| Upkeep energy | 288 Pz (0.01 Pz/s) |
| **Total draw** | **527 Pz** (790.5 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 0.0276 |
| Energy-equivalent tier T_E | 1.41 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** long cast.

**Assumptions:** Sympathetic link treated as distance-independent; enchantment rate for target and messenger.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Dream (5-I-L-DRM) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Illusion | 5 | `0000000001011` |
| k3 Damage | Psychic | 10 | `0000000010101` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Special | 14 | `0000000011101` |
| k6 Duration | 8 hours | 8 | `0000000010001` |

### Incantation

Spoken as **Taichar-’intixiy** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Ritaichar-’intixiy* · T7: *Mitaichar-’intixiy* · T8: *Nitaichar-’intixiy* · T9: *Xyitaichar-’intixiy*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 1→12 3→1 | 3 |
| k3 Damage | 0→10 2→12 4→1 | 3 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 3→11 4→12 | 4 |
| k6 Duration | 0→7 4→11 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#0e9ec8`.

![[Dream (5-I-L-DRM) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| Damage | Psychic | 0.714 | 0.977 | `#004dff` (486 nm eq.) | source grid |
| School | Illusion | 0.625 | 0.992 | `#00c5ff` (512 nm eq.) | source grid |
| Duration | 8 hours | 0.474 | 1.000 | `#00ff66` (558 nm eq.) | source grid |
| Range | Special | 0.824 | 0.949 | `#4a00ff` (453 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.16): swatch `#4edecf`, measured lines at 0.474, 0.501, 0.626, 0.715, 0.824. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.72. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·I·Psychic`; the k4 to k6 lines (None, Special, 8 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·I·Psychic` |
| Standard spectrometer detection range | 2.30 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 1,969 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Dark, Potential, Introspection, Hopelessness and the school lean is Light, Introspection, 2x Flexibility. The working vector used by [[Recast Tension and Combination Affinity]] is `1F 2G 2h 1I` (Potential, 2x Introspection, 2x Flexibility, Hopelessness).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 87.8 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 5th Tier quantum of 19,109 Pz (2.8% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 5th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Illusion school with aspect lean Light, Introspection, 2x Flexibility. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 5 Workings]] |
| School | [[Illusion]] |
| Affinity | [[Illusion]] (I) |
| Function | [[Mind and Will]], [[Precision Strikes]] |
| Element | [[Psychic Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Phantasmal Killer (4-I-L-PK)|Phantasmal Killer]] (4) · [[Feeblemind (8-E-L-FBL)|Feeblemind]] (8) · [[Vicious Mockery (0-E-L-VM)|Vicious Mockery]] (0) · [[Awaken (5-T-H-AWK)|Awaken]] (5) · [[Dominate Person (5-E-L-DP)|Dominate Person]] (5) · [[Fear (3-I-L-FEA)|Fear]] (3) · [[Geas (5-E-M-GEA)|Geas]] (5) · [[Hold Monster (5-E-L-HML)|Hold Monster]] (5).


---

## Tactical Assessment

Covert long-distance messaging without transmitters, or degradation of an enemy commander rest.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Illusion]] · [[Spell Breakdown Procedure]] · [[Parzival]]
