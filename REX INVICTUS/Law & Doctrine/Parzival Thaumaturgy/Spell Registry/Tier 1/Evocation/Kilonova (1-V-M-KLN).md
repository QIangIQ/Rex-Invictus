---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/evocation
  - source/science-spellbook
aliases:
  - "1st Tier Spell: Kilonova"
  - "1-V-M-KLN"
  - "Kilonova (Science)"
registry_id: 1-V-M-KLN
attribute_code: "1·Evo·Fire·sphere (10)·30 feet·Instantaneous"
incantation: "Suire-Seusin"
tier: 1
school: Evocation
affinity: V
grade: M
pz_total: 1054.2
pz_quantum: 350.0
t_e: 2.10
updated: 2026-11-16
---

**Kilonova** (`1-V-M-KLN`) is a 1st Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **1,054 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E 2.10 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Evocation]]
        - **Kilonova** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-V-M-KLN` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Evo·Fire·sphere (10)·30 feet·Instantaneous` |
| Incantation | *Suire-Seusin* |
| Affinity | V (Evocation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Evocation]] |
| Casting time | 1 Action |
| Range | 30 feet |
| Area | sphere (10) |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A small ball bearing |
| Ritual | no |
| Injury | 2d8 fire (mean 9) |
| Injury by tier | T1: 2d8, T2: 2d8, T3: 2d8, T4: 2d8, T5: 6d8, T6: 7d8, T7: 8d8, T8: 9d8, T9: 10d8 |
| Resistance check | agility; on success: no effect |
| Practitioner lineages | Wizard, Sorcerer |

### Mechanism

A bright, hot gas burst fills a 10 ft radius and blinds those caught in it.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Hot gas burst | `9 HP x 0.7 (fire) x S/A_c, S = sphere r=3.048 m = 116.7 m^2` | 1,051 |
| Pattern cost | `0.01 × Q1 × (1 + 0.00)` | 3.5 |

| Quantity | Value |
|---|---|
| Effect energy | 1,051 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **1,054 Pz** (1,581.3 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 3.01 |
| Energy-equivalent tier T_E | 2.10 |
| Handling points | 0.00 |
| Grade score | 0.55 → M |

**Handling flags:** none.

**Assumptions:** Fire 2d8 = 9 over a 10 ft sphere; the flash light is a few kJ and is ignored.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Kilonova (1-V-M-KLN) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Fire | 3 | `0000000000111` |
| k4 Area | sphere (10) | 27 | `0000000110111` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Suire-Seusin** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisuire-Seusin* · T3: *Lisuire-Seusin* · T4: *Visuire-Seusin* · T5: *Tisuire-Seusin* · T6: *Risuire-Seusin* · T7: *Misuire-Seusin* · T8: *Nisuire-Seusin* · T9: *Xyisuire-Seusin*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 | 3 |
| k4 Area | 0→9 1→10 2→11 4→0 5→1 | 5 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#8d9441`.

![[Kilonova (1-V-M-KLN) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| Damage | Fire | 0.286 | 0.983 | `#9cff00` (614 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.923 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.995 | `#ff0028` (700 nm eq.) | source grid |
| Area | sphere (10) | 0.750 | 0.810 | `#0017ff` (475 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.981 | `#91ff00` (612 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 3.02. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·V·Fire`; the k4 to k6 lines (sphere (10), 30 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·V·Fire` |
| Standard spectrometer detection range | 3.25 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.0 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Energy, Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `2b 1c 3f 2j` (2x Heat, Light, 3x Energy, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 176 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 3.01 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 1st Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Area Destruction]] |
| Element | [[Fire Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Burning Hands (1-V-L-BH)|Burning Hands]] (1) · [[Galaxy Whirl (2-V-L-GWL)|Galaxy Whirl]] (2) · [[Fireball (3-V-M-FRB)|Fireball]] (3) · [[Fire Shield (4-V-L-FSR)|Fire Shield]] (4) · [[Wall of Fire (4-V-M-WF)|Wall of Fire]] (4) · [[Blast (1-V-L-BLS)|Blast]] (1) · [[Faerie Fire (1-V-L-FF)|Faerie Fire]] (1) · [[Flame Strike (5-V-L-FSM)|Flame Strike]] (5).


---

## Tactical Assessment

Close assault flash and burn for clearing a room or a trench bay.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
