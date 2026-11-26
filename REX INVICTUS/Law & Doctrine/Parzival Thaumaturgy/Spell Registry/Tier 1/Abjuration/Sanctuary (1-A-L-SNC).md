---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/abjuration
  - source/srd
aliases:
  - "1st Tier Spell: Sanctuary"
  - "Sanctuary"
  - "1-A-L-SNC"
registry_id: 1-A-L-SNC
attribute_code: "1·Abj·None·None·30 feet·1 minute"
incantation: "Sausine"
tier: 1
school: Abjuration
affinity: A
grade: L
pz_total: 22.9
pz_quantum: 350.0
t_e: -1.73
updated: 2026-11-16
---

**Sanctuary** (`1-A-L-SNC`) is a 1st Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **22.9 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -1.73 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Abjuration]]
        - **Sanctuary** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-A-L-SNC` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Abj·None·None·30 feet·1 minute` |
| Incantation | *Sausine* |
| Affinity | A (Abjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Abjuration]] |
| Casting time | 1 bonus action |
| Range | 30 feet |
| Area | single point or target |
| Duration | 1 minute |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A small silver mirror |
| Ritual | no |
| Practitioner lineages | Cleric |

### Mechanism

A compulsion field around one creature makes attackers break off and pick other targets unless they resist.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| attacks diverted, 50% of 15 points/round over 10 rounds | `0.20*0.5*15*10` | 15.0 |
| [upkeep] diversion compulsion on 3 attackers, 1 min | `0.005*3*60` | 0.9 |
| Pattern cost | `0.01 × Q1 × (1 + 1.00)` | 7.0 |

| Quantity | Value |
|---|---|
| Effect energy | 15.0 Pz |
| Upkeep energy | 0.9 Pz (0.015 Pz/s) |
| **Total draw** | **22.9 Pz** (34.3 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.0654 |
| Energy-equivalent tier T_E | -1.73 |
| Handling points | 1.00 |
| Grade score | 0.00 → L |

**Handling flags:** fragile.

**Assumptions:** 3 attackers; half the attacks diverted; 15 points per round.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Sanctuary (1-A-L-SNC) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | 1 minute | 1 | `0000000000011` |

### Incantation

Spoken as **Sausine** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisausine* · T3: *Lisausine* · T4: *Visausine* · T5: *Tisausine* · T6: *Risausine* · T7: *Misausine* · T8: *Nisausine* · T9: *Xyisausine*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#e36f0a`.

![[Sanctuary (1-A-L-SNC) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.995 | `#ff0028` (700 nm eq.) | source grid |
| Duration | 1 minute | 0.105 | 1.000 | `#ff6300` (668 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.981 | `#91ff00` (612 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.22): swatch `#fa562e`, measured lines at 0.006, 0.102, 0.295. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.36. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·A·None`; the k4 to k6 lines (None, 30 feet, 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·A·None` |
| Standard spectrometer detection range | 0.48 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.2 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 3.8 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (6.5% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
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

Similar workings: [[Arcane Ward (1-A-L-AW)|Arcane Ward]] (1) · [[Mage Armor (1-P-L-MA)|Mage Armor]] (1) · [[Protection from Evil and Good (1-A-L-PEG)|Protection from Evil and Good]] (1) · [[Shield (1-P-L-SHL)|Shield]] (1) · [[Shield of Faith (1-A-L-SFI)|Shield of Faith]] (1) · [[Aid (2-A-L-AID)|Aid]] (2) · [[Leadskin (2-A-L-LDS)|Leadskin]] (2) · [[Protection from Poison (2-A-L-PP)|Protection from Poison]] (2).


---

## Tactical Assessment

Protects medics, negotiators or civilians; ends if the protected person attacks.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
