---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-7
  - spell/conjuration
  - source/srd
aliases:
  - "7th Tier Spell: Magnificent Mansion"
  - "Magnificent Mansion"
  - "7-C-M-MMN"
registry_id: 7-C-M-MMN
attribute_code: "7·Con·None·cube (5)·300 feet·24 hours"
incantation: "Me’-Busphinl"
tier: 7
school: Conjuration
affinity: C
grade: M
pz_total: 230924.0
pz_quantum: 141200.1
t_e: 7.49
updated: 2026-11-16
---

**Magnificent Mansion** (`7-C-M-MMN`) is a 7th Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **230,924 Pz** against a slot quantum of 141,200 Pz, which puts its energy-equivalent tier at T_E 7.49 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 7 Workings]]
      - [[Conjuration]]
        - **Magnificent Mansion** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `7-C-M-MMN` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `7·Con·None·cube (5)·300 feet·24 hours` |
| Incantation | *Me’-Busphinl* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 7th Tier |
| School | [[Conjuration]] |
| Casting time | 1 minute |
| Range | 300 feet |
| Area | cube (5) |
| Duration | 24 hours |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A miniature portal carved from ivory, a small piece of polished marble, and a tiny silver spoon, each item worth at least 5 gp |
| Ritual | no |
| Practitioner lineages | Bard, Wizard |

### Mechanism

The field opens a pocket dwelling of up to 50 rooms 10 ft on a side behind a single portal, fills it with clean warm air, furnishings, food for 100 and a staff of 100 obedient semi-transparent servants. Anything taken out dissolves and occupants are expelled when it ends.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Conjured atmosphere | `1 Pz/kg * (1415.8 m^3 * 1.2 kg/m^3)` | 1,699 |
| Warming atmosphere by 10 K | `1699 kg * 1005 * 10 K / 1500` | 11,380 |
| Banquet food (semi-living matter) | `10 Pz/kg * 200 kg` | 2,000 |
| Furnishings (structured solids) | `3 Pz/kg * 5000 kg` | 15,000 |
| Servant bodies | `10 Pz/kg * 10 kg * 100` | 10,000 |
| Occupant transit across pocket boundary | `10 * 0.01 * 80 kg * 15 * 1e6 m / 1500` | 80,000 |
| Servant autonomy at 25% duty (upkeep) | `0.05 Pz/s * 100 * 0.25 * 86400 s` | 108,000 |
| Pattern cost | `0.01 × Q7 × (1 + 1.00)` | 2,824 |

| Quantity | Value |
|---|---|
| Effect energy | 120,100 Pz |
| Upkeep energy | 108,000 Pz (1.2 Pz/s) |
| **Total draw** | **230,924 Pz** (346,386.0 kJ) |
| Slot quantum Q7 | 141,200 Pz |
| Field gain (draw / quantum) | 1.64 |
| Energy-equivalent tier T_E | 7.49 |
| Handling points | 1.00 |
| Grade score | 1.25 → M |

**Handling flags:** costly material, multi target control, long cast.

**Assumptions:** Order-of-magnitude model; pocket walls costed into the pattern; 200 kg food and 5000 kg furnishings; servants 10 kg equivalent each, active a quarter of the time; 10 occupants transit once.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Magnificent Mansion (7-C-M-MMN) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 7 | 7 | `0000000001111` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | cube (5) | 15 | `0000000011111` |
| k5 Range | 300 feet | 6 | `0000000001101` |
| k6 Duration | 24 hours | 5 | `0000000001011` |

### Incantation

Spoken as **Me’-Busphinl** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T8: *Nime’-Busphinl* · T9: *Xyime’-Busphinl*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 3→2 | 4 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 2→11 3→12 4→0 | 5 |
| k5 Range | 0→8 2→10 3→11 | 3 |
| k6 Duration | 0→7 1→8 3→10 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#52c63a`.

![[Magnificent Mansion (7-C-M-MMN) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 7 | 0.700 | 1.000 | `#005eff` (490 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.848 | `#ff8300` (662 nm eq.) | source grid |
| Duration | 24 hours | 0.316 | 0.929 | `#76ff00` (605 nm eq.) | source grid |
| Area | cube (5) | 0.417 | 0.961 | `#00ff15` (575 nm eq.) | source grid |
| Range | 300 feet | 0.353 | 0.942 | `#40ff00` (594 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.20): swatch `#a5b488`, measured lines at 0.126, 0.316, 0.354, 0.417, 0.701. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 5.36. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `7·C·None`; the k4 to k6 lines (cube (5), 300 feet, 24 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `7·C·None` |
| Standard spectrometer detection range | 48.05 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 7,060 Pz (0.05 × Q7) |
| Counter drawn cold (all six layers) | 14,120 Pz (0.10 × Q7) |
| Unravel after completion | 35,720 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 38,487 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 1.64 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 7th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 7th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 7 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Teleportation and Planar Travel]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Dream of the Blue Veil (7-C-M-DBV)|Dream of the Blue Veil]] (7) · [[Plane Shift (7-C-L-PSN)|Plane Shift]] (7) · [[Teleport (7-C-L-TLP)|Teleport]] (7) · [[Demiplane (8-C-L-DMP)|Demiplane]] (8) · [[Maze (8-C-L-MAZ)|Maze]] (8) · [[Transport via Plants (6-C-L-TP)|Transport via Plants]] (6) · [[Word of Recall (6-C-L-WR)|Word of Recall]] (6) · [[Etherealness (7-T-L-ETH)|Etherealness]] (7).


---

## Tactical Assessment

Provides a concealed, secure rest and command post for a unit for a full day, closed off from pursuit. The portal location is its main vulnerability.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 7 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
