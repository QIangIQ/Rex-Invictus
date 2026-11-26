---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/conjuration
  - source/srd
aliases:
  - "1st Tier Spell: Floating Disk"
  - "Floating Disk"
  - "1-P-M-FD"
registry_id: 1-P-M-FD
attribute_code: "1·Con·None·None·30 feet·1 hour"
incantation: "Seusina"
tier: 1
school: Conjuration
affinity: P
grade: M
pz_total: 116.0
pz_quantum: 350.0
t_e: -0.10
updated: 2026-11-16
---

**Floating Disk** (`1-P-M-FD`) is a 1st Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **116 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -0.10 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Conjuration]]
        - **Floating Disk** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-P-M-FD` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Con·None·None·30 feet·1 hour` |
| Incantation | *Seusina* |
| Affinity | P (Pure field construct) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | 30 feet |
| Area | single point or target |
| Duration | 1 hour |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A drop of mercury |
| Ritual | yes |
| Practitioner lineages | Wizard |

### Mechanism

A 0.9 m force plate hovers 0.9 m above the ground carrying up to 227 kg and follows the caster at a set distance over gentle terrain.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| lift load to 3 ft | `226.8 kg * 9.81 * 0.914 m / 1500` | 1.4 |
| hover 500 lb | `0.02 * 226.8 kg * 9.81 / 1500 = 0.0296654 Pz/s * 3600 s` | 107 |
| Pattern cost | `0.01 × Q1 × (1 + 1.25)` | 7.9 |

| Quantity | Value |
|---|---|
| Effect energy | 1.4 Pz |
| Upkeep energy | 107 Pz (0.0297 Pz/s) |
| **Total draw** | **116 Pz** (174.0 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.332 |
| Energy-equivalent tier T_E | -0.10 |
| Handling points | 1.25 |
| Grade score | 0.70 → M |

**Handling flags:** ritual, fragile.

**Assumptions:** Full 500 lb load for 1 hour; hover rule 0.02*m*g.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Floating Disk (1-P-M-FD) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | 1 hour | 0 | `0000000000001` |

### Incantation

Spoken as **Seusina** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hiseusina* · T3: *Liseusina* · T4: *Viseusina* · T5: *Tiseusina* · T6: *Riseusina* · T7: *Miseusina* · T8: *Niseusina* · T9: *Xyiseusina*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 | 1 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#e37e00`.

![[Floating Disk (1-P-M-FD) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Conjuration | 0.125 | 1.000 | `#ff8300` (662 nm eq.) | source grid |
| Duration | 1 hour | 0.053 | 0.999 | `#ff1c00` (684 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.981 | `#91ff00` (612 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.17): swatch `#fb6535`, measured lines at 0.053, 0.101, 0.126, 0.295. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.06. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·C·None`; the k4 to k6 lines (None, 30 feet, 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·C·None` |
| Standard spectrometer detection range | 1.08 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 56.4 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 19.3 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (33.2% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Pure]] (P) |
| Function | [[Movement and Flight]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Mage Hand (0-P-L-MH)|Mage Hand]] (0) · [[Expeditious Retreat (1-T-L-ER)|Expeditious Retreat]] (1) · [[Feather Fall (1-T-L-FFA)|Feather Fall]] (1) · [[Jump (1-T-L-JMP)|Jump]] (1) · [[Longstrider (1-T-L-LNG)|Longstrider]] (1) · [[Skyward (1-T-L-SKY)|Skyward]] (1) · [[Accelerate (2-T-L-ACC)|Accelerate]] (2) · [[Levitate (2-T-L-LVT)|Levitate]] (2).


---

## Tactical Assessment

Logistics support for foot patrols: carries ammunition, casualties or salvage without vehicles, but it cannot cross a 3 m drop.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
