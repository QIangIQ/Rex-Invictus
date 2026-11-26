---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/divination
  - source/science-spellbook
aliases:
  - "1st Tier Spell: Mycelium Network"
  - "1-D-M-MN"
  - "Mycelium Network (Science)"
registry_id: 1-D-M-MN
attribute_code: "1·Div·None·sphere (300)·Touch·Up to 8 hours"
incantation: "Si’-Soalixos"
tier: 1
school: Divination
affinity: D
grade: M
pz_total: 272.1
pz_quantum: 350.0
t_e: 0.75
updated: 2026-11-16
---

**Mycelium Network** (`1-D-M-MN`) is a 1st Tier working of the [[Divination]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **272 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E 0.75 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Divination]]
        - **Mycelium Network** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-D-M-MN` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Div·None·sphere (300)·Touch·Up to 8 hours` |
| Incantation | *Si’-Soalixos* |
| Affinity | D (Divination) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Divination]] |
| Casting time | 1 Action |
| Range | Touch |
| Area | sphere (300) |
| Duration | Up to 8 hours (concentration) |
| Components | spoken (incantation), material focus. Material: A rare preserved mushroom worth 10GP |
| Ritual | no |

### Mechanism

Taps an underground fungal network to sense movement within 300 ft while the caster stays in contact with the ground.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Network sensing (upkeep) | `divination 0.001 x (91.44/10): 0.009144 Pz/s x 28800 s` | 263 |
| Pattern cost | `0.01 × Q1 × (1 + 1.50)` | 8.8 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 263 Pz (0.00914 Pz/s) |
| **Total draw** | **272 Pz** (408.1 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.777 |
| Energy-equivalent tier T_E | 0.75 |
| Handling points | 1.50 |
| Grade score | 1.37 → M |

**Handling flags:** concentration, costly material, fragile.

**Assumptions:** Divination rate for 91.44 m held 8 hours; an existing network is assumed (seeding a new one adds about 260 Pz of living matter).

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Mycelium Network (1-D-M-MN) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Divination | 2 | `0000000000101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (300) | 41 | `0000001010011` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Up to 8 hours | 18 | `0000000100101` |

### Incantation

Spoken as **Si’-Soalixos** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisi’-Soalixos* · T3: *Lisi’-Soalixos* · T4: *Visi’-Soalixos* · T5: *Tisi’-Soalixos* · T6: *Risi’-Soalixos* · T7: *Misi’-Soalixos* · T8: *Nisi’-Soalixos* · T9: *Xyisi’-Soalixos*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 2→0 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 4→0 6→2 | 4 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 2→9 5→12 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#cd5285`.

![[Mycelium Network (1-D-M-MN) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Divination | 0.250 | 0.989 | `#cdff00` (625 nm eq.) | source grid |
| Duration | Up to 8 hours | 0.947 | 0.698 | `#f800ff` (416 nm eq.) | source grid |
| Area | sphere (300) | 0.875 | 0.741 | `#9600ff` (438 nm eq.) | RI half-step |
| Range | Touch | 0.882 | 0.736 | `#9b00ff` (435 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 2.43. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·D·None`; the k4 to k6 lines (sphere (300), Touch, Up to 8 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·D·None` |
| Standard spectrometer detection range | 1.65 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 87.7 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Light, 2x Extraspection. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 2c 1d 1F 2g 1J` (Beyond, 2x Light, Life, Potential, 2x Extraspection, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 45.3 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (77.7% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Divination school with aspect lean Beyond, Light, 2x Extraspection. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Divination]] |
| Affinity | [[Divination]] (D) |
| Function | [[Negation and Counterspell]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Hunter's Mark (1-D-L-HSM)|Hunter's Mark]] (1) · [[Hawking's Mark (1-N-L-HSMK)|Hawking's Mark]] (1) · [[Animal Messenger (2-E-L-AM)|Animal Messenger]] (2) · [[Arcane Die (0-C-L-ADC)|Arcane Die]] (0) · [[Arcane Lock (2-A-L-AL)|Arcane Lock]] (2) · [[Blindness-Deafness (2-N-L-BD)|Blindness/Deafness]] (2) · [[Gust of Wind (2-V-M-GW)|Gust of Wind]] (2) · [[Hooke's Compelled Duel (0-E-L-HSCD)|Hooke's Compelled Duel]] (0).


---

## Tactical Assessment

Static perimeter sensing for camps and outposts.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Divination]] · [[Spell Breakdown Procedure]] · [[Parzival]]
