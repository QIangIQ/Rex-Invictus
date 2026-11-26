---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-9
  - spell/conjuration
  - source/srd
aliases:
  - "9th Tier Spell: Mass Heal"
  - "Mass Heal"
  - "9-C-L-MHS"
registry_id: 9-C-L-MHS
attribute_code: "9·Con·None·None·60 feet·Instantaneous"
incantation: "Xyewyn"
tier: 9
school: Conjuration
affinity: C
grade: L
pz_total: 10664.4
pz_quantum: 1043335.3
t_e: 4.42
updated: 2026-11-16
---

**Mass Heal** (`9-C-L-MHS`) is a 9th Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **10,664 Pz** against a slot quantum of 1.04 MPz Pz, which puts its energy-equivalent tier at T_E 4.42 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 9 Workings]]
      - [[Conjuration]]
        - **Mass Heal** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `9-C-L-MHS` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `9·Con·None·None·60 feet·Instantaneous` |
| Incantation | *Xyewyn* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 9th Tier |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Restoration | 700 restored (mean 0, modifier taken as +3) |
| Practitioner lineages | Cleric |

### Mechanism

A flood of restorative energy repairs up to 700 units of injury divided among visible creatures, also curing disease, blindness and deafness. It does not affect the undead or constructs.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Healing pool | `700 HP * 0.30` | 210 |
| Clearing disease and sensory loss, 7 creatures | `7 * 10 HP equivalent * 0.30` | 21.0 |
| Pattern cost | `0.01 × Q9 × (1 + 0.00)` | 10,433 |

| Quantity | Value |
|---|---|
| Effect energy | 231 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **10,664 Pz** (15,996.5 kJ) |
| Slot quantum Q9 | 1.04 MPz Pz |
| Field gain (draw / quantum) | 0.0102 |
| Energy-equivalent tier T_E | 4.42 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Full 700 pool used; condition removal valued at 10 healing units for 7 recipients.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Mass Heal (9-C-L-MHS) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 9 | 9 | `0000000010011` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Xyewyn** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 4→3 | 3 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#a0649c`.

![[Mass Heal (9-C-L-MHS) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 9 | 0.900 | 1.000 | `#b600ff` (430 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.741 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.667 | `#ff0028` (700 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.953 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.20): swatch `#96719c`, measured lines at 0.004, 0.126, 0.589, 0.901. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.03. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `9·C·None`; the k4 to k6 lines (None, 60 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `9·C·None` |
| Standard spectrometer detection range | 10.33 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 52,167 Pz (0.05 × Q9) |
| Counter drawn cold (all six layers) | 104,334 Pz (0.10 × Q9) |
| Unravel after completion | 104,334 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1,777 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 9th Tier quantum of 1.04 MPz Pz (1.0% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 9th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 9 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Healing and Restoration]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Time Stop (9-T-M-TSM)|Time Stop]] (9) · [[True Resurrection (9-N-L-TR)|True Resurrection]] (9) · [[Heroes' Feast (6-C-L-HF)|Heroes' Feast]] (6) · [[Gate (9-C-L-GAT)|Gate]] (9) · [[Mass Cure Wounds (5-C-L-MCW)|Mass Cure Wounds]] (5) · [[Regenerate (7-T-L-RGN)|Regenerate]] (7) · [[Resurrection (7-N-L-RSR)|Resurrection]] (7) · [[Storm of Vengeance (9-C-M-SV)|Storm of Vengeance]] (9).


---

## Tactical Assessment

Can restore a whole company after mass casualties in one action. Its value lies in recovery and morale.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 9 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
