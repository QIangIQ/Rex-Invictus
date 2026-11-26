---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/conjuration
  - source/science-spellbook
aliases:
  - "4th Tier Spell: Conjure Magic Prism"
  - "4-C-L-CMPJ"
  - "Conjure Magic Prism (Science)"
registry_id: 4-C-L-CMPJ
attribute_code: "4·Con·None·cone (15)·30 feet·Up to 1 minute"
incantation: "Ve’-Nuusinse"
tier: 4
school: Conjuration
affinity: C
grade: L
pz_total: 892.5
pz_quantum: 7029.9
t_e: 1.94
updated: 2026-11-16
---

**Conjure Magic Prism** (`4-C-L-CMPJ`) is a 4th Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **893 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E 1.94 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Conjuration]]
        - **Conjure Magic Prism** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-C-L-CMPJ` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Con·None·cone (15)·30 feet·Up to 1 minute` |
| Incantation | *Ve’-Nuusinse* |
| Affinity | C (Conjuration) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Conjuration]] |
| Casting time | 1 Action |
| Range | 30 feet |
| Area | cone (15) |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A small glass prism |
| Ritual | no |
| Practitioner lineages | Wizard |

### Mechanism

Conjures a floating glass prism that splits any single-target damaging working cast through it into a 15 ft cone.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Glass prism conjured | `0.5 kg x 3 Pz/kg` | 1.5 |
| Prism hover (upkeep) | `0.02 x 0.5 kg x 9.81 x 60 s / 1500` | 0.0039 |
| Spreading routed workings (upkeep) | `3 x (18.0 HP fire cone 15 ft - ray F 0.5) = 3 x 244.3` | 733 |
| Pattern cost | `0.01 × Q4 × (1 + 1.25)` | 158 |

| Quantity | Value |
|---|---|
| Effect energy | 1.5 Pz |
| Upkeep energy | 733 Pz (12.2 Pz/s) |
| **Total draw** | **893 Pz** (1,338.8 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 0.127 |
| Energy-equivalent tier T_E | 1.94 |
| Handling points | 1.25 |
| Grade score | 0.25 → L |

**Handling flags:** concentration, fragile.

**Assumptions:** Prism 0.5 kg structured solid; hover for 1 minute; three routed workings, each a reference 4d8 = 18 fire ray, spread to a 15 ft cone (extra 244 Pz each).

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Conjure Magic Prism (4-C-L-CMPJ) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 4 | 4 | `0000000001001` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | cone (15) | 1 | `0000000000011` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Ve’-Nuusinse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T5: *Tive’-Nuusinse* · T6: *Rive’-Nuusinse* · T7: *Mive’-Nuusinse* · T8: *Nive’-Nuusinse* · T9: *Xyive’-Nuusinse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 3→2 | 2 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 | 2 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#819933`.

![[Conjure Magic Prism (4-C-L-CMPJ) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.963 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.960 | `#0074ff` (495 nm eq.) | source grid |
| Area | cone (15) | 0.028 | 0.933 | `#ff0003` (692 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.994 | `#91ff00` (612 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 2.95. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·C·None`; the k4 to k6 lines (cone (15), 30 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·C·None` |
| Standard spectrometer detection range | 2.99 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 850 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 149 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 4th Tier quantum of 7,030 Pz (12.7% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 4th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 4 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Summoning and Conjured Creatures]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Conjure Minor Elementals (4-C-M-CME)|Conjure Minor Elementals]] (4) · [[Conjure Woodland Beings (4-C-L-CWB)|Conjure Woodland Beings]] (4) · [[Faithful Hound (4-C-L-FH)|Faithful Hound]] (4) · [[Guardian of Faith (4-C-L-GFA)|Guardian of Faith]] (4) · [[Magic Polarising Filter (4-C-L-MPF)|Magic Polarising Filter]] (4) · [[Arcane Singularity (3-C-L-ASA)|Arcane Singularity]] (3) · [[Conjure Animals (3-C-M-CA)|Conjure Animals]] (3) · [[Conjure Elemental (5-C-M-CEN)|Conjure Elemental]] (5).


---

## Tactical Assessment

Turns precision weapons into area weapons against clustered infantry; the prism is a fragile target.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
