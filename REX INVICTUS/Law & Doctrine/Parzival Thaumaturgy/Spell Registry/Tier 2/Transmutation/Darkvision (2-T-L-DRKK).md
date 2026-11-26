---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/transmutation
  - source/srd
aliases:
  - "2nd Tier Spell: Darkvision"
  - "Darkvision"
  - "2-T-L-DRKK"
registry_id: 2-T-L-DRKK
attribute_code: "2·Tra·None·None·Touch·8 hours"
incantation: "Hielixiy"
tier: 2
school: Transmutation
affinity: T
grade: L
pz_total: 62.7
pz_quantum: 951.4
t_e: -0.72
updated: 2026-11-16
---

**Darkvision** (`2-T-L-DRKK`) is a 2nd Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **62.7 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E -0.72 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Transmutation]]
        - **Darkvision** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-T-L-DRKK` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Tra·None·None·Touch·8 hours` |
| Incantation | *Hielixiy* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Transmutation]] |
| Casting time | 1 action |
| Range | Touch |
| Area | single point or target |
| Duration | 8 hours |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Either a pinch of dried carrot or an agate |
| Ritual | no |
| Practitioner lineages | Druid, Ranger, Sorcerer, Wizard |

### Mechanism

A touch extends the subject eyes into low-light vision out to 60 ft for 8 hours.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| retina sensitivity shift | `0.5` | 0.5 |
| upkeep: low-light perception to 60 ft for 8 h (divination rate) | `0.001*(60*ft/10)*8*3600` | 52.7 |
| Pattern cost | `0.01 × Q2 × (1 + 0.00)` | 9.5 |

| Quantity | Value |
|---|---|
| Effect energy | 0.5 Pz |
| Upkeep energy | 52.7 Pz (0.00183 Pz/s) |
| **Total draw** | **62.7 Pz** (94.0 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.0659 |
| Energy-equivalent tier T_E | -0.72 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Modeled with the divination rate at 18.3 m range for 28800 s.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Darkvision (2-T-L-DRKK) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | 8 hours | 8 | `0000000010001` |

### Incantation

Spoken as **Hielixiy** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihielixiy* · T4: *Vihielixiy* · T5: *Tihielixiy* · T6: *Rihielixiy* · T7: *Mihielixiy* · T8: *Nihielixiy* · T9: *Xyihielixiy*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 4→11 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#8b878d`.

![[Darkvision (2-T-L-DRKK) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.796 | `#9600ff` (438 nm eq.) | source grid |
| Duration | 8 hours | 0.474 | 0.963 | `#00ff66` (558 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.792 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.15): swatch `#8e8cb4`, measured lines at 0.201, 0.474, 0.878. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.80. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·T·None`; the k4 to k6 lines (None, Touch, 8 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·T·None` |
| Standard spectrometer detection range | 0.79 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 106 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 10.4 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (6.6% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Divination and Sensing]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Alter Projectile Velocity (2-T-L-APV)|Alter Projectile Velocity]] (2) · [[Knock (2-T-L-KNC)|Knock]] (2) · [[Speak with Plants (3-T-L-SP)|Speak with Plants]] (3) · [[Animal Messenger (2-E-L-AM)|Animal Messenger]] (2) · [[Arcanist's Magic Aura (2-I-L-ASMA)|Arcanist's Magic Aura]] (2) · [[Augury (2-D-L-AGR)|Augury]] (2) · [[Blindness-Deafness (2-N-L-BD)|Blindness/Deafness]] (2) · [[Detect Thoughts (2-D-L-DT)|Detect Thoughts]] (2).


---

## Tactical Assessment

A substitute for night-vision equipment for one soldier for a full night patrol.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
