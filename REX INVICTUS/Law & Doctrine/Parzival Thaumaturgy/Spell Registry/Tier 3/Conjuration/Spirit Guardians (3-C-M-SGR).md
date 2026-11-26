---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/conjuration
  - source/srd
aliases:
  - "3rd Tier Spell: Spirit Guardians"
  - "Spirit Guardians"
  - "3-C-M-SGR"
registry_id: 3-C-M-SGR
attribute_code: "3·Con·None·None·Self·Up to 10 minutes"
incantation: "Leporly"
tier: 3
school: Conjuration
affinity: C
grade: M
pz_total: 7751.3
pz_quantum: 2586.2
t_e: 4.10
updated: 2026-11-16
---

**Spirit Guardians** (`3-C-M-SGR`) is a 3rd Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **7,751 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E 4.10 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Conjuration]]
        - **Spirit Guardians** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-C-M-SGR` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Con·None·None·Self·Up to 10 minutes` |
| Incantation | *Leporly* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | Self |
| Area | single point or target |
| Duration | Up to 10 minutes (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A holy symbol |
| Ritual | no |
| Practitioner lineages | Cleric |

### Mechanism

Bound guardian entities circle the caster at 4.5 m, slowing hostile movers and dealing radiant (or necrotic) injury to those who enter or linger.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Radiant field injury, 3 triggers | `13.5 HP * 0.50 * 262.7 m^2 / 0.7 * 3` | 7,599 |
| Upkeep: Four guardian entities sustained | `0.05 Pz/s * 4 * 600 s` | 120 |
| Pattern cost | `0.01 × Q3 × (1 + 0.25)` | 32.3 |

| Quantity | Value |
|---|---|
| Effect energy | 7,599 Pz |
| Upkeep energy | 120 Pz (0.2 Pz/s) |
| **Total draw** | **7,751 Pz** (11,627.0 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 3 |
| Energy-equivalent tier T_E | 4.10 |
| Handling points | 0.25 |
| Grade score | 0.80 → M |

**Handling flags:** concentration.

**Assumptions:** Average 3d8 = 13.5; good-aligned radiant kappa; 15 ft emanation as sphere; 3 triggers; 4 guardians.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Spirit Guardians (3-C-M-SGR) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Up to 10 minutes | 15 | `0000000011111` |

### Incantation

Spoken as **Leporly** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vileporly* · T5: *Tileporly* · T6: *Rileporly* · T7: *Mileporly* · T8: *Nileporly* · T9: *Xyileporly*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 2→9 3→10 4→11 | 5 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#6e7a79`.

![[Spirit Guardians (3-C-M-SGR) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.985 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Up to 10 minutes | 0.789 | 0.887 | `#1e00ff` (463 nm eq.) | source grid |
| Range | Self | 0.706 | 0.921 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.23): swatch `#ae9d80`, measured lines at 0.126, 0.300, 0.706, 0.790. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.89. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·C·None`; the k4 to k6 lines (None, Self, Up to 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·C·None` |
| Standard spectrometer detection range | 8.80 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 283 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1,292 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 3.00 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 3rd Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Mind and Will]], [[Divination and Sensing]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Plagarise (4-E-L-PLG)|Plagarise]] (4) · [[Suspend Motion (4-T-L-SMS)|Suspend Motion]] (4) · [[Arcane Singularity (3-C-L-ASA)|Arcane Singularity]] (3) · [[Awaken (5-T-H-AWK)|Awaken]] (5) · [[Scattered Path (2-C-L-SPA)|Scattered Path]] (2) · [[Beacon of Hope (3-A-L-BHA)|Beacon of Hope]] (3) · [[Bestow Curse (3-N-L-BC)|Bestow Curse]] (3) · [[Clairvoyance (3-D-L-CLR)|Clairvoyance]] (3).


---

## Tactical Assessment

A close-defence aura for holding a doorway or command post against assault; allies can be exempted.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
