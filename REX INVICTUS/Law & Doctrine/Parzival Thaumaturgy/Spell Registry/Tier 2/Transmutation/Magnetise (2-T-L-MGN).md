---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/transmutation
  - source/science-spellbook
aliases:
  - "2nd Tier Spell: Magnetise"
  - "2-T-L-MGN"
  - "Magnetise (Science)"
registry_id: 2-T-L-MGN
attribute_code: "2·Tra·None·sphere (5)·30 feet·1 minute"
incantation: "Hie’-Suusine"
tier: 2
school: Transmutation
affinity: T
grade: L
pz_total: 29.2
pz_quantum: 951.4
t_e: -1.49
updated: 2026-11-16
---

**Magnetise** (`2-T-L-MGN`) is a 2nd Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **29.2 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E -1.49 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Transmutation]]
        - **Magnetise** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-T-L-MGN` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Tra·None·sphere (5)·30 feet·1 minute` |
| Incantation | *Hie’-Suusine* |
| Affinity | T (Transmutation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Transmutation]] |
| Casting time | 1 Action |
| Range | 30 feet |
| Area | sphere (5) |
| Duration | 1 minute |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A small magnetic metal |
| Ritual | no |
| Resistance check | strength; on success: no effect |
| Practitioner lineages | Wizard, Sorcerer |

### Mechanism

Turns a metal object into a strong magnet that pulls iron and steel within 5 ft onto it.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Magnetic field energy | `1 T^2/(2 mu0) x 0.05 m^3 = 1.989e+04 J / 1500` | 13.3 |
| Field losses (upkeep) | `100 W x 60 s = 6000 J / 1500` | 4.0 |
| Pattern cost | `0.01 × Q2 × (1 + 0.25)` | 11.9 |

| Quantity | Value |
|---|---|
| Effect energy | 13.3 Pz |
| Upkeep energy | 4.0 Pz (0.0667 Pz/s) |
| **Total draw** | **29.2 Pz** (43.7 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.0306 |
| Energy-equivalent tier T_E | -1.49 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** save or suck.

**Assumptions:** Field of 1 T over 0.05 m^3 (B^2/2mu0 x V) plus 100 W eddy and hysteresis losses for 1 minute.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Magnetise (2-T-L-MGN) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (5) | 34 | `0000001000101` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | 1 minute | 1 | `0000000000011` |

### Incantation

Spoken as **Hie’-Suusine** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihie’-Suusine* · T4: *Vihie’-Suusine* · T5: *Tihie’-Suusine* · T6: *Rihie’-Suusine* · T7: *Mihie’-Suusine* · T8: *Nihie’-Suusine* · T9: *Xyihie’-Suusine*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 2→11 6→2 | 3 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#d28157`.

![[Magnetise (2-T-L-MGN) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.796 | `#9600ff` (438 nm eq.) | source grid |
| Duration | 1 minute | 0.105 | 0.996 | `#ff6300` (668 nm eq.) | source grid |
| Area | sphere (5) | 0.944 | 0.758 | `#f200ff` (417 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.996 | `#91ff00` (612 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 1.46. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·T·None`; the k4 to k6 lines (sphere (5), 30 feet, 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·T·None` |
| Standard spectrometer detection range | 0.54 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 95.9 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 4.9 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (3.1% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
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
| Function | [[Utility Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Momentum Transfer (2-T-L-MT)|Momentum Transfer]] (2) · [[Alter Weight (1-T-L-AWT)|Alter Weight]] (1) · [[Arcane Gyroscope (1-T-L-AG)|Arcane Gyroscope]] (1) · [[Sublimation (3-T-L-SBL)|Sublimation]] (3) · [[Vapour Deposition (1-T-L-VD)|Vapour Deposition]] (1) · [[Carbon Dating (2-D-L-CDR)|Carbon Dating]] (2) · [[Moderator (2-A-L-MDR)|Moderator]] (2) · [[Predict Projectiles (2-D-L-PPE)|Predict Projectiles]] (2).


---

## Tactical Assessment

Disarms and pins armoured soldiers by magnetising their armour or nearby structures.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
