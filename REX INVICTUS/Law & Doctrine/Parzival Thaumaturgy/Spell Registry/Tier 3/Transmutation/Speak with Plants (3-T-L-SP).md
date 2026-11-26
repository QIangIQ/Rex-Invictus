---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/transmutation
  - source/srd
aliases:
  - "3rd Tier Spell: Speak with Plants"
  - "Speak with Plants"
  - "3-T-L-SP"
registry_id: 3-T-L-SP
attribute_code: "3·Tra·None·sphere (30)·Self·10 minutes"
incantation: "Lie’-Sorpors"
tier: 3
school: Transmutation
affinity: T
grade: L
pz_total: 86.9
pz_quantum: 2586.2
t_e: -0.39
updated: 2026-11-16
---

**Speak with Plants** (`3-T-L-SP`) is a 3rd Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **86.9 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E -0.39 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Transmutation]]
        - **Speak with Plants** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-T-L-SP` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Tra·None·sphere (30)·Self·10 minutes` |
| Incantation | *Lie’-Sorpors* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Transmutation]] |
| Casting time | 1 action |
| Range | Self |
| Area | sphere (30) |
| Duration | 10 minutes |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Bard, Druid, Ranger |

### Mechanism

Vegetation within 9 m gains limited awareness and motor control of branches and stalks, and can report recent events and reshape the terrain into or out of obstruction.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Kinetic work, first branch motion | `0.5 * 525 kg * (1 m/s)^2 / 1500` | 0.175 |
| Upkeep: Branch and tendril motion | `0.5*525 kg*(1 m/s)^2 per 6 s round * 100 rounds / 1500` | 17.3 |
| Upkeep: Sentience given to plant community (10 effective agents) | `0.005 Pz/s * 10 * 600 s` | 30.0 |
| Upkeep: Recall of the past day in a 30 ft radius | `0.001 Pz/s * (9.144/10) * 600 s` | 0.549 |
| Pattern cost | `0.01 × Q3 × (1 + 0.50)` | 38.8 |

| Quantity | Value |
|---|---|
| Effect energy | 0.175 Pz |
| Upkeep energy | 47.9 Pz (0.0801 Pz/s) |
| **Total draw** | **86.9 Pz** (130.3 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 0.0336 |
| Energy-equivalent tier T_E | -0.39 |
| Handling points | 0.50 |
| Grade score | -0.50 → L |

**Handling flags:** multi target control.

**Assumptions:** Moved vegetation 2 kg/m^2 over 263 m^2 at 1 m/s once per round; plant community counted as 10 agents.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Speak with Plants (3-T-L-SP) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (30) | 31 | `0000000111111` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | 10 minutes | 4 | `0000000001001` |

### Incantation

Spoken as **Lie’-Sorpors** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vilie’-Sorpors* · T5: *Tilie’-Sorpors* · T6: *Rilie’-Sorpors* · T7: *Milie’-Sorpors* · T8: *Nilie’-Sorpors* · T9: *Xyilie’-Sorpors*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 2→11 3→12 4→0 5→1 | 6 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 3→10 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#7a7f90`.

![[Speak with Plants (3-T-L-SP) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.848 | `#9600ff` (438 nm eq.) | source grid |
| Duration | 10 minutes | 0.263 | 0.999 | `#bdff00` (621 nm eq.) | source grid |
| Area | sphere (30) | 0.861 | 0.854 | `#8000ff` (442 nm eq.) | source grid |
| Range | Self | 0.706 | 0.921 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.23): swatch `#86a1b8`, measured lines at 0.264, 0.300, 0.706, 0.872. One or more predicted lines have no measured counterpart; the plate may merge overlapping lines.

Relative luminosity scales with initial energy: log10(E) = 1.94. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·T·None`; the k4 to k6 lines (sphere (30), Self, 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·T·None` |
| Standard spectrometer detection range | 0.93 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 268 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 14.5 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 3rd Tier quantum of 2,586 Pz (3.4% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Divination and Sensing]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Alter Projectile Velocity (2-T-L-APV)|Alter Projectile Velocity]] (2) · [[Darkvision (2-T-L-DRKK)|Darkvision]] (2) · [[Knock (2-T-L-KNC)|Knock]] (2) · [[Suspend Motion (4-T-L-SMS)|Suspend Motion]] (4) · [[Arcane Singularity (3-C-L-ASA)|Arcane Singularity]] (3) · [[Awaken (5-T-H-AWK)|Awaken]] (5) · [[Clairvoyance (3-D-L-CLR)|Clairvoyance]] (3) · [[Nondetection (3-A-L-NND)|Nondetection]] (3).


---

## Tactical Assessment

Useful for route denial in woodland, for clearing an approach, and for questioning plants about traffic through an area in the past day.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
