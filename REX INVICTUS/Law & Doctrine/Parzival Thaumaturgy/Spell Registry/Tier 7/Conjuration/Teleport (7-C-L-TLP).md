---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-7
  - spell/conjuration
  - source/srd
aliases:
  - "7th Tier Spell: Teleport"
  - "Teleport"
  - "7-C-L-TLP"
registry_id: 7-C-L-TLP
attribute_code: "7·Con·None·cube (10)·10 feet·Instantaneous"
incantation: "Me’-Bespul"
tier: 7
school: Conjuration
affinity: C
grade: L
pz_total: 73412.0
pz_quantum: 141200.1
t_e: 6.35
updated: 2026-11-16
---

**Teleport** (`7-C-L-TLP`) is a 7th Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **73,412 Pz** against a slot quantum of 141,200 Pz, which puts its energy-equivalent tier at T_E 6.35 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 7 Workings]]
      - [[Conjuration]]
        - **Teleport** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `7-C-L-TLP` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `7·Con·None·cube (10)·10 feet·Instantaneous` |
| Incantation | *Me’-Bespul* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 7th Tier |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | 10 feet |
| Area | cube (10) |
| Duration | Instantaneous |
| Components | spoken (incantation) |
| Ritual | no |
| Practitioner lineages | Bard, Sorcerer, Wizard |

### Mechanism

The caster and up to eight companions, or one object fitting a 3 m cube, are moved to a known destination on the same plane; accuracy depends on familiarity with the target.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Translocation of 9 creatures, 1000 km | `0.01 * 720 kg * 15 * 1e6 m / 1500` | 72,000 |
| Pattern cost | `0.01 × Q7 × (1 + 0.00)` | 1,412 |

| Quantity | Value |
|---|---|
| Effect energy | 72,000 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **73,412 Pz** (110,118.0 kJ) |
| Slot quantum Q7 | 141,200 Pz |
| Field gain (draw / quantum) | 0.52 |
| Energy-equivalent tier T_E | 6.35 |
| Handling points | 0.00 |
| Grade score | -0.33 → L |

**Handling flags:** none.

**Assumptions:** 9 x 80 kg; representative 1000 km jump; mishap injury not included.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Teleport (7-C-L-TLP) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 7 | 7 | `0000000001111` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | cube (10) | 5 | `0000000001011` |
| k5 Range | 10 feet | 1 | `0000000000011` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Me’-Bespul** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T8: *Nime’-Bespul* · T9: *Xyime’-Bespul*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 3→2 | 4 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 3→12 | 3 |
| k5 Range | 0→8 1→9 | 2 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#c35442`.

![[Teleport (7-C-L-TLP) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 7 | 0.700 | 1.000 | `#005eff` (490 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.848 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.783 | `#ff0028` (700 nm eq.) | source grid |
| Area | cube (10) | 0.139 | 0.854 | `#ff9300` (658 nm eq.) | source grid |
| Range | 10 feet | 0.059 | 0.814 | `#ff2700` (682 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.23): swatch `#b07766`, measured lines at 0.004, 0.060, 0.124, 0.139, 0.701. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.87. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `7·C·None`; the k4 to k6 lines (cube (10), 10 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `7·C·None` |
| Standard spectrometer detection range | 27.09 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 7,060 Pz (0.05 × Q7) |
| Counter drawn cold (all six layers) | 14,120 Pz (0.10 × Q7) |
| Unravel after completion | 14,120 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 12,235 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 7th Tier quantum of 141,200 Pz (52.0% of it). |
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
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Dream of the Blue Veil (7-C-M-DBV)|Dream of the Blue Veil]] (7) · [[Magnificent Mansion (7-C-M-MMN)|Magnificent Mansion]] (7) · [[Plane Shift (7-C-L-PSN)|Plane Shift]] (7) · [[Demiplane (8-C-L-DMP)|Demiplane]] (8) · [[Maze (8-C-L-MAZ)|Maze]] (8) · [[Transport via Plants (6-C-L-TP)|Transport via Plants]] (6) · [[Word of Recall (6-C-L-WR)|Word of Recall]] (6) · [[Etherealness (7-T-L-ETH)|Etherealness]] (7).


---

## Tactical Assessment

Strategic insertion and extraction with no transit exposure; poor intelligence on the destination risks scatter or injury.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 7 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
