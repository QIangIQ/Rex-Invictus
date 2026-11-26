---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/abjuration
  - source/srd
aliases:
  - "4th Tier Spell: Banishment"
  - "Banishment"
  - "4-A-M-BNS"
registry_id: 4-A-M-BNS
attribute_code: "4·Abj·None·None·60 feet·Up to 1 minute"
incantation: "Vawynse"
tier: 4
school: Abjuration
affinity: A
grade: M
pz_total: 16105.7
pz_quantum: 7029.9
t_e: 4.83
updated: 2026-11-16
---

**Banishment** (`4-A-M-BNS`) is a 4th Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **16,106 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E 4.83 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Abjuration]]
        - **Banishment** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-A-M-BNS` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Abj·None·None·60 feet·Up to 1 minute` |
| Incantation | *Vawynse* |
| Affinity | A (Abjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Abjuration]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | single point or target |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: An item distasteful to the target |
| Ritual | no |
| Resistance check | presence; on success: no effect |
| Practitioner lineages | Cleric, Paladin, Sorcerer, Warlock, Wizard |

### Mechanism

One creature is pushed across a plane boundary, into a holding pocket if native, or back to its home plane if foreign.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| transfer out | `0.01 * 80 kg * 15 m/s^2 * 1e+06 m / 1500 * 1` | 8,000 |
| return transfer | `0.01 * 80 kg * 15 m/s^2 * 1e+06 m / 1500 * 1` | 8,000 |
| demiplane holding | `0.005 Pz/s * 1 creature(s) * 60 s` | 0.3 |
| Pattern cost | `0.01 × Q4 × (1 + 0.50)` | 105 |

| Quantity | Value |
|---|---|
| Effect energy | 16,000 Pz |
| Upkeep energy | 0.3 Pz (0.005 Pz/s) |
| **Total draw** | **16,106 Pz** (24,158.6 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 2.29 |
| Energy-equivalent tier T_E | 4.83 |
| Handling points | 0.50 |
| Grade score | 0.91 → M |

**Handling flags:** concentration, save or suck.

**Assumptions:** Medium target 80 kg; one boundary each way; 1 min hold.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Banishment (4-A-M-BNS) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 4 | 4 | `0000000001001` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Vawynse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T5: *Tivawynse* · T6: *Rivawynse* · T7: *Mivawynse* · T8: *Nivawynse* · T9: *Xyivawynse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 3→2 | 2 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#3c9e89`.

![[Banishment (4-A-M-BNS) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.923 | `#ff0028` (700 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.960 | `#0074ff` (495 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.982 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.13): swatch `#94b78e`, measured lines at 0.007, 0.401, 0.589, 0.685. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.21. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·A·None`; the k4 to k6 lines (None, 60 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·A·None` |
| Standard spectrometer detection range | 12.69 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 703 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 2,684 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 2.29 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 4th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 4th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 4 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Teleportation and Planar Travel]], [[Negation and Counterspell]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Secret Chest (4-C-M-SCC)|Secret Chest]] (4) · [[Arcane Insulation (4-A-L-AI)|Arcane Insulation]] (4) · [[Private Sanctum (4-A-L-PSI)|Private Sanctum]] (4) · [[Antilife Shell (5-A-L-ASI)|Antilife Shell]] (5) · [[Counterspell (3-A-L-CNT)|Counterspell]] (3) · [[Dispel Evil and Good (5-A-L-DEGP)|Dispel Evil and Good]] (5) · [[Dispel Magic (3-A-L-DM)|Dispel Magic]] (3) · [[Magic Circle (3-A-L-MC)|Magic Circle]] (3).


---

## Tactical Assessment

Removes a key enemy or extraplanar asset from the fight, permanently in the case of summoned outsiders.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
