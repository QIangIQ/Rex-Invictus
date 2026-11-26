---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-6
  - spell/conjuration
  - source/srd
aliases:
  - "6th Tier Spell: Transport via Plants"
  - "Transport via Plants"
  - "6-C-L-TP"
registry_id: 6-C-L-TP
attribute_code: "6·Con·None·None·10 feet·1 round"
incantation: "Respuli"
tier: 6
school: Conjuration
affinity: C
grade: L
pz_total: 64519.4
pz_quantum: 51944.6
t_e: 6.22
updated: 2026-11-16
---

**Transport via Plants** (`6-C-L-TP`) is a 6th Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **64,519 Pz** against a slot quantum of 51,945 Pz, which puts its energy-equivalent tier at T_E 6.22 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 6 Workings]]
      - [[Conjuration]]
        - **Transport via Plants** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `6-C-L-TP` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `6·Con·None·None·10 feet·1 round` |
| Incantation | *Respuli* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 6th Tier |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | 10 feet |
| Area | single point or target |
| Duration | 1 round |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Druid |

### Mechanism

A large living plant is linked to a known plant anywhere on the plane for one round, so creatures can step in at one and out at the other.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Plant gate transit, 8 creatures, 1000 km | `0.01 * 640 kg * 15 * 1e6 m / 1500` | 64,000 |
| Pattern cost | `0.01 × Q6 × (1 + 0.00)` | 519 |

| Quantity | Value |
|---|---|
| Effect energy | 64,000 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **64,519 Pz** (96,779.2 kJ) |
| Slot quantum Q6 | 51,945 Pz |
| Field gain (draw / quantum) | 1.24 |
| Energy-equivalent tier T_E | 6.22 |
| Handling points | 0.00 |
| Grade score | 0.11 → L |

**Handling flags:** none.

**Assumptions:** 8 creatures cross; 1000 km link.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Transport via Plants (6-C-L-TP) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 6 | 6 | `0000000001101` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 10 feet | 1 | `0000000000011` |
| k6 Duration | 1 round | 2 | `0000000000101` |

### Incantation

Spoken as **Respuli** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T7: *Mirespuli* · T8: *Nirespuli* · T9: *Xyirespuli*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 3→2 | 3 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 | 2 |
| k6 Duration | 0→7 2→9 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#b99445`.

![[Transport via Plants (6-C-L-TP) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 6 | 0.600 | 1.000 | `#00ebff` (520 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.893 | `#ff8300` (662 nm eq.) | source grid |
| Duration | 1 round | 0.158 | 0.907 | `#ffae00` (653 nm eq.) | source grid |
| Range | 10 feet | 0.059 | 0.864 | `#ff2700` (682 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.23): swatch `#c48c63`, measured lines at 0.059, 0.126, 0.158, 0.601. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.81. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `6·C·None`; the k4 to k6 lines (None, 10 feet, 1 round) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `6·C·None` |
| Standard spectrometer detection range | 25.40 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 2,597 Pz (0.05 × Q6) |
| Counter drawn cold (all six layers) | 5,194 Pz (0.10 × Q6) |
| Unravel after completion | 5,194 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 10,753 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 1.24 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 6th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 6th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 6 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Teleportation and Planar Travel]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Word of Recall (6-C-L-WR)|Word of Recall]] (6) · [[Dream of the Blue Veil (7-C-M-DBV)|Dream of the Blue Veil]] (7) · [[Magnificent Mansion (7-C-M-MMN)|Magnificent Mansion]] (7) · [[Plane Shift (7-C-L-PSN)|Plane Shift]] (7) · [[Teleport (7-C-L-TLP)|Teleport]] (7) · [[Teleportation Circle (5-C-M-TC)|Teleportation Circle]] (5) · [[Tree Stride (5-C-L-TSE)|Tree Stride]] (5) · [[Demiplane (8-C-L-DMP)|Demiplane]] (8).


---

## Tactical Assessment

Rapid movement of a small team between forested regions, using known trees as unmarked gates.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 6 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
