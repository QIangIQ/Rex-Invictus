---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-9
  - spell/conjuration
  - source/srd
aliases:
  - "9th Tier Spell: Storm of Vengeance"
  - "Storm of Vengeance"
  - "9-C-M-SV"
registry_id: 9-C-M-SV
attribute_code: "9·Con·Thunder·sphere (360)·Sight·Up to 1 minute"
incantation: "Xyeder-Saitorse"
tier: 9
school: Conjuration
affinity: C
grade: M
pz_total: 1682078.4
pz_quantum: 1043335.3
t_e: 9.48
updated: 2026-11-16
---

**Storm of Vengeance** (`9-C-M-SV`) is a 9th Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **1.68 MPz Pz** against a slot quantum of 1.04 MPz Pz, which puts its energy-equivalent tier at T_E 9.48 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 9 Workings]]
      - [[Conjuration]]
        - **Storm of Vengeance** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `9-C-M-SV` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `9·Con·Thunder·sphere (360)·Sight·Up to 1 minute` |
| Incantation | *Xyeder-Saitorse* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 9th Tier |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | Sight |
| Area | sphere (360) |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 2d6 thunder (mean 7) |
| Injury by tier | T9: 2d6 |
| Resistance check | constitution; on success: no effect |
| Practitioner lineages | Druid |

### Mechanism

A storm cell 110 m in radius forms overhead and runs a fixed sequence over ten rounds: concussive thunder, acid rain, six directed lightning discharges, hail, then gusting freezing rain.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Round 1 thunder | `7 HP * 0.60 * 39927 m^2 / 0.7` | 239,600 |
| Round 2 acid rain | `3.5 HP * 0.25 * 39927 / 0.7` | 49,910 |
| Round 3 six lightning bolts | `35 HP * 0.30 * 0.5 * 6` | 31.5 |
| Round 4 hail | `7 HP * 0.46 * 39927 / 0.7` | 183,700 |
| Rounds 5-10 freezing rain | `3.5 HP * 0.90 * 39927 / 0.7 * 6` | 1.08 MPz |
| Conjured rain water | `1 Pz/kg * 2 mm * 37826 m^2 * 1000 kg/m^3` | 75,650 |
| Upkeep: Wind field in 10 m layer | `0.5 * 453906 kg * (15.6 m/s)^2 / 1500` | 36,820 |
| Pattern cost | `0.01 × Q9 × (1 + 0.75)` | 18,258 |

| Quantity | Value |
|---|---|
| Effect energy | 1.63 MPz Pz |
| Upkeep energy | 36,820 Pz (682 Pz/s) |
| **Total draw** | **1.68 MPz Pz** (2,523,117.6 kJ) |
| Slot quantum Q9 | 1.04 MPz Pz |
| Field gain (draw / quantum) | 1.61 |
| Energy-equivalent tier T_E | 9.48 |
| Handling points | 0.75 |
| Grade score | 0.99 → M |

**Handling flags:** concentration, multi target control.

**Assumptions:** Exposure cylinder r=360 ft with a 10 ft ground layer; 2 mm of rain; mean wind 15.6 m/s in a 10 m air layer refreshed once.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Storm of Vengeance (9-C-M-SV) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 9 | 9 | `0000000010011` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | Thunder | 13 | `0000000011011` |
| k4 Area | sphere (360) | 32 | `0000001000001` |
| k5 Range | Sight | 13 | `0000000011011` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Xyeder-Saitorse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 4→3 | 3 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 3→0 4→1 | 4 |
| k4 Area | 0→9 6→2 | 2 |
| k5 Range | 0→8 1→9 3→11 4→12 | 4 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#8426dd`.

![[Storm of Vengeance (9-C-M-SV) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 9 | 0.900 | 1.000 | `#b600ff` (430 nm eq.) | source grid |
| Damage | Thunder | 0.929 | 1.000 | `#dc00ff` (421 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.741 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.977 | `#0074ff` (495 nm eq.) | source grid |
| Area | sphere (360) | 0.889 | 1.000 | `#a600ff` (433 nm eq.) | source grid |
| Range | Sight | 0.765 | 0.991 | `#0007ff` (471 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.23): swatch `#676dca`, measured lines at 0.126, 0.685, 0.765, 0.898, 0.929. One or more predicted lines have no measured counterpart; the plate may merge overlapping lines.

Relative luminosity scales with initial energy: log10(E) = 6.23. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `9·C·Thunder`; the k4 to k6 lines (sphere (360), Sight, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `9·C·Thunder` |
| Standard spectrometer detection range | 129.69 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 52,167 Pz (0.05 × Q9) |
| Counter drawn cold (all six layers) | 104,334 Pz (0.10 × Q9) |
| Unravel after completion | 111,698 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is 2x Heat, Dark, Movement and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 2b 1C 1e 1F 2j` (Beyond, 2x Heat, Dark, Prodigious, Potential, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 280,346 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 1.61 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 9th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 9th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 9 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Area Destruction]] |
| Element | [[Thunder and Concussion Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Wormhole (9-P-L-WRM)|Wormhole]] (9) · [[Incendiary Cloud (8-C-M-IC)|Incendiary Cloud]] (8) · [[Supermassive Black Hole (10-C-X-SBH)|Supermassive Black Hole]] (10) · [[Eruption (9-V-M-ERP)|Eruption]] (9) · [[Meteor Swarm (9-V-L-MST)|Meteor Swarm]] (9) · [[Starburst (9-A-L-STR)|Starburst]] (9) · [[Thermonuclear Fireball (9-P-L-TFE)|Thermonuclear Fireball]] (9) · [[Sunburst (8-V-L-SNBB)|Sunburst]] (8).


---

## Tactical Assessment

A theatre-scale denial weapon that strips infantry, grounds small aircraft and blinds ranged fire across an entire position for a minute.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 9 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
