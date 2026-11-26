---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/transmutation
  - source/srd
aliases:
  - "2nd Tier Spell: Enlarge/Reduce"
  - "Enlarge/Reduce"
  - "2-T-M-ERL"
registry_id: 2-T-M-ERL
attribute_code: "2·Tra·None·None·30 feet·Up to 1 minute"
incantation: "Hieusinse"
tier: 2
school: Transmutation
affinity: T
grade: M
pz_total: 5616.2
pz_quantum: 951.4
t_e: 3.78
updated: 2026-11-16
---

**Enlarge/Reduce** (`2-T-M-ERL`) is a 2nd Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **5,616 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E 3.78 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Transmutation]]
        - **Enlarge/Reduce** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-T-M-ERL` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Tra·None·None·30 feet·Up to 1 minute` |
| Incantation | *Hieusinse* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Transmutation]] |
| Casting time | 1 action |
| Range | 30 feet |
| Area | single point or target |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A pinch iron powder |
| Ritual | no |
| Resistance check | constitution; on success: no effect |
| Practitioner lineages | Sorcerer, Wizard |

### Mechanism

The field doubles or halves a creature or object in each dimension, multiplying its mass by eight or one eighth, with matching changes in strength and weapon impact.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| add 560 kg of body mass (80 kg x8) | `10*(8-1)*80` | 5,600 |
| raise centre of mass about 0.9 m | `640*g*0.9/J` | 3.8 |
| weapon damage +1d4 slashing on 6.5 strikes | `2.5*0.40*0.08*6.5` | 0.52 |
| Pattern cost | `0.01 × Q2 × (1 + 0.25)` | 11.9 |

| Quantity | Value |
|---|---|
| Effect energy | 5,604 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **5,616 Pz** (8,424.3 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 5.9 |
| Energy-equivalent tier T_E | 3.78 |
| Handling points | 0.25 |
| Grade score | 1.14 → M |

**Handling flags:** concentration.

**Assumptions:** Enlarge case on an 80 kg target; added tissue billed at 10 Pz/kg as conjured living matter.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Enlarge-Reduce (2-T-M-ERL) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Hieusinse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihieusinse* · T4: *Vihieusinse* · T5: *Tihieusinse* · T6: *Rihieusinse* · T7: *Mihieusinse* · T8: *Nihieusinse* · T9: *Xyihieusinse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#8ca074`.

![[Enlarge-Reduce (2-T-M-ERL) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.796 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.889 | `#0074ff` (495 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.996 | `#91ff00` (612 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.16): swatch `#9a98a4`, measured lines at 0.201, 0.295, 0.685, 0.876. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.75. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·T·None`; the k4 to k6 lines (None, 30 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·T·None` |
| Standard spectrometer detection range | 7.49 km (r = 1 km × √(E/100 Pz)) |
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
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 936 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 5.90 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 2nd Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
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
| Function | [[Transformation]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Alter Self (2-T-L-AST)|Alter Self]] (2) · [[Chemical Transition (3-T-L-CTE)|Chemical Transition]] (3) · [[Crystalise (1-T-L-CRY)|Crystalise]] (1) · [[Gaseous Form (3-T-M-GF)|Gaseous Form]] (3) · [[Reduce Relative Velocity (1-T-L-RRV)|Reduce Relative Velocity]] (1) · [[Polymorph (4-T-L-PLY)|Polymorph]] (4) · [[Temporary Magic Prism (2-C-L-TMP)|Temporary Magic Prism]] (2) · [[Arcane Redirection (3-A-L-AR)|Arcane Redirection]] (3).


---

## Tactical Assessment

Enlarging heavy weapons, vehicles or fighters for a breach, or shrinking a target to make it carryable.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
