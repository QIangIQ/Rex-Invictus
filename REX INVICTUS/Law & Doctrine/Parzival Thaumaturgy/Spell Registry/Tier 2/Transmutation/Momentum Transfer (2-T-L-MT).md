---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/transmutation
  - source/science-spellbook
aliases:
  - "2nd Tier Spell: Momentum Transfer"
  - "2-T-L-MT"
  - "Momentum Transfer (Science)"
registry_id: 2-T-L-MT
attribute_code: "2·Tra·None·None·Touch·until the beginning of your next turn"
incantation: "Hielixbey"
tier: 2
school: Transmutation
affinity: T
grade: L
pz_total: 9.8
pz_quantum: 951.4
t_e: -2.58
updated: 2026-11-16
---

**Momentum Transfer** (`2-T-L-MT`) is a 2nd Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **9.8 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E -2.58 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Transmutation]]
        - **Momentum Transfer** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-T-L-MT` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Tra·None·None·Touch·until the beginning of your next turn` |
| Incantation | *Hielixbey* |
| Affinity | T (Transmutation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Transmutation]] |
| Casting time | 1 Action |
| Range | Touch |
| Area | single point or target |
| Duration | until the beginning of your next turn |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Wizard, Sorcerer, Druid |

### Mechanism

Moves the caster's remaining motion into a touched ally, who gains that much speed while the caster stops.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Kinetic energy transferred | `0.5 x 80 kg x (3.05^2 - 1.52^2) = 278.7 J / 1500` | 0.186 |
| Motion link, 2 creatures (upkeep) | `enchantment 0.005 x 2: 0.01 Pz/s x 6 s` | 0.06 |
| Pattern cost | `0.01 × Q2 × (1 + 0.00)` | 9.5 |

| Quantity | Value |
|---|---|
| Effect energy | 0.186 Pz |
| Upkeep energy | 0.06 Pz (0.01 Pz/s) |
| **Total draw** | **9.8 Pz** (14.6 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.0103 |
| Energy-equivalent tier T_E | -2.58 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** 80 kg ally raised from 1.52 to 3.05 m/s; enchantment on 2 creatures for one round.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Momentum Transfer (2-T-L-MT) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | until the beginning of your next turn | 23 | `0000000101111` |

### Incantation

Spoken as **Hielixbey** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihielixbey* · T4: *Vihielixbey* · T5: *Tihielixbey* · T6: *Rihielixbey* · T7: *Mihielixbey* · T8: *Nihielixbey* · T9: *Xyihielixbey*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 2→9 3→10 5→12 | 5 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#ce46ab`.

![[Momentum Transfer (2-T-L-MT) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.796 | `#9600ff` (438 nm eq.) | source grid |
| Duration | until the beginning of your next turn | 0.974 | 0.741 | `#ff00df` (408 nm eq.) | RI half-step |
| Range | Touch | 0.882 | 0.792 | `#9b00ff` (435 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 0.99. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·T·None`; the k4 to k6 lines (None, Touch, until the beginning of your next turn) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·T·None` |
| Standard spectrometer detection range | 0.31 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 95.2 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1.6 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (1.0% of it). |
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

Similar workings: [[Magnetise (2-T-L-MGN)|Magnetise]] (2) · [[Alter Weight (1-T-L-AWT)|Alter Weight]] (1) · [[Arcane Gyroscope (1-T-L-AG)|Arcane Gyroscope]] (1) · [[Sublimation (3-T-L-SBL)|Sublimation]] (3) · [[Vapour Deposition (1-T-L-VD)|Vapour Deposition]] (1) · [[Carbon Dating (2-D-L-CDR)|Carbon Dating]] (2) · [[Moderator (2-A-L-MDR)|Moderator]] (2) · [[Predict Projectiles (2-D-L-PPE)|Predict Projectiles]] (2).


---

## Tactical Assessment

Lets a runner or medic outpace pursuit for a moment.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
