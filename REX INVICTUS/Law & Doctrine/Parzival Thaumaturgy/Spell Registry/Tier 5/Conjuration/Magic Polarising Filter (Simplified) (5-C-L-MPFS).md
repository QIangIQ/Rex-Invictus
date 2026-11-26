---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/conjuration
  - source/science-spellbook
aliases:
  - "5th Tier Spell: Magic Polarising Filter (Simplified)"
  - "5-C-L-MPFS"
  - "Magic Polarising Filter (Simplified) (Science)"
registry_id: 5-C-L-MPFS
attribute_code: "5·Con·None·line (60)·30 feet·Up to 10 minutes"
incantation: "Te’-Leusinly"
tier: 5
school: Conjuration
affinity: C
grade: L
pz_total: 253.9
pz_quantum: 19109.4
t_e: 0.68
updated: 2026-11-16
---

**Magic Polarising Filter (Simplified)** (`5-C-L-MPFS`) is a 5th Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **254 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 0.68 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Conjuration]]
        - **Magic Polarising Filter (Simplified)** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-C-L-MPFS` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Con·None·line (60)·30 feet·Up to 10 minutes` |
| Incantation | *Te’-Leusinly* |
| Affinity | C (Conjuration) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Conjuration]] |
| Casting time | 1 Action |
| Range | 30 feet |
| Area | line (60) |
| Duration | Up to 10 minutes (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A coloured shard of glass |
| Ritual | no |
| Practitioner lineages | Wizard |

### Mechanism

Raises a 60 ft by 20 ft transparent wall that halves workings crossing it from the disfavoured side of its normal.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Filtered injury | `0.20 x 7.5 x 10 rounds` | 15.0 |
| Pattern cost | `0.01 × Q5 × (1 + 0.25)` | 239 |

| Quantity | Value |
|---|---|
| Effect energy | 15.0 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **254 Pz** (380.8 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 0.0133 |
| Energy-equivalent tier T_E | 0.68 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** concentration.

**Assumptions:** Incoming crossing workings 30 injury per round, half of them from the disfavoured side and halved: 7.5 absorbed per round for 10 rounds, 0.20 Pz each.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Magic Polarising Filter (Simplified) (5-C-L-MPFS) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | line (60) | 25 | `0000000110011` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Up to 10 minutes | 15 | `0000000011111` |

### Incantation

Spoken as **Te’-Leusinly** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Rite’-Leusinly* · T7: *Mite’-Leusinly* · T8: *Nite’-Leusinly* · T9: *Xyite’-Leusinly*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 4→0 5→1 | 4 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 2→9 3→10 4→11 | 5 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#549682`.

![[Magic Polarising Filter (Simplified) (5-C-L-MPFS) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.932 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Up to 10 minutes | 0.789 | 0.959 | `#1e00ff` (463 nm eq.) | source grid |
| Area | line (60) | 0.694 | 0.981 | `#0069ff` (492 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.979 | `#91ff00` (612 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 2.40. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·C·None`; the k4 to k6 lines (line (60), 30 feet, Up to 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·C·None` |
| Standard spectrometer detection range | 1.59 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 1,911 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 42.3 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 5th Tier quantum of 19,109 Pz (1.3% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
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
| Function | [[Walls and Barriers]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Magic Polarising Filter (4-C-L-MPF)|Magic Polarising Filter]] (4) · [[Wall of Thorns (6-C-L-WT)|Wall of Thorns]] (6) · [[Passwall (5-T-L-PSS)|Passwall]] (5) · [[Wall of Force (5-P-L-WFL)|Wall of Force]] (5) · [[Wall of Stone (5-V-M-WS)|Wall of Stone]] (5) · [[Blade Barrier (6-V-L-BB)|Blade Barrier]] (6) · [[Wall of Fire (4-V-M-WF)|Wall of Fire]] (4) · [[Wall of Ice (6-V-M-WI)|Wall of Ice]] (6).


---

## Tactical Assessment

Defensive line against enemy casters that leaves physical traffic unaffected.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
