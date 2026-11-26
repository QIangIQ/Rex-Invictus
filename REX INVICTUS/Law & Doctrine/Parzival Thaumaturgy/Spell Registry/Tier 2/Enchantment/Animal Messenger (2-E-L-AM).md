---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/enchantment
  - source/srd
aliases:
  - "2nd Tier Spell: Animal Messenger"
  - "Animal Messenger"
  - "2-E-L-AM"
registry_id: 2-E-L-AM
attribute_code: "2·Enc·None·None·30 feet·24 hours"
incantation: "Housinl"
tier: 2
school: Enchantment
affinity: E
grade: L
pz_total: 445.9
pz_quantum: 951.4
t_e: 1.24
updated: 2026-11-16
---

**Animal Messenger** (`2-E-L-AM`) is a 2nd Tier working of the [[Enchantment]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **446 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E 1.24 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Enchantment]]
        - **Animal Messenger** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-E-L-AM` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Enc·None·None·30 feet·24 hours` |
| Incantation | *Housinl* |
| Affinity | E (Enchantment) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Enchantment]] |
| Casting time | 1 action |
| Range | 30 feet |
| Area | single point or target |
| Duration | 24 hours |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A morsel of food |
| Ritual | yes |
| Practitioner lineages | Bard, Druid, Ranger |

### Mechanism

A tiny animal is directed to carry a short spoken message to a described recipient at a known location, travelling under its own power for a day.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| instant information | `1 * 1 Pz` | 1.0 |
| voice imprint | `25-word message stored and replayed` | 1.0 |
| enchantment upkeep | `0.005 Pz/s * 1 creature(s) * 86400 s` | 432 |
| Pattern cost | `0.01 × Q2 × (1 + 0.25)` | 11.9 |

| Quantity | Value |
|---|---|
| Effect energy | 2.0 Pz |
| Upkeep energy | 432 Pz (0.005 Pz/s) |
| **Total draw** | **446 Pz** (668.8 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.469 |
| Energy-equivalent tier T_E | 1.24 |
| Handling points | 0.25 |
| Grade score | -0.13 → L |

**Handling flags:** ritual.

**Assumptions:** Animal travels under its own metabolism; 24 h guidance at 0.005 Pz/s; message storage counted as 1 Pz.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Animal Messenger (2-E-L-AM) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Enchantment | 3 | `0000000000111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | 24 hours | 5 | `0000000001011` |

### Incantation

Spoken as **Housinl** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihousinl* · T4: *Vihousinl* · T5: *Tihousinl* · T6: *Rihousinl* · T7: *Mihousinl* · T8: *Nihousinl* · T9: *Xyihousinl*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 1→12 2→0 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 3→10 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#89f900`.

![[Animal Messenger (2-E-L-AM) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Enchantment | 0.375 | 0.985 | `#20ff00` (588 nm eq.) | source grid |
| Duration | 24 hours | 0.316 | 0.993 | `#76ff00` (605 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.996 | `#91ff00` (612 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.13): swatch `#dec872`, measured lines at 0.201, 0.295, 0.316, 0.376. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.65. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·E·None`; the k4 to k6 lines (None, 30 feet, 24 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·E·None` |
| Standard spectrometer detection range | 2.11 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 182 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Introspection, Flexibility, Hope. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1G 1h 1i 1J` (Within, Light, Life, Potential, Introspection, Flexibility, Hope, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 74.3 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (46.9% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Enchantment school with aspect lean Within, Introspection, Flexibility, Hope. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Enchantment]] |
| Affinity | [[Enchantment]] (E) |
| Function | [[Divination and Sensing]], [[Negation and Counterspell]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Blindness-Deafness (2-N-L-BD)|Blindness/Deafness]] (2) · [[Hooke's Compelled Duel (0-E-L-HSCD)|Hooke's Compelled Duel]] (0) · [[Knock (2-T-L-KNC)|Knock]] (2) · [[Hunter's Mark (1-D-L-HSM)|Hunter's Mark]] (1) · [[Nondetection (3-A-L-NND)|Nondetection]] (3) · [[Time Dilation (5-I-L-TD)|Time Dilation]] (5) · [[Alter Projectile Velocity (2-T-L-APV)|Alter Projectile Velocity]] (2) · [[Arcane Lock (2-A-L-AL)|Arcane Lock]] (2).


---

## Tactical Assessment

A courier channel that cannot be intercepted by signals intelligence, useful under jamming or emission control.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Enchantment]] · [[Spell Breakdown Procedure]] · [[Parzival]]
