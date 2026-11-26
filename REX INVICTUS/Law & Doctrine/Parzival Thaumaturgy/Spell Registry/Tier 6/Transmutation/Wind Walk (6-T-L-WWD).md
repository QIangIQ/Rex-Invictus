---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-6
  - spell/transmutation
  - source/srd
aliases:
  - "6th Tier Spell: Wind Walk"
  - "Wind Walk"
  - "6-T-L-WWD"
registry_id: 6-T-L-WWD
attribute_code: "6·Tra·None·None·30 feet·8 hours"
incantation: "Rieusiniy"
tier: 6
school: Transmutation
affinity: T
grade: L
pz_total: 12832.3
pz_quantum: 51944.6
t_e: 4.60
updated: 2026-11-16
---

**Wind Walk** (`6-T-L-WWD`) is a 6th Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **12,832 Pz** against a slot quantum of 51,945 Pz, which puts its energy-equivalent tier at T_E 4.60 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 6 Workings]]
      - [[Transmutation]]
        - **Wind Walk** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `6-T-L-WWD` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `6·Tra·None·None·30 feet·8 hours` |
| Incantation | *Rieusiniy* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 6th Tier |
| School | [[Transmutation]] |
| Casting time | 1 minute |
| Range | 30 feet |
| Area | single point or target |
| Duration | 8 hours |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Fire and holy water |
| Ritual | no |
| Practitioner lineages | Druid |

### Mechanism

Up to eleven subjects become drifting cloud for eight hours, flying at about 15 m/s and shrugging off ordinary weapons; changing form takes a minute.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Gaseous restructuring, 11 bodies | `10 Pz/kg * 880 kg` | 8,800 |
| Acceleration to 15.24 m/s | `0.5 * 880 * 15.24^2 / 1500` | 68.1 |
| Upkeep: Buoyant flight support, 8 h | `0.02 * 880 * 9.81 * 28800 / 1500` | 3,315 |
| Pattern cost | `0.01 × Q6 × (1 + 0.25)` | 649 |

| Quantity | Value |
|---|---|
| Effect energy | 8,868 Pz |
| Upkeep energy | 3,315 Pz (0.115 Pz/s) |
| **Total draw** | **12,832 Pz** (19,248.5 kJ) |
| Slot quantum Q6 | 51,945 Pz |
| Field gain (draw / quantum) | 0.247 |
| Energy-equivalent tier T_E | 4.60 |
| Handling points | 0.25 |
| Grade score | -0.45 → L |

**Handling flags:** long cast.

**Assumptions:** 11 x 80 kg; one transformation each way counted once; flight for full duration.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Wind Walk (6-T-L-WWD) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 6 | 6 | `0000000001101` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | 8 hours | 8 | `0000000010001` |

### Incantation

Spoken as **Rieusiniy** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T7: *Mirieusiniy* · T8: *Nirieusiniy* · T9: *Xyirieusiniy*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 3→2 | 3 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 4→11 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#48bb99`.

![[Wind Walk (6-T-L-WWD) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 6 | 0.600 | 1.000 | `#00ebff` (520 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.963 | `#9600ff` (438 nm eq.) | source grid |
| Duration | 8 hours | 0.474 | 0.992 | `#00ff66` (558 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.954 | `#91ff00` (612 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 4.11. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `6·T·None`; the k4 to k6 lines (None, 30 feet, 8 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `6·T·None` |
| Standard spectrometer detection range | 11.33 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 2,597 Pz (0.05 × Q6) |
| Counter drawn cold (all six layers) | 5,194 Pz (0.10 × Q6) |
| Unravel after completion | 5,857 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 2,139 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 6th Tier quantum of 51,945 Pz (24.7% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 6th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 6 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Movement and Flight]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Reverse Gravity (7-T-L-RG)|Reverse Gravity]] (7) · [[Sequester (7-T-L-SQS)|Sequester]] (7) · [[Telekinesis (5-P-L-TLK)|Telekinesis]] (5) · [[Freefall (4-T-L-FRF)|Freefall]] (4) · [[Fly (3-T-L-FLY)|Fly]] (3) · [[Gaseous Form (3-T-M-GF)|Gaseous Form]] (3) · [[Haste (3-T-L-HST)|Haste]] (3) · [[Slow (3-T-L-SLW)|Slow]] (3).


---

## Tactical Assessment

Long-range covert movement of a team over hostile terrain with low sensor signature.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 6 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
