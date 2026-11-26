---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-0
  - spell/conjuration
  - source/science-spellbook
aliases:
  - "Cantrip Spell: Telescope"
  - "0-C-L-TLS"
  - "Telescope (Science)"
registry_id: 0-C-L-TLS
attribute_code: "0·Con·None·None·Self·1 hour"
incantation: "Cepora"
tier: 0
school: Conjuration
affinity: C
grade: L
pz_total: 18.7
pz_quantum: 128.8
t_e: -1.93
updated: 2026-11-16
---

**Telescope** (`0-C-L-TLS`) is a Cantrip (Tier 0) working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **18.7 Pz** against a slot quantum of 129 Pz, which puts its energy-equivalent tier at T_E -1.93 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 0 Workings]]
      - [[Conjuration]]
        - **Telescope** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `0-C-L-TLS` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `0·Con·None·None·Self·1 hour` |
| Incantation | *Cepora* |
| Affinity | C (Conjuration) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | Cantrip (Tier 0) |
| School | [[Conjuration]] |
| Casting time | 1 Action |
| Range | Self |
| Area | single point or target |
| Duration | 1 hour |
| Components | material focus. Material: One brass telescope set for approximatley 1000 feet |
| Ritual | no |
| Practitioner lineages | Wizard, Sorcerer, Ranger, Druid, Warlock |

### Mechanism

Conjures a tripod-mounted brass telescope that gathers and amplifies distant light.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Telescope conjured | `5 kg x 3 Pz/kg` | 15.0 |
| Light amplification (upkeep) | `1 W x 3600 s = 3600 J / 1500` | 2.4 |
| Pattern cost | `0.01 × Q0 × (1 + 0.00)` | 1.3 |

| Quantity | Value |
|---|---|
| Effect energy | 15.0 Pz |
| Upkeep energy | 2.4 Pz (0.000667 Pz/s) |
| **Total draw** | **18.7 Pz** (28.0 kJ) |
| Slot quantum Q0 | 129 Pz |
| Field gain (draw / quantum) | 0.145 |
| Energy-equivalent tier T_E | -1.93 |
| Handling points | 0.00 |
| Grade score | -0.97 → L |

**Handling flags:** none.

**Assumptions:** Telescope and tripod 5 kg at 3 Pz/kg; light amplification 1 W for 1 hour.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Telescope (0-C-L-TLS) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 0 | 0 | `0000000000001` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | 1 hour | 0 | `0000000000001` |

### Incantation

Spoken as **Cepora** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T1: *Sicepora* · T2: *Hicepora* · T3: *Licepora* · T4: *Vicepora* · T5: *Ticepora* · T6: *Ricepora* · T7: *Micepora* · T8: *Nicepora* · T9: *Xyicepora*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 | 1 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 | 1 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#ca3c3f`.

![[Telescope (0-C-L-TLS) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 0 | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.992 | `#ff8300` (662 nm eq.) | source grid |
| Duration | 1 hour | 0.053 | 0.999 | `#ff1c00` (684 nm eq.) | source grid |
| Range | Self | 0.706 | 0.779 | `#0058ff` (488 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 1.27. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `0·C·None`; the k4 to k6 lines (None, Self, 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `0·C·None` |
| Standard spectrometer detection range | 0.43 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 6.4 Pz (0.05 × Q0) |
| Counter drawn cold (all six layers) | 12.9 Pz (0.10 × Q0) |
| Unravel after completion | 13.4 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 3.1 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the Cantrip (Tier 0) quantum of 129 Pz (14.5% of it). |
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
| Function | [[Divination and Sensing]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Hubble's Constant (0-C-L-HSC)|Hubble's Constant]] (0) · [[Arcane Gravitational Lens (0-D-L-AGL)|Arcane Gravitational Lens]] (0) · [[Guidance (0-D-L-GDN)|Guidance]] (0) · [[Hooke's Compelled Duel (0-E-L-HSCD)|Hooke's Compelled Duel]] (0) · [[Identify Medicinal Herbs (0-D-L-IMH)|Identify Medicinal Herbs]] (0) · [[Message (0-T-L-MSS)|Message]] (0) · [[Modify Food (0-T-L-MF)|Modify Food]] (0) · [[Mutual Information (0-D-L-MIT)|Mutual Information]] (0).


---

## Tactical Assessment

Fixed observation post optics; an issued telescope does the same job.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 0 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
