---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-6
  - spell/abjuration
  - source/science-spellbook
aliases:
  - "6th Tier Spell: Summon Demon Core"
  - "6-A-M-SDC"
  - "Summon Demon Core (Science)"
registry_id: 6-A-M-SDC
attribute_code: "6·Abj·Radiant·sphere (10)·30 feet·Until dispelled"
incantation: "Ranat-Seusinis"
tier: 6
school: Abjuration
affinity: A
grade: M
pz_total: 343600.7
pz_quantum: 51944.6
t_e: 7.89
updated: 2026-11-16
---

**Summon Demon Core** (`6-A-M-SDC`) is a 6th Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **343,601 Pz** against a slot quantum of 51,945 Pz, which puts its energy-equivalent tier at T_E 7.89 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 6 Workings]]
      - [[Abjuration]]
        - **Summon Demon Core** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `6-A-M-SDC` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `6·Abj·Radiant·sphere (10)·30 feet·Until dispelled` |
| Incantation | *Ranat-Seusinis* |
| Affinity | A (Abjuration) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 6th Tier |
| School | [[Abjuration]] |
| Casting time | 1 Action |
| Range | 30 feet |
| Area | sphere (10) |
| Duration | Until dispelled |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A screwdriver |
| Ritual | no |
| Injury | 1d10 radiant (mean 5.5) |
| Injury by tier | T6: 1d10, T7: 1d10, T8: 1d10, T9: 1d10 |
| Resistance check | constitution; on success: half injury |
| Practitioner lineages | Wizard, Sorcerer, Warlock |

### Mechanism

Conjures a glowing 1 ft metal sphere near criticality that irradiates everything within 10 ft and can go prompt-critical if handled badly when dispelled.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Core conjured | `116.7 kg x 3 Pz/kg` | 350 |
| Continuous emission (upkeep) | `458.6 Pz per 6 s x 3600 s` | 275,186 |
| Criticality burst (50% weight) | `45 HP x 0.5 (radiant) x S/A_c, S = sphere r=18.29 m = 4202.8 m^2 x 0.5` | 67,546 |
| Pattern cost | `0.01 × Q6 × (1 + 0.00)` | 519 |

| Quantity | Value |
|---|---|
| Effect energy | 67,896 Pz |
| Upkeep energy | 275,186 Pz (76.4 Pz/s) |
| **Total draw** | **343,601 Pz** (515,401.0 kJ) |
| Slot quantum Q6 | 51,945 Pz |
| Field gain (draw / quantum) | 6.61 |
| Energy-equivalent tier T_E | 7.89 |
| Handling points | 0.00 |
| Grade score | 0.94 → M |

**Handling flags:** none.

**Assumptions:** Sphere 116.7 kg of iron-density metal at 3 Pz/kg; continuous emission sized to deliver 1d10 = 5.5 radiant over 10 ft every 6 s (76 Pz/s), held for the 1 hour convention used for open durations; failed removal (taken as 50% likely) bursts at the 60 ft fluence limit 10d8 = 45 radiant.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Summon Demon Core (6-A-M-SDC) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 6 | 6 | `0000000001101` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | Radiant | 11 | `0000000010111` |
| k4 Area | sphere (10) | 27 | `0000000110111` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Until dispelled | 11 | `0000000010111` |

### Incantation

Spoken as **Ranat-Seusinis** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T7: *Miranat-Seusinis* · T8: *Niranat-Seusinis* · T9: *Xyiranat-Seusinis*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 3→2 | 3 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 4→1 | 4 |
| k4 Area | 0→9 1→10 2→11 4→0 5→1 | 5 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 2→9 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#4183b4`.

![[Summon Demon Core (6-A-M-SDC) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 6 | 0.600 | 1.000 | `#00ebff` (520 nm eq.) | source grid |
| Damage | Radiant | 0.786 | 0.983 | `#1900ff` (464 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.835 | `#ff0028` (700 nm eq.) | source grid |
| Duration | Until dispelled | 0.579 | 1.000 | `#00fff7` (526 nm eq.) | source grid |
| Area | sphere (10) | 0.750 | 0.989 | `#0017ff` (475 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.954 | `#91ff00` (612 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 5.54. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `6·A·Radiant`; the k4 to k6 lines (sphere (10), 30 feet, Until dispelled) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `6·A·Radiant` |
| Standard spectrometer detection range | 58.62 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 2,597 Pz (0.05 × Q6) |
| Counter drawn cold (all six layers) | 5,194 Pz (0.10 × Q6) |
| Unravel after completion | 60,232 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Life, Hope and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1b 1c 1d 1H 2i 1J` (Within, Heat, Light, Life, Rigidity, 2x Hope, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 57,267 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 6.61 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 6th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Endures independently once set, which places it under the decay clause of ULMTU-XIII. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIII]] | Lex Impermanentiae | Long-lived patterns drift toward reversion unless refreshed from a source that satisfies ULMTU-I. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 6th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 6 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Summoning and Conjured Creatures]], [[Area Destruction]] |
| Element | [[Radiant Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Guardian of Faith (4-C-L-GFA)|Guardian of Faith]] (4) · [[Burst Radiation (6-V-L-BR)|Burst Radiation]] (6) · [[Sunbeam (6-V-L-SNB)|Sunbeam]] (6) · [[Solve Olber's Paradox (4-I-L-SOSP)|Solve Olber's Paradox]] (4) · [[Sunburst (8-V-L-SNBB)|Sunburst]] (8) · [[Outflows (5-A-L-OTF)|Outflows]] (5) · [[Pauli Exclusion Principle (5-A-L-PEP)|Pauli Exclusion Principle]] (5) · [[Planar Binding (5-A-L-PB)|Planar Binding]] (5).


---

## Tactical Assessment

Area denial device and a hazardous trap for whoever tries to remove it.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 6 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
