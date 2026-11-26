---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/evocation
  - source/srd
aliases:
  - "2nd Tier Spell: Prayer of Healing"
  - "Prayer of Healing"
  - "2-V-L-PH"
registry_id: 2-V-L-PH
attribute_code: "2·Evo·None·None·30 feet·Instantaneous"
incantation: "Huusin"
tier: 2
school: Evocation
affinity: V
grade: L
pz_total: 33.5
pz_quantum: 951.4
t_e: -1.35
updated: 2026-11-16
---

**Prayer of Healing** (`2-V-L-PH`) is a 2nd Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **33.5 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E -1.35 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Evocation]]
        - **Prayer of Healing** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-V-L-PH` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Evo·None·None·30 feet·Instantaneous` |
| Incantation | *Huusin* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Evocation]] |
| Casting time | 10 minutes |
| Range | 30 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation) |
| Ritual | no |
| Restoration | 2d8 + MOD restored (mean 12, modifier taken as +3) |
| Practitioner lineages | Cleric |

### Mechanism

A ten-minute invocation drives tissue repair in up to six allies at once.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| healing 6 targets x (2d8+3 = 12) | `0.30*12*6` | 21.6 |
| Pattern cost | `0.01 × Q2 × (1 + 0.25)` | 11.9 |

| Quantity | Value |
|---|---|
| Effect energy | 21.6 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **33.5 Pz** (50.2 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.0352 |
| Energy-equivalent tier T_E | -1.35 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** long cast.

**Assumptions:** Six targets; modifier +3; healing at 0.30 Pz per point.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Prayer of Healing (2-V-L-PH) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Huusin** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihuusin* · T4: *Vihuusin* · T5: *Tihuusin* · T6: *Rihuusin* · T7: *Mihuusin* · T8: *Nihuusin* · T9: *Xyihuusin*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#a5ba2b`.

![[Prayer of Healing (2-V-L-PH) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.956 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.980 | `#ff0028` (700 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.996 | `#91ff00` (612 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.21): swatch `#c9ba75`, measured lines at 0.004, 0.201, 0.295, 0.501. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.52. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·V·None`; the k4 to k6 lines (None, 30 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·V·None` |
| Standard spectrometer detection range | 0.58 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 95.1 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1b 1c 1d 1f` (Heat, Light, Life, Energy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 5.6 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (3.5% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Healing and Restoration]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Cure Wounds (1-V-L-CW)|Cure Wounds]] (1) · [[Healing Word (1-V-L-HW)|Healing Word]] (1) · [[Mass Healing Word (3-V-L-MHW)|Mass Healing Word]] (3) · [[Lesser Restoration (2-A-L-LR)|Lesser Restoration]] (2) · [[Thomson's Plum Pudding (2-T-L-TSPP)|Thomson's Plum Pudding]] (2) · [[Goodberry (1-T-L-GDB)|Goodberry]] (1) · [[Remove Curse (3-A-L-RC)|Remove Curse]] (3) · [[Revivify (3-C-L-RVV)|Revivify]] (3).


---

## Tactical Assessment

An efficient post-engagement triage measure for a squad, too slow to use under fire.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
