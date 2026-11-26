---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/evocation
  - source/science-spellbook
aliases:
  - "2nd Tier Spell: Galaxy Whirl"
  - "2-V-L-GWL"
  - "Galaxy Whirl (Science)"
registry_id: 2-V-L-GWL
attribute_code: "2·Evo·Fire·sphere (5)·60 feet·Up to 1 minute"
incantation: "Huire-Suwynse"
tier: 2
school: Evocation
affinity: V
grade: L
pz_total: 1186.2
pz_quantum: 951.4
t_e: 2.22
updated: 2026-11-16
---

**Galaxy Whirl** (`2-V-L-GWL`) is a 2nd Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **1,186 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E 2.22 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Evocation]]
        - **Galaxy Whirl** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-V-L-GWL` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Evo·Fire·sphere (5)·60 feet·Up to 1 minute` |
| Incantation | *Huire-Suwynse* |
| Affinity | V (Evocation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Evocation]] |
| Casting time | 1 Action |
| Range | 60 feet |
| Area | sphere (5) |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: An object with a spiral carved into it |
| Ritual | no |
| Injury | 2d12 fire (mean 13) |
| Injury by tier | T2: 2d12, T3: 2d12, T4: 2d12, T5: 2d12, T6: 2d12, T7: 2d12, T8: 2d12, T9: 2d12 |
| Resistance check | agility; on success: half injury |
| Practitioner lineages | Wizard, Sorcerer, Warlock |

### Mechanism

Spins a ring of burning gas around a target creature that burns anyone entering it while the center stays unharmed.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Whirl burns | `13 HP x 0.7 (fire) x S/A_c, S = sphere r=1.524 m = 29.2 m^2 x 3` | 1,138 |
| Illumination (upkeep) | `900 W x 60 s = 5.4e+04 J / 1500` | 36.0 |
| Pattern cost | `0.01 × Q2 × (1 + 0.25)` | 11.9 |

| Quantity | Value |
|---|---|
| Effect energy | 1,138 Pz |
| Upkeep energy | 36.0 Pz (0.6 Pz/s) |
| **Total draw** | **1,186 Pz** (1,779.2 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 1.25 |
| Energy-equivalent tier T_E | 2.22 |
| Handling points | 0.25 |
| Grade score | 0.36 → L |

**Handling flags:** concentration.

**Assumptions:** Fire 2d12 = 13 over a 5 ft sphere around the target, 3 triggers; light 900 W (60 ft radius) for 1 minute.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Galaxy Whirl (2-V-L-GWL) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Fire | 3 | `0000000000111` |
| k4 Area | sphere (5) | 34 | `0000001000101` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Huire-Suwynse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihuire-Suwynse* · T4: *Vihuire-Suwynse* · T5: *Tihuire-Suwynse* · T6: *Rihuire-Suwynse* · T7: *Mihuire-Suwynse* · T8: *Nihuire-Suwynse* · T9: *Xyihuire-Suwynse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 | 3 |
| k4 Area | 0→9 2→11 6→2 | 3 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#6bc18e`.

![[Galaxy Whirl (2-V-L-GWL) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| Damage | Fire | 0.286 | 0.996 | `#9cff00` (614 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.956 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.889 | `#0074ff` (495 nm eq.) | source grid |
| Area | sphere (5) | 0.944 | 0.758 | `#f200ff` (417 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.927 | `#00fbff` (524 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 3.07. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·V·Fire`; the k4 to k6 lines (sphere (5), 60 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·V·Fire` |
| Standard spectrometer detection range | 3.44 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 102 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Energy, Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `2b 1c 3f 2j` (2x Heat, Light, 3x Energy, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 198 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 1.25 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 2nd Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
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
| Function | [[Area Destruction]] |
| Element | [[Fire Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Burning Hands (1-V-L-BH)|Burning Hands]] (1) · [[Fireball (3-V-M-FRB)|Fireball]] (3) · [[Kilonova (1-V-M-KLN)|Kilonova]] (1) · [[Fire Shield (4-V-L-FSR)|Fire Shield]] (4) · [[Wall of Fire (4-V-M-WF)|Wall of Fire]] (4) · [[Flame Strike (5-V-L-FSM)|Flame Strike]] (5) · [[Bohr's Model (2-P-L-BSM)|Bohr's Model]] (2) · [[Continual Flame (2-V-M-CF)|Continual Flame]] (2).


---

## Tactical Assessment

Escort fire ring for a VIP or a way to trap an enemy's guards.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
