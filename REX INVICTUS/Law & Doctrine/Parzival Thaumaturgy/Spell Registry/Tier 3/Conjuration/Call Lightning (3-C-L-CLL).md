---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/conjuration
  - source/srd
aliases:
  - "3rd Tier Spell: Call Lightning"
  - "Call Lightning"
  - "3-C-L-CLL"
registry_id: 3-C-L-CLL
attribute_code: "3·Con·Lightning·sphere (5)·120 feet·Up to 10 minutes"
incantation: "Lenin-Sumully"
tier: 3
school: Conjuration
affinity: C
grade: L
pz_total: 2097.8
pz_quantum: 2586.2
t_e: 2.79
updated: 2026-11-16
---

**Call Lightning** (`3-C-L-CLL`) is a 3rd Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **2,098 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E 2.79 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Conjuration]]
        - **Call Lightning** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-C-L-CLL` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Con·Lightning·sphere (5)·120 feet·Up to 10 minutes` |
| Incantation | *Lenin-Sumully* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | 120 feet |
| Area | sphere (5) |
| Duration | Up to 10 minutes (concentration) |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 3d10 lightning (mean 16.5) |
| Injury by tier | T3: 3d10, T4: 4d10, T5: 5d10, T6: 6d10, T7: 7d10, T8: 8d10, T9: 9d10 |
| Practitioner lineages | Druid |

### Mechanism

A storm cell forms 30 m above the caster and discharges bolts at chosen points within range.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| storm cloud condensate | `3202 m^3 * 0.5 g/m^3 * 1 Pz/kg` | 1.6 |
| lightning strikes | `16.5 HP * 0.3 Pz/HP (lightning) * (sphere 5 ft: 4*pi*1.524^2 = 29.186 m^2 / 0.7 m^2) * 10 triggers` | 2,064 |
| Pattern cost | `0.01 × Q3 × (1 + 0.25)` | 32.3 |

| Quantity | Value |
|---|---|
| Effect energy | 2,065 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **2,098 Pz** (3,146.7 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 0.811 |
| Energy-equivalent tier T_E | 2.79 |
| Handling points | 0.25 |
| Grade score | 0.15 → L |

**Handling flags:** concentration.

**Assumptions:** 10 strikes over the engagement minute; cloud water 0.5 g/m^3.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Call Lightning (3-C-L-CLL) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | Lightning | 5 | `0000000001011` |
| k4 Area | sphere (5) | 34 | `0000001000101` |
| k5 Range | 120 feet | 3 | `0000000000111` |
| k6 Duration | Up to 10 minutes | 15 | `0000000011111` |

### Incantation

Spoken as **Lenin-Sumully** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vilenin-Sumully* · T5: *Tilenin-Sumully* · T6: *Rilenin-Sumully* · T7: *Milenin-Sumully* · T8: *Nilenin-Sumully* · T9: *Xyilenin-Sumully*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 3→0 | 3 |
| k4 Area | 0→9 2→11 6→2 | 3 |
| k5 Range | 0→8 1→9 2→10 | 3 |
| k6 Duration | 0→7 1→8 2→9 3→10 4→11 | 5 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#999352`.

![[Call Lightning (3-C-L-CLL) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| Damage | Lightning | 0.429 | 0.992 | `#00ff25` (571 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.985 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Up to 10 minutes | 0.789 | 0.887 | `#1e00ff` (463 nm eq.) | source grid |
| Area | sphere (5) | 0.944 | 0.812 | `#f200ff` (417 nm eq.) | source grid |
| Range | 120 feet | 0.176 | 0.992 | `#ffc900` (647 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.14): swatch `#c79d77`, measured lines at 0.126, 0.177, 0.300, 0.429, 0.790, 0.945. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.32. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·C·Lightning`; the k4 to k6 lines (sphere (5), 120 feet, Up to 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·C·Lightning` |
| Standard spectrometer detection range | 4.58 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 259 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is 2x Heat, Light, Movement and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 2b 1c 1e 1F 2j` (Beyond, 2x Heat, Light, Prodigious, Potential, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 350 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 3rd Tier quantum of 2,586 Pz (81.1% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Light and Radiance]], [[Area Destruction]] |
| Element | [[Lightning Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Lightning Bolt (3-V-L-LB)|Lightning Bolt]] (3) · [[Moonbeam (2-V-M-MNB)|Moonbeam]] (2) · [[Voltaic Arc (5-V-L-VA)|Voltaic Arc]] (5) · [[Black Tentacles (4-C-L-BT)|Black Tentacles]] (4) · [[Chain Lightning (6-V-L-CLA)|Chain Lightning]] (6) · [[Guardian of Faith (4-C-L-GFA)|Guardian of Faith]] (4) · [[Sunbeam (6-V-L-SNB)|Sunbeam]] (6) · [[Cloudkill (5-C-L-CLD)|Cloudkill]] (5).


---

## Tactical Assessment

Repeatable indirect fire against light vehicles and grouped infantry; existing storms can be harnessed.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
