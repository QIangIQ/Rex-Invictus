---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-0
  - spell/transmutation
  - source/science-spellbook
aliases:
  - "Cantrip Spell: Stress (Battle)"
  - "0-P-L-SB"
  - "Stress (Battle) (Science)"
registry_id: 0-P-L-SB
attribute_code: "0·Tra·Force·None·15 feet·Instantaneous"
incantation: "Cieton-’bal"
tier: 0
school: Transmutation
affinity: P
grade: L
pz_total: 2.0
pz_quantum: 128.8
t_e: -4.17
updated: 2026-11-16
---

**Stress (Battle)** (`0-P-L-SB`) is a Cantrip (Tier 0) working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **2.0 Pz** against a slot quantum of 129 Pz, which puts its energy-equivalent tier at T_E -4.17 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 0 Workings]]
      - [[Transmutation]]
        - **Stress (Battle)** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `0-P-L-SB` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `0·Tra·Force·None·15 feet·Instantaneous` |
| Incantation | *Cieton-’bal* |
| Affinity | P (Pure field construct) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | Cantrip (Tier 0) |
| School | [[Transmutation]] |
| Casting time | 1 Action |
| Range | 15 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A copy of "Theory of Magic" |
| Ritual | no |
| Injury | 1d6 force (mean 3.5) |
| Injury by caster maturity bands | T1: 1d6, T5: 2d6, T11: 3d6, T17: 4d6 |
| Resistance check | strength; on success: no effect |
| Practitioner lineages | Druid, Sorcerer, Warlock, Wizard |

### Mechanism

Applies directed bending, shear or twisting stress to a target body, wrenching joints and impairing it.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Mechanical stress | `3.5 HP x 0.4 (force) x F 0.5` | 0.7 |
| Pattern cost | `0.01 × Q0 × (1 + 0.00)` | 1.3 |

| Quantity | Value |
|---|---|
| Effect energy | 0.7 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **2.0 Pz** (3.0 kJ) |
| Slot quantum Q0 | 129 Pz |
| Field gain (draw / quantum) | 0.0154 |
| Energy-equivalent tier T_E | -4.17 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Force 1d6 = 3.5 on one target, directed F 0.5.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Stress (Battle) (0-P-L-SB) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 0 | 0 | `0000000000001` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | Force | 4 | `0000000001001` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 15 feet | 18 | `0000000100101` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Cieton-’bal** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T1: *Sicieton-’bal* · T2: *Hicieton-’bal* · T3: *Licieton-’bal* · T4: *Vicieton-’bal* · T5: *Ticieton-’bal* · T6: *Ricieton-’bal* · T7: *Micieton-’bal* · T8: *Nicieton-’bal* · T9: *Xyicieton-’bal*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 | 1 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 3→0 | 2 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 5→0 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#c76637`.

![[Stress (Battle) (0-P-L-SB) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 0 | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| Damage | Force | 0.357 | 0.938 | `#3bff00` (593 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.682 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| Range | 15 feet | 0.206 | 0.979 | `#ffef00` (638 nm eq.) | RI half-step |

Relative luminosity scales with initial energy: log10(E) = 0.30. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `0·T·Force`; the k4 to k6 lines (None, 15 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `0·T·Force` |
| Standard spectrometer detection range | 0.14 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 6.4 Pz (0.05 × Q0) |
| Counter drawn cold (all six layers) | 12.9 Pz (0.10 × Q0) |
| Unravel after completion | 12.9 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Beyond, Introspection, 2x Movement and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1d 1G 2h 3j` (Beyond, Life, Introspection, 2x Flexibility, 3x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 0.331 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the Cantrip (Tier 0) quantum of 129 Pz (1.5% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at Cantrip (Tier 0) up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 0 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Pure]] (P) |
| Function | [[Precision Strikes]] |
| Element | [[Force Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Eldritch Blast (0-P-L-EB)|Eldritch Blast]] (0) · [[Magic Missile (1-P-L-MM)|Magic Missile]] (1) · [[Spiritual Weapon (2-P-L-SW)|Spiritual Weapon]] (2) · [[Tidal Force (4-P-L-TF)|Tidal Force]] (4) · [[Acid Splash (0-C-L-AS)|Acid Splash]] (0) · [[Chill Touch (0-N-L-CT)|Chill Touch]] (0) · [[Cool Metal (2-T-L-CM)|Cool Metal]] (2) · [[Dimension Door (4-P-L-DD)|Dimension Door]] (4).


---

## Tactical Assessment

Close harassment that spoils aim or grip.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 0 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
