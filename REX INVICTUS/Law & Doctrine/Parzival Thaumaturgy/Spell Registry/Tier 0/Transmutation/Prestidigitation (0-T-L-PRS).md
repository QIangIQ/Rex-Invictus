---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-0
  - spell/transmutation
  - source/srd
aliases:
  - "Cantrip Spell: Prestidigitation"
  - "Prestidigitation"
  - "0-T-L-PRS"
registry_id: 0-T-L-PRS
attribute_code: "0·Tra·None·None·10 feet·1 hour"
incantation: "Ciespula"
tier: 0
school: Transmutation
affinity: T
grade: L
pz_total: 29.4
pz_quantum: 128.8
t_e: -1.48
updated: 2026-11-16
---

**Prestidigitation** (`0-T-L-PRS`) is a Cantrip (Tier 0) working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **29.4 Pz** against a slot quantum of 129 Pz, which puts its energy-equivalent tier at T_E -1.48 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 0 Workings]]
      - [[Transmutation]]
        - **Prestidigitation** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `0-T-L-PRS` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `0·Tra·None·None·10 feet·1 hour` |
| Incantation | *Ciespula* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | Cantrip (Tier 0) |
| School | [[Transmutation]] |
| Casting time | 1 action |
| Range | 10 feet |
| Area | single point or target |
| Duration | 1 hour |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Bard, Sorcerer, Warlock, Wizard |

### Mechanism

A low-grade utility field that performs small thermal, optical, acoustic and cleaning tasks within arm's reach.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| warm or chill 1 cubic foot of water-density material by 10 K | `1 kg*4186*10 K/1500  [C7]` | 27.9 |
| minor sensory effect (sparks, puff, notes) | `0.1` | 0.1 |
| clean or soil 1 cubic foot object | `0.1` | 0.1 |
| Pattern cost | `0.01 × Q0 × (1 + 0.00)` | 1.3 |

| Quantity | Value |
|---|---|
| Effect energy | 28.1 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **29.4 Pz** (44.1 kJ) |
| Slot quantum Q0 | 129 Pz |
| Field gain (draw / quantum) | 0.228 |
| Energy-equivalent tier T_E | -1.48 |
| Handling points | 0.00 |
| Grade score | -0.74 → L |

Calibration applied: C7 (Domestic transmutation), see [[Parzival Energy Budget#Registry calibration rules]].

**Handling flags:** none.

**Assumptions:** Thermal option at full 1 cubic foot of water-density material and 10 K change dominates; one thermal effect counted; held temperature losses ignored.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Prestidigitation (0-T-L-PRS) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 0 | 0 | `0000000000001` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 10 feet | 1 | `0000000000011` |
| k6 Duration | 1 hour | 0 | `0000000000001` |

### Incantation

Spoken as **Ciespula** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T1: *Siciespula* · T2: *Hiciespula* · T3: *Liciespula* · T4: *Viciespula* · T5: *Ticiespula* · T6: *Riciespula* · T7: *Miciespula* · T8: *Niciespula* · T9: *Xyiciespula*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 | 1 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 | 2 |
| k6 Duration | 0→7 | 1 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#eb123a`.

![[Prestidigitation (0-T-L-PRS) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 0 | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.682 | `#9600ff` (438 nm eq.) | source grid |
| Duration | 1 hour | 0.053 | 0.999 | `#ff1c00` (684 nm eq.) | source grid |
| Range | 10 feet | 0.059 | 0.998 | `#ff2700` (682 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.21): swatch `#be345f`, measured lines at 0.006, 0.057, 0.876. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.47. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `0·T·None`; the k4 to k6 lines (None, 10 feet, 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `0·T·None` |
| Standard spectrometer detection range | 0.54 km (r = 1 km × √(E/100 Pz)) |
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
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 4.9 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the Cantrip (Tier 0) quantum of 129 Pz (22.8% of it). |
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
| Function | [[Terrain and Matter Shaping]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Druidcraft (0-T-L-DRD)|Druidcraft]] (0) · [[Mending (0-T-L-MND)|Mending]] (0) · [[Reflective Coating (0-T-L-RCF)|Reflective Coating]] (0) · [[Sharpen (0-T-L-SHR)|Sharpen]] (0) · [[Stress (Non-Battle) (0-T-L-SNBE)|Stress (Non-Battle)]] (0) · [[Thaumaturgy (0-T-L-THM)|Thaumaturgy]] (0) · [[Create or Destroy Water (1-T-L-CDW)|Create or Destroy Water]] (1) · [[Glue (1-T-L-GLU)|Glue]] (1).


---

## Tactical Assessment

A field-craft convenience for warming rations, marking surfaces and lighting fires without equipment.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 0 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
