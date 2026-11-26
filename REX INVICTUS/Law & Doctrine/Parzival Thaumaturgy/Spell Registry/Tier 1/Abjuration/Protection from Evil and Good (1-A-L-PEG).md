---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/abjuration
  - source/srd
aliases:
  - "1st Tier Spell: Protection from Evil and Good"
  - "Protection from Evil and Good"
  - "1-A-L-PEG"
registry_id: 1-A-L-PEG
attribute_code: "1·Abj·None·None·Touch·Up to 10 minutes"
incantation: "Salixly"
tier: 1
school: Abjuration
affinity: A
grade: L
pz_total: 15.8
pz_quantum: 350.0
t_e: -2.10
updated: 2026-11-16
---

**Protection from Evil and Good** (`1-A-L-PEG`) is a 1st Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **15.8 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -2.10 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Abjuration]]
        - **Protection from Evil and Good** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-A-L-PEG` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Abj·None·None·Touch·Up to 10 minutes` |
| Incantation | *Salixly* |
| Affinity | A (Abjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Abjuration]] |
| Casting time | 1 action |
| Range | Touch |
| Area | single point or target |
| Duration | Up to 10 minutes (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Holy water or powdered silver and iron, which the spell consumes |
| Ritual | no |
| Practitioner lineages | Cleric, Paladin, Warlock, Wizard |

### Mechanism

A consecrated field around one creature degrades attacks from extraplanar and undead beings and blocks their mental intrusion and possession.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| attacks deflected, 25% of 15 points/round over 10 rounds | `0.20*0.25*15*10` | 7.5 |
| [upkeep] mental intrusion ward, 1 creature, 10 min | `0.005*600` | 3.0 |
| Pattern cost | `0.01 × Q1 × (1 + 0.50)` | 5.2 |

| Quantity | Value |
|---|---|
| Effect energy | 7.5 Pz |
| Upkeep energy | 3.0 Pz (0.005 Pz/s) |
| **Total draw** | **15.8 Pz** (23.6 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.045 |
| Energy-equivalent tier T_E | -2.10 |
| Handling points | 0.50 |
| Grade score | -0.50 → L |

**Handling flags:** concentration, consumed material.

**Assumptions:** One 10-round engagement; attack deflection ~25% of incoming; consumed holy water carries no listed value.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Protection from Evil and Good (1-A-L-PEG) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Up to 10 minutes | 15 | `0000000011111` |

### Incantation

Spoken as **Salixly** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisalixly* · T3: *Lisalixly* · T4: *Visalixly* · T5: *Tisalixly* · T6: *Risalixly* · T7: *Misalixly* · T8: *Nisalixly* · T9: *Xyisalixly*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 2→9 3→10 4→11 | 5 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#b71a79`.

![[Protection from Evil and Good (1-A-L-PEG) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.995 | `#ff0028` (700 nm eq.) | source grid |
| Duration | Up to 10 minutes | 0.789 | 0.788 | `#1e00ff` (463 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.736 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.21): swatch `#b84963`, measured lines at 0.007, 0.101, 0.790, 0.883. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.20. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·A·None`; the k4 to k6 lines (None, Touch, Up to 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·A·None` |
| Standard spectrometer detection range | 0.40 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.6 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 2.6 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (4.5% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
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

Similar workings: [[Arcane Ward (1-A-L-AW)|Arcane Ward]] (1) · [[Mage Armor (1-P-L-MA)|Mage Armor]] (1) · [[Sanctuary (1-A-L-SNC)|Sanctuary]] (1) · [[Shield (1-P-L-SHL)|Shield]] (1) · [[Shield of Faith (1-A-L-SFI)|Shield of Faith]] (1) · [[Aid (2-A-L-AID)|Aid]] (2) · [[Leadskin (2-A-L-LDS)|Leadskin]] (2) · [[Protection from Poison (2-A-L-PP)|Protection from Poison]] (2).


---

## Tactical Assessment

Protection for a point soldier or negotiator facing extraplanar or undead forces.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
