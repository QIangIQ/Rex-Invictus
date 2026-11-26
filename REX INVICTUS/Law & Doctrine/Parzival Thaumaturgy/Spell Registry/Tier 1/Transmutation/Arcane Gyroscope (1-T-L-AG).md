---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/transmutation
  - source/science-spellbook
aliases:
  - "1st Tier Spell: Arcane Gyroscope"
  - "1-T-L-AG"
  - "Arcane Gyroscope (Science)"
registry_id: 1-T-L-AG
attribute_code: "1·Tra·None·None·Touch·1 hour"
incantation: "Sielixa"
tier: 1
school: Transmutation
affinity: T
grade: L
pz_total: 21.5
pz_quantum: 350.0
t_e: -1.79
updated: 2026-11-16
---

**Arcane Gyroscope** (`1-T-L-AG`) is a 1st Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **21.5 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -1.79 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Transmutation]]
        - **Arcane Gyroscope** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-T-L-AG` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Tra·None·None·Touch·1 hour` |
| Incantation | *Sielixa* |
| Affinity | T (Transmutation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Transmutation]] |
| Casting time | 1 Action |
| Range | Touch |
| Area | single point or target |
| Duration | 1 hour |
| Components | spoken (incantation), material focus. Material: A spinning top |
| Ritual | no |
| Practitioner lineages | Wizard |

### Mechanism

Installs a corrective balance field in one willing body that counters tipping torques for an hour.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Balance field, 1 creature (upkeep) | `enchantment rate: 0.005 Pz/s x 3600 s` | 18.0 |
| Pattern cost | `0.01 × Q1 × (1 + 0.00)` | 3.5 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 18.0 Pz (0.005 Pz/s) |
| **Total draw** | **21.5 Pz** (32.2 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.0614 |
| Energy-equivalent tier T_E | -1.79 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Treated as a one-creature enchantment at 0.005 Pz/s for 1 hour; the physical corrective torque is a few watts and is covered by that rate.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Arcane Gyroscope (1-T-L-AG) glyph.svg]]

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

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]]. This attribute set is shared with other workings, so the glyph carries 1 centre dot(s) to tell it apart.

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

![[Arcane Gyroscope (1-T-L-AG) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.741 | `#9600ff` (438 nm eq.) | source grid |
| Duration | 1 hour | 0.053 | 0.999 | `#ff1c00` (684 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.736 | `#9b00ff` (435 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 1.33. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·T·None`; the k4 to k6 lines (None, Touch, 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·T·None` |
| Standard spectrometer detection range | 0.46 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 38.6 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 3.6 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (6.1% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Utility Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Alter Weight (1-T-L-AWT)|Alter Weight]] (1) · [[Vapour Deposition (1-T-L-VD)|Vapour Deposition]] (1) · [[Magnetise (2-T-L-MGN)|Magnetise]] (2) · [[Momentum Transfer (2-T-L-MT)|Momentum Transfer]] (2) · [[Ladder Operation (1-E-L-LOD)|Ladder Operation]] (1) · [[Pascal's Revenge (1-I-L-PSR)|Pascal's Revenge]] (1) · [[Reverb (1-I-L-RVR)|Reverb]] (1) · [[Sublimation (3-T-L-SBL)|Sublimation]] (3).


---

## Tactical Assessment

Keeps troops steady on ship decks, moving vehicles, rope lines and broken ground; improves boarding actions.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
