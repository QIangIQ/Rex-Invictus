---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/conjuration
  - source/srd
aliases:
  - "4th Tier Spell: Black Tentacles"
  - "Black Tentacles"
  - "4-C-L-BT"
registry_id: 4-C-L-BT
attribute_code: "4·Con·Bludgeoning·cube (20)·90 feet·Up to 1 minute"
incantation: "Vedeg-Boylarse"
tier: 4
school: Conjuration
affinity: C
grade: L
pz_total: 5709.7
pz_quantum: 7029.9
t_e: 3.79
updated: 2026-11-16
---

**Black Tentacles** (`4-C-L-BT`) is a 4th Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **5,710 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E 3.79 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Conjuration]]
        - **Black Tentacles** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-C-L-BT` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Con·Bludgeoning·cube (20)·90 feet·Up to 1 minute` |
| Incantation | *Vedeg-Boylarse* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | 90 feet |
| Area | cube (20) |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A piece of tentacle from a giant octopus or a giant squid |
| Ritual | no |
| Injury | 3d6 bludgeoning (mean 10.5) |
| Injury by tier | T4: 3d6 |
| Resistance check | agility; on success: no effect |
| Practitioner lineages | Wizard |

### Mechanism

Semi-living tentacles sprout across a 6 m square, crushing and pinning anyone in or entering it.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| tentacle crushing | `10.5 HP * 0.46 Pz/HP (bludgeoning) * (cube 20 ft: 4*pi*(0.62*6.096)^2 = 179.508 m^2 / 0.7 m^2) * 3 triggers` | 3,716 |
| conjured tentacle mass | `37.16 m^2 * 5 kg/m^2 * 10 Pz/kg` | 1,858 |
| animation upkeep | `16 squares * 0.05 Pz/s * 60 s` | 48.0 |
| Pattern cost | `0.01 × Q4 × (1 + 0.25)` | 87.9 |

| Quantity | Value |
|---|---|
| Effect energy | 5,574 Pz |
| Upkeep energy | 48.0 Pz (0.8 Pz/s) |
| **Total draw** | **5,710 Pz** (8,564.5 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 0.812 |
| Energy-equivalent tier T_E | 3.79 |
| Handling points | 0.25 |
| Grade score | 0.15 → L |

**Handling flags:** concentration.

**Assumptions:** 3 triggers per creature; tentacle mass 5 kg/m^2; 16 animated 1.5 m cells for 1 min.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Black Tentacles (4-C-L-BT) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 4 | 4 | `0000000001001` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | Bludgeoning | 1 | `0000000000011` |
| k4 Area | cube (20) | 9 | `0000000010011` |
| k5 Range | 90 feet | 11 | `0000000010111` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Vedeg-Boylarse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T5: *Tivedeg-Boylarse* · T6: *Rivedeg-Boylarse* · T7: *Mivedeg-Boylarse* · T8: *Nivedeg-Boylarse* · T9: *Xyivedeg-Boylarse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 3→2 | 2 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 | 2 |
| k4 Area | 0→9 1→10 4→0 | 3 |
| k5 Range | 0→8 1→9 2→10 4→12 | 4 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#76b454`.

![[Black Tentacles (4-C-L-BT) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| Damage | Bludgeoning | 0.143 | 0.967 | `#ff9900` (657 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.963 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.960 | `#0074ff` (495 nm eq.) | source grid |
| Area | cube (20) | 0.250 | 0.989 | `#cdff00` (625 nm eq.) | source grid |
| Range | 90 feet | 0.647 | 0.970 | `#00aaff` (506 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.13): swatch `#b6aa79`, measured lines at 0.125, 0.144, 0.251, 0.401, 0.648, 0.685. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.76. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·C·Bludgeoning`; the k4 to k6 lines (cube (20), 90 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·C·Bludgeoning` |
| Standard spectrometer detection range | 7.56 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 713 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Within, Rigidity, 2x Movement and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1e 1F 1H 3j` (Prodigious, Potential, Rigidity, 3x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 952 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 4th Tier quantum of 7,030 Pz (81.2% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 4th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 4 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Area Destruction]] |
| Element | [[Bludgeoning Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Supersonic Omnidirectional Jet (5-C-M-SOJ)|Supersonic Omnidirectional Jet]] (5) · [[Control Water (4-T-H-CWN)|Control Water]] (4) · [[Ice Storm (4-V-L-ISE)|Ice Storm]] (4) · [[Wind Wall (3-V-L-WWN)|Wind Wall]] (3) · [[Geyser (2-V-L-GYS)|Geyser]] (2) · [[Guardian of Faith (4-C-L-GFA)|Guardian of Faith]] (4) · [[Splash (0-C-L-SPL)|Splash]] (0) · [[Call Lightning (3-C-L-CLL)|Call Lightning]] (3).


---

## Tactical Assessment

Area denial for chokepoints and landing zones; pinned troops become easy targets.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
