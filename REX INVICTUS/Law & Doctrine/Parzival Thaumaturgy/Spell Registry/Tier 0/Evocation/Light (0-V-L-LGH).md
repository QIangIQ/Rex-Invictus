---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-0
  - spell/evocation
  - source/srd
aliases:
  - "Cantrip Spell: Light"
  - "Light"
  - "0-V-L-LGH"
registry_id: 0-V-L-LGH
attribute_code: "0·Evo·None·None·Touch·1 hour"
incantation: "Culixa"
tier: 0
school: Evocation
affinity: V
grade: L
pz_total: 241.3
pz_quantum: 128.8
t_e: 0.63
updated: 2026-11-16
---

**Light** (`0-V-L-LGH`) is a Cantrip (Tier 0) working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **241 Pz** against a slot quantum of 129 Pz, which puts its energy-equivalent tier at T_E 0.63 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 0 Workings]]
      - [[Evocation]]
        - **Light** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `0-V-L-LGH` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `0·Evo·None·None·Touch·1 hour` |
| Incantation | *Culixa* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | Cantrip (Tier 0) |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | Touch |
| Area | single point or target |
| Duration | 1 hour |
| Components | spoken (incantation), material focus. Material: A firefly or phosphorescent moss |
| Ritual | no |
| Resistance check | agility; on success: no effect |
| Practitioner lineages | Bard, Cleric, Sorcerer, Wizard |

### Mechanism

The field makes one object emit visible light in a 20 ft bright radius with dimmer light beyond, in any chosen colour. Covering the object blocks it.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Light emission, 20 ft bright radius (upkeep) | `100 W / 1500 * 3600 s` | 240 |
| Pattern cost | `0.01 × Q0 × (1 + 0.00)` | 1.3 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 240 Pz (0.0667 Pz/s) |
| **Total draw** | **241 Pz** (361.9 kJ) |
| Slot quantum Q0 | 129 Pz |
| Field gain (draw / quantum) | 1.87 |
| Energy-equivalent tier T_E | 0.63 |
| Handling points | 0.00 |
| Grade score | 0.31 → L |

**Handling flags:** none.

**Assumptions:** Torch-equivalent 100 W for 1 hour.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Light (0-V-L-LGH) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 0 | 0 | `0000000000001` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | 1 hour | 0 | `0000000000001` |

### Incantation

Spoken as **Culixa** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T1: *Siculixa* · T2: *Hiculixa* · T3: *Liculixa* · T4: *Viculixa* · T5: *Ticulixa* · T6: *Riculixa* · T7: *Miculixa* · T8: *Niculixa* · T9: *Xyiculixa*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 | 1 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 | 1 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#ac475e`.

![[Light (0-V-L-LGH) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 0 | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.882 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | 1 hour | 0.053 | 0.999 | `#ff1c00` (684 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.678 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.19): swatch `#ac8478`, measured lines at 0.006, 0.053, 0.501, 0.883. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.38. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `0·V·None`; the k4 to k6 lines (None, Touch, 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `0·V·None` |
| Standard spectrometer detection range | 1.55 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 6.4 Pz (0.05 × Q0) |
| Counter drawn cold (all six layers) | 12.9 Pz (0.10 × Q0) |
| Unravel after completion | 60.9 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1b 1c 1d 1f` (Heat, Light, Life, Energy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 40.2 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 1.87 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full Cantrip (Tier 0) pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at Cantrip (Tier 0) up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 0 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Light and Radiance]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Dancing Lights (0-V-L-DL)|Dancing Lights]] (0) · [[Magelight (0-V-L-MGL)|Magelight]] (0) · [[Sacred Flame (0-V-L-SF)|Sacred Flame]] (0) · [[Faerie Fire (1-V-L-FF)|Faerie Fire]] (1) · [[Guiding Bolt (1-V-L-GB)|Guiding Bolt]] (1) · [[Continual Flame (2-V-M-CF)|Continual Flame]] (2) · [[Moonbeam (2-V-M-MNB)|Moonbeam]] (2) · [[Color Spray (1-I-L-CS)|Color Spray]] (1).


---

## Tactical Assessment

A cheap illumination source that cannot be shot out like a lamp, useful for marking points and lighting work areas. It reveals the holder's position.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 0 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
