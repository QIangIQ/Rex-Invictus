---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/conjuration
  - source/srd
aliases:
  - "5th Tier Spell: Insect Plague"
  - "Insect Plague"
  - "5-C-L-IP"
registry_id: 5-C-L-IP
attribute_code: "5·Con·Piercing·sphere (20)·300 feet·Up to 10 minutes"
incantation: "Teix-Sosphinly"
tier: 5
school: Conjuration
affinity: C
grade: L
pz_total: 21768.9
pz_quantum: 19109.4
t_e: 5.13
updated: 2026-11-16
---

**Insect Plague** (`5-C-L-IP`) is a 5th Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **21,769 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 5.13 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Conjuration]]
        - **Insect Plague** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-C-L-IP` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Con·Piercing·sphere (20)·300 feet·Up to 10 minutes` |
| Incantation | *Teix-Sosphinly* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | 300 feet |
| Area | sphere (20) |
| Duration | Up to 10 minutes (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A few grains of sugar, some kernels of grain, and a smear of fat |
| Ritual | no |
| Injury | 4d10 piercing (mean 22) |
| Injury by tier | T5: 4d10, T6: 5d10, T7: 6d10, T8: 7d10, T9: 8d10 |
| Resistance check | constitution; on success: half injury |
| Practitioner lineages | Cleric, Druid, Sorcerer |

### Mechanism

The field assembles a dense locust swarm in a 20 ft radius sphere and keeps it biting anything inside for up to 10 minutes. The swarm also obscures vision and slows movement through the area.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Biting swarm, initial exposure | `22 HP * 0.35 * (467.0 m^2 / 0.7)` | 5,137 |
| Repeat exposure, 3 rounds | `3 * 22 HP * 0.35 * (467.0 m^2 / 0.7)` | 15,410 |
| Conjured locust biomass | `10 Pz/kg * (948.9 m^3 * 0.1 kg/m^3)` | 949 |
| Swarm autonomy (one aggregate swarm) (upkeep) | `0.05 Pz/s * 1 * 600 s` | 30.0 |
| Pattern cost | `0.01 × Q5 × (1 + 0.25)` | 239 |

| Quantity | Value |
|---|---|
| Effect energy | 21,500 Pz |
| Upkeep energy | 30.0 Pz (0.05 Pz/s) |
| **Total draw** | **21,769 Pz** (32,653.3 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 1.14 |
| Energy-equivalent tier T_E | 5.13 |
| Handling points | 0.25 |
| Grade score | 0.32 → L |

**Handling flags:** concentration.

**Assumptions:** Sphere 20 ft radius; 4d10 = 22 per exposure, full value; initial plus 3 repeats; swarm density 0.1 kg/m^3; swarm treated as one summoned entity over 10 minutes.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Insect Plague (5-C-L-IP) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | Piercing | 8 | `0000000010001` |
| k4 Area | sphere (20) | 30 | `0000000111101` |
| k5 Range | 300 feet | 6 | `0000000001101` |
| k6 Duration | Up to 10 minutes | 15 | `0000000011111` |

### Incantation

Spoken as **Teix-Sosphinly** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Riteix-Sosphinly* · T7: *Miteix-Sosphinly* · T8: *Niteix-Sosphinly* · T9: *Xyiteix-Sosphinly*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 4→1 | 2 |
| k4 Area | 0→9 2→11 3→12 4→0 5→1 | 5 |
| k5 Range | 0→8 2→10 3→11 | 3 |
| k6 Duration | 0→7 1→8 2→9 3→10 4→11 | 5 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#479793`.

![[Insect Plague (5-C-L-IP) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| Damage | Piercing | 0.571 | 0.997 | `#00ffec` (529 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.932 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Up to 10 minutes | 0.789 | 0.959 | `#1e00ff` (463 nm eq.) | source grid |
| Area | sphere (20) | 0.833 | 0.946 | `#5a00ff` (450 nm eq.) | source grid |
| Range | 300 feet | 0.353 | 0.989 | `#40ff00` (594 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.19): swatch `#94bb99`, measured lines at 0.126, 0.354, 0.501, 0.572, 0.790, 0.834. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.34. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·C·Piercing`; the k4 to k6 lines (sphere (20), 300 feet, Up to 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·C·Piercing` |
| Standard spectrometer detection range | 14.75 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 1,917 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Beyond, Cold, Hopelessness, Movement and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `2a 1B 1e 1F 1I 2j` (2x Beyond, Cold, Prodigious, Potential, Hopelessness, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 3,628 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 1.14 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 5th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 5th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 5 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Area Destruction]] |
| Element | [[Piercing Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Wall of Thorns (6-C-L-WT)|Wall of Thorns]] (6) · [[Cloudkill (5-C-L-CLD)|Cloudkill]] (5) · [[Supersonic Omnidirectional Jet (5-C-M-SOJ)|Supersonic Omnidirectional Jet]] (5) · [[Black Tentacles (4-C-L-BT)|Black Tentacles]] (4) · [[Faithful Hound (4-C-L-FH)|Faithful Hound]] (4) · [[Guardian of Faith (4-C-L-GFA)|Guardian of Faith]] (4) · [[Call Lightning (3-C-L-CLL)|Call Lightning]] (3) · [[Cone of Cold (5-V-L-CC)|Cone of Cold]] (5).


---

## Tactical Assessment

Denies an area to unarmoured troops for an extended period and harasses crews of open vehicles. Sealed armour and environmental suits largely negate it.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
