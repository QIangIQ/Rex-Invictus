---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-9
  - spell/transmutation
  - source/srd
aliases:
  - "9th Tier Spell: Time Stop"
  - "Time Stop"
  - "9-T-M-TSM"
registry_id: 9-T-M-TSM
attribute_code: "9·Tra·None·None·Self·Instantaneous"
incantation: "Xyiepor"
tier: 9
school: Transmutation
affinity: T
grade: M
pz_total: 1020866.7
pz_quantum: 1043335.3
t_e: 8.98
updated: 2026-11-16
---

**Time Stop** (`9-T-M-TSM`) is a 9th Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **1.02 MPz Pz** against a slot quantum of 1.04 MPz Pz, which puts its energy-equivalent tier at T_E 8.98 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 9 Workings]]
      - [[Transmutation]]
        - **Time Stop** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `9-T-M-TSM` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `9·Tra·None·None·Self·Instantaneous` |
| Incantation | *Xyiepor* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 9th Tier |
| School | [[Transmutation]] |
| Casting time | 1 action |
| Range | Self |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation) |
| Ritual | no |
| Practitioner lineages | Sorcerer, Wizard |

### Mechanism

The caster's local frame is decoupled from surrounding time for a few subjective turns inside a 300 m radius; any interaction with another creature restores coupling.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Local causal decoupling (order of magnitude) | `Q9 envelope ~ 350 * e^8` | 1.00 MPz |
| Pattern cost | `0.01 × Q9 × (1 + 1.00)` | 20,867 |

| Quantity | Value |
|---|---|
| Effect energy | 1.00 MPz Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **1.02 MPz Pz** (1,531,300.1 kJ) |
| Slot quantum Q9 | 1.04 MPz Pz |
| Field gain (draw / quantum) | 0.978 |
| Energy-equivalent tier T_E | 8.98 |
| Handling points | 1.00 |
| Grade score | 0.99 → M |

**Handling flags:** fragile.

**Assumptions:** No physical model fits; order-of-magnitude estimate set at the tier-9 field return.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Time Stop (9-T-M-TSM) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 9 | 9 | `0000000010011` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Xyiepor** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 4→3 | 3 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#8917d7`.

![[Time Stop (9-T-M-TSM) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 9 | 0.900 | 1.000 | `#b600ff` (430 nm eq.) | source grid |
| School | Transmutation | 0.875 | 1.000 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.667 | `#ff0028` (700 nm eq.) | source grid |
| Range | Self | 0.706 | 0.981 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.23): swatch `#4968e7`, measured lines at 0.004, 0.706, 0.876, 0.900. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 6.01. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `9·T·None`; the k4 to k6 lines (None, Self, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `9·T·None` |
| Standard spectrometer detection range | 101.04 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 52,167 Pz (0.05 × Q9) |
| Counter drawn cold (all six layers) | 104,334 Pz (0.10 × Q9) |
| Unravel after completion | 104,334 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 170,144 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 9th Tier quantum of 1.04 MPz Pz (97.8% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 9th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 9 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Summoning and Conjured Creatures]], [[Healing and Restoration]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Imprisonment (9-A-L-IMP)|Imprisonment]] (9) · [[Mass Heal (9-C-L-MHS)|Mass Heal]] (9) · [[Regenerate (7-T-L-RGN)|Regenerate]] (7) · [[True Resurrection (9-N-L-TR)|True Resurrection]] (9) · [[Clone (8-N-L-CLN)|Clone]] (8) · [[Gravitational Wave (8-V-L-GWV)|Gravitational Wave]] (8) · [[Thomson's Plum Pudding (2-T-L-TSPP)|Thomson's Plum Pudding]] (2) · [[Alter Biome (9-T-X-AB)|Alter Biome]] (9).


---

## Tactical Assessment

Buys several free actions for repositioning, preparation or escape, though it cannot be used to strike enemies directly.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 9 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
