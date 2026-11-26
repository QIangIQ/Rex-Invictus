---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-0
  - spell/transmutation
  - source/srd
aliases:
  - "Cantrip Spell: Shillelagh"
  - "Shillelagh"
  - "0-T-L-SHLL"
registry_id: 0-T-L-SHLL
attribute_code: "0·Tra·None·None·Touch·1 minute"
incantation: "Cielixe"
tier: 0
school: Transmutation
affinity: T
grade: L
pz_total: 1.8
pz_quantum: 128.8
t_e: -4.29
updated: 2026-11-16
---

**Shillelagh** (`0-T-L-SHLL`) is a Cantrip (Tier 0) working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **1.8 Pz** against a slot quantum of 129 Pz, which puts its energy-equivalent tier at T_E -4.29 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 0 Workings]]
      - [[Transmutation]]
        - **Shillelagh** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `0-T-L-SHLL` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `0·Tra·None·None·Touch·1 minute` |
| Incantation | *Cielixe* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | Cantrip (Tier 0) |
| School | [[Transmutation]] |
| Casting time | 1 bonus action |
| Range | Touch |
| Area | single point or target |
| Duration | 1 minute |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Mistletoe, a shamrock leaf, and a club or quarterstaff |
| Ritual | no |
| Practitioner lineages | Druid |

### Mechanism

A wooden club or staff is reinforced by the field so its strikes hit harder and count as charged.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| added blunt injury, 6.5 hits x 2 points, focused | `6.5*2*0.46*0.08` | 0.478 |
| Pattern cost | `0.01 × Q0 × (1 + 0.00)` | 1.3 |

| Quantity | Value |
|---|---|
| Effect energy | 0.478 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **1.8 Pz** (2.6 kJ) |
| Slot quantum Q0 | 129 Pz |
| Field gain (draw / quantum) | 0.0137 |
| Energy-equivalent tier T_E | -4.29 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** 10 rounds; 65% hit rate; +2 points per hit.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Shillelagh (0-T-L-SHLL) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 0 | 0 | `0000000000001` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | 1 minute | 1 | `0000000000011` |

### Incantation

Spoken as **Cielixe** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T1: *Sicielixe* · T2: *Hicielixe* · T3: *Licielixe* · T4: *Vicielixe* · T5: *Ticielixe* · T6: *Ricielixe* · T7: *Micielixe* · T8: *Nicielixe* · T9: *Xyicielixe*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 | 1 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#d51d73`.

![[Shillelagh (0-T-L-SHLL) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 0 | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.682 | `#9600ff` (438 nm eq.) | source grid |
| Duration | 1 minute | 0.105 | 0.994 | `#ff6300` (668 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.678 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.22): swatch `#994690`, measured lines at 0.006, 0.106, 0.878. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 0.25. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `0·T·None`; the k4 to k6 lines (None, Touch, 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `0·T·None` |
| Standard spectrometer detection range | 0.13 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 6.4 Pz (0.05 × Q0) |
| Counter drawn cold (all six layers) | 12.9 Pz (0.10 × Q0) |
| Unravel after completion | 12.9 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 0.294 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the Cantrip (Tier 0) quantum of 129 Pz (1.4% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at Cantrip (Tier 0) up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 0 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Negation and Counterspell]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Reverse Entropy (0-T-L-REV)|Reverse Entropy]] (0) · [[Arcane Die (0-C-L-ADC)|Arcane Die]] (0) · [[Hooke's Compelled Duel (0-E-L-HSCD)|Hooke's Compelled Duel]] (0) · [[Knock (2-T-L-KNC)|Knock]] (2) · [[Magic Weapon (2-T-L-MW)|Magic Weapon]] (2) · [[Hawking's Mark (1-N-L-HSMK)|Hawking's Mark]] (1) · [[Hunter's Mark (1-D-L-HSM)|Hunter's Mark]] (1) · [[Mycelium Network (1-D-M-MN)|Mycelium Network]] (1).


---

## Tactical Assessment

A low-cost melee enhancement for lightly armed troops.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 0 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
