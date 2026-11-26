---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-7
  - spell/conjuration
  - source/srd
aliases:
  - "7th Tier Spell: Plane Shift"
  - "Plane Shift"
  - "7-C-L-PSN"
registry_id: 7-C-L-PSN
attribute_code: "7·Con·None·None·Touch·Instantaneous"
incantation: "Melix"
tier: 7
school: Conjuration
affinity: C
grade: L
pz_total: 73765.0
pz_quantum: 141200.1
t_e: 6.35
updated: 2026-11-16
---

**Plane Shift** (`7-C-L-PSN`) is a 7th Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **73,765 Pz** against a slot quantum of 141,200 Pz, which puts its energy-equivalent tier at T_E 6.35 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 7 Workings]]
      - [[Conjuration]]
        - **Plane Shift** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `7-C-L-PSN` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `7·Con·None·None·Touch·Instantaneous` |
| Incantation | *Melix* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 7th Tier |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | Touch |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A forked, metal rod worth at least 250 gp, attuned to a particular plane of existence |
| Ritual | no |
| Resistance check | presence; on success: no effect |
| Delivery | aimed melee working |
| Practitioner lineages | Cleric, Druid, Sorcerer, Warlock, Wizard |

### Mechanism

The tuned rod locks the field onto a target plane and carries a hand-linked circle across one plane boundary. Used offensively, it throws a single touched target to a random point on the chosen plane.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| transport of 9 linked creatures, 80 kg each, 1 plane boundary | `0.01*9*80*15*1e6/1500` | 72,000 |
| Pattern cost | `0.01 × Q7 × (1 + 0.25)` | 1,765 |

| Quantity | Value |
|---|---|
| Effect energy | 72,000 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **73,765 Pz** (110,647.5 kJ) |
| Slot quantum Q7 | 141,200 Pz |
| Field gain (draw / quantum) | 0.522 |
| Energy-equivalent tier T_E | 6.35 |
| Handling points | 0.25 |
| Grade score | -0.07 → L |

**Handling flags:** costly material.

**Assumptions:** Full group of 9 at 80 kg; one boundary crossing at d_eff 1e6 m; banishment mode (8000 Pz for one target) is lower and not summed.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Plane Shift (7-C-L-PSN) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 7 | 7 | `0000000001111` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Melix** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T8: *Nimelix* · T9: *Xyimelix*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 3→2 | 4 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#9d3894`.

![[Plane Shift (7-C-L-PSN) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 7 | 0.700 | 1.000 | `#005eff` (490 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.848 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.783 | `#ff0028` (700 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.984 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.21): swatch `#877e96`, measured lines at 0.004, 0.126, 0.701, 0.883. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.87. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `7·C·None`; the k4 to k6 lines (None, Touch, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `7·C·None` |
| Standard spectrometer detection range | 27.16 km (r = 1 km × √(E/100 Pz)) |
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
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 12,294 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 7th Tier quantum of 141,200 Pz (52.2% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
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

Similar workings: [[Dream of the Blue Veil (7-C-M-DBV)|Dream of the Blue Veil]] (7) · [[Magnificent Mansion (7-C-M-MMN)|Magnificent Mansion]] (7) · [[Teleport (7-C-L-TLP)|Teleport]] (7) · [[Demiplane (8-C-L-DMP)|Demiplane]] (8) · [[Maze (8-C-L-MAZ)|Maze]] (8) · [[Transport via Plants (6-C-L-TP)|Transport via Plants]] (6) · [[Word of Recall (6-C-L-WR)|Word of Recall]] (6) · [[Etherealness (7-T-L-ETH)|Etherealness]] (7).


---

## Tactical Assessment

Strategic insertion or extraction of a small team between planes without staging infrastructure. The touch banishment mode removes a single high-value opponent from the theatre outright.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 7 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
