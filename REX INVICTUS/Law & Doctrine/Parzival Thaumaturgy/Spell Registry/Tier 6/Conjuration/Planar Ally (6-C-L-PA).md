---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-6
  - spell/conjuration
  - source/srd
aliases:
  - "6th Tier Spell: Planar Ally"
  - "Planar Ally"
  - "6-C-L-PA"
registry_id: 6-C-L-PA
attribute_code: "6·Con·None·None·60 feet·Instantaneous"
incantation: "Rewyn"
tier: 6
school: Conjuration
affinity: C
grade: L
pz_total: 25650.3
pz_quantum: 51944.6
t_e: 5.29
updated: 2026-11-16
---

**Planar Ally** (`6-C-L-PA`) is a 6th Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **25,650 Pz** against a slot quantum of 51,945 Pz, which puts its energy-equivalent tier at T_E 5.29 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 6 Workings]]
      - [[Conjuration]]
        - **Planar Ally** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `6-C-L-PA` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `6·Con·None·None·60 feet·Instantaneous` |
| Incantation | *Rewyn* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 6th Tier |
| School | [[Conjuration]] |
| Casting time | 10 minutes |
| Range | 60 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Cleric |

### Mechanism

The working opens a petition line to a distant patron and accepts the translocated arrival of one of its servants. The field pays for the crossing; the servant acts on its own will under a negotiated contract.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| inbound translocation of a 250 kg extraplanar servant, 1 plane boundary | `0.01*250*15*1e6/1500` | 25,000 |
| negotiation channel, instant information | `1` | 1.0 |
| Pattern cost | `0.01 × Q6 × (1 + 0.25)` | 649 |

| Quantity | Value |
|---|---|
| Effect energy | 25,001 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **25,650 Pz** (38,475.5 kJ) |
| Slot quantum Q6 | 51,945 Pz |
| Field gain (draw / quantum) | 0.494 |
| Energy-equivalent tier T_E | 5.29 |
| Handling points | 0.25 |
| Grade score | -0.10 → L |

**Handling flags:** long cast.

**Assumptions:** Servant mass 250 kg; one plane boundary at d_eff 1e6 m; return trip paid by the servant; payment treated as a contract outside the material flags.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Planar Ally (6-C-L-PA) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 6 | 6 | `0000000001101` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Rewyn** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T7: *Mirewyn* · T8: *Nirewyn* · T9: *Xyirewyn*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 3→2 | 3 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#76a191`.

![[Planar Ally (6-C-L-PA) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 6 | 0.600 | 1.000 | `#00ebff` (520 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.893 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.835 | `#ff0028` (700 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 1.000 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.21): swatch `#9fa882`, measured lines at 0.004, 0.126, 0.596. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.41. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `6·C·None`; the k4 to k6 lines (None, 60 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `6·C·None` |
| Standard spectrometer detection range | 16.02 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 2,597 Pz (0.05 × Q6) |
| Counter drawn cold (all six layers) | 5,194 Pz (0.10 × Q6) |
| Unravel after completion | 5,194 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 4,275 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 6th Tier quantum of 51,945 Pz (49.4% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 6th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 6 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Summoning and Conjured Creatures]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Conjure Fey (6-C-L-CFN)|Conjure Fey]] (6) · [[Instant Summons (6-C-L-ISS)|Instant Summons]] (6) · [[Conjure Celestial (7-C-L-CCN)|Conjure Celestial]] (7) · [[Conjure Elemental (5-C-M-CEN)|Conjure Elemental]] (5) · [[Conjure Magic Prism (4-C-L-CMPJ)|Conjure Magic Prism]] (4) · [[Conjure Minor Elementals (4-C-M-CME)|Conjure Minor Elementals]] (4) · [[Conjure Woodland Beings (4-C-L-CWB)|Conjure Woodland Beings]] (4) · [[Create Undead (6-N-L-CU)|Create Undead]] (6).


---

## Tactical Assessment

Delivers a high-end extraplanar specialist for hire, with the price paid in treasure while the field cost stays modest. Useful for missions measured in hours or days where native forces lack the capability.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 6 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
