---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/illusion
  - source/science-spellbook
aliases:
  - "5th Tier Spell: Time Dilation"
  - "5-I-L-TD"
  - "Time Dilation (Science)"
registry_id: 5-I-L-TD
attribute_code: "5·Ill·None·None·30 feet·Up to 1 hour"
incantation: "Taiusinsi"
tier: 5
school: Illusion
affinity: I
grade: L
pz_total: 601.4
pz_quantum: 19109.4
t_e: 1.54
updated: 2026-11-16
---

**Time Dilation** (`5-I-L-TD`) is a 5th Tier working of the [[Illusion]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **601 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 1.54 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Illusion]]
        - **Time Dilation** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-I-L-TD` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Ill·None·None·30 feet·Up to 1 hour` |
| Incantation | *Taiusinsi* |
| Affinity | I (Illusion) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Illusion]] |
| Casting time | 1 Action |
| Range | 30 feet |
| Area | single point or target |
| Duration | Up to 1 hour (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A sandtimer or timepiece |
| Ritual | no |
| Resistance check | intellect; on success: no effect |
| Practitioner lineages | Wizard |

### Mechanism

Slows one creature's experienced time so it lives several hours as one, dulling its senses and reactions.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Proper-time suppression (upkeep) | `100 W x (1 - 1/3.5) x 3600 s = 2.571e+05 J / 1500` | 171 |
| Pattern cost | `0.01 × Q5 × (1 + 1.25)` | 430 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 171 Pz (0.0476 Pz/s) |
| **Total draw** | **601 Pz** (902.1 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 0.0315 |
| Energy-equivalent tier T_E | 1.54 |
| Handling points | 1.25 |
| Grade score | 0.25 → L |

**Handling flags:** concentration, fragile.

**Assumptions:** Reasoned order of magnitude: suppressing 100 W of metabolism by a factor 3.5 for an hour; true relativistic dilation of 3.5 for an 80 kg body needs about 1.2e16 Pz.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Time Dilation (5-I-L-TD) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Illusion | 5 | `0000000001011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Up to 1 hour | 12 | `0000000011001` |

### Incantation

Spoken as **Taiusinsi** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Ritaiusinsi* · T7: *Mitaiusinsi* · T8: *Nitaiusinsi* · T9: *Xyitaiusinsi*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 1→12 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 3→10 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#23e0a2`.

![[Time Dilation (5-I-L-TD) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| School | Illusion | 0.625 | 0.992 | `#00c5ff` (512 nm eq.) | source grid |
| Duration | Up to 1 hour | 0.632 | 0.991 | `#00c0ff` (511 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.979 | `#91ff00` (612 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 2.78. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·I·None`; the k4 to k6 lines (None, 30 feet, Up to 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·I·None` |
| Standard spectrometer detection range | 2.45 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 1,945 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Light, Introspection, 2x Flexibility. The working vector used by [[Recast Tension and Combination Affinity]] is `2c 1d 1F 1G 2h 1J` (2x Light, Life, Potential, Introspection, 2x Flexibility, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 100 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 5th Tier quantum of 19,109 Pz (3.1% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 5th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Illusion school with aspect lean Light, Introspection, 2x Flexibility. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 5 Workings]] |
| School | [[Illusion]] |
| Affinity | [[Illusion]] (I) |
| Function | [[Divination and Sensing]], [[Negation and Counterspell]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Nondetection (3-A-L-NND)|Nondetection]] (3) · [[Animal Messenger (2-E-L-AM)|Animal Messenger]] (2) · [[Blindness-Deafness (2-N-L-BD)|Blindness/Deafness]] (2) · [[Knock (2-T-L-KNC)|Knock]] (2) · [[Antilife Shell (5-A-L-ASI)|Antilife Shell]] (5) · [[Arcane Hand (5-P-L-AH)|Arcane Hand]] (5) · [[Awaken (5-T-H-AWK)|Awaken]] (5) · [[Commune (5-D-L-CMMM)|Commune]] (5).


---

## Tactical Assessment

Removes a target from effective action for hours and spoils its rest.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Illusion]] · [[Spell Breakdown Procedure]] · [[Parzival]]
