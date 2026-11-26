---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/evocation
  - source/srd
aliases:
  - "3rd Tier Spell: Sending"
  - "Sending"
  - "3-V-L-SND"
registry_id: 3-V-L-SND
attribute_code: "3·Evo·None·None·Unlimited·1 round"
incantation: "Luashi"
tier: 3
school: Evocation
affinity: V
grade: L
pz_total: 626.9
pz_quantum: 2586.2
t_e: 1.58
updated: 2026-11-16
---

**Sending** (`3-V-L-SND`) is a 3rd Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **627 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E 1.58 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Evocation]]
        - **Sending** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-V-L-SND` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Evo·None·None·Unlimited·1 round` |
| Incantation | *Luashi* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | Unlimited |
| Area | single point or target |
| Duration | 1 round |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A short piece of fine copper wire |
| Ritual | no |
| Practitioner lineages | Bard, Cleric, Wizard |

### Mechanism

A short message is placed directly into the mind of a known recipient anywhere, with a reply returned the same way.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| mind-to-mind message across one boundary or 1000 km, 1 round | `0.001*(1e6/10)*6` | 600 |
| message encoding, instant information | `1` | 1.0 |
| Pattern cost | `0.01 × Q3 × (1 + 0.00)` | 25.9 |

| Quantity | Value |
|---|---|
| Effect energy | 601 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **627 Pz** (940.3 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 0.242 |
| Energy-equivalent tier T_E | 1.58 |
| Handling points | 0.00 |
| Grade score | -0.71 → L |

**Handling flags:** none.

**Assumptions:** Effective range 1e6 m; 6 s link.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Sending (3-V-L-SND) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Unlimited | 16 | `0000000100001` |
| k6 Duration | 1 round | 2 | `0000000000101` |

### Incantation

Spoken as **Luashi** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Viluashi* · T5: *Tiluashi* · T6: *Riluashi* · T7: *Miluashi* · T8: *Niluashi* · T9: *Xyiluashi*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 5→0 | 2 |
| k6 Duration | 0→7 2→9 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#9ab25a`.

![[Sending (3-V-L-SND) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.980 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | 1 round | 0.158 | 0.990 | `#ffae00` (653 nm eq.) | source grid |
| Range | Unlimited | 0.941 | 0.814 | `#ed00ff` (418 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.22): swatch `#afbb99`, measured lines at 0.159, 0.300, 0.501, 0.942. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.80. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·V·None`; the k4 to k6 lines (None, Unlimited, 1 round) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·V·None` |
| Standard spectrometer detection range | 2.50 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 259 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1b 1c 1d 1f` (Heat, Light, Life, Energy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 104 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 3rd Tier quantum of 2,586 Pz (24.2% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Divination and Sensing]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Arcane Hand (5-P-L-AH)|Arcane Hand]] (5) · [[Arcane Singularity (3-C-L-ASA)|Arcane Singularity]] (3) · [[Clairvoyance (3-D-L-CLR)|Clairvoyance]] (3) · [[Focusing Lens (1-V-L-FLC)|Focusing Lens]] (1) · [[Nondetection (3-A-L-NND)|Nondetection]] (3) · [[Shannon's Coding Theorem (3-D-L-SSCT)|Shannon's Coding Theorem]] (3) · [[Speak with Dead (3-N-L-SDE)|Speak with Dead]] (3) · [[Speak with Plants (3-T-L-SP)|Speak with Plants]] (3).


---

## Tactical Assessment

Unjammable long-range and interplanar signalling for brief orders and reports.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
