---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/abjuration
  - source/srd
aliases:
  - "2nd Tier Spell: Warding Bond"
  - "Warding Bond"
  - "2-A-L-WB"
registry_id: 2-A-L-WB
attribute_code: "2·Abj·None·None·Touch·1 hour"
incantation: "Halixa"
tier: 2
school: Abjuration
affinity: A
grade: L
pz_total: 44.7
pz_quantum: 951.4
t_e: -1.06
updated: 2026-11-16
---

**Warding Bond** (`2-A-L-WB`) is a 2nd Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **44.7 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E -1.06 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Abjuration]]
        - **Warding Bond** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-A-L-WB` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Abj·None·None·Touch·1 hour` |
| Incantation | *Halixa* |
| Affinity | A (Abjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Abjuration]] |
| Casting time | 1 action |
| Range | Touch |
| Area | single point or target |
| Duration | 1 hour |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A pair of platinum rings worth at least 50gp each, which you and the target must wear for the duration |
| Ritual | no |
| Practitioner lineages | Cleric |

### Mechanism

A paired-ring link shields the ward, halving injury and slightly improving its defence, while routing the injury it does take to the caster.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Upkeep: Absorption on ward | `0.20 * 82.5 HP (75 halved + 7.5 from +1 defence)` | 16.5 |
| Upkeep: Injury transfer to caster | `67.5 HP * 0.20 * 0.5` | 6.8 |
| Pattern cost | `0.01 × Q2 × (1 + 1.25)` | 21.4 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 23.2 Pz (0.00646 Pz/s) |
| **Total draw** | **44.7 Pz** (67.0 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.0469 |
| Energy-equivalent tier T_E | -1.06 |
| Handling points | 1.25 |
| Grade score | 0.25 → L |

**Handling flags:** costly material, fragile.

**Assumptions:** 10 rounds of 15 HP incoming in the hour; transfer costed as directed necrotic-type delivery.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Warding Bond (2-A-L-WB) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | 1 hour | 0 | `0000000000001` |

### Incantation

Spoken as **Halixa** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihalixa* · T4: *Vihalixa* · T5: *Tihalixa* · T6: *Rihalixa* · T7: *Mihalixa* · T8: *Nihalixa* · T9: *Xyihalixa*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]]. This attribute set is shared with other workings, so the glyph carries 1 centre dot(s) to tell it apart.

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 | 1 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#e94540`.

![[Warding Bond (2-A-L-WB) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.980 | `#ff0028` (700 nm eq.) | source grid |
| Duration | 1 hour | 0.053 | 0.989 | `#ff1c00` (684 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.792 | `#9b00ff` (435 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 1.65. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·A·None`; the k4 to k6 lines (None, Touch, 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·A·None` |
| Standard spectrometer detection range | 0.67 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 99.8 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 7.4 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (4.7% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Wards and Shields]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Aid (2-A-L-AID)|Aid]] (2) · [[Leadskin (2-A-L-LDS)|Leadskin]] (2) · [[Protection from Poison (2-A-L-PP)|Protection from Poison]] (2) · [[Arcane Ward (1-A-L-AW)|Arcane Ward]] (1) · [[Bulwark (3-A-L-BLW)|Bulwark]] (3) · [[Glyph of Warding (3-A-H-GWY)|Glyph of Warding]] (3) · [[Mage Armor (1-P-L-MA)|Mage Armor]] (1) · [[Nondetection (3-A-L-NND)|Nondetection]] (3).


---

## Tactical Assessment

Protects a VIP or specialist at the cost of the bodyguard's health; separation beyond 18 m breaks it.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
