---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/evocation
  - source/science-spellbook
aliases:
  - "2nd Tier Spell: Universal Expansion"
  - "2-V-L-UE"
  - "Universal Expansion (Science)"
registry_id: 2-V-L-UE
attribute_code: "2·Evo·None·sphere (30)·150 feet·Instantaneous"
incantation: "Hu’-Sornosin"
tier: 2
school: Evocation
affinity: V
grade: L
pz_total: 23.7
pz_quantum: 951.4
t_e: -1.69
updated: 2026-11-16
---

**Universal Expansion** (`2-V-L-UE`) is a 2nd Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **23.7 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E -1.69 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Evocation]]
        - **Universal Expansion** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-V-L-UE` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Evo·None·sphere (30)·150 feet·Instantaneous` |
| Incantation | *Hu’-Sornosin* |
| Affinity | V (Evocation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Evocation]] |
| Casting time | 1 Bonus Action |
| Range | 150 feet |
| Area | sphere (30) |
| Duration | Instantaneous |
| Components | spoken (incantation), material focus. Material: A star-speckled marble |
| Ritual | no |
| Resistance check | strength; on success: half injury |
| Practitioner lineages | Wizard |

### Mechanism

Expands the space around a point so every creature and object within 30 ft is pushed outward without harm.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Outward displacement | `0.5 x 1140 kg x 9.81 x 3.81 m = 2.13e+04 J / 1500` | 14.2 |
| Pattern cost | `0.01 × Q2 × (1 + 0.00)` | 9.5 |

| Quantity | Value |
|---|---|
| Effect energy | 14.2 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **23.7 Pz** (35.6 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.0249 |
| Energy-equivalent tier T_E | -1.69 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** 8 creatures and 500 kg of objects (1140 kg) moved 3.81 m against friction mu 0.5.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Universal Expansion (2-V-L-UE) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (30) | 31 | `0000000111111` |
| k5 Range | 150 feet | 4 | `0000000001001` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Hu’-Sornosin** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihu’-Sornosin* · T4: *Vihu’-Sornosin* · T5: *Tihu’-Sornosin* · T6: *Rihu’-Sornosin* · T7: *Mihu’-Sornosin* · T8: *Nihu’-Sornosin* · T9: *Xyihu’-Sornosin*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 2→11 3→12 4→0 5→1 | 6 |
| k5 Range | 0→8 3→11 | 2 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#b09a4f`.

![[Universal Expansion (2-V-L-UE) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.956 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.980 | `#ff0028` (700 nm eq.) | source grid |
| Area | sphere (30) | 0.861 | 0.804 | `#8000ff` (442 nm eq.) | source grid |
| Range | 150 feet | 0.235 | 0.999 | `#e3ff00` (629 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 1.38. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·V·None`; the k4 to k6 lines (sphere (30), 150 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·V·None` |
| Standard spectrometer detection range | 0.49 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 95.1 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1b 1c 1d 1f` (Heat, Light, Life, Energy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 4.0 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (2.5% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Utility Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Synchrotron Spell (3-V-M-SSN)|Synchrotron Spell]] (3) · [[Carbon Dating (2-D-L-CDR)|Carbon Dating]] (2) · [[Magnetise (2-T-L-MGN)|Magnetise]] (2) · [[Moderator (2-A-L-MDR)|Moderator]] (2) · [[Momentum Transfer (2-T-L-MT)|Momentum Transfer]] (2) · [[Predict Projectiles (2-D-L-PPE)|Predict Projectiles]] (2) · [[Quantum Tunnelling (2-C-L-QT)|Quantum Tunnelling]] (2) · [[Alter Weight (1-T-L-AWT)|Alter Weight]] (1).


---

## Tactical Assessment

Breaks up a formation or clears a landing zone.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
