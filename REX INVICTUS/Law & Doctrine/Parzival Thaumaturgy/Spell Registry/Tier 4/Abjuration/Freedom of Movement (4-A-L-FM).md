---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/abjuration
  - source/srd
aliases:
  - "4th Tier Spell: Freedom of Movement"
  - "Freedom of Movement"
  - "4-A-L-FM"
registry_id: 4-A-L-FM
attribute_code: "4·Abj·None·None·Touch·1 hour"
incantation: "Valixa"
tier: 4
school: Abjuration
affinity: A
grade: L
pz_total: 374.8
pz_quantum: 7029.9
t_e: 1.07
updated: 2026-11-16
---

**Freedom of Movement** (`4-A-L-FM`) is a 4th Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **375 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E 1.07 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Abjuration]]
        - **Freedom of Movement** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-A-L-FM` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Abj·None·None·Touch·1 hour` |
| Incantation | *Valixa* |
| Affinity | A (Abjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Abjuration]] |
| Casting time | 1 action |
| Range | Touch |
| Area | single point or target |
| Duration | 1 hour |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A leather strap, bound around the arm or a similar appendage |
| Ritual | no |
| Practitioner lineages | Bard, Cleric, Druid, Ranger |

### Mechanism

Cancels drag and binding forces on a touched creature, letting it move normally through water and rough ground and slip physical and field-based restraints.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| restraint escapes | `3 * 1000 N * 1.5 m / 1500` | 3.0 |
| drag and terrain assist (10% duty) | `0.1 * (0.5*1000*1.0*0.7*1.5^2 N * 1.5 m/s)/1500 = 0.07875 Pz/s * 3600 s` | 284 |
| paralysis and binding immunity | `0.005 Pz/s = 0.005 Pz/s * 3600 s` | 18.0 |
| Pattern cost | `0.01 × Q4 × (1 + 0.00)` | 70.3 |

| Quantity | Value |
|---|---|
| Effect energy | 3.0 Pz |
| Upkeep energy | 302 Pz (0.0838 Pz/s) |
| **Total draw** | **375 Pz** (562.2 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 0.0533 |
| Energy-equivalent tier T_E | 1.07 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Water drag at 1.5 m/s on 0.7 m^2 for 10% of the hour; 3 escapes of 1 kN over 1.5 m; anti-binding at enchantment rate.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Freedom of Movement (4-A-L-FM) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 4 | 4 | `0000000001001` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | 1 hour | 0 | `0000000000001` |

### Incantation

Spoken as **Valixa** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T5: *Tivalixa* · T6: *Rivalixa* · T7: *Mivalixa* · T8: *Nivalixa* · T9: *Xyivalixa*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 3→2 | 2 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 | 1 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#a34a46`.

![[Freedom of Movement (4-A-L-FM) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.923 | `#ff0028` (700 nm eq.) | source grid |
| Duration | 1 hour | 0.053 | 0.941 | `#ff1c00` (684 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.890 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.17): swatch `#bc7670`, measured lines at 0.007, 0.053, 0.401, 0.883. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.57. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·A·None`; the k4 to k6 lines (None, Touch, 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·A·None` |
| Standard spectrometer detection range | 1.94 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 763 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 62.5 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 4th Tier quantum of 7,030 Pz (5.3% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 4th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 4 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Movement and Flight]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Freefall (4-T-L-FRF)|Freefall]] (4) · [[Fly (3-T-L-FLY)|Fly]] (3) · [[Gaseous Form (3-T-M-GF)|Gaseous Form]] (3) · [[Haste (3-T-L-HST)|Haste]] (3) · [[Phantom Steed (3-I-H-PSA)|Phantom Steed]] (3) · [[Slow (3-T-L-SLW)|Slow]] (3) · [[Telekinesis (5-P-L-TLK)|Telekinesis]] (5) · [[Water Breathing (3-T-L-WBT)|Water Breathing]] (3).


---

## Tactical Assessment

Counters nets, grapples, entanglement munitions and paralytic workings; ideal for combat divers and boarding parties.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
