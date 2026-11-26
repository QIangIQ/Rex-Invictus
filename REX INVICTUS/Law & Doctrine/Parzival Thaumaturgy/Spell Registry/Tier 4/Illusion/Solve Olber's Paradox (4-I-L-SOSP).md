---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/illusion
  - source/science-spellbook
aliases:
  - "4th Tier Spell: Solve Olber's Paradox"
  - "4-I-L-SOSP"
  - "Solve Olber's Paradox (Science)"
registry_id: 4-I-L-SOSP
attribute_code: "4·Ill·Radiant·sphere (30)·120 feet·Up to 1 minute"
incantation: "Vainat-Sormulse"
tier: 4
school: Illusion
affinity: I
grade: L
pz_total: 10219.7
pz_quantum: 7029.9
t_e: 4.37
updated: 2026-11-16
---

**Solve Olber's Paradox** (`4-I-L-SOSP`) is a 4th Tier working of the [[Illusion]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **10,220 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E 4.37 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Illusion]]
        - **Solve Olber's Paradox** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-I-L-SOSP` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Ill·Radiant·sphere (30)·120 feet·Up to 1 minute` |
| Incantation | *Vainat-Sormulse* |
| Affinity | I (Illusion) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Illusion]] |
| Casting time | 1 Action |
| Range | 120 feet |
| Area | sphere (30) |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation) |
| Ritual | no |
| Injury | 3d8 radiant (mean 13.5) |
| Injury by tier | T4: 3d8, T5: 3d8, T6: 3d8, T7: 3d8, T8: 3d8, T9: 3d8 |
| Resistance check | constitution; on success: half injury |
| Practitioner lineages | Wizard, Sorcerer, Warlock, Bard |

### Mechanism

Floods everyone within 30 ft of a point with the light of a sky filled with stars, burning and blinding them.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Radiant sky | `13.5 HP x 0.5 (radiant) x S/A_c, S = sphere r=9.144 m = 1050.7 m^2` | 10,132 |
| Pattern cost | `0.01 × Q4 × (1 + 0.25)` | 87.9 |

| Quantity | Value |
|---|---|
| Effect energy | 10,132 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **10,220 Pz** (15,329.6 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 1.45 |
| Energy-equivalent tier T_E | 4.37 |
| Handling points | 0.25 |
| Grade score | 0.44 → L |

**Handling flags:** concentration.

**Assumptions:** Radiant 3d8 = 13.5 over a 30 ft sphere; the perceived sky itself is an illusion.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Solve Olber's Paradox (4-I-L-SOSP) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 4 | 4 | `0000000001001` |
| k2 School | Illusion | 5 | `0000000001011` |
| k3 Damage | Radiant | 11 | `0000000010111` |
| k4 Area | sphere (30) | 31 | `0000000111111` |
| k5 Range | 120 feet | 3 | `0000000000111` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Vainat-Sormulse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T5: *Tivainat-Sormulse* · T6: *Rivainat-Sormulse* · T7: *Mivainat-Sormulse* · T8: *Nivainat-Sormulse* · T9: *Xyivainat-Sormulse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 3→2 | 2 |
| k2 School | 0→11 1→12 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 4→1 | 4 |
| k4 Area | 0→9 1→10 2→11 3→12 4→0 5→1 | 6 |
| k5 Range | 0→8 1→9 2→10 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#4383a7`.

![[Solve Olber's Paradox (4-I-L-SOSP) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| Damage | Radiant | 0.786 | 0.928 | `#1900ff` (464 nm eq.) | source grid |
| School | Illusion | 0.625 | 0.975 | `#00c5ff` (512 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.960 | `#0074ff` (495 nm eq.) | source grid |
| Area | sphere (30) | 0.861 | 0.899 | `#8000ff` (442 nm eq.) | source grid |
| Range | 120 feet | 0.176 | 0.975 | `#ffc900` (647 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 4.01. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·I·Radiant`; the k4 to k6 lines (sphere (30), 120 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·I·Radiant` |
| Standard spectrometer detection range | 10.11 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 703 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Life, Hope and the school lean is Light, Introspection, 2x Flexibility. The working vector used by [[Recast Tension and Combination Affinity]] is `1b 2c 1d 1G 2h 1i` (Heat, 2x Light, Life, Introspection, 2x Flexibility, Hope).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1,703 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 1.45 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 4th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 4th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Illusion school with aspect lean Light, Introspection, 2x Flexibility. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 4 Workings]] |
| School | [[Illusion]] |
| Affinity | [[Illusion]] (I) |
| Function | [[Area Destruction]] |
| Element | [[Radiant Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Guardian of Faith (4-C-L-GFA)|Guardian of Faith]] (4) · [[Burst Radiation (6-V-L-BR)|Burst Radiation]] (6) · [[Moonbeam (2-V-M-MNB)|Moonbeam]] (2) · [[Summon Demon Core (6-A-M-SDC)|Summon Demon Core]] (6) · [[Sunbeam (6-V-L-SNB)|Sunbeam]] (6) · [[Black Tentacles (4-C-L-BT)|Black Tentacles]] (4) · [[Control Water (4-T-H-CWN)|Control Water]] (4) · [[Fire Shield (4-V-L-FSR)|Fire Shield]] (4).


---

## Tactical Assessment

Blinds and burns a fire team in one action.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Illusion]] · [[Spell Breakdown Procedure]] · [[Parzival]]
