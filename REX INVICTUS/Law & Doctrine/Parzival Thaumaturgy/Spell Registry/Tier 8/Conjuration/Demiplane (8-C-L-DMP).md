---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-8
  - spell/conjuration
  - source/srd
aliases:
  - "8th Tier Spell: Demiplane"
  - "Demiplane"
  - "8-C-L-DMP"
registry_id: 8-C-L-DMP
attribute_code: "8·Con·None·None·60 feet·1 hour"
incantation: "Newyna"
tier: 8
school: Conjuration
affinity: C
grade: L
pz_total: 427145.8
pz_quantum: 383821.6
t_e: 8.11
updated: 2026-11-16
---

**Demiplane** (`8-C-L-DMP`) is a 8th Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **427,146 Pz** against a slot quantum of 383,822 Pz, which puts its energy-equivalent tier at T_E 8.11 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 8 Workings]]
      - [[Conjuration]]
        - **Demiplane** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `8-C-L-DMP` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `8·Con·None·None·60 feet·1 hour` |
| Incantation | *Newyna* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 8th Tier |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | single point or target |
| Duration | 1 hour |
| Components | somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Warlock, Wizard |

### Mechanism

The field opens a door on a flat surface into a sealed pocket room 30 ft on a side made of wood or stone. The room persists after the door closes and later castings can reconnect to it.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| 30 ft room lined with 0.1 m stone (6 faces) | `3*6*(30*ft)**2*0.1*2600` | 391,308 |
| 4 Medium crossings through the door (1 plane boundary) | `4*0.01*80*15*1e6/J` | 32,000 |
| Pattern cost | `0.01 × Q8 × (1 + 0.00)` | 3,838 |

| Quantity | Value |
|---|---|
| Effect energy | 423,308 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **427,146 Pz** (640,718.7 kJ) |
| Slot quantum Q8 | 383,822 Pz |
| Field gain (draw / quantum) | 1.11 |
| Energy-equivalent tier T_E | 8.11 |
| Handling points | 0.00 |
| Grade score | 0.05 → L |

**Handling flags:** none.

**Assumptions:** Room lining 0.1 m stone; 4 crossings at the translocation rule with d_eff = 1e6 m; door hold has no separate upkeep.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Demiplane (8-C-L-DMP) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 8 | 8 | `0000000010001` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | 1 hour | 0 | `0000000000001` |

### Incantation

Spoken as **Newyna** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T9: *Xyinewyna*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 4→3 | 2 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 | 1 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#7b698e`.

![[Demiplane (8-C-L-DMP) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 8 | 0.800 | 1.000 | `#2900ff` (460 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.796 | `#ff8300` (662 nm eq.) | source grid |
| Duration | 1 hour | 0.053 | 0.756 | `#ff1c00` (684 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.978 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.15): swatch `#8d898f`, measured lines at 0.053, 0.126, 0.589, 0.801. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 5.63. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `8·C·None`; the k4 to k6 lines (None, 60 feet, 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `8·C·None` |
| Standard spectrometer detection range | 65.36 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 19,191 Pz (0.05 × Q8) |
| Counter drawn cold (all six layers) | 38,382 Pz (0.10 × Q8) |
| Unravel after completion | 38,382 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 71,191 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 1.11 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 8th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 8th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 8 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Teleportation and Planar Travel]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Maze (8-C-L-MAZ)|Maze]] (8) · [[Dream of the Blue Veil (7-C-M-DBV)|Dream of the Blue Veil]] (7) · [[Gate (9-C-L-GAT)|Gate]] (9) · [[Magnificent Mansion (7-C-M-MMN)|Magnificent Mansion]] (7) · [[Plane Shift (7-C-L-PSN)|Plane Shift]] (7) · [[Teleport (7-C-L-TLP)|Teleport]] (7) · [[Wish (9-C-L-WSH)|Wish]] (9) · [[Transport via Plants (6-C-L-TP)|Transport via Plants]] (6).


---

## Tactical Assessment

Secure storage, safe rooms and prisons outside normal space; anything left inside when the door closes is cut off.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 8 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
