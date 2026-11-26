---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/transmutation
  - source/srd
aliases:
  - "2nd Tier Spell: Magic Weapon"
  - "Magic Weapon"
  - "2-T-L-MW"
registry_id: 2-T-L-MW
attribute_code: "2·Tra·None·None·Touch·Up to 1 hour"
incantation: "Hielixsi"
tier: 2
school: Transmutation
affinity: T
grade: L
pz_total: 13.3
pz_quantum: 951.4
t_e: -2.27
updated: 2026-11-16
---

**Magic Weapon** (`2-T-L-MW`) is a 2nd Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **13.3 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E -2.27 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Transmutation]]
        - **Magic Weapon** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-T-L-MW` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Tra·None·None·Touch·Up to 1 hour` |
| Incantation | *Hielixsi* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Transmutation]] |
| Casting time | 1 bonus action |
| Range | Touch |
| Area | single point or target |
| Duration | Up to 1 hour (concentration) |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Paladin, Wizard |

### Mechanism

The field charges an ordinary weapon so it strikes truer and harder, and it counts as enchanted against beings that resist mundane arms.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Added strike injury | `(10 hits * 1 + 0.5 extra hits * 7) HP * 0.40 * 0.08` | 0.432 |
| Weapon pattern imprint (instant info) | `instant info = 1 Pz` | 1.0 |
| Pattern cost | `0.01 × Q2 × (1 + 0.25)` | 11.9 |

| Quantity | Value |
|---|---|
| Effect energy | 1.4 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **13.3 Pz** (20.0 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.014 |
| Energy-equivalent tier T_E | -2.27 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** concentration.

**Assumptions:** Ten hits in a 1-minute engagement at +1 each, plus half an extra hit of 7 from improved accuracy; slashing blade.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Magic Weapon (2-T-L-MW) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Up to 1 hour | 12 | `0000000011001` |

### Incantation

Spoken as **Hielixsi** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihielixsi* · T4: *Vihielixsi* · T5: *Tihielixsi* · T6: *Rihielixsi* · T7: *Mihielixsi* · T8: *Nihielixsi* · T9: *Xyihielixsi*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]]. This attribute set is shared with other workings, so the glyph carries 2 centre dot(s) to tell it apart.

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 3→10 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#8e74b6`.

![[Magic Weapon (2-T-L-MW) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.796 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Up to 1 hour | 0.632 | 0.911 | `#00c0ff` (511 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.792 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.20): swatch `#8188ba`, measured lines at 0.201, 0.632, 0.878. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.12. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·T·None`; the k4 to k6 lines (None, Touch, Up to 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·T·None` |
| Standard spectrometer detection range | 0.37 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 95.1 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 2.2 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (1.4% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Negation and Counterspell]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Knock (2-T-L-KNC)|Knock]] (2) · [[Animal Messenger (2-E-L-AM)|Animal Messenger]] (2) · [[Arcane Lock (2-A-L-AL)|Arcane Lock]] (2) · [[Blindness-Deafness (2-N-L-BD)|Blindness/Deafness]] (2) · [[Gust of Wind (2-V-M-GW)|Gust of Wind]] (2) · [[Oscillate (2-C-L-OSC)|Oscillate]] (2) · [[Ray of Enfeeblement (2-N-L-RE)|Ray of Enfeeblement]] (2) · [[Reverse Entropy (0-T-L-REV)|Reverse Entropy]] (0).


---

## Tactical Assessment

Lets standard-issue blades and bayonets harm creatures that ignore conventional weapons. The gain in raw damage is small.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
