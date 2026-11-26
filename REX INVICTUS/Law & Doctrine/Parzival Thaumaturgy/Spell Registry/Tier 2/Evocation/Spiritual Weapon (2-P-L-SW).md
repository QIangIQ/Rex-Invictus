---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/evocation
  - source/srd
aliases:
  - "2nd Tier Spell: Spiritual Weapon"
  - "Spiritual Weapon"
  - "2-P-L-SW"
registry_id: 2-P-L-SW
attribute_code: "2·Evo·Force·None·60 feet·1 minute"
incantation: "Huton-’wyne"
tier: 2
school: Evocation
affinity: P
grade: L
pz_total: 15.3
pz_quantum: 951.4
t_e: -2.13
updated: 2026-11-16
---

**Spiritual Weapon** (`2-P-L-SW`) is a 2nd Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **15.3 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E -2.13 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Evocation]]
        - **Spiritual Weapon** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-P-L-SW` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Evo·Force·None·60 feet·1 minute` |
| Incantation | *Huton-’wyne* |
| Affinity | P (Pure field construct) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Evocation]] |
| Casting time | 1 bonus action |
| Range | 60 feet |
| Area | single point or target |
| Duration | 1 minute |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 1d8 + MOD force (mean 7.5) |
| Injury by tier | T2: 1d8 + MOD, T3: 1d8 + MOD, T4: 2d8 + MOD, T5: 2d8 + MOD, T6: 3d8 + MOD, T7: 3d8 + MOD, T8: 4d8 + MOD, T9: 4d8 + MOD |
| Delivery | aimed melee working |
| Practitioner lineages | Cleric |

### Mechanism

A floating force construct shaped as a weapon strikes targets near it and can be steered 6 m per round for one minute.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Force strikes, 10 over 1 min | `7.5 HP * 0.40 * 0.08 * 10` | 2.4 |
| Weapon translation 6.1 m per round | `0.5 * 3 kg * (6.1 m/s)^2 * 10 / 1500` | 0.372 |
| Upkeep: Construct autonomy | `0.05 Pz/s * 60 s` | 3.0 |
| Pattern cost | `0.01 × Q2 × (1 + 0.00)` | 9.5 |

| Quantity | Value |
|---|---|
| Effect energy | 2.8 Pz |
| Upkeep energy | 3.0 Pz (0.05 Pz/s) |
| **Total draw** | **15.3 Pz** (22.9 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.0161 |
| Energy-equivalent tier T_E | -2.13 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** 1d8 + 3 modifier = 7.5; 10 strikes; construct treated as 3 kg equivalent moving 6.1 m/s.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Spiritual Weapon (2-P-L-SW) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Force | 4 | `0000000001001` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | 1 minute | 1 | `0000000000011` |

### Incantation

Spoken as **Huton-’wyne** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihuton-’wyne* · T4: *Vihuton-’wyne* · T5: *Tihuton-’wyne* · T6: *Rihuton-’wyne* · T7: *Mihuton-’wyne* · T8: *Nihuton-’wyne* · T9: *Xyihuton-’wyne*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 3→0 | 2 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#74da4b`.

![[Spiritual Weapon (2-P-L-SW) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| Damage | Force | 0.357 | 0.988 | `#3bff00` (593 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.956 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | 1 minute | 0.105 | 0.996 | `#ff6300` (668 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.927 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.23): swatch `#b7c884`, measured lines at 0.106, 0.201, 0.358, 0.501, 0.589. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.18. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·V·Force`; the k4 to k6 lines (None, 60 feet, 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·V·Force` |
| Standard spectrometer detection range | 0.39 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 95.7 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Beyond, Introspection, 2x Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1b 2f 1G 3j` (Beyond, Heat, 2x Energy, Introspection, 3x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 2.5 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (1.6% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Pure]] (P) |
| Function | [[Summoning and Conjured Creatures]], [[Precision Strikes]] |
| Element | [[Force Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Arcane Sword (7-P-L-ASC)|Arcane Sword]] (7) · [[Magic Missile (1-P-L-MM)|Magic Missile]] (1) · [[Eldritch Blast (0-P-L-EB)|Eldritch Blast]] (0) · [[Acid Arrow (2-V-L-AA)|Acid Arrow]] (2) · [[Bohr's Model (2-P-L-BSM)|Bohr's Model]] (2) · [[Branding Smite (2-V-L-BS)|Branding Smite]] (2) · [[Dimension Door (4-P-L-DD)|Dimension Door]] (4) · [[Faithful Hound (4-C-L-FH)|Faithful Hound]] (4).


---

## Tactical Assessment

A remote striking tool that does not tie the caster down, good for harrying a target behind cover.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
