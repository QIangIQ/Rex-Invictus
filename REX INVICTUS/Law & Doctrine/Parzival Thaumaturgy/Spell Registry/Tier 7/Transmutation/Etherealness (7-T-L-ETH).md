---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-7
  - spell/transmutation
  - source/srd
aliases:
  - "7th Tier Spell: Etherealness"
  - "Etherealness"
  - "7-T-L-ETH"
registry_id: 7-T-L-ETH
attribute_code: "7·Tra·None·None·Self·8 hours"
incantation: "Mieporiy"
tier: 7
school: Transmutation
affinity: T
grade: L
pz_total: 1572.0
pz_quantum: 141200.1
t_e: 2.50
updated: 2026-11-16
---

**Etherealness** (`7-T-L-ETH`) is a 7th Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **1,572 Pz** against a slot quantum of 141,200 Pz, which puts its energy-equivalent tier at T_E 2.50 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 7 Workings]]
      - [[Transmutation]]
        - **Etherealness** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `7-T-L-ETH` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `7·Tra·None·None·Self·8 hours` |
| Incantation | *Mieporiy* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 7th Tier |
| School | [[Transmutation]] |
| Casting time | 1 action |
| Range | Self |
| Area | single point or target |
| Duration | 8 hours |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Bard, Cleric, Sorcerer, Warlock, Wizard |

### Mechanism

The caster shifts into the border region of a neighbouring plane, able to move through solid matter unseen while seeing the origin plane dimly.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| cross into and back from the border region (2 boundary crossings) | `2*0.01*80*15*1e3/1500  [C1]` | 16.0 |
| upkeep: phase hold, 1 creature, 8 h | `0.005*1*8*3600` | 144 |
| Pattern cost | `0.01 × Q7 × (1 + 0.00)` | 1,412 |

| Quantity | Value |
|---|---|
| Effect energy | 16.0 Pz |
| Upkeep energy | 144 Pz (0.005 Pz/s) |
| **Total draw** | **1,572 Pz** (2,358.0 kJ) |
| Slot quantum Q7 | 141,200 Pz |
| Field gain (draw / quantum) | 0.0111 |
| Energy-equivalent tier T_E | 2.50 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

Calibration applied: C1 (Coterminous crossing), see [[Parzival Energy Budget#Registry calibration rules]].

**Handling flags:** none.

**Assumptions:** Two boundary crossings at d_eff = 1e6 m; phase hold at enchantment rate.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Etherealness (7-T-L-ETH) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 7 | 7 | `0000000001111` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | 8 hours | 8 | `0000000010001` |

### Incantation

Spoken as **Mieporiy** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T8: *Nimieporiy* · T9: *Xyimieporiy*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 3→2 | 4 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 4→11 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#256cd9`.

![[Etherealness (7-T-L-ETH) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 7 | 0.700 | 1.000 | `#005eff` (490 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.985 | `#9600ff` (438 nm eq.) | source grid |
| Duration | 8 hours | 0.474 | 0.975 | `#00ff66` (558 nm eq.) | source grid |
| Range | Self | 0.706 | 1.000 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.16): swatch `#39ace4`, measured lines at 0.474, 0.703, 0.876. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.20. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `7·T·None`; the k4 to k6 lines (None, Self, 8 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `7·T·None` |
| Standard spectrometer detection range | 3.96 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 7,060 Pz (0.05 × Q7) |
| Counter drawn cold (all six layers) | 14,120 Pz (0.10 × Q7) |
| Unravel after completion | 14,149 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 262 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 7th Tier quantum of 141,200 Pz (1.1% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 7th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 7 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Teleportation and Planar Travel]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Dream of the Blue Veil (7-C-M-DBV)|Dream of the Blue Veil]] (7) · [[Magnificent Mansion (7-C-M-MMN)|Magnificent Mansion]] (7) · [[Plane Shift (7-C-L-PSN)|Plane Shift]] (7) · [[Teleport (7-C-L-TLP)|Teleport]] (7) · [[Demiplane (8-C-L-DMP)|Demiplane]] (8) · [[Maze (8-C-L-MAZ)|Maze]] (8) · [[Transport via Plants (6-C-L-TP)|Transport via Plants]] (6) · [[Word of Recall (6-C-L-WR)|Word of Recall]] (6).


---

## Tactical Assessment

Covert reconnaissance and bypassing walls; the return can injure if the caster rematerialises inside matter.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 7 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
