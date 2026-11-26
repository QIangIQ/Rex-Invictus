---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-0
  - spell/illusion
  - source/srd
aliases:
  - "Cantrip Spell: Minor Illusion"
  - "Minor Illusion"
  - "0-I-L-MI"
registry_id: 0-I-L-MI
attribute_code: "0·Ill·None·None·30 feet·1 minute"
incantation: "Caiusine"
tier: 0
school: Illusion
affinity: I
grade: L
pz_total: 1.3
pz_quantum: 128.8
t_e: -4.57
updated: 2026-11-16
---

**Minor Illusion** (`0-I-L-MI`) is a Cantrip (Tier 0) working of the [[Illusion]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **1.3 Pz** against a slot quantum of 129 Pz, which puts its energy-equivalent tier at T_E -4.57 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 0 Workings]]
      - [[Illusion]]
        - **Minor Illusion** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `0-I-L-MI` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `0·Ill·None·None·30 feet·1 minute` |
| Incantation | *Caiusine* |
| Affinity | I (Illusion) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | Cantrip (Tier 0) |
| School | [[Illusion]] |
| Casting time | 1 action |
| Range | 30 feet |
| Area | single point or target |
| Duration | 1 minute |
| Components | somatic (glyph kata), material focus. Material: A bit of fleece |
| Ritual | no |
| Practitioner lineages | Bard, Sorcerer, Warlock, Wizard |

### Mechanism

The field produces either a static image no larger than a 5 ft cube or a sound from whisper to scream for up to a minute. Touch passes through the image.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Image volume, 5 ft cube (upkeep) | `0.002 Pz/s * (3.540 m^3/1000) * 60 s` | 0.000425 |
| Sound option, scream level (upkeep) | `1 W / 1500 * 60 s` | 0.04 |
| Pattern cost | `0.01 × Q0 × (1 + 0.00)` | 1.3 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 0.0404 Pz (0.000674 Pz/s) |
| **Total draw** | **1.3 Pz** (2.0 kJ) |
| Slot quantum Q0 | 129 Pz |
| Field gain (draw / quantum) | 0.0103 |
| Energy-equivalent tier T_E | -4.57 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Both options costed together as an upper bound; 1 W acoustic for a scream.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Minor Illusion (0-I-L-MI) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 0 | 0 | `0000000000001` |
| k2 School | Illusion | 5 | `0000000001011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | 1 minute | 1 | `0000000000011` |

### Incantation

Spoken as **Caiusine** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T1: *Sicaiusine* · T2: *Hicaiusine* · T3: *Licaiusine* · T4: *Vicaiusine* · T5: *Ticaiusine* · T6: *Ricaiusine* · T7: *Micaiusine* · T8: *Nicaiusine* · T9: *Xyicaiusine*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 | 1 |
| k2 School | 0→11 1→12 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#ab8542`.

![[Minor Illusion (0-I-L-MI) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 0 | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| School | Illusion | 0.625 | 0.823 | `#00c5ff` (512 nm eq.) | source grid |
| Duration | 1 minute | 0.105 | 0.994 | `#ff6300` (668 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.958 | `#91ff00` (612 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.20): swatch `#b09672`, measured lines at 0.006, 0.106, 0.295, 0.626. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 0.12. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `0·I·None`; the k4 to k6 lines (None, 30 feet, 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `0·I·None` |
| Standard spectrometer detection range | 0.12 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 6.4 Pz (0.05 × Q0) |
| Counter drawn cold (all six layers) | 12.9 Pz (0.10 × Q0) |
| Unravel after completion | 12.9 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Light, Introspection, 2x Flexibility. The working vector used by [[Recast Tension and Combination Affinity]] is `2c 1d 1F 1G 2h 1J` (2x Light, Life, Potential, Introspection, 2x Flexibility, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 0.221 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the Cantrip (Tier 0) quantum of 129 Pz (1.0% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at Cantrip (Tier 0) up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Illusion school with aspect lean Light, Introspection, 2x Flexibility. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 0 Workings]] |
| School | [[Illusion]] |
| Affinity | [[Illusion]] (I) |
| Function | [[Concealment and Illusion]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Alter Difraction Pattern (1-I-L-ADP)|Alter Difraction Pattern]] (1) · [[Disguise Self (1-I-L-DS)|Disguise Self]] (1) · [[Illusory Script (1-I-L-IS)|Illusory Script]] (1) · [[Moe's Sensory Illusion (1-I-L-MSSI)|Moe's Sensory Illusion]] (1) · [[One Way Mirror (1-I-L-OWM)|One Way Mirror]] (1) · [[Silent Image (1-I-L-SI)|Silent Image]] (1) · [[Arcanist's Magic Aura (2-I-L-ASMA)|Arcanist's Magic Aura]] (2) · [[Blur (2-I-L-BLR)|Blur]] (2).


---

## Tactical Assessment

A cheap distraction, such as footsteps down a corridor or a crate to hide behind. Close inspection reveals it.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 0 Workings]] · [[Illusion]] · [[Spell Breakdown Procedure]] · [[Parzival]]
