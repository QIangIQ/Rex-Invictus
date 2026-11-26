---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-9
  - spell/conjuration
  - source/science-spellbook
aliases:
  - "9th Tier Spell: Wormhole"
  - "9-P-L-WRM"
  - "Wormhole (Science)"
registry_id: 9-P-L-WRM
attribute_code: "9·Con·Force·sphere (60)·Unlimited·Instantaneous"
incantation: "Xyeton-Siash"
tier: 9
school: Conjuration
affinity: P
grade: L
pz_total: 928107.3
pz_quantum: 1043335.3
t_e: 8.88
updated: 2026-11-16
---

**Wormhole** (`9-P-L-WRM`) is a 9th Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **928,107 Pz** against a slot quantum of 1.04 MPz Pz, which puts its energy-equivalent tier at T_E 8.88 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 9 Workings]]
      - [[Conjuration]]
        - **Wormhole** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `9-P-L-WRM` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `9·Con·Force·sphere (60)·Unlimited·Instantaneous` |
| Incantation | *Xyeton-Siash* |
| Affinity | P (Pure field construct) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 9th Tier |
| School | [[Conjuration]] |
| Casting time | 1 day |
| Range | Unlimited |
| Area | sphere (60) |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A piece of paper and a writing impliment |
| Ritual | no |
| Injury | 9d8 force (mean 40.5) |
| Injury by tier | T9: 9d8 |
| Practitioner lineages | Wizard, Sorcerer |

### Mechanism

A day-long working links two known locations with a permanent 10 ft spherical gateway; a failed attempt collapses into brief black holes at both ends.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Link established | `0.01 x 17.8 kg x 15 x 1e+07 m / 1500` | 17,800 |
| Failure collapse (50% weight, 2 ends) | `40.5 HP x 0.4 (force) x S/A_c, S = sphere r=18.29 m = 4202.8 m^2` | 97,266 |
| Traffic carried (upkeep) | `10 x 0.01 x 80 kg x 15 x 1e+07 m / 1500` | 800,000 |
| Pattern cost | `0.01 × Q9 × (1 + 0.25)` | 13,042 |

| Quantity | Value |
|---|---|
| Effect energy | 115,066 Pz |
| Upkeep energy | 800,000 Pz (222 Pz/s) |
| **Total draw** | **928,107 Pz** (1,392,160.9 kJ) |
| Slot quantum Q9 | 1.04 MPz Pz |
| Field gain (draw / quantum) | 0.89 |
| Energy-equivalent tier T_E | 8.88 |
| Handling points | 0.25 |
| Grade score | 0.19 → L |

**Handling flags:** long cast.

**Assumptions:** Link distance 1e7 m; establishing cost the translocation of the aperture's 17.8 kg of air over that distance; traffic of 10 crossings of 80 kg in the 1 hour convention used for open durations; failure taken as 50% likely, 9d8 = 40.5 force over 60 ft at both ends. A real traversable wormhole would need exotic energy near 1e41 Pz.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Wormhole (9-P-L-WRM) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 9 | 9 | `0000000010011` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | Force | 4 | `0000000001001` |
| k4 Area | sphere (60) | 35 | `0000001000111` |
| k5 Range | Unlimited | 16 | `0000000100001` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Xyeton-Siash** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 4→3 | 3 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 3→0 | 2 |
| k4 Area | 0→9 1→10 2→11 6→2 | 4 |
| k5 Range | 0→8 5→0 | 2 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#cd3c91`.

![[Wormhole (9-P-L-WRM) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 9 | 0.900 | 1.000 | `#b600ff` (430 nm eq.) | source grid |
| Damage | Force | 0.357 | 0.863 | `#3bff00` (593 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.741 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.667 | `#ff0028` (700 nm eq.) | source grid |
| Area | sphere (60) | 0.972 | 0.997 | `#ff00e5` (408 nm eq.) | source grid |
| Range | Unlimited | 0.941 | 0.999 | `#ed00ff` (418 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 5.97. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `9·C·Force`; the k4 to k6 lines (sphere (60), Unlimited, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `9·C·Force` |
| Standard spectrometer detection range | 96.34 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 52,167 Pz (0.05 × Q9) |
| Counter drawn cold (all six layers) | 104,334 Pz (0.10 × Q9) |
| Unravel after completion | 264,334 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Beyond, Introspection, 2x Movement and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `2a 1e 1F 1G 3j` (2x Beyond, Prodigious, Potential, Introspection, 3x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 154,685 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 9th Tier quantum of 1.04 MPz Pz (89.0% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 9th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 9 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Pure]] (P) |
| Function | [[Area Destruction]] |
| Element | [[Force Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Thermonuclear Fireball (9-P-L-TFE)|Thermonuclear Fireball]] (9) · [[Storm of Vengeance (9-C-M-SV)|Storm of Vengeance]] (9) · [[Disintegrate (6-P-L-DSN)|Disintegrate]] (6) · [[Incendiary Cloud (8-C-M-IC)|Incendiary Cloud]] (8) · [[Supermassive Black Hole (10-C-X-SBH)|Supermassive Black Hole]] (10) · [[Eruption (9-V-M-ERP)|Eruption]] (9) · [[Meteor Swarm (9-V-L-MST)|Meteor Swarm]] (9) · [[Starburst (9-A-L-STR)|Starburst]] (9).


---

## Tactical Assessment

Strategic logistics link between bases at any distance.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 9 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
