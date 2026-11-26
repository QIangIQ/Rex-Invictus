---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-6
  - spell/divination
  - source/srd
aliases:
  - "6th Tier Spell: True Seeing"
  - "True Seeing"
  - "6-D-L-TSU"
registry_id: 6-D-L-TSU
attribute_code: "6·Div·None·None·Touch·1 hour"
incantation: "Rilixa"
tier: 6
school: Divination
affinity: D
grade: L
pz_total: 805.5
pz_quantum: 51944.6
t_e: 1.83
updated: 2026-11-16
---

**True Seeing** (`6-D-L-TSU`) is a 6th Tier working of the [[Divination]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **805 Pz** against a slot quantum of 51,945 Pz, which puts its energy-equivalent tier at T_E 1.83 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 6 Workings]]
      - [[Divination]]
        - **True Seeing** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `6-D-L-TSU` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `6·Div·None·None·Touch·1 hour` |
| Incantation | *Rilixa* |
| Affinity | D (Divination) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 6th Tier |
| School | [[Divination]] |
| Casting time | 1 action |
| Range | Touch |
| Area | single point or target |
| Duration | 1 hour |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: An ointment for the eyes that costs 25gp; is made from mushroom powder, saffron, and fat; and is consumed by the spell |
| Ritual | no |
| Practitioner lineages | Bard, Cleric, Sorcerer, Warlock, Wizard |

### Mechanism

The subject perceives objects as they actually are to 36 m, penetrating disguise, invisibility and concealment, and sees into the adjacent ethereal layer.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Upkeep: Truesight to 120 ft, material and ethereal layers | `2 * 0.001 Pz/s * (36.58/10) * 3600 s` | 26.3 |
| Pattern cost | `0.01 × Q6 × (1 + 0.50)` | 779 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 26.3 Pz (0.00732 Pz/s) |
| **Total draw** | **805 Pz** (1,208.2 kJ) |
| Slot quantum Q6 | 51,945 Pz |
| Field gain (draw / quantum) | 0.0155 |
| Energy-equivalent tier T_E | 1.83 |
| Handling points | 0.50 |
| Grade score | -0.50 → L |

**Handling flags:** costly material, consumed material.

**Assumptions:** 1 h; ethereal view counted as a second layer at the same rate.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[True Seeing (6-D-L-TSU) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 6 | 6 | `0000000001101` |
| k2 School | Divination | 2 | `0000000000101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | 1 hour | 0 | `0000000000001` |

### Incantation

Spoken as **Rilixa** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T7: *Mirilixa* · T8: *Nirilixa* · T9: *Xyirilixa*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 3→2 | 3 |
| k2 School | 0→11 2→0 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 | 1 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#958484`.

![[True Seeing (6-D-L-TSU) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 6 | 0.600 | 1.000 | `#00ebff` (520 nm eq.) | source grid |
| School | Divination | 0.250 | 0.941 | `#cdff00` (625 nm eq.) | source grid |
| Duration | 1 hour | 0.053 | 0.861 | `#ff1c00` (684 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.961 | `#9b00ff` (435 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 2.91. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `6·D·None`; the k4 to k6 lines (None, Touch, 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `6·D·None` |
| Standard spectrometer detection range | 2.84 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 2,597 Pz (0.05 × Q6) |
| Counter drawn cold (all six layers) | 5,194 Pz (0.10 × Q6) |
| Unravel after completion | 5,200 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Light, 2x Extraspection. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 2c 1d 1F 2g 1J` (Beyond, 2x Light, Life, Potential, 2x Extraspection, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 134 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 6th Tier quantum of 51,945 Pz (1.6% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 6th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Divination school with aspect lean Beyond, Light, 2x Extraspection. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 6 Workings]] |
| School | [[Divination]] |
| Affinity | [[Divination]] (D) |
| Function | [[Divination and Sensing]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Find the Path (6-D-L-FP)|Find the Path]] (6) · [[Commune (5-D-L-CMMM)|Commune]] (5) · [[Commune With Nature (5-D-L-CN)|Commune With Nature]] (5) · [[Contact Other Plane (5-D-L-COP)|Contact Other Plane]] (5) · [[Legend Lore (5-D-L-LLG)|Legend Lore]] (5) · [[Scrying (5-D-L-SCR)|Scrying]] (5) · [[Telepathic Bond (5-D-L-TB)|Telepathic Bond]] (5) · [[Arcane Eye (4-D-L-AE)|Arcane Eye]] (4).


---

## Tactical Assessment

Counter-deception for assault leaders and inspectors facing illusions, shapeshifters or cloaked threats.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 6 Workings]] · [[Divination]] · [[Spell Breakdown Procedure]] · [[Parzival]]
