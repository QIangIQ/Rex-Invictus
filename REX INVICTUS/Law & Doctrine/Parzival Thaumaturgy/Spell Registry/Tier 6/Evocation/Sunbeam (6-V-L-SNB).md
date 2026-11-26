---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-6
  - spell/evocation
  - source/srd
aliases:
  - "6th Tier Spell: Sunbeam"
  - "Sunbeam"
  - "6-V-L-SNB"
registry_id: 6-V-L-SNB
attribute_code: "6·Evo·Radiant·line (60)·Self·Up to 1 minute"
incantation: "Runat-Leporse"
tier: 6
school: Evocation
affinity: V
grade: L
pz_total: 11489.3
pz_quantum: 51944.6
t_e: 4.49
updated: 2026-11-16
---

**Sunbeam** (`6-V-L-SNB`) is a 6th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **11,489 Pz** against a slot quantum of 51,945 Pz, which puts its energy-equivalent tier at T_E 4.49 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 6 Workings]]
      - [[Evocation]]
        - **Sunbeam** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `6-V-L-SNB` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `6·Evo·Radiant·line (60)·Self·Up to 1 minute` |
| Incantation | *Runat-Leporse* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 6th Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | Self |
| Area | line (60) |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A magnifying glass |
| Ritual | no |
| Injury | 6d8 radiant (mean 27) |
| Injury by tier | T6: 6d8 |
| Resistance check | constitution; on success: half injury |
| Practitioner lineages | Druid, Sorcerer, Wizard |

### Mechanism

A 1.5 m wide, 18 m long beam of sunlight-grade radiation burns and blinds everything along it, and can be re-fired each round while a bright mote shines in the caster's hand.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Radiant beams, 10 over 1 min | `27 HP * 0.50 * 55.7 m^2 / 0.7 * 10` | 10,750 |
| Upkeep: Sunlight mote, 30 ft radius | `100 W * (30/20)^2 * 10 (sunlight grade) * 60 s / 1500` | 90.0 |
| Pattern cost | `0.01 × Q6 × (1 + 0.25)` | 649 |

| Quantity | Value |
|---|---|
| Effect energy | 10,750 Pz |
| Upkeep energy | 90.0 Pz (1.5 Pz/s) |
| **Total draw** | **11,489 Pz** (17,234.0 kJ) |
| Slot quantum Q6 | 51,945 Pz |
| Field gain (draw / quantum) | 0.221 |
| Energy-equivalent tier T_E | 4.49 |
| Handling points | 0.25 |
| Grade score | -0.50 → L |

**Handling flags:** concentration.

**Assumptions:** 6d8 = 27; one beam per round for 10 rounds; mote 10x torch luminance.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Sunbeam (6-V-L-SNB) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 6 | 6 | `0000000001101` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Radiant | 11 | `0000000010111` |
| k4 Area | line (60) | 25 | `0000000110011` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Runat-Leporse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T7: *Mirunat-Leporse* · T8: *Nirunat-Leporse* · T9: *Xyirunat-Leporse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 3→2 | 3 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 4→1 | 4 |
| k4 Area | 0→9 1→10 4→0 5→1 | 4 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#0485eb`.

![[Sunbeam (6-V-L-SNB) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 6 | 0.600 | 1.000 | `#00ebff` (520 nm eq.) | source grid |
| Damage | Radiant | 0.786 | 0.983 | `#1900ff` (464 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.995 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.996 | `#0074ff` (495 nm eq.) | source grid |
| Area | line (60) | 0.694 | 0.996 | `#0069ff` (492 nm eq.) | source grid |
| Range | Self | 0.706 | 0.994 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.23): swatch `#42ddd3`, measured lines at 0.501, 0.601, 0.687, 0.705, 0.786. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.06. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `6·V·Radiant`; the k4 to k6 lines (line (60), Self, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `6·V·Radiant` |
| Standard spectrometer detection range | 10.72 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 2,597 Pz (0.05 × Q6) |
| Counter drawn cold (all six layers) | 5,194 Pz (0.10 × Q6) |
| Unravel after completion | 5,212 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Life, Hope and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `2b 1c 1d 2f 1i 1j` (2x Heat, Light, Life, 2x Energy, Hope, Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1,915 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 6th Tier quantum of 51,945 Pz (22.1% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 6th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 6 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Light and Radiance]], [[Area Destruction]] |
| Element | [[Radiant Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Sunburst (8-V-L-SNBB)|Sunburst]] (8) · [[Burst Radiation (6-V-L-BR)|Burst Radiation]] (6) · [[Moonbeam (2-V-M-MNB)|Moonbeam]] (2) · [[Summon Demon Core (6-A-M-SDC)|Summon Demon Core]] (6) · [[Lightning Bolt (3-V-L-LB)|Lightning Bolt]] (3) · [[Absolute Zero (6-V-L-AZ)|Absolute Zero]] (6) · [[Blade Barrier (6-V-L-BB)|Blade Barrier]] (6) · [[Chain Lightning (6-V-L-CLA)|Chain Lightning]] (6).


---

## Tactical Assessment

A repeatable line weapon for clearing corridors and blinding optics, strongest against undead.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 6 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
