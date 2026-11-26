---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/evocation
  - source/srd
aliases:
  - "2nd Tier Spell: Acid Arrow"
  - "Acid Arrow"
  - "2-V-L-AA"
registry_id: 2-V-L-AA
attribute_code: "2·Evo·Acid·None·90 feet·Instantaneous"
incantation: "Hucid-’ylar"
tier: 2
school: Evocation
affinity: V
grade: L
pz_total: 11.4
pz_quantum: 951.4
t_e: -2.43
updated: 2026-11-16
---

**Acid Arrow** (`2-V-L-AA`) is a 2nd Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **11.4 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E -2.43 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Evocation]]
        - **Acid Arrow** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-V-L-AA` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Evo·Acid·None·90 feet·Instantaneous` |
| Incantation | *Hucid-’ylar* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 90 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Powdered rhubarb leaf and an adder's stomach |
| Ritual | no |
| Injury | 4d4 acid (mean 10) |
| Injury by tier | T2: 4d4, T3: 5d4, T4: 6d4, T5: 7d4, T6: 8d4, T7: 9d4, T8: 10d4, T9: 11d4 |
| Delivery | aimed ranged working |
| Practitioner lineages | Wizard |

### Mechanism

A condensed bolt of field-bound acid is projected at one target and ruptures on contact, leaving a corrosive film that keeps reacting until the following round.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| initial acid burst | `10 HP * 0.25 Pz/HP (acid) * F 0.5 * 1 target(s)/hit(s)` | 1.2 |
| residual acid burn | `5 HP * 0.25 Pz/HP (acid) * F 0.5 * 1 target(s)/hit(s)` | 0.625 |
| Pattern cost | `0.01 × Q2 × (1 + 0.00)` | 9.5 |

| Quantity | Value |
|---|---|
| Effect energy | 1.9 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **11.4 Pz** (17.1 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.012 |
| Energy-equivalent tier T_E | -2.43 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Average 10 injury points on impact plus 5 delayed; directed bolt factor 0.5; single target; full damage on a hit.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Acid Arrow (2-V-L-AA) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Acid | 0 | `0000000000001` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 90 feet | 11 | `0000000010111` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Hucid-’ylar** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihucid-’ylar* · T4: *Vihucid-’ylar* · T5: *Tihucid-’ylar* · T6: *Rihucid-’ylar* · T7: *Mihucid-’ylar* · T8: *Nihucid-’ylar* · T9: *Xyihucid-’ylar*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 | 1 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 4→12 | 4 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#9c8d53`.

![[Acid Arrow (2-V-L-AA) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| Damage | Acid | 0.071 | 0.992 | `#ff3700` (679 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.956 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.980 | `#ff0028` (700 nm eq.) | source grid |
| Range | 90 feet | 0.647 | 0.905 | `#00aaff` (506 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.13): swatch `#b9a573`, measured lines at 0.004, 0.072, 0.201, 0.501, 0.648. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.06. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·V·Acid`; the k4 to k6 lines (None, 90 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·V·Acid` |
| Standard spectrometer detection range | 0.34 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 95.1 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Death, 2x Diminutive and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `2b 1D 2E 2f 1j` (2x Heat, Death, 2x Diminutive, 2x Energy, Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1.9 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (1.2% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Precision Strikes]] |
| Element | [[Acid Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Acid Splash (0-C-L-AS)|Acid Splash]] (0) · [[Branding Smite (2-V-L-BS)|Branding Smite]] (2) · [[Flame Blade (2-V-L-FBA)|Flame Blade]] (2) · [[Scorching Ray (2-V-L-SR)|Scorching Ray]] (2) · [[Spiritual Weapon (2-P-L-SW)|Spiritual Weapon]] (2) · [[Divine Favor (1-V-L-DF)|Divine Favor]] (1) · [[Electrify (1-V-L-ELC)|Electrify]] (1) · [[Focusing Lens (1-V-L-FLC)|Focusing Lens]] (1).


---

## Tactical Assessment

Useful against soft-skinned crews and exposed optics; the lingering film degrades seals and sensor windows on light vehicles.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
