---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/abjuration
  - source/srd
aliases:
  - "5th Tier Spell: Dispel Evil and Good"
  - "Dispel Evil and Good"
  - "5-A-L-DEGP"
registry_id: 5-A-L-DEGP
attribute_code: "5·Abj·None·None·Self·Up to 1 minute"
incantation: "Taporse"
tier: 5
school: Abjuration
affinity: A
grade: L
pz_total: 8247.4
pz_quantum: 19109.4
t_e: 4.16
updated: 2026-11-16
---

**Dispel Evil and Good** (`5-A-L-DEGP`) is a 5th Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **8,247 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 4.16 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Abjuration]]
        - **Dispel Evil and Good** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-A-L-DEGP` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Abj·None·None·Self·Up to 1 minute` |
| Incantation | *Taporse* |
| Affinity | A (Abjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Abjuration]] |
| Casting time | 1 action |
| Range | Self |
| Area | single point or target |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Holy water or powdered silver and iron |
| Ritual | no |
| Resistance check | presence; on success: other |
| Practitioner lineages | Cleric, Paladin |

### Mechanism

A protective shell makes extraplanar creatures and undead miss more often, and can be spent to break their hold on a person or force one back to its home plane.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| banish 1 extraplanar creature (1 plane boundary) | `0.01*80*15*1e6/J` | 8,000 |
| break enchantment | `1` | 1.0 |
| upkeep: deflection shell: 25% of 15 per round over 10 rounds | `0.20*0.25*15*10` | 7.5 |
| Pattern cost | `0.01 × Q5 × (1 + 0.25)` | 239 |

| Quantity | Value |
|---|---|
| Effect energy | 8,001 Pz |
| Upkeep energy | 7.5 Pz (0.125 Pz/s) |
| **Total draw** | **8,247 Pz** (12,371.1 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 0.432 |
| Energy-equivalent tier T_E | 4.16 |
| Handling points | 0.25 |
| Grade score | -0.17 → L |

**Handling flags:** concentration.

**Assumptions:** 80 kg banished creature; one boundary at d_eff = 1e6 m; deflection absorbs a quarter of 15 per round.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Dispel Evil and Good (5-A-L-DEGP) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Taporse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Ritaporse* · T7: *Mitaporse* · T8: *Nitaporse* · T9: *Xyitaporse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#3a76af`.

![[Dispel Evil and Good (5-A-L-DEGP) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.882 | `#ff0028` (700 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.983 | `#0074ff` (495 nm eq.) | source grid |
| Range | Self | 0.706 | 0.979 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.16): swatch `#72b5a1`, measured lines at 0.007, 0.501, 0.685, 0.706. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.92. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·A·None`; the k4 to k6 lines (None, Self, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·A·None` |
| Standard spectrometer detection range | 9.08 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 1,912 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1,375 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 5th Tier quantum of 19,109 Pz (43.2% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 5th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 5 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Negation and Counterspell]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Antilife Shell (5-A-L-ASI)|Antilife Shell]] (5) · [[Arcane Insulation (4-A-L-AI)|Arcane Insulation]] (4) · [[Banishment (4-A-M-BNS)|Banishment]] (4) · [[Forbiddance (6-A-L-FRBB)|Forbiddance]] (6) · [[Globe of Invulnerability (6-A-L-GIO)|Globe of Invulnerability]] (6) · [[Private Sanctum (4-A-L-PSI)|Private Sanctum]] (4) · [[Counterspell (3-A-L-CNT)|Counterspell]] (3) · [[Dispel Magic (3-A-L-DM)|Dispel Magic]] (3).


---

## Tactical Assessment

Counter-summoning tool for units facing extraplanar or undead forces.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
