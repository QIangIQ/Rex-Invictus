---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-9
  - spell/abjuration
  - source/srd
aliases:
  - "9th Tier Spell: Prismatic Wall"
  - "Prismatic Wall"
  - "9-A-L-PW"
registry_id: 9-A-L-PW
attribute_code: "9·Abj·None·line (90)·60 feet·10 minutes"
incantation: "Xya’-Léwyns"
tier: 9
school: Abjuration
affinity: A
grade: L
pz_total: 91455.8
pz_quantum: 1043335.3
t_e: 6.57
updated: 2026-11-16
---

**Prismatic Wall** (`9-A-L-PW`) is a 9th Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **91,456 Pz** against a slot quantum of 1.04 MPz Pz, which puts its energy-equivalent tier at T_E 6.57 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 9 Workings]]
      - [[Abjuration]]
        - **Prismatic Wall** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `9-A-L-PW` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `9·Abj·None·line (90)·60 feet·10 minutes` |
| Incantation | *Xya’-Léwyns* |
| Affinity | A (Abjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 9th Tier |
| School | [[Abjuration]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | line (90) |
| Duration | 10 minutes |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Wizard |

### Mechanism

A seven-layer field sheet, each layer tuned to one effect band, stands for ten minutes and blocks projectiles, energy and workings. The layers must be stripped in order by specific counter-energies.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| stored damage potential of 5 layers, 10d6 each, 90x30 ft line face | `35*(0.70+0.25+0.30+0.05+0.90)*(2*(90*ft)*(30*ft))/Ac` | 55,184 |
| violet layer plane ejection, 3 crossers | `3*0.01*80*15*1e6/1500` | 24,000 |
| indigo layer petrification, 3 crossers, 80 kg at 3 Pz/kg | `3*3*80` | 720 |
| barrier absorption of incoming fire, 10 rounds at 50 points | `0.20*50*10` | 100 |
| [upkeep] light output, bright 100 ft (2500 W), 10 min | `2500*600/1500` | 1,000 |
| [upkeep] blinding aura, 6 creatures, 10 min | `0.005*6*600` | 18.0 |
| Pattern cost | `0.01 × Q9 × (1 + 0.00)` | 10,433 |

| Quantity | Value |
|---|---|
| Effect energy | 80,004 Pz |
| Upkeep energy | 1,018 Pz (1.7 Pz/s) |
| **Total draw** | **91,456 Pz** (137,183.6 kJ) |
| Slot quantum Q9 | 1.04 MPz Pz |
| Field gain (draw / quantum) | 0.0877 |
| Energy-equivalent tier T_E | 6.57 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Wall form 90x30 ft; layer potential at full damage with line S=2*l*h; 3 attempted crossings; 50 points per round of incoming fire for 10 rounds; light scaled from 100 W per 20 ft radius.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Prismatic Wall (9-A-L-PW) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 9 | 9 | `0000000010011` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | line (90) | 26 | `0000000110101` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | 10 minutes | 4 | `0000000001001` |

### Incantation

Spoken as **Xya’-Léwyns** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 4→3 | 3 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 2→11 4→0 5→1 | 4 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 3→10 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#7274af`.

![[Prismatic Wall (9-A-L-PW) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 9 | 0.900 | 1.000 | `#b600ff` (430 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.667 | `#ff0028` (700 nm eq.) | source grid |
| Duration | 10 minutes | 0.263 | 0.816 | `#bdff00` (621 nm eq.) | source grid |
| Area | line (90) | 0.722 | 0.984 | `#0043ff` (483 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.953 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.21): swatch `#7e81b1`, measured lines at 0.006, 0.264, 0.589, 0.723, 0.901. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.96. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `9·A·None`; the k4 to k6 lines (line (90), 60 feet, 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `9·A·None` |
| Standard spectrometer detection range | 30.24 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 52,167 Pz (0.05 × Q9) |
| Counter drawn cold (all six layers) | 104,334 Pz (0.10 × Q9) |
| Unravel after completion | 104,537 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 15,243 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 9th Tier quantum of 1.04 MPz Pz (8.8% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 9th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 9 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Walls and Barriers]], [[Light and Radiance]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Sunburst (8-V-L-SNBB)|Sunburst]] (8) · [[Forcecage (7-P-L-FRC)|Forcecage]] (7) · [[Imprisonment (9-A-L-IMP)|Imprisonment]] (9) · [[Prismatic Spray (7-V-L-PSM)|Prismatic Spray]] (7) · [[Starburst (9-A-L-STR)|Starburst]] (9) · [[Antimagic Field (8-A-L-AFT)|Antimagic Field]] (8) · [[Blade Barrier (6-V-L-BB)|Blade Barrier]] (6) · [[Chain Lightning (6-V-L-CLA)|Chain Lightning]] (6).


---

## Tactical Assessment

An almost impassable strategic barrier for holding a gate or covering a withdrawal; the outer glare blinds observers near the wall.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 9 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
