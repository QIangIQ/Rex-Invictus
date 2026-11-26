---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-8
  - spell/abjuration
  - source/science-spellbook
aliases:
  - "8th Tier Spell: Medic's Tent"
  - "8-A-L-MSTI"
  - "Medic's Tent (Science)"
registry_id: 8-A-L-MSTI
attribute_code: "8·Abj·None·cylinder (30)·60 feet·1 day"
incantation: "Na’-Xoawynbe"
tier: 8
school: Abjuration
affinity: A
grade: L
pz_total: 23289.7
pz_quantum: 383821.6
t_e: 5.20
updated: 2026-11-16
---

**Medic's Tent** (`8-A-L-MSTI`) is a 8th Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **23,290 Pz** against a slot quantum of 383,822 Pz, which puts its energy-equivalent tier at T_E 5.20 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 8 Workings]]
      - [[Abjuration]]
        - **Medic's Tent** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `8-A-L-MSTI` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `8·Abj·None·cylinder (30)·60 feet·1 day` |
| Incantation | *Na’-Xoawynbe* |
| Affinity | A (Abjuration) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 8th Tier |
| School | [[Abjuration]] |
| Casting time | 1 hour |
| Range | 60 feet |
| Area | cylinder (30) |
| Duration | 1 day |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A tent of any size |
| Ritual | yes |
| Practitioner lineages | Druid, Cleric |

### Mechanism

Raises a glowing illusory tent 30 ft in radius in which all healing works at full strength and recovery from poison, disease and dying is favoured.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Maximised healing | `20 healings x 7.5 x 0.30 Pz` | 45.0 |
| Golden light (upkeep) | `225 W x 86400 s = 1.944e+07 J / 1500` | 12,960 |
| Tent illusion (upkeep) | `illusion rate x 1200 m^3: 0.0024 Pz/s x 86400 s` | 207 |
| Recovery support, 10 patients (upkeep) | `enchantment 0.005 x 10: 0.05 Pz/s x 86400 s` | 4,320 |
| Pattern cost | `0.01 × Q8 × (1 + 0.50)` | 5,757 |

| Quantity | Value |
|---|---|
| Effect energy | 45.0 Pz |
| Upkeep energy | 17,487 Pz (0.202 Pz/s) |
| **Total draw** | **23,290 Pz** (34,934.5 kJ) |
| Slot quantum Q8 | 383,822 Pz |
| Field gain (draw / quantum) | 0.0607 |
| Energy-equivalent tier T_E | 5.20 |
| Handling points | 0.50 |
| Grade score | -0.50 → L |

**Handling flags:** ritual, long cast.

**Assumptions:** Daylong soft light 225 W; illusion volume 1200 m^3; 20 healings gain 7.5 each at 0.30 Pz; recovery support for 10 patients at the enchantment rate for 24 hours.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Medic's Tent (8-A-L-MSTI) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 8 | 8 | `0000000010001` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | cylinder (30) | 37 | `0000001001011` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | 1 day | 19 | `0000000100111` |

### Incantation

Spoken as **Na’-Xoawynbe** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T9: *Xyina’-Xoawynbe*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 4→3 | 2 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 3→12 6→2 | 4 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 2→9 5→12 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#5e6f9c`.

![[Medic's Tent (8-A-L-MSTI) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 8 | 0.800 | 1.000 | `#2900ff` (460 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.726 | `#ff0028` (700 nm eq.) | source grid |
| Duration | 1 day | 0.026 | 0.741 | `#ff0008` (692 nm eq.) | RI half-step |
| Area | cylinder (30) | 0.514 | 0.960 | `#00ff9b` (546 nm eq.) | RI half-step |
| Range | 60 feet | 0.588 | 0.978 | `#00fbff` (524 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 4.37. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `8·A·None`; the k4 to k6 lines (cylinder (30), 60 feet, 1 day) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `8·A·None` |
| Standard spectrometer detection range | 15.26 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 19,191 Pz (0.05 × Q8) |
| Counter drawn cold (all six layers) | 38,382 Pz (0.10 × Q8) |
| Unravel after completion | 41,880 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 3,882 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 8th Tier quantum of 383,822 Pz (6.1% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Endures independently once set, which places it under the decay clause of ULMTU-XIII. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIII]] | Lex Impermanentiae | Long-lived patterns drift toward reversion unless refreshed from a source that satisfies ULMTU-I. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 8th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 8 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Divination and Sensing]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Divine Word (7-V-L-DWV)|Divine Word]] (7) · [[Foresight (9-D-L-FRS)|Foresight]] (9) · [[Antimagic Field (8-A-L-AFT)|Antimagic Field]] (8) · [[Find the Path (6-D-L-FP)|Find the Path]] (6) · [[Holy Aura (8-A-L-HA)|Holy Aura]] (8) · [[Mind Blank (8-A-L-MB)|Mind Blank]] (8) · [[True Seeing (6-D-L-TSU)|True Seeing]] (6) · [[Arcane Hand (5-P-L-AH)|Arcane Hand]] (5).


---

## Tactical Assessment

Field hospital multiplier for a day; made permanent by a year of daily castings at one site.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 8 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
