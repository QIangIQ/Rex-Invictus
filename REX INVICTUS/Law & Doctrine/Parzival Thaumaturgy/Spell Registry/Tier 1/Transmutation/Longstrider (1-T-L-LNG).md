---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/transmutation
  - source/srd
aliases:
  - "1st Tier Spell: Longstrider"
  - "Longstrider"
  - "1-T-L-LNG"
registry_id: 1-T-L-LNG
attribute_code: "1·Tra·None·None·Touch·1 hour"
incantation: "Sielixa"
tier: 1
school: Transmutation
affinity: T
grade: L
pz_total: 198.6
pz_quantum: 350.0
t_e: 0.43
updated: 2026-11-16
---

**Longstrider** (`1-T-L-LNG`) is a 1st Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **199 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E 0.43 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Transmutation]]
        - **Longstrider** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-T-L-LNG` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Tra·None·None·Touch·1 hour` |
| Incantation | *Sielixa* |
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
| Duration | 1 hour |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A pinch of dirt |
| Ritual | no |
| Practitioner lineages | Bard, Druid, Ranger, Wizard |

### Mechanism

The field assists the subject's gait, raising sustained travel speed by about a third for an hour. Energy goes into the additional distance covered.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Assisted extra stride distance (upkeep) | `2 J/(kg m) * 80 kg * (3.048 m / 6 s) / 1500 * 3600 s` | 195 |
| Pattern cost | `0.01 × Q1 × (1 + 0.00)` | 3.5 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 195 Pz (0.0542 Pz/s) |
| **Total draw** | **199 Pz** (297.9 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.567 |
| Energy-equivalent tier T_E | 0.43 |
| Handling points | 0.00 |
| Grade score | -0.28 → L |

**Handling flags:** none.

**Assumptions:** Subject moves continuously for the hour; cost of transport 2 J per kg per m applied to the extra 10 ft per round.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Longstrider (1-T-L-LNG) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | 1 hour | 0 | `0000000000001` |

### Incantation

Spoken as **Sielixa** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisielixa* · T3: *Lisielixa* · T4: *Visielixa* · T5: *Tisielixa* · T6: *Risielixa* · T7: *Misielixa* · T8: *Nisielixa* · T9: *Xyisielixa*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 | 1 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#d3226c`.

![[Longstrider (1-T-L-LNG) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.741 | `#9600ff` (438 nm eq.) | source grid |
| Duration | 1 hour | 0.053 | 0.999 | `#ff1c00` (684 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.736 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.19): swatch `#a54f88`, measured lines at 0.053, 0.101, 0.878. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.30. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·T·None`; the k4 to k6 lines (None, Touch, 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·T·None` |
| Standard spectrometer detection range | 1.41 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 74.0 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 33.1 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (56.7% of it). |
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

Similar workings: [[Expeditious Retreat (1-T-L-ER)|Expeditious Retreat]] (1) · [[Feather Fall (1-T-L-FFA)|Feather Fall]] (1) · [[Jump (1-T-L-JMP)|Jump]] (1) · [[Skyward (1-T-L-SKY)|Skyward]] (1) · [[Accelerate (2-T-L-ACC)|Accelerate]] (2) · [[Levitate (2-T-L-LVT)|Levitate]] (2) · [[Spider Climb (2-T-L-SC)|Spider Climb]] (2) · [[Floating Disk (1-P-M-FD)|Floating Disk]] (1).


---

## Tactical Assessment

Speeds patrols, runners and casualty evacuation on foot. It helps only unmounted personnel.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
