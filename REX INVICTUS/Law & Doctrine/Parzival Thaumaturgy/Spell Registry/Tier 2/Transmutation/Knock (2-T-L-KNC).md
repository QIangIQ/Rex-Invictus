---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/transmutation
  - source/srd
aliases:
  - "2nd Tier Spell: Knock"
  - "Knock"
  - "2-T-L-KNC"
registry_id: 2-T-L-KNC
attribute_code: "2·Tra·None·None·60 feet·Instantaneous"
incantation: "Hiewyn"
tier: 2
school: Transmutation
affinity: T
grade: L
pz_total: 10.6
pz_quantum: 951.4
t_e: -2.50
updated: 2026-11-16
---

**Knock** (`2-T-L-KNC`) is a 2nd Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **10.6 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E -2.50 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Transmutation]]
        - **Knock** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-T-L-KNC` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Tra·None·None·60 feet·Instantaneous` |
| Incantation | *Hiewyn* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Transmutation]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation) |
| Ritual | no |
| Practitioner lineages | Bard, Sorcerer, Wizard |

### Mechanism

The field actuates one mechanical lock or lifts a bar holding a closure, or suppresses a sealing ward for 10 minutes. A loud report carries about 300 ft from the target.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Release bolt or bar | `20 kg * 9.81 * 0.3 m / 1500` | 0.0392 |
| Lock mechanism actuation | `50 N * 0.02 m / 1500` | 0.000667 |
| Loud knock acoustic pulse | `10 W * 0.1 s / 1500` | 0.000667 |
| Suppressing a sealing ward (instant info) | `instant info = 1 Pz` | 1.0 |
| Pattern cost | `0.01 × Q2 × (1 + 0.00)` | 9.5 |

| Quantity | Value |
|---|---|
| Effect energy | 1.0 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **10.6 Pz** (15.8 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.0111 |
| Energy-equivalent tier T_E | -2.50 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Bar 20 kg lifted 0.3 m; lock needs 50 N over 2 cm; knock as a 10 W pulse lasting 0.1 s.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Knock (2-T-L-KNC) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Hiewyn** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihiewyn* · T4: *Vihiewyn* · T5: *Tihiewyn* · T6: *Rihiewyn* · T7: *Mihiewyn* · T8: *Nihiewyn* · T9: *Xyihiewyn*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#a87e81`.

![[Knock (2-T-L-KNC) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.796 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.980 | `#ff0028` (700 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.927 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.19): swatch `#9b859b`, measured lines at 0.004, 0.201, 0.589, 0.876. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.02. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·T·None`; the k4 to k6 lines (None, 60 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·T·None` |
| Standard spectrometer detection range | 0.32 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 95.1 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1.8 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (1.1% of it). |
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
| Function | [[Divination and Sensing]], [[Negation and Counterspell]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Animal Messenger (2-E-L-AM)|Animal Messenger]] (2) · [[Blindness-Deafness (2-N-L-BD)|Blindness/Deafness]] (2) · [[Hunter's Mark (1-D-L-HSM)|Hunter's Mark]] (1) · [[Nondetection (3-A-L-NND)|Nondetection]] (3) · [[Alter Projectile Velocity (2-T-L-APV)|Alter Projectile Velocity]] (2) · [[Darkvision (2-T-L-DRKK)|Darkvision]] (2) · [[Hooke's Compelled Duel (0-E-L-HSCD)|Hooke's Compelled Duel]] (0) · [[Magic Weapon (2-T-L-MW)|Magic Weapon]] (2).


---

## Tactical Assessment

A silent-entry tool that is anything but silent; it trades stealth for speed at a breach. Useful when breaching charges would damage what lies behind the door.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
