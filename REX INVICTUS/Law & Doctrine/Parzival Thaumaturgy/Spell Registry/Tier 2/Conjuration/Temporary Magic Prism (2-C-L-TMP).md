---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/conjuration
  - source/science-spellbook
aliases:
  - "2nd Tier Spell: Temporary Magic Prism"
  - "2-C-L-TMP"
  - "Temporary Magic Prism (Science)"
registry_id: 2-C-L-TMP
attribute_code: "2·Con·None·cone (15)·Self·until the end of your turn or a spell is cast through the prism"
incantation: "He’-Nuporbes"
tier: 2
school: Conjuration
affinity: C
grade: L
pz_total: 255.3
pz_quantum: 951.4
t_e: 0.68
updated: 2026-11-16
---

**Temporary Magic Prism** (`2-C-L-TMP`) is a 2nd Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **255 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E 0.68 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Conjuration]]
        - **Temporary Magic Prism** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-C-L-TMP` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Con·None·cone (15)·Self·until the end of your turn or a spell is cast through the prism` |
| Incantation | *He’-Nuporbes* |
| Affinity | C (Conjuration) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Conjuration]] |
| Casting time | 1 Bonus Action |
| Range | Self |
| Area | cone (15) |
| Duration | until the end of your turn or a spell is cast through the prism |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A small glass prism |
| Ritual | no |
| Practitioner lineages | Wizard |

### Mechanism

A hand-held prism spreads one single-target damaging working into a 15 ft cone, then breaks.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Prism conjured | `0.5 kg x 3 Pz/kg` | 1.5 |
| Spreading routed working | `244.3 Pz extra` | 244 |
| Pattern cost | `0.01 × Q2 × (1 + 0.00)` | 9.5 |

| Quantity | Value |
|---|---|
| Effect energy | 246 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **255 Pz** (383.0 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.268 |
| Energy-equivalent tier T_E | 0.68 |
| Handling points | 0.00 |
| Grade score | -0.66 → L |

**Handling flags:** none.

**Assumptions:** Prism 0.5 kg at 3 Pz/kg; reference routed working 4d8 = 18 fire, spread from a ray (F 0.5) to a 15 ft cone.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Temporary Magic Prism (2-C-L-TMP) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | cone (15) | 1 | `0000000000011` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | until the end of your turn or a spell is cast through the prism | 25 | `0000000110011` |

### Incantation

Spoken as **He’-Nuporbes** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihe’-Nuporbes* · T4: *Vihe’-Nuporbes* · T5: *Tihe’-Nuporbes* · T6: *Rihe’-Nuporbes* · T7: *Mihe’-Nuporbes* · T8: *Nihe’-Nuporbes* · T9: *Xyihe’-Nuporbes*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 | 2 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 5→12 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#ce6055`.

![[Temporary Magic Prism (2-C-L-TMP) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.997 | `#ff8300` (662 nm eq.) | source grid |
| Duration | until the end of your turn or a spell is cast through the prism | 0.974 | 0.741 | `#ff00df` (408 nm eq.) | RI half-step |
| Area | cone (15) | 0.028 | 0.985 | `#ff0003` (692 nm eq.) | source grid |
| Range | Self | 0.706 | 0.880 | `#0058ff` (488 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 2.41. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·C·None`; the k4 to k6 lines (cone (15), Self, until the end of your turn or a spell is cast through the prism) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·C·None` |
| Standard spectrometer detection range | 1.60 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 95.1 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 42.6 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (26.8% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Summoning and Conjured Creatures]], [[Transformation]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Find Steed (2-C-H-FS)|Find Steed]] (2) · [[Arcane Singularity (3-C-L-ASA)|Arcane Singularity]] (3) · [[Conjure Animals (3-C-M-CA)|Conjure Animals]] (3) · [[Find Familiar (1-C-H-FFN)|Find Familiar]] (1) · [[Stinking Cloud (3-C-M-SCI)|Stinking Cloud]] (3) · [[Unseen Servant (1-C-M-US)|Unseen Servant]] (1) · [[Alter Self (2-T-L-AST)|Alter Self]] (2) · [[Arcane Die (0-C-L-ADC)|Arcane Die]] (0).


---

## Tactical Assessment

One-shot conversion of a precision strike into an area strike.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
