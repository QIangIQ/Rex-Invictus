---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-6
  - spell/transmutation
  - source/srd
aliases:
  - "6th Tier Spell: Disintegrate"
  - "Disintegrate"
  - "6-P-L-DSN"
registry_id: 6-P-L-DSN
attribute_code: "6·Tra·Force·cube (10)·60 feet·Instantaneous"
incantation: "Rieton-Bewyn"
tier: 6
school: Transmutation
affinity: P
grade: L
pz_total: 19734.4
pz_quantum: 51944.6
t_e: 5.03
updated: 2026-11-16
---

**Disintegrate** (`6-P-L-DSN`) is a 6th Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **19,734 Pz** against a slot quantum of 51,945 Pz, which puts its energy-equivalent tier at T_E 5.03 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 6 Workings]]
      - [[Transmutation]]
        - **Disintegrate** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `6-P-L-DSN` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `6·Tra·Force·cube (10)·60 feet·Instantaneous` |
| Incantation | *Rieton-Bewyn* |
| Affinity | P (Pure field construct) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 6th Tier |
| School | [[Transmutation]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | cube (10) |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A lodestone and a pinch of dust |
| Ritual | no |
| Injury | 10d6 + 40 force (mean 75) |
| Injury by tier | T6: 10d6 + 40 |
| Resistance check | agility; on success: no effect |
| Practitioner lineages | Sorcerer, Wizard |

### Mechanism

A thin ray delivers a heavy force load and, if the target fails, reduces it with its gear to fine dust. It also removes a Large object or a 10 ft section of a larger one or of a force construct.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| 10d6+40 = 75 force, ray | `75*0.40*0.5` | 15.0 |
| reduce 80 kg target to fine dust (comminution ~100 kWh/t) | `80*3.6e5/J` | 19,200 |
| Pattern cost | `0.01 × Q6 × (1 + 0.00)` | 519 |

| Quantity | Value |
|---|---|
| Effect energy | 19,215 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **19,734 Pz** (29,601.7 kJ) |
| Slot quantum Q6 | 51,945 Pz |
| Field gain (draw / quantum) | 0.38 |
| Energy-equivalent tier T_E | 5.03 |
| Handling points | 0.00 |
| Grade score | -0.48 → L |

**Handling flags:** none.

**Assumptions:** Comminution term applies when the target collapses; 3.6e5 J/kg for grinding to powder.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Disintegrate (6-P-L-DSN) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 6 | 6 | `0000000001101` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | Force | 4 | `0000000001001` |
| k4 Area | cube (10) | 5 | `0000000001011` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Rieton-Bewyn** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T7: *Mirieton-Bewyn* · T8: *Nirieton-Bewyn* · T9: *Xyirieton-Bewyn*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 3→2 | 3 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 3→0 | 2 |
| k4 Area | 0→9 1→10 3→12 | 3 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#71988b`.

![[Disintegrate (6-P-L-DSN) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 6 | 0.600 | 1.000 | `#00ebff` (520 nm eq.) | source grid |
| Damage | Force | 0.357 | 0.971 | `#3bff00` (593 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.963 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.835 | `#ff0028` (700 nm eq.) | source grid |
| Area | cube (10) | 0.139 | 0.899 | `#ff9300` (658 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 1.000 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.16): swatch `#75acb9`, measured lines at 0.004, 0.140, 0.358, 0.596, 0.876. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.30. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `6·T·Force`; the k4 to k6 lines (cube (10), 60 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `6·T·Force` |
| Standard spectrometer detection range | 14.05 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 2,597 Pz (0.05 × Q6) |
| Counter drawn cold (all six layers) | 5,194 Pz (0.10 × Q6) |
| Unravel after completion | 5,194 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Beyond, Introspection, 2x Movement and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1d 1G 2h 3j` (Beyond, Life, Introspection, 2x Flexibility, 3x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 3,289 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 6th Tier quantum of 51,945 Pz (38.0% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 6th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 6 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Pure]] (P) |
| Function | [[Necromantic and Soul Workings]], [[Area Destruction]] |
| Element | [[Force Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Circle of Death (6-N-L-CD)|Circle of Death]] (6) · [[Planetary Rings (4-P-L-PR)|Planetary Rings]] (4) · [[Sonic Boom (3-P-L-SBN)|Sonic Boom]] (3) · [[Thermonuclear Fireball (9-P-L-TFE)|Thermonuclear Fireball]] (9) · [[Turbulent Gas (3-P-L-TG)|Turbulent Gas]] (3) · [[Wormhole (9-P-L-WRM)|Wormhole]] (9) · [[Absolute Zero (6-V-L-AZ)|Absolute Zero]] (6) · [[Blade Barrier (6-V-L-BB)|Blade Barrier]] (6).


---

## Tactical Assessment

Breaching walls, hulls and force barriers, and permanent elimination of a single target.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 6 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
