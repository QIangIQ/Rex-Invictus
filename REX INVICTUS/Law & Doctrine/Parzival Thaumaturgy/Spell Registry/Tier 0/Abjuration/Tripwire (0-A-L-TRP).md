---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-0
  - spell/abjuration
  - source/rex-invictus
aliases:
  - "Cantrip Spell: Tripwire"
  - "Tripwire"
  - "0-A-L-TRP"
registry_id: 0-A-L-TRP
attribute_code: "0·Abj·None·None·30 feet·8 hours"
incantation: "Causiniy"
tier: 0
school: Abjuration
affinity: A
grade: L
pz_total: 4.7
pz_quantum: 128.8
t_e: -3.32
updated: 2026-11-16
---

**Tripwire** (`0-A-L-TRP`) is a Cantrip (Tier 0) working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Rex Invictus original working. Its modelled draw is **4.7 Pz** against a slot quantum of 129 Pz, which puts its energy-equivalent tier at T_E -3.32 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 0 Workings]]
      - [[Abjuration]]
        - **Tripwire** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `0-A-L-TRP` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `0·Abj·None·None·30 feet·8 hours` |
| Incantation | *Causiniy* |
| Affinity | A (Abjuration) |
| Source | Rex Invictus |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | Cantrip (Tier 0) |
| School | [[Abjuration]] |
| Casting time | 1 action |
| Range | 30 feet |
| Area | single point or target |
| Duration | 8 hours |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Wizard, Sorcerer, Ranger |

### Effect

Strings an invisible field thread between two points up to 30 feet apart. When it is crossed, or when its linked timer runs out, it releases any working tied to it.

### Mechanism

A dormant ward thread that listens for a crossing or a timed release.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| thread | `instant info` | 0.5 |
| [upkeep] dormant thread, 8 h | `0.0001 Pz/s*28800` | 2.9 |
| Pattern cost | `0.01 × Q0 × (1 + 0.00)` | 1.3 |

| Quantity | Value |
|---|---|
| Effect energy | 0.5 Pz |
| Upkeep energy | 2.9 Pz (0.0001 Pz/s) |
| **Total draw** | **4.7 Pz** (7.0 kJ) |
| Slot quantum Q0 | 129 Pz |
| Field gain (draw / quantum) | 0.0363 |
| Energy-equivalent tier T_E | -3.32 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Dormant rate 0.0001 Pz/s.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Tripwire (0-A-L-TRP) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 0 | 0 | `0000000000001` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | 8 hours | 8 | `0000000010001` |

### Incantation

Spoken as **Causiniy** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T1: *Sicausiniy* · T2: *Hicausiniy* · T3: *Licausiniy* · T4: *Vicausiniy* · T5: *Ticausiniy* · T6: *Ricausiniy* · T7: *Micausiniy* · T8: *Nicausiniy* · T9: *Xyicausiniy*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 | 1 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 4→11 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#a87a2c`.

![[Tripwire (0-A-L-TRP) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 0 | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| School | Abjuration | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| Duration | 8 hours | 0.474 | 0.894 | `#00ff66` (558 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.958 | `#91ff00` (612 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 0.67. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `0·A·None`; the k4 to k6 lines (None, 30 feet, 8 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `0·A·None` |
| Standard spectrometer detection range | 0.22 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 6.4 Pz (0.05 × Q0) |
| Counter drawn cold (all six layers) | 12.9 Pz (0.10 × Q0) |
| Unravel after completion | 13.5 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 0.778 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the Cantrip (Tier 0) quantum of 129 Pz (3.6% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at Cantrip (Tier 0) up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 0 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Linking and Triggers]], [[Walls and Barriers]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Alarm (1-A-L-ALR)|Alarm]] (1) · [[Faraday Cage (1-A-L-FCR)|Faraday Cage]] (1) · [[Glyph of Warding (3-A-H-GWY)|Glyph of Warding]] (3) · [[Magic Link (1-P-L-MLK)|Magic Link]] (1) · [[Magic Mouth (2-I-L-MMG)|Magic Mouth]] (2) · [[Resistance (0-A-L-RSS)|Resistance]] (0) · [[Transfiguration Inheritance (2-T-L-TI)|Transfiguration Inheritance]] (2) · [[Arcane Ward (1-A-L-AW)|Arcane Ward]] (1).


---

## Tactical Assessment

Synchronizes prepared workings. Several bolts held by one tripwire leave together as a volley.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 0 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
