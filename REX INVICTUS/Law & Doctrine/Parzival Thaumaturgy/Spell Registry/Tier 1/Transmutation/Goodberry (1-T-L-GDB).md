---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/transmutation
  - source/srd
aliases:
  - "1st Tier Spell: Goodberry"
  - "Goodberry"
  - "1-T-L-GDB"
registry_id: 1-T-L-GDB
attribute_code: "1·Tra·None·None·Touch·Instantaneous"
incantation: "Sielix"
tier: 1
school: Transmutation
affinity: T
grade: L
pz_total: 564.9
pz_quantum: 350.0
t_e: 1.48
updated: 2026-11-16
---

**Goodberry** (`1-T-L-GDB`) is a 1st Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **565 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E 1.48 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Transmutation]]
        - **Goodberry** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-T-L-GDB` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Tra·None·None·Touch·Instantaneous` |
| Incantation | *Sielix* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Transmutation]] |
| Casting time | 1 action |
| Range | Touch |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A sprig of mistletoe |
| Ritual | no |
| Practitioner lineages | Druid, Ranger |

### Mechanism

Creates ten berries that each repair minor injury and supply a full day's nourishment to whoever eats one within 24 hours.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| healing, 10 berries x 1 HP | `0.30 Pz * 10 HP` | 3.0 |
| berry matter | `10 Pz/kg * 10 * 0.005 kg` | 0.5 |
| nutritional energy | `0.01*10*2000 kcal*4184/1500  [C3]` | 558 |
| Pattern cost | `0.01 × Q1 × (1 + 0.00)` | 3.5 |

| Quantity | Value |
|---|---|
| Effect energy | 561 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **565 Pz** (847.3 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 1.61 |
| Energy-equivalent tier T_E | 1.48 |
| Handling points | 0.00 |
| Grade score | 0.24 → L |

Calibration applied: C3 (Borrowed sustenance), see [[Parzival Energy Budget#Registry calibration rules]].

**Handling flags:** none.

**Assumptions:** Each berry supplies 2000 kcal of real metabolic energy; this term dominates; berry mass 5 g.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Goodberry (1-T-L-GDB) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Sielix** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisielix* · T3: *Lisielix* · T4: *Visielix* · T5: *Tisielix* · T6: *Risielix* · T7: *Misielix* · T8: *Nisielix* · T9: *Xyisielix*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#d31a77`.

![[Goodberry (1-T-L-GDB) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.741 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.995 | `#ff0028` (700 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.736 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.18): swatch `#9e4d8f`, measured lines at 0.004, 0.101, 0.878. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.75. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·T·None`; the k4 to k6 lines (None, Touch, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·T·None` |
| Standard spectrometer detection range | 2.38 km (r = 1 km × √(E/100 Pz)) |
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
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 94.1 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 1.61 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 1st Tier pattern; a degraded pattern falls back to the quantum. |
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
| Function | [[Healing and Restoration]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Reverse Entropy (0-T-L-REV)|Reverse Entropy]] (0) · [[Thomson's Plum Pudding (2-T-L-TSPP)|Thomson's Plum Pudding]] (2) · [[Cure Wounds (1-V-L-CW)|Cure Wounds]] (1) · [[Healing Word (1-V-L-HW)|Healing Word]] (1) · [[Lesser Restoration (2-A-L-LR)|Lesser Restoration]] (2) · [[Prayer of Healing (2-V-L-PH)|Prayer of Healing]] (2) · [[Spare the Dying (0-N-L-SD)|Spare the Dying]] (0) · [[Alter Weight (1-T-L-AWT)|Alter Weight]] (1).


---

## Tactical Assessment

Field rations for ten soldier-days in a pocket, removing a supply line for small units in hostile terrain.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
