---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/transmutation
  - source/srd
aliases:
  - "1st Tier Spell: Feather Fall"
  - "Feather Fall"
  - "1-T-L-FFA"
registry_id: 1-T-L-FFA
attribute_code: "1·Tra·None·None·60 feet·1 minute"
incantation: "Siewyne"
tier: 1
school: Transmutation
affinity: T
grade: L
pz_total: 482.8
pz_quantum: 350.0
t_e: 1.32
updated: 2026-11-16
---

**Feather Fall** (`1-T-L-FFA`) is a 1st Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **483 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E 1.32 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Transmutation]]
        - **Feather Fall** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-T-L-FFA` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Tra·None·None·60 feet·1 minute` |
| Incantation | *Siewyne* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Transmutation]] |
| Casting time | 1 reaction |
| Range | 60 feet |
| Area | single point or target |
| Duration | 1 minute |
| Components | spoken (incantation), material focus. Material: A small feather or a piece of down |
| Ritual | no |
| Practitioner lineages | Bard, Sorcerer, Wizard |

### Mechanism

The field couples to up to five falling bodies and caps their descent at about 3 m/s, dumping the arrested potential energy as a gentle braking drag until each body lands.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| arrested fall, 5 creatures | `5 * 80 kg * 9.81 * (600 ft*0.3048 = 182.88 m) / 1500` | 478 |
| Pattern cost | `0.01 × Q1 × (1 + 0.25)` | 4.4 |

| Quantity | Value |
|---|---|
| Effect energy | 478 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **483 Pz** (724.2 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 1.38 |
| Energy-equivalent tier T_E | 1.32 |
| Handling points | 0.25 |
| Grade score | 0.41 → L |

**Handling flags:** reaction cast.

**Assumptions:** 5 targets at 80 kg; full 1 minute of descent at 60 ft/round (182.9 m) arrested; energy booked as m*g*h of the slowed fall.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Feather Fall (1-T-L-FFA) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | 1 minute | 1 | `0000000000011` |

### Incantation

Spoken as **Siewyne** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisiewyne* · T3: *Lisiewyne* · T4: *Visiewyne* · T5: *Tisiewyne* · T6: *Risiewyne* · T7: *Misiewyne* · T8: *Nisiewyne* · T9: *Xyisiewyne*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#ab7272`.

![[Feather Fall (1-T-L-FFA) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.741 | `#9600ff` (438 nm eq.) | source grid |
| Duration | 1 minute | 0.105 | 1.000 | `#ff6300` (668 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.888 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.17): swatch `#a57286`, measured lines at 0.102, 0.589, 0.876. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.68. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·T·None`; the k4 to k6 lines (None, 60 feet, 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·T·None` |
| Standard spectrometer detection range | 2.20 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.0 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 80.5 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 1.38 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 1st Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Movement and Flight]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Expeditious Retreat (1-T-L-ER)|Expeditious Retreat]] (1) · [[Jump (1-T-L-JMP)|Jump]] (1) · [[Longstrider (1-T-L-LNG)|Longstrider]] (1) · [[Skyward (1-T-L-SKY)|Skyward]] (1) · [[Accelerate (2-T-L-ACC)|Accelerate]] (2) · [[Levitate (2-T-L-LVT)|Levitate]] (2) · [[Spider Climb (2-T-L-SC)|Spider Climb]] (2) · [[Floating Disk (1-P-M-FD)|Floating Disk]] (1).


---

## Tactical Assessment

A reaction-speed safety net for airborne insertion, ejected aircrew or troops blown off structures; a single caster can recover a fire team in free fall without chutes.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
