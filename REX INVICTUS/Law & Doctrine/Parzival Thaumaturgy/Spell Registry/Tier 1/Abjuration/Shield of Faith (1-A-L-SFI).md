---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/abjuration
  - source/srd
aliases:
  - "1st Tier Spell: Shield of Faith"
  - "Shield of Faith"
  - "1-A-L-SFI"
registry_id: 1-A-L-SFI
attribute_code: "1·Abj·None·None·60 feet·Up to 10 minutes"
incantation: "Sawynly"
tier: 1
school: Abjuration
affinity: A
grade: L
pz_total: 7.4
pz_quantum: 350.0
t_e: -2.86
updated: 2026-11-16
---

**Shield of Faith** (`1-A-L-SFI`) is a 1st Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **7.4 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -2.86 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Abjuration]]
        - **Shield of Faith** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-A-L-SFI` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Abj·None·None·60 feet·Up to 10 minutes` |
| Incantation | *Sawynly* |
| Affinity | A (Abjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Abjuration]] |
| Casting time | 1 bonus action |
| Range | 60 feet |
| Area | single point or target |
| Duration | Up to 10 minutes (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A small parchment with a bit of holy text written on it |
| Ritual | no |
| Practitioner lineages | Cleric, Paladin |

### Mechanism

A thin deflection field around one creature lowers the chance of hits.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| +2 defence, 10% of 15 points/round over 10 rounds | `0.20*0.10*15*10` | 3.0 |
| Pattern cost | `0.01 × Q1 × (1 + 0.25)` | 4.4 |

| Quantity | Value |
|---|---|
| Effect energy | 3.0 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **7.4 Pz** (11.1 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.0211 |
| Energy-equivalent tier T_E | -2.86 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** concentration.

**Assumptions:** One 10-round engagement in the ten minutes.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Shield of Faith (1-A-L-SFI) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Up to 10 minutes | 15 | `0000000011111` |

### Incantation

Spoken as **Sawynly** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisawynly* · T3: *Lisawynly* · T4: *Visawynly* · T5: *Tisawynly* · T6: *Risawynly* · T7: *Misawynly* · T8: *Nisawynly* · T9: *Xyisawynly*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 2→9 3→10 4→11 | 5 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#91567f`.

![[Shield of Faith (1-A-L-SFI) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.995 | `#ff0028` (700 nm eq.) | source grid |
| Duration | Up to 10 minutes | 0.789 | 0.788 | `#1e00ff` (463 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.888 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.22): swatch `#b7685f`, measured lines at 0.007, 0.101, 0.589, 0.790. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 0.87. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·A·None`; the k4 to k6 lines (None, 60 feet, Up to 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·A·None` |
| Standard spectrometer detection range | 0.27 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.0 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1.2 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (2.1% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Wards and Shields]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Arcane Ward (1-A-L-AW)|Arcane Ward]] (1) · [[Mage Armor (1-P-L-MA)|Mage Armor]] (1) · [[Protection from Evil and Good (1-A-L-PEG)|Protection from Evil and Good]] (1) · [[Sanctuary (1-A-L-SNC)|Sanctuary]] (1) · [[Shield (1-P-L-SHL)|Shield]] (1) · [[Aid (2-A-L-AID)|Aid]] (2) · [[Leadskin (2-A-L-LDS)|Leadskin]] (2) · [[Protection from Poison (2-A-L-PP)|Protection from Poison]] (2).


---

## Tactical Assessment

A cheap persistent protection for a frontline trooper.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
