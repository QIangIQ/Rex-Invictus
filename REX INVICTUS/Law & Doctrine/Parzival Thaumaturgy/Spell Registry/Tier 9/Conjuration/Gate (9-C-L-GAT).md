---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-9
  - spell/conjuration
  - source/srd
aliases:
  - "9th Tier Spell: Gate"
  - "Gate"
  - "9-C-L-GAT"
registry_id: 9-C-L-GAT
attribute_code: "9·Con·None·None·60 feet·Up to 1 minute"
incantation: "Xyewynse"
tier: 9
school: Conjuration
affinity: C
grade: L
pz_total: 823650.0
pz_quantum: 1043335.3
t_e: 8.76
updated: 2026-11-16
---

**Gate** (`9-C-L-GAT`) is a 9th Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **823,650 Pz** against a slot quantum of 1.04 MPz Pz, which puts its energy-equivalent tier at T_E 8.76 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 9 Workings]]
      - [[Conjuration]]
        - **Gate** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `9-C-L-GAT` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `9·Con·None·None·60 feet·Up to 1 minute` |
| Incantation | *Xyewynse* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 9th Tier |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | single point or target |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A diamond worth at least 5,000gp |
| Ritual | no |
| Practitioner lineages | Cleric, Sorcerer, Wizard |

### Mechanism

Opens a 1.5 to 6 m aperture to a precise location on another plane for one minute, or reaches out to pull a named being through.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| drawing a named creature across | `0.01 * 80 kg * 15 * 1e6 m / 1500` | 8,000 |
| portal transit flux (100 crossings) | `100 * 8000 Pz / 60 s = 13333.3 Pz/s * 60 s` | 800,000 |
| Pattern cost | `0.01 × Q9 × (1 + 0.50)` | 15,650 |

| Quantity | Value |
|---|---|
| Effect energy | 8,000 Pz |
| Upkeep energy | 800,000 Pz (13,333 Pz/s) |
| **Total draw** | **823,650 Pz** (1,235,475.0 kJ) |
| Slot quantum Q9 | 1.04 MPz Pz |
| Field gain (draw / quantum) | 0.789 |
| Energy-equivalent tier T_E | 8.76 |
| Handling points | 0.50 |
| Grade score | 0.38 → L |

**Handling flags:** concentration, costly material.

**Assumptions:** Order-of-magnitude: 100 Medium crossings over the minute at 1e6 m effective distance each; one named creature of 80 kg drawn through.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Gate (9-C-L-GAT) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 9 | 9 | `0000000010011` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Xyewynse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 4→3 | 3 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#657acb`.

![[Gate (9-C-L-GAT) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 9 | 0.900 | 1.000 | `#b600ff` (430 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.741 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.977 | `#0074ff` (495 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.953 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.17): swatch `#7b8ab2`, measured lines at 0.126, 0.589, 0.685, 0.901. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 5.92. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `9·C·None`; the k4 to k6 lines (None, 60 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `9·C·None` |
| Standard spectrometer detection range | 90.76 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 52,167 Pz (0.05 × Q9) |
| Counter drawn cold (all six layers) | 104,334 Pz (0.10 × Q9) |
| Unravel after completion | 264,334 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 137,275 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 9th Tier quantum of 1.04 MPz Pz (78.9% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
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
| Function | [[Teleportation and Planar Travel]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Wish (9-C-L-WSH)|Wish]] (9) · [[Demiplane (8-C-L-DMP)|Demiplane]] (8) · [[Maze (8-C-L-MAZ)|Maze]] (8) · [[Astral Projection (9-N-M-AP)|Astral Projection]] (9) · [[Dream of the Blue Veil (7-C-M-DBV)|Dream of the Blue Veil]] (7) · [[Imprisonment (9-A-L-IMP)|Imprisonment]] (9) · [[Magnificent Mansion (7-C-M-MMN)|Magnificent Mansion]] (7) · [[Plane Shift (7-C-L-PSN)|Plane Shift]] (7).


---

## Tactical Assessment

Strategic-scale troop and materiel transfer between planes, or a summons that can bring an allied power or an enemy leader to the field.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 9 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
