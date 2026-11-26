---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/evocation
  - source/science-spellbook
aliases:
  - "5th Tier Spell: Voltaic Arc"
  - "5-V-L-VA"
  - "Voltaic Arc (Science)"
registry_id: 5-V-L-VA
attribute_code: "5·Evo·Lightning·line (60)·60 feet·Up to 1 minute"
incantation: "Tunin-Lewynse"
tier: 5
school: Evocation
affinity: V
grade: L
pz_total: 12070.0
pz_quantum: 19109.4
t_e: 4.54
updated: 2026-11-16
---

**Voltaic Arc** (`5-V-L-VA`) is a 5th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **12,070 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 4.54 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Evocation]]
        - **Voltaic Arc** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-V-L-VA` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Evo·Lightning·line (60)·60 feet·Up to 1 minute` |
| Incantation | *Tunin-Lewynse* |
| Affinity | V (Evocation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Evocation]] |
| Casting time | 1 Action |
| Range | 60 feet |
| Area | line (60) |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Two materials capable of creating static electricity when rubbed together |
| Ritual | no |
| Injury | 6d6 lightning (mean 21) |
| Injury by tier | T5: 6d6, T6: 7d6, T7: 8d6, T8: 9d6, T9: 10d6 |
| Resistance check | agility; on success: half injury |
| Practitioner lineages | Wizard, Sorcerer |

### Mechanism

Drives a large potential difference between two metal objects so a 5 ft wide arc bridges them for a minute.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Arc strikes | `21 HP x 0.3 (lightning) x S/A_c, S = line 18.29 m x 4.572 m = 167.2 m^2 x 3` | 4,515 |
| Arc sustained (upkeep) | `10 kW/m x 18.29 m x 60 s = 1.097e+07 J / 1500` | 7,316 |
| Pattern cost | `0.01 × Q5 × (1 + 0.25)` | 239 |

| Quantity | Value |
|---|---|
| Effect energy | 4,515 Pz |
| Upkeep energy | 7,316 Pz (122 Pz/s) |
| **Total draw** | **12,070 Pz** (18,104.9 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 0.632 |
| Energy-equivalent tier T_E | 4.54 |
| Handling points | 0.25 |
| Grade score | 0.02 → L |

**Handling flags:** concentration.

**Assumptions:** Lightning 6d6 = 21 over a 60 ft by 15 ft line band, 3 triggers; sustaining the arc at 10 kW per metre over 18.3 m for 1 minute (real arc physics).

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Voltaic Arc (5-V-L-VA) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Lightning | 5 | `0000000001011` |
| k4 Area | line (60) | 25 | `0000000110011` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Tunin-Lewynse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Ritunin-Lewynse* · T7: *Mitunin-Lewynse* · T8: *Nitunin-Lewynse* · T9: *Xyitunin-Lewynse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 3→0 | 3 |
| k4 Area | 0→9 1→10 4→0 5→1 | 4 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#00ceb3`.

![[Voltaic Arc (5-V-L-VA) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| Damage | Lightning | 0.429 | 0.997 | `#00ff25` (571 nm eq.) | source grid |
| School | Evocation | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.983 | `#0074ff` (495 nm eq.) | source grid |
| Area | line (60) | 0.694 | 0.981 | `#0069ff` (492 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.996 | `#00fbff` (524 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 4.08. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·V·Lightning`; the k4 to k6 lines (line (60), 60 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·V·Lightning` |
| Standard spectrometer detection range | 10.99 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 3,374 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is 2x Heat, Light, Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `3b 1c 2f 2j` (3x Heat, Light, 2x Energy, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 2,012 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 5th Tier quantum of 19,109 Pz (63.2% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 5th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 5 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Area Destruction]] |
| Element | [[Lightning Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Lightning Bolt (3-V-L-LB)|Lightning Bolt]] (3) · [[Call Lightning (3-C-L-CLL)|Call Lightning]] (3) · [[Cone of Cold (5-V-L-CC)|Cone of Cold]] (5) · [[Flame Strike (5-V-L-FSM)|Flame Strike]] (5) · [[Absolute Zero (6-V-L-AZ)|Absolute Zero]] (6) · [[Blade Barrier (6-V-L-BB)|Blade Barrier]] (6) · [[Burst Radiation (6-V-L-BR)|Burst Radiation]] (6) · [[Chain Lightning (6-V-L-CLA)|Chain Lightning]] (6).


---

## Tactical Assessment

Electrified barrier across a corridor or gap; armoured troops are hit hardest.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
