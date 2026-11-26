---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-0
  - spell/conjuration
  - source/science-spellbook
aliases:
  - "Cantrip Spell: Hubble's Constant"
  - "0-C-L-HSC"
  - "Hubble's Constant (Science)"
registry_id: 0-C-L-HSC
attribute_code: "0·Con·Radiant·sphere (120)·30 feet·Up to 1 minute"
incantation: "Cenat-Seiusinse"
tier: 0
school: Conjuration
affinity: C
grade: L
pz_total: 26.6
pz_quantum: 128.8
t_e: -1.58
updated: 2026-11-16
---

**Hubble's Constant** (`0-C-L-HSC`) is a Cantrip (Tier 0) working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **26.6 Pz** against a slot quantum of 129 Pz, which puts its energy-equivalent tier at T_E -1.58 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 0 Workings]]
      - [[Conjuration]]
        - **Hubble's Constant** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `0-C-L-HSC` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `0·Con·Radiant·sphere (120)·30 feet·Up to 1 minute` |
| Incantation | *Cenat-Seiusinse* |
| Affinity | C (Conjuration) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | Cantrip (Tier 0) |
| School | [[Conjuration]] |
| Casting time | 1 Bonus Action |
| Range | 30 feet |
| Area | sphere (120) |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A tuning fork |
| Ritual | no |
| Injury | 1 radiant (mean 0) |
| Injury by caster maturity bands | T1: 1, T5: 2, T11: 3, T17: 4 |
| Practitioner lineages | Wizard |

### Mechanism

A small star-like source irradiates every creature within 120 ft with a weak radiant dose each round.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Radiant dose, 120 ft | `1 HP*0.5*0.5*10 creatures*10 pulses  [C8]` | 25.0 |
| Pattern cost | `0.01 × Q0 × (1 + 0.25)` | 1.6 |

| Quantity | Value |
|---|---|
| Effect energy | 25.0 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **26.6 Pz** (39.9 kJ) |
| Slot quantum Q0 | 129 Pz |
| Field gain (draw / quantum) | 0.207 |
| Energy-equivalent tier T_E | -1.58 |
| Handling points | 0.25 |
| Grade score | -0.54 → L |

Calibration applied: C8 (Sub-injury dose), see [[Parzival Energy Budget#Registry calibration rules]].

**Handling flags:** concentration.

**Assumptions:** 1 radiant per round over a 120 ft sphere for 10 rounds; the isotropic fluence model makes the large radius expensive, and a per-target delivery would cost about 0.25 Pz per creature per round instead.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Hubble's Constant (0-C-L-HSC) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 0 | 0 | `0000000000001` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | Radiant | 11 | `0000000010111` |
| k4 Area | sphere (120) | 39 | `0000001001111` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Cenat-Seiusinse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T1: *Sicenat-Seiusinse* · T2: *Hicenat-Seiusinse* · T3: *Licenat-Seiusinse* · T4: *Vicenat-Seiusinse* · T5: *Ticenat-Seiusinse* · T6: *Ricenat-Seiusinse* · T7: *Micenat-Seiusinse* · T8: *Nicenat-Seiusinse* · T9: *Xyicenat-Seiusinse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 | 1 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 4→1 | 4 |
| k4 Area | 0→9 1→10 2→11 3→12 6→2 | 5 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#835976`.

![[Hubble's Constant (0-C-L-HSC) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 0 | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| Damage | Radiant | 0.786 | 0.734 | `#1900ff` (464 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.992 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.791 | `#0074ff` (495 nm eq.) | source grid |
| Area | sphere (120) | 0.792 | 0.731 | `#1e00ff` (462 nm eq.) | RI half-step |
| Range | 30 feet | 0.294 | 0.958 | `#91ff00` (612 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 1.43. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `0·C·Radiant`; the k4 to k6 lines (sphere (120), 30 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `0·C·Radiant` |
| Standard spectrometer detection range | 0.52 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 6.4 Pz (0.05 × Q0) |
| Counter drawn cold (all six layers) | 12.9 Pz (0.10 × Q0) |
| Unravel after completion | 12.9 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Life, Hope and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1b 1c 1d 1e 1F 1i 1j` (Beyond, Heat, Light, Life, Prodigious, Potential, Hope, Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 4.4 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the Cantrip (Tier 0) quantum of 129 Pz (20.7% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
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
| Function | [[Divination and Sensing]], [[Area Destruction]] |
| Element | [[Radiant Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Guardian of Faith (4-C-L-GFA)|Guardian of Faith]] (4) · [[Moonbeam (2-V-M-MNB)|Moonbeam]] (2) · [[Splash (0-C-L-SPL)|Splash]] (0) · [[Telescope (0-C-L-TLS)|Telescope]] (0) · [[Arcane Gravitational Lens (0-D-L-AGL)|Arcane Gravitational Lens]] (0) · [[Guidance (0-D-L-GDN)|Guidance]] (0) · [[Hooke's Compelled Duel (0-E-L-HSCD)|Hooke's Compelled Duel]] (0) · [[Identify Medicinal Herbs (0-D-L-IMH)|Identify Medicinal Herbs]] (0).


---

## Tactical Assessment

Wide-area harassment that reveals and wears down hidden infantry; costly for its effect.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 0 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
