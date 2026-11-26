---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-0
  - spell/conjuration
  - source/rex-invictus
aliases:
  - "Cantrip Spell: Splash"
  - "Splash"
  - "0-C-L-SPL"
registry_id: 0-C-L-SPL
attribute_code: "0·Con·Bludgeoning·sphere (5)·30 feet·Instantaneous"
incantation: "Cedeg-Suusin"
tier: 0
school: Conjuration
affinity: C
grade: L
pz_total: 51.4
pz_quantum: 128.8
t_e: -0.92
updated: 2026-11-16
---

**Splash** (`0-C-L-SPL`) is a Cantrip (Tier 0) working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Rex Invictus original working. Its modelled draw is **51.4 Pz** against a slot quantum of 129 Pz, which puts its energy-equivalent tier at T_E -0.92 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 0 Workings]]
      - [[Conjuration]]
        - **Splash** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `0-C-L-SPL` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `0·Con·Bludgeoning·sphere (5)·30 feet·Instantaneous` |
| Incantation | *Cedeg-Suusin* |
| Affinity | C (Conjuration) |
| Source | Rex Invictus |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | Cantrip (Tier 0) |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | 30 feet |
| Area | sphere (5) |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Wizard, Sorcerer, Druid |

### Effect

Hurls about 2 litres of conjured liquid at a point. Creatures in a 5 foot radius are drenched and take 1d4 bludgeoning injury from the impact.

### Mechanism

A small conjured mass thrown as a burst. Its liquid stays liquid after impact, which matters when it is bound into a penetrator.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| conjured liquid 2 kg | `1*2` | 2.0 |
| throw at 15 m/s | `0.5*2*15^2/1500` | 0.15 |
| impact 2.5 injury, 5 ft sphere | `2.5*0.46*4*pi*1.524^2/0.7` | 47.9 |
| Pattern cost | `0.01 × Q0 × (1 + 0.00)` | 1.3 |

| Quantity | Value |
|---|---|
| Effect energy | 50.1 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **51.4 Pz** (77.1 kJ) |
| Slot quantum Q0 | 129 Pz |
| Field gain (draw / quantum) | 0.399 |
| Energy-equivalent tier T_E | -0.92 |
| Handling points | 0.00 |
| Grade score | -0.46 → L |

**Handling flags:** none.

**Assumptions:** 2 kg liquid; 1d4 = 2.5 average.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Splash (0-C-L-SPL) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 0 | 0 | `0000000000001` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | Bludgeoning | 1 | `0000000000011` |
| k4 Area | sphere (5) | 34 | `0000001000101` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Cedeg-Suusin** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T1: *Sicedeg-Suusin* · T2: *Hicedeg-Suusin* · T3: *Licedeg-Suusin* · T4: *Vicedeg-Suusin* · T5: *Ticedeg-Suusin* · T6: *Ricedeg-Suusin* · T7: *Micedeg-Suusin* · T8: *Nicedeg-Suusin* · T9: *Xyicedeg-Suusin*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 | 1 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 | 2 |
| k4 Area | 0→9 2→11 6→2 | 3 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#ea5e2b`.

![[Splash (0-C-L-SPL) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 0 | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| Damage | Bludgeoning | 0.143 | 0.990 | `#ff9900` (657 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.992 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| Area | sphere (5) | 0.944 | 0.640 | `#f200ff` (417 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.958 | `#91ff00` (612 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 1.71. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `0·C·Bludgeoning`; the k4 to k6 lines (sphere (5), 30 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `0·C·Bludgeoning` |
| Standard spectrometer detection range | 0.72 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 6.4 Pz (0.05 × Q0) |
| Counter drawn cold (all six layers) | 12.9 Pz (0.10 × Q0) |
| Unravel after completion | 12.9 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Within, Rigidity, 2x Movement and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1e 1F 1H 3j` (Prodigious, Potential, Rigidity, 3x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 8.6 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the Cantrip (Tier 0) quantum of 129 Pz (39.9% of it). |
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
| Function | [[Area Destruction]] |
| Element | [[Bludgeoning Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Black Tentacles (4-C-L-BT)|Black Tentacles]] (4) · [[Geyser (2-V-L-GYS)|Geyser]] (2) · [[Hubble's Constant (0-C-L-HSC)|Hubble's Constant]] (0) · [[Supersonic Omnidirectional Jet (5-C-M-SOJ)|Supersonic Omnidirectional Jet]] (5) · [[Wind Wall (3-V-L-WWN)|Wind Wall]] (3) · [[Control Water (4-T-H-CWN)|Control Water]] (4) · [[Ice Storm (4-V-L-ISE)|Ice Storm]] (4) · [[Blast (1-V-L-BLS)|Blast]] (1).


---

## Tactical Assessment

On its own it douses a fire or a sentry. Inside a shaped charge its fluid keeps a breach open.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 0 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
