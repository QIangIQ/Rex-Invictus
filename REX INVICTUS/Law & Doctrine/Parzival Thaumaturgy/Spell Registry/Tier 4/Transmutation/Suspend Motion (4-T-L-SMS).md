---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/transmutation
  - source/science-spellbook
aliases:
  - "4th Tier Spell: Suspend Motion"
  - "4-T-L-SMS"
  - "Suspend Motion (Science)"
registry_id: 4-T-L-SMS
attribute_code: "4·Tra·None·None·30 feet·Instantaneous"
incantation: "Vieusin"
tier: 4
school: Transmutation
affinity: T
grade: L
pz_total: 105.5
pz_quantum: 7029.9
t_e: -0.20
updated: 2026-11-16
---

**Suspend Motion** (`4-T-L-SMS`) is a 4th Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **106 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E -0.20 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Transmutation]]
        - **Suspend Motion** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-T-L-SMS` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Tra·None·None·30 feet·Instantaneous` |
| Incantation | *Vieusin* |
| Affinity | T (Transmutation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Transmutation]] |
| Casting time | 1 Action |
| Range | 30 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Resistance check | constitution; on success: no effect |
| Practitioner lineages | Wizard, Sorcerer |

### Mechanism

Strips the motion from one creature, holding it nearly still and blunting its strikes.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Motion arrested | `0.5 x 80 kg x (5 m/s)^2 = 1000 J / 1500` | 0.667 |
| Effort resisted (upkeep) | `300 W x 60 s = 1.8e+04 J / 1500` | 12.0 |
| Outgoing injury blunted | `0.20 x 25` | 5.0 |
| Pattern cost | `0.01 × Q4 × (1 + 0.25)` | 87.9 |

| Quantity | Value |
|---|---|
| Effect energy | 5.7 Pz |
| Upkeep energy | 12.0 Pz (0.2 Pz/s) |
| **Total draw** | **106 Pz** (158.3 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 0.015 |
| Energy-equivalent tier T_E | -0.20 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** save or suck.

**Assumptions:** Duration taken as 1 minute; stopping an 80 kg body at 5 m/s, resisting 300 W of muscular effort, and halving 50 of its outgoing injury (25 absorbed at 0.20 Pz).

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Suspend Motion (4-T-L-SMS) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 4 | 4 | `0000000001001` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Vieusin** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T5: *Tivieusin* · T6: *Rivieusin* · T7: *Mivieusin* · T8: *Nivieusin* · T9: *Xyivieusin*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 3→2 | 2 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#868545`.

![[Suspend Motion (4-T-L-SMS) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.893 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.923 | `#ff0028` (700 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.994 | `#91ff00` (612 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 2.02. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·T·None`; the k4 to k6 lines (None, 30 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·T·None` |
| Standard spectrometer detection range | 1.03 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 705 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 17.6 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 4th Tier quantum of 7,030 Pz (1.5% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 4th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 4 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Mind and Will]], [[Divination and Sensing]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Awaken (5-T-H-AWK)|Awaken]] (5) · [[Plagarise (4-E-L-PLG)|Plagarise]] (4) · [[Spirit Guardians (3-C-M-SGR)|Spirit Guardians]] (3) · [[Divine Word (7-V-L-DWV)|Divine Word]] (7) · [[Speak with Plants (3-T-L-SP)|Speak with Plants]] (3) · [[Alter Projectile Velocity (2-T-L-APV)|Alter Projectile Velocity]] (2) · [[Arcane Eye (4-D-L-AE)|Arcane Eye]] (4) · [[Compulsion (4-E-L-CMP)|Compulsion]] (4).


---

## Tactical Assessment

Takes a single enemy leader or heavy out of action.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
