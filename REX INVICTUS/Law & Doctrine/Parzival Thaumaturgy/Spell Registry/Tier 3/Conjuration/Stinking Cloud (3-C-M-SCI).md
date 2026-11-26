---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/conjuration
  - source/srd
aliases:
  - "3rd Tier Spell: Stinking Cloud"
  - "Stinking Cloud"
  - "3-C-M-SCI"
registry_id: 3-C-M-SCI
attribute_code: "3·Con·None·sphere (20)·90 feet·Up to 1 minute"
incantation: "Le’-Soylarse"
tier: 3
school: Conjuration
affinity: C
grade: M
pz_total: 1204.9
pz_quantum: 2586.2
t_e: 2.24
updated: 2026-11-16
---

**Stinking Cloud** (`3-C-M-SCI`) is a 3rd Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **1,205 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E 2.24 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Conjuration]]
        - **Stinking Cloud** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-C-M-SCI` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Con·None·sphere (20)·90 feet·Up to 1 minute` |
| Incantation | *Le’-Soylarse* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | 90 feet |
| Area | sphere (20) |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A rotten egg or several skunk cabbage leaves |
| Ritual | no |
| Resistance check | constitution; on success: no effect |
| Practitioner lineages | Bard, Sorcerer, Wizard |

### Mechanism

A 6 m sphere of dense, opaque nauseant gas forms and lingers, causing breathing creatures inside to spend their effort retching.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Conjured nauseant gas | `1 Pz/kg * 1139 kg (949 m^3 * 1.2 kg/m^3)` | 1,139 |
| Upkeep: Nausea induction, 4 creatures | `0.005 Pz/s * 4 * 60 s` | 1.2 |
| Pattern cost | `0.01 × Q3 × (1 + 1.50)` | 64.7 |

| Quantity | Value |
|---|---|
| Effect energy | 1,139 Pz |
| Upkeep energy | 1.2 Pz (0.02 Pz/s) |
| **Total draw** | **1,205 Pz** (1,807.3 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 0.466 |
| Energy-equivalent tier T_E | 2.24 |
| Handling points | 1.50 |
| Grade score | 1.12 → M |

**Handling flags:** concentration, fragile, save or suck.

**Assumptions:** Full sphere filled with conjured gas at air density; 4 creatures affected; wind can end it early.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Stinking Cloud (3-C-M-SCI) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (20) | 30 | `0000000111101` |
| k5 Range | 90 feet | 11 | `0000000010111` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Le’-Soylarse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vile’-Soylarse* · T5: *Tile’-Soylarse* · T6: *Rile’-Soylarse* · T7: *Mile’-Soylarse* · T8: *Nile’-Soylarse* · T9: *Xyile’-Soylarse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 2→11 3→12 4→0 5→1 | 5 |
| k5 Range | 0→8 1→9 2→10 4→12 | 4 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#638a93`.

![[Stinking Cloud (3-C-M-SCI) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.985 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.929 | `#0074ff` (495 nm eq.) | source grid |
| Area | sphere (20) | 0.833 | 0.867 | `#5a00ff` (450 nm eq.) | source grid |
| Range | 90 feet | 0.647 | 0.942 | `#00aaff` (506 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.23): swatch `#aaa785`, measured lines at 0.126, 0.300, 0.648, 0.685, 0.834. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.08. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·C·None`; the k4 to k6 lines (sphere (20), 90 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·C·None` |
| Standard spectrometer detection range | 3.47 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 259 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 201 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 3rd Tier quantum of 2,586 Pz (46.6% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Summoning and Conjured Creatures]], [[Healing and Restoration]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Thomson's Plum Pudding (2-T-L-TSPP)|Thomson's Plum Pudding]] (2) · [[Arcane Singularity (3-C-L-ASA)|Arcane Singularity]] (3) · [[Conjure Animals (3-C-M-CA)|Conjure Animals]] (3) · [[Revivify (3-C-L-RVV)|Revivify]] (3) · [[Conjure Magic Prism (4-C-L-CMPJ)|Conjure Magic Prism]] (4) · [[Conjure Minor Elementals (4-C-M-CME)|Conjure Minor Elementals]] (4) · [[Conjure Woodland Beings (4-C-L-CWB)|Conjure Woodland Beings]] (4) · [[Faithful Hound (4-C-L-FH)|Faithful Hound]] (4).


---

## Tactical Assessment

Suppresses defenders in rooms or trenches and blocks sight lines; wind disperses it, and sealed or non-breathing troops ignore it.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
