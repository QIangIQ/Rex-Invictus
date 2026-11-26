---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/conjuration
  - source/rex-invictus
aliases:
  - "2nd Tier Spell: Misted Leap"
  - "Misted Leap"
  - "2-C-L-ML"
registry_id: 2-C-L-ML
attribute_code: "2·Con·None·sphere (10)·Self·1 minute"
incantation: "He’-Sepore"
tier: 2
school: Conjuration
affinity: C
grade: L
pz_total: 82.5
pz_quantum: 951.4
t_e: -0.44
updated: 2026-11-16
---

**Misted Leap** (`2-C-L-ML`) is a 2nd Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Rex Invictus original working. Its modelled draw is **82.5 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E -0.44 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Conjuration]]
        - **Misted Leap** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-C-L-ML` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Con·None·sphere (10)·Self·1 minute` |
| Incantation | *He’-Sepore* |
| Affinity | C (Conjuration) |
| Source | Rex Invictus |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Conjuration]] |
| Casting time | 1 bonus action |
| Range | Self |
| Area | sphere (10) |
| Duration | 1 minute |
| Components | spoken (incantation) |
| Ritual | no |
| Practitioner lineages | Wizard, Sorcerer, Warlock, Bard |

### Effect

The caster steps through a fold of the Mist to a visible point up to 30 feet away. A sphere of divine haze 10 feet in radius blooms at both the departure and arrival points and lingers for one minute. The haze blocks sight and smothers any fire of non-divine origin inside it.

### Mechanism

The working folds the space between two near points through the Mist and vents the displaced field as a cold, divine haze. The haze carries a flame-inhibiting charge that breaks the combustion chain of ordinary fire, while divine fire is protected by its own source under Lex Fontis.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| short fold, one 80 kg body over 9.1 m | `0.01*80*15*9.144/1500` | 0.0732 |
| divine haze, two 10 ft spheres at 5 g/m^3 | `2*1 Pz/kg*(4/3*pi*(3.048)^3*0.005)` | 1.2 |
| flame-inhibiting charge, 0.3 kg/m^3 over both spheres | `2*1 Pz/kg*(4/3*pi*(3.048)^3*0.3)` | 71.2 |
| [upkeep] haze held for 60 s | `0.01 Pz/s*60` | 0.6 |
| Pattern cost | `0.01 × Q2 × (1 + 0.00)` | 9.5 |

| Quantity | Value |
|---|---|
| Effect energy | 72.4 Pz |
| Upkeep energy | 0.6 Pz (0.01 Pz/s) |
| **Total draw** | **82.5 Pz** (123.8 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.0868 |
| Energy-equivalent tier T_E | -0.44 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** 80 kg caster; 30 ft hop; haze at 5 g/m^3 water-equivalent; inhibitor loading similar to a gaseous fire suppressant at 0.3 kg/m^3; haze lasts 1 minute.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Misted Leap (2-C-L-ML) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (10) | 27 | `0000000110111` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | 1 minute | 1 | `0000000000011` |

### Incantation

Spoken as **He’-Sepore** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihe’-Sepore* · T4: *Vihe’-Sepore* · T5: *Tihe’-Sepore* · T6: *Rihe’-Sepore* · T7: *Mihe’-Sepore* · T8: *Nihe’-Sepore* · T9: *Xyihe’-Sepore*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 2→11 4→0 5→1 | 5 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#a1765d`.

![[Misted Leap (2-C-L-ML) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.997 | `#ff8300` (662 nm eq.) | source grid |
| Duration | 1 minute | 0.105 | 0.996 | `#ff6300` (668 nm eq.) | source grid |
| Area | sphere (10) | 0.750 | 0.860 | `#0017ff` (475 nm eq.) | source grid |
| Range | Self | 0.706 | 0.880 | `#0058ff` (488 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 1.92. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·C·None`; the k4 to k6 lines (sphere (10), Self, 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·C·None` |
| Standard spectrometer detection range | 0.91 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 95.3 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 13.8 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (8.7% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Teleportation and Planar Travel]], [[Concealment and Illusion]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Misty Step (2-C-L-MS)|Misty Step]] (2) · [[Scattered Path (2-C-L-SPA)|Scattered Path]] (2) · [[Dream of the Blue Veil (7-C-M-DBV)|Dream of the Blue Veil]] (7) · [[Fog Cloud (1-C-L-FC)|Fog Cloud]] (1) · [[Arcanist's Magic Aura (2-I-L-ASMA)|Arcanist's Magic Aura]] (2) · [[Blur (2-I-L-BLR)|Blur]] (2) · [[Cloak (2-I-L-CLK)|Cloak]] (2) · [[Darkness (2-V-L-DRK)|Darkness]] (2).


---

## Tactical Assessment

Infantry use it as smoke on demand: one cast blinds a doorway or a trench bay and kills small fires started by incendiaries. It is quiet in Pz terms and sits under most ELINT thresholds when cast slowly.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
