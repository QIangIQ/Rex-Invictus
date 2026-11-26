---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-7
  - spell/transmutation
  - source/srd
aliases:
  - "7th Tier Spell: Sequester"
  - "Sequester"
  - "7-T-L-SQS"
registry_id: 7-T-L-SQS
attribute_code: "7·Tra·None·None·Touch·Until dispelled"
incantation: "Mielixis"
tier: 7
school: Transmutation
affinity: T
grade: L
pz_total: 6700.7
pz_quantum: 141200.1
t_e: 3.95
updated: 2026-11-16
---

**Sequester** (`7-T-L-SQS`) is a 7th Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **6,701 Pz** against a slot quantum of 141,200 Pz, which puts its energy-equivalent tier at T_E 3.95 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 7 Workings]]
      - [[Transmutation]]
        - **Sequester** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `7-T-L-SQS` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `7·Tra·None·None·Touch·Until dispelled` |
| Incantation | *Mielixis* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 7th Tier |
| School | [[Transmutation]] |
| Casting time | 1 action |
| Range | Touch |
| Area | single point or target |
| Duration | Until dispelled |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A powder composed of diamond, emerald, ruby, and sapphire dust worth at least 5,000 gp, which the spell consumes |
| Ritual | no |
| Practitioner lineages | Wizard |

### Mechanism

A target is placed in timeless stasis, made invisible and screened from remote sensing until a set condition occurs.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| stasis lock, 1% of 80 kg body thermal content | `0.01*80*3500*310/1500` | 579 |
| [upkeep] trigger watch over 1 mile + screen, 30-day reference | `0.01*0.1 Pz/s*30 d  [C4]` | 2,592 |
| Pattern cost | `0.01 × Q7 × (1 + 1.50)` | 3,530 |

| Quantity | Value |
|---|---|
| Effect energy | 579 Pz |
| Upkeep energy | 2,592 Pz (0.162 Pz/s) |
| **Total draw** | **6,701 Pz** (10,051.0 kJ) |
| Slot quantum Q7 | 141,200 Pz |
| Field gain (draw / quantum) | 0.0475 |
| Energy-equivalent tier T_E | 3.95 |
| Handling points | 1.50 |
| Grade score | 0.50 → L |

Calibration applied: C4 (Dormant patterns), see [[Parzival Energy Budget#Registry calibration rules]].

**Handling flags:** costly material, consumed material, fragile.

**Assumptions:** Stasis cost set as 1% of body thermal content; open-ended duration counted over a 30-day reference.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Sequester (7-T-L-SQS) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 7 | 7 | `0000000001111` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Until dispelled | 11 | `0000000010111` |

### Incantation

Spoken as **Mielixis** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T8: *Nimielixis* · T9: *Xyimielixis*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 3→2 | 4 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 2→9 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#4b57fc`.

![[Sequester (7-T-L-SQS) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 7 | 0.700 | 1.000 | `#005eff` (490 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.985 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Until dispelled | 0.579 | 0.993 | `#00fff7` (526 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.984 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.22): swatch `#3997ec`, measured lines at 0.580, 0.701, 0.878. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.83. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `7·T·None`; the k4 to k6 lines (None, Touch, Until dispelled) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `7·T·None` |
| Standard spectrometer detection range | 8.19 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 7,060 Pz (0.05 × Q7) |
| Counter drawn cold (all six layers) | 14,120 Pz (0.10 × Q7) |
| Unravel after completion | 14,638 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1,117 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 7th Tier quantum of 141,200 Pz (4.7% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Endures independently once set, which places it under the decay clause of ULMTU-XIII. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIII]] | Lex Impermanentiae | Long-lived patterns drift toward reversion unless refreshed from a source that satisfies ULMTU-I. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 7th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 7 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Concealment and Illusion]], [[Movement and Flight]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Reverse Gravity (7-T-L-RG)|Reverse Gravity]] (7) · [[Wind Walk (6-T-L-WWD)|Wind Walk]] (6) · [[Dream of the Blue Veil (7-C-M-DBV)|Dream of the Blue Veil]] (7) · [[Mirage Arcane (7-I-M-MAR)|Mirage Arcane]] (7) · [[Project Image (7-I-L-PIO)|Project Image]] (7) · [[Telekinesis (5-P-L-TLK)|Telekinesis]] (5) · [[Freefall (4-T-L-FRF)|Freefall]] (4) · [[Programmed Illusion (6-I-L-PI)|Programmed Illusion]] (6).


---

## Tactical Assessment

Long-term concealment of assets, or holding a person in stasis until a set condition occurs.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 7 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
