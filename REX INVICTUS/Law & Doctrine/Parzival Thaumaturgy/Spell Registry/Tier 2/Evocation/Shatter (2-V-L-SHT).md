---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/evocation
  - source/srd
aliases:
  - "2nd Tier Spell: Shatter"
  - "Shatter"
  - "2-V-L-SHT"
registry_id: 2-V-L-SHT
attribute_code: "2·Evo·Thunder·sphere (10)·60 feet·Instantaneous"
incantation: "Huder-Sewyn"
tier: 2
school: Evocation
affinity: V
grade: L
pz_total: 1360.4
pz_quantum: 951.4
t_e: 2.36
updated: 2026-11-16
---

**Shatter** (`2-V-L-SHT`) is a 2nd Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **1,360 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E 2.36 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Evocation]]
        - **Shatter** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-V-L-SHT` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Evo·Thunder·sphere (10)·60 feet·Instantaneous` |
| Incantation | *Huder-Sewyn* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | sphere (10) |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A burst of mica |
| Ritual | no |
| Injury | 3d8 thunder (mean 13.5) |
| Injury by tier | T2: 3d8, T3: 4d8, T4: 5d8, T5: 6d8, T6: 7d8, T7: 8d8, T8: 9d8, T9: 10d8 |
| Resistance check | constitution; on success: half injury |
| Practitioner lineages | Bard, Sorcerer, Warlock, Wizard |

### Mechanism

An intense acoustic burst resonates in a small sphere and harms bodies and loose objects, especially rigid inorganic ones.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| 3d8 thunder (13.5), sphere r 10 ft | `13.5*0.60*(4*pi*(10*ft)**2)/Ac` | 1,351 |
| Pattern cost | `0.01 × Q2 × (1 + 0.00)` | 9.5 |

| Quantity | Value |
|---|---|
| Effect energy | 1,351 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **1,360 Pz** (2,040.6 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 1.43 |
| Energy-equivalent tier T_E | 2.36 |
| Handling points | 0.00 |
| Grade score | 0.18 → L |

**Handling flags:** none.

**Assumptions:** Full damage; edge surface of 10 ft radius sphere.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Shatter (2-V-L-SHT) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Thunder | 13 | `0000000011011` |
| k4 Area | sphere (10) | 27 | `0000000110111` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Huder-Sewyn** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihuder-Sewyn* · T4: *Vihuder-Sewyn* · T5: *Tihuder-Sewyn* · T6: *Rihuder-Sewyn* · T7: *Mihuder-Sewyn* · T8: *Nihuder-Sewyn* · T9: *Xyihuder-Sewyn*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 3→0 4→1 | 4 |
| k4 Area | 0→9 1→10 2→11 4→0 5→1 | 5 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#7a8595`.

![[Shatter (2-V-L-SHT) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| Damage | Thunder | 0.929 | 0.767 | `#dc00ff` (421 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.956 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.980 | `#ff0028` (700 nm eq.) | source grid |
| Area | sphere (10) | 0.750 | 0.860 | `#0017ff` (475 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.927 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.22): swatch `#97ac9d`, measured lines at 0.004, 0.201, 0.501, 0.589, 0.751, 0.929. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.13. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·V·Thunder`; the k4 to k6 lines (sphere (10), 60 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·V·Thunder` |
| Standard spectrometer detection range | 3.69 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 95.1 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is 2x Heat, Dark, Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `3b 1C 2f 2j` (3x Heat, Dark, 2x Energy, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 227 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 1.43 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 2nd Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Area Destruction]] |
| Element | [[Thunder and Concussion Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Blast (1-V-L-BLS)|Blast]] (1) · [[Thunderwave (1-V-L-THN)|Thunderwave]] (1) · [[Bohr's Model (2-P-L-BSM)|Bohr's Model]] (2) · [[Galaxy Whirl (2-V-L-GWL)|Galaxy Whirl]] (2) · [[Geyser (2-V-L-GYS)|Geyser]] (2) · [[Moonbeam (2-V-M-MNB)|Moonbeam]] (2) · [[Burning Hands (1-V-L-BH)|Burning Hands]] (1) · [[Fireball (3-V-M-FRB)|Fireball]] (3).


---

## Tactical Assessment

Breaks windows, vehicle glass and constructs.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
