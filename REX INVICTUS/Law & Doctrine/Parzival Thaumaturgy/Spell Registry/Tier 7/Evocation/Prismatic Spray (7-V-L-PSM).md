---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-7
  - spell/evocation
  - source/srd
aliases:
  - "7th Tier Spell: Prismatic Spray"
  - "Prismatic Spray"
  - "7-V-L-PSM"
registry_id: 7-V-L-PSM
attribute_code: "7·Evo·None·cone (60)·Self·Instantaneous"
incantation: "Mu’-Nopor"
tier: 7
school: Evocation
affinity: V
grade: L
pz_total: 13295.5
pz_quantum: 141200.1
t_e: 4.64
updated: 2026-11-16
---

**Prismatic Spray** (`7-V-L-PSM`) is a 7th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **13,296 Pz** against a slot quantum of 141,200 Pz, which puts its energy-equivalent tier at T_E 4.64 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 7 Workings]]
      - [[Evocation]]
        - **Prismatic Spray** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `7-V-L-PSM` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `7·Evo·None·cone (60)·Self·Instantaneous` |
| Incantation | *Mu’-Nopor* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 7th Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | Self |
| Area | cone (60) |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 10d6 untyped (mean 35) |
| Injury by tier | T7: 10d6 |
| Resistance check | agility; on success: other |
| Practitioner lineages | Sorcerer, Wizard |

### Mechanism

Eight spectral bands fan out in a cone, each target intercepting one or two at random. Five bands carry thermal, chemical, electrical or toxic injury, one petrifies and one ejects the target off-plane.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| band damage in 60 ft cone, 10d6 (35) x expected kappa 1.125*(2.2/7) | `35*1.125*(0.70+0.25+0.30+0.05+0.90)/7*(0.666*(60*ft)**2)/Ac` | 3,938 |
| indigo band petrification, 6 targets x P(1.125/7) x 80 kg stone at 3 Pz/kg | `6*(1.125/7)*3*80` | 231 |
| violet band plane ejection, 6 targets x P(1.125/7) | `6*(1.125/7)*0.01*80*15*1e6/1500` | 7,714 |
| Pattern cost | `0.01 × Q7 × (1 + 0.00)` | 1,412 |

| Quantity | Value |
|---|---|
| Effect energy | 11,884 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **13,296 Pz** (19,943.3 kJ) |
| Slot quantum Q7 | 141,200 Pz |
| Field gain (draw / quantum) | 0.0942 |
| Energy-equivalent tier T_E | 4.64 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Cone length 60 ft; expected 1.125 bands per target over 7 colours; 6 creatures in the cone for the special bands; full damage.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Prismatic Spray (7-V-L-PSM) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 7 | 7 | `0000000001111` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | cone (60) | 4 | `0000000001001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Mu’-Nopor** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T8: *Nimu’-Nopor* · T9: *Xyimu’-Nopor*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 3→2 | 4 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 3→12 | 2 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#597193`.

![[Prismatic Spray (7-V-L-PSM) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 7 | 0.700 | 1.000 | `#005eff` (490 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.980 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.783 | `#ff0028` (700 nm eq.) | source grid |
| Area | cone (60) | 0.111 | 0.841 | `#ff6e00` (667 nm eq.) | source grid |
| Range | Self | 0.706 | 1.000 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.21): swatch `#5fc9b5`, measured lines at 0.004, 0.112, 0.501, 0.703. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.12. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `7·V·None`; the k4 to k6 lines (cone (60), Self, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `7·V·None` |
| Standard spectrometer detection range | 11.53 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 7,060 Pz (0.05 × Q7) |
| Counter drawn cold (all six layers) | 14,120 Pz (0.10 × Q7) |
| Unravel after completion | 14,120 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1b 1c 1d 1f` (Heat, Light, Life, Energy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 2,216 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 7th Tier quantum of 141,200 Pz (9.4% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 7th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 7 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Light and Radiance]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Chain Lightning (6-V-L-CLA)|Chain Lightning]] (6) · [[Sunbeam (6-V-L-SNB)|Sunbeam]] (6) · [[Sunburst (8-V-L-SNBB)|Sunburst]] (8) · [[Arcane Sword (7-P-L-ASC)|Arcane Sword]] (7) · [[Dark Matter Sword (7-V-L-DMS)|Dark Matter Sword]] (7) · [[Daylight (3-V-L-DYL)|Daylight]] (3) · [[Delayed Blast Fireball (7-V-M-DBF)|Delayed Blast Fireball]] (7) · [[Divine Word (7-V-L-DWV)|Divine Word]] (7).


---

## Tactical Assessment

A wide-area disruptor with unpredictable per-target results, good against massed infantry in a cone.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 7 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
