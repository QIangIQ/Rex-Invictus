---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/transmutation
  - source/rex-invictus
aliases:
  - "2nd Tier Spell: Transfiguration Inheritance"
  - "Transfiguration Inheritance"
  - "2-T-L-TI"
registry_id: 2-T-L-TI
attribute_code: "2·Tra·None·None·Touch·Up to 1 minute"
incantation: "Hielixse"
tier: 2
school: Transmutation
affinity: T
grade: L
pz_total: 56.4
pz_quantum: 951.4
t_e: -0.83
updated: 2026-11-16
---

**Transfiguration Inheritance** (`2-T-L-TI`) is a 2nd Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Rex Invictus original working. Its modelled draw is **56.4 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E -0.83 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Transmutation]]
        - **Transfiguration Inheritance** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-T-L-TI` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Tra·None·None·Touch·Up to 1 minute` |
| Incantation | *Hielixse* |
| Affinity | T (Transmutation) |
| Source | Rex Invictus |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Transmutation]] |
| Casting time | 1 action |
| Range | Touch |
| Area | single point or target |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: a drop of quicksilver |
| Ritual | no |
| Practitioner lineages | Wizard, Sorcerer |

### Effect

Binds up to four other workings into one host working, so that the host's matter or construct inherits their properties in a chosen order. Each inherited property can be held dormant and released by a trigger.

### Mechanism

Acts as the stitching layer of a combination. It carries the pattern of each bound working into the host and halves the aspect friction between them, which is why compound tactics route through it.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| binding lattice, 3 links | `3*0.01*Q2` | 28.5 |
| property imprint, 1 property-equivalent on 100 kg host | `0.1 Pz/kg*100` | 10.0 |
| [upkeep] lattice hold, 60 s | `0.02 Pz/s*60` | 1.2 |
| Pattern cost | `0.01 × Q2 × (1 + 0.75)` | 16.6 |

| Quantity | Value |
|---|---|
| Effect energy | 38.5 Pz |
| Upkeep energy | 1.2 Pz (0.02 Pz/s) |
| **Total draw** | **56.4 Pz** (84.6 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.0593 |
| Energy-equivalent tier T_E | -0.83 |
| Handling points | 0.75 |
| Grade score | -0.25 → L |

**Handling flags:** concentration, multi target control.

**Assumptions:** 3 links at 1% of the Tier-2 quantum each; 0.1 Pz/kg per imprinted property; concentration up to 1 minute.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Transfiguration Inheritance (2-T-L-TI) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Hielixse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihielixse* · T4: *Vihielixse* · T5: *Tihielixse* · T6: *Rihielixse* · T7: *Mihielixse* · T8: *Nihielixse* · T9: *Xyihielixse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#8e60b5`.

![[Transfiguration Inheritance (2-T-L-TI) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.796 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.889 | `#0074ff` (495 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.792 | `#9b00ff` (435 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 1.75. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·T·None`; the k4 to k6 lines (None, Touch, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·T·None` |
| Standard spectrometer detection range | 0.75 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 95.4 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 9.4 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (5.9% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Linking and Triggers]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Magic Mouth (2-I-L-MMG)|Magic Mouth]] (2) · [[Alarm (1-A-L-ALR)|Alarm]] (1) · [[Glyph of Warding (3-A-H-GWY)|Glyph of Warding]] (3) · [[Magic Link (1-P-L-MLK)|Magic Link]] (1) · [[Accelerate (2-T-L-ACC)|Accelerate]] (2) · [[Alter Projectile Velocity (2-T-L-APV)|Alter Projectile Velocity]] (2) · [[Alter Self (2-T-L-AST)|Alter Self]] (2) · [[Barkskin (2-T-L-BRK)|Barkskin]] (2).


---

## Tactical Assessment

The standard binder for field combinations. Its own draw is small; its value is the friction it removes from expensive links.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
