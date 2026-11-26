---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-0
  - spell/conjuration
  - source/science-spellbook
aliases:
  - "Cantrip Spell: Aquire Funding"
  - "0-C-L-AFU"
  - "Aquire Funding (Science)"
registry_id: 0-C-L-AFU
attribute_code: "0·Con·None·None·Self·Instantaneous"
incantation: "Cepor"
tier: 0
school: Conjuration
affinity: C
grade: L
pz_total: 15.8
pz_quantum: 128.8
t_e: -2.10
updated: 2026-11-16
---

**Aquire Funding** (`0-C-L-AFU`) is a Cantrip (Tier 0) working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **15.8 Pz** against a slot quantum of 129 Pz, which puts its energy-equivalent tier at T_E -2.10 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 0 Workings]]
      - [[Conjuration]]
        - **Aquire Funding** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `0-C-L-AFU` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `0·Con·None·None·Self·Instantaneous` |
| Incantation | *Cepor* |
| Affinity | C (Conjuration) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | Cantrip (Tier 0) |
| School | [[Conjuration]] |
| Casting time | 1 Day |
| Range | Self |
| Area | single point or target |
| Duration | Instantaneous |
| Components | material focus. Material: Paper, quill, and ink for writing application |
| Ritual | yes |
| Practitioner lineages | Wizard, Warlock |

### Mechanism

A day-long petition to the field returns coin in proportion to the request and the result of the casting.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Coin conjured | `4.5 kg x 3 Pz/kg` | 13.5 |
| Pattern cost | `0.01 × Q0 × (1 + 0.75)` | 2.3 |

| Quantity | Value |
|---|---|
| Effect energy | 13.5 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **15.8 Pz** (23.6 kJ) |
| Slot quantum Q0 | 129 Pz |
| Field gain (draw / quantum) | 0.122 |
| Energy-equivalent tier T_E | -2.10 |
| Handling points | 0.75 |
| Grade score | -0.25 → L |

**Handling flags:** ritual, consumed material, long cast.

**Assumptions:** Return of 500 gold coins (4.5 kg) conjured as structured metal at 3 Pz/kg; nuclear transmutation into gold would cost vastly more.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Aquire Funding (0-C-L-AFU) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 0 | 0 | `0000000000001` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Cepor** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T1: *Sicepor* · T2: *Hicepor* · T3: *Licepor* · T4: *Vicepor* · T5: *Ticepor* · T6: *Ricepor* · T7: *Micepor* · T8: *Nicepor* · T9: *Xyicepor*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 | 1 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#ca3449`.

![[Aquire Funding (0-C-L-AFU) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 0 | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.992 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| Range | Self | 0.706 | 0.779 | `#0058ff` (488 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 1.20. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `0·C·None`; the k4 to k6 lines (None, Self, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `0·C·None` |
| Standard spectrometer detection range | 0.40 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 6.4 Pz (0.05 × Q0) |
| Counter drawn cold (all six layers) | 12.9 Pz (0.10 × Q0) |
| Unravel after completion | 12.9 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 2.6 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the Cantrip (Tier 0) quantum of 129 Pz (12.2% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at Cantrip (Tier 0) up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 0 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Utility Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Manipulate Uncertainty (0-I-L-MU)|Manipulate Uncertainty]] (0) · [[Quantum Tunnelling (2-C-L-QT)|Quantum Tunnelling]] (2) · [[Alter Weight (1-T-L-AWT)|Alter Weight]] (1) · [[Arcane Gyroscope (1-T-L-AG)|Arcane Gyroscope]] (1) · [[Ladder Operation (1-E-L-LOD)|Ladder Operation]] (1) · [[Pascal's Revenge (1-I-L-PSR)|Pascal's Revenge]] (1) · [[Reverb (1-I-L-RVR)|Reverb]] (1) · [[Vapour Deposition (1-T-L-VD)|Vapour Deposition]] (1).


---

## Tactical Assessment

Field funding for operations; slow and unreliable.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 0 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
