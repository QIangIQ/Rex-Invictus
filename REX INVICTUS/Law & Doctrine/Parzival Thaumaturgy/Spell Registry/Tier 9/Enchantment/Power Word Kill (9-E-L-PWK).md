---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-9
  - spell/enchantment
  - source/srd
aliases:
  - "9th Tier Spell: Power Word Kill"
  - "Power Word Kill"
  - "9-E-L-PWK"
registry_id: 9-E-L-PWK
attribute_code: "9·Enc·None·None·60 feet·Instantaneous"
incantation: "Xyowyn"
tier: 9
school: Enchantment
affinity: E
grade: L
pz_total: 13052.7
pz_quantum: 1043335.3
t_e: 4.62
updated: 2026-11-16
---

**Power Word Kill** (`9-E-L-PWK`) is a 9th Tier working of the [[Enchantment]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **13,053 Pz** against a slot quantum of 1.04 MPz Pz, which puts its energy-equivalent tier at T_E 4.62 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 9 Workings]]
      - [[Enchantment]]
        - **Power Word Kill** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `9-E-L-PWK` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `9·Enc·None·None·60 feet·Instantaneous` |
| Incantation | *Xyowyn* |
| Affinity | E (Enchantment) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 9th Tier |
| School | [[Enchantment]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation) |
| Ritual | no |
| Practitioner lineages | Bard, Sorcerer, Warlock, Wizard |

### Mechanism

A spoken trigger couples the field to a target's vital processes and halts them outright if total vitality is below a fixed threshold.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| lethal disruption of 100 points, necrotic-class, directed | `100*0.20*0.5` | 10.0 |
| word-carrier, instant information | `1` | 1.0 |
| Pattern cost | `0.01 × Q9 × (1 + 0.25)` | 13,042 |

| Quantity | Value |
|---|---|
| Effect energy | 11.0 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **13,053 Pz** (19,579.0 kJ) |
| Slot quantum Q9 | 1.04 MPz Pz |
| Field gain (draw / quantum) | 0.0125 |
| Energy-equivalent tier T_E | 4.62 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** save or suck.

**Assumptions:** Threshold 100 points delivered as necrotic-class kappa 0.20 with directed F 0.5; real cost dominated by pattern complexity.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Power Word Kill (9-E-L-PWK) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 9 | 9 | `0000000010011` |
| k2 School | Enchantment | 3 | `0000000000111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Xyowyn** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 4→3 | 3 |
| k2 School | 0→11 1→12 2→0 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#6c8496`.

![[Power Word Kill (9-E-L-PWK) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 9 | 0.900 | 1.000 | `#b600ff` (430 nm eq.) | source grid |
| School | Enchantment | 0.375 | 0.871 | `#20ff00` (588 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.667 | `#ff0028` (700 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.953 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.21): swatch `#85a4b8`, measured lines at 0.004, 0.376, 0.589, 0.901. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.12. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `9·E·None`; the k4 to k6 lines (None, 60 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `9·E·None` |
| Standard spectrometer detection range | 11.42 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 52,167 Pz (0.05 × Q9) |
| Counter drawn cold (all six layers) | 104,334 Pz (0.10 × Q9) |
| Unravel after completion | 104,334 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Introspection, Flexibility, Hope. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1G 1h 1i 1J` (Within, Light, Life, Potential, Introspection, Flexibility, Hope, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 2,175 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 9th Tier quantum of 1.04 MPz Pz (1.3% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 9th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Enchantment school with aspect lean Within, Introspection, Flexibility, Hope. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 9 Workings]] |
| School | [[Enchantment]] |
| Affinity | [[Enchantment]] (E) |
| Function | [[Mind and Will]], [[Necromantic and Soul Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Antipathy-Sympathy (8-E-L-ASP)|Antipathy/Sympathy]] (8) · [[Dominate Monster (8-E-L-DMM)|Dominate Monster]] (8) · [[Feeblemind (8-E-L-FBL)|Feeblemind]] (8) · [[Power Word Stun (8-E-L-PWS)|Power Word Stun]] (8) · [[True Resurrection (9-N-L-TR)|True Resurrection]] (9) · [[Weird (9-I-L-WRD)|Weird]] (9) · [[Clone (8-N-L-CLN)|Clone]] (8) · [[Glibness (8-T-L-GLB)|Glibness]] (8).


---

## Tactical Assessment

A no-resistance assassination tool for officers and specialists of modest durability. Hardened or augmented targets above the threshold are immune.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 9 Workings]] · [[Enchantment]] · [[Spell Breakdown Procedure]] · [[Parzival]]
