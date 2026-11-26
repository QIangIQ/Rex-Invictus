---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/evocation
  - source/srd
aliases:
  - "5th Tier Spell: Wall of Force"
  - "Wall of Force"
  - "5-P-L-WFL"
registry_id: 5-P-L-WFL
attribute_code: "5·Evo·None·None·120 feet·Up to 10 minutes"
incantation: "Tumully"
tier: 5
school: Evocation
affinity: P
grade: L
pz_total: 1239.7
pz_quantum: 19109.4
t_e: 2.26
updated: 2026-11-16
---

**Wall of Force** (`5-P-L-WFL`) is a 5th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **1,240 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 2.26 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Evocation]]
        - **Wall of Force** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-P-L-WFL` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Evo·None·None·120 feet·Up to 10 minutes` |
| Incantation | *Tumully* |
| Affinity | P (Pure field construct) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 120 feet |
| Area | single point or target |
| Duration | Up to 10 minutes (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A pinch of powder made by crushing a clear gemstone |
| Ritual | no |
| Practitioner lineages | Wizard |

### Mechanism

An invisible plane or sphere of force, 6 mm thick, blocks all passage including ethereal travel and cannot be damaged.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Displacing 2 creatures aside | `2 * 0.5 * 80 kg * 9.81 * 1.5 m / 1500` | 0.785 |
| Upkeep: Barrier absorption | `0.20 * 50 HP/round * 100 rounds` | 1,000 |
| Pattern cost | `0.01 × Q5 × (1 + 0.25)` | 239 |

| Quantity | Value |
|---|---|
| Effect energy | 0.785 Pz |
| Upkeep energy | 1,000 Pz (1.7 Pz/s) |
| **Total draw** | **1,240 Pz** (1,859.5 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 0.0649 |
| Energy-equivalent tier T_E | 2.26 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** concentration.

**Assumptions:** Absorbs 50 HP per round of incoming fire for 100 rounds.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Wall of Force (5-P-L-WFL) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 120 feet | 3 | `0000000000111` |
| k6 Duration | Up to 10 minutes | 15 | `0000000011111` |

### Incantation

Spoken as **Tumully** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Ritumully* · T7: *Mitumully* · T8: *Nitumully* · T9: *Xyitumully*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 | 3 |
| k6 Duration | 0→7 1→8 2→9 3→10 4→11 | 5 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#45b385`.

![[Wall of Force (5-P-L-WFL) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| School | Evocation | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Up to 10 minutes | 0.789 | 0.959 | `#1e00ff` (463 nm eq.) | source grid |
| Range | 120 feet | 0.176 | 0.949 | `#ffc900` (647 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 3.09. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·V·None`; the k4 to k6 lines (None, 120 feet, Up to 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·V·None` |
| Standard spectrometer detection range | 3.52 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 2,111 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1b 1c 1d 1f` (Heat, Light, Life, Energy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 207 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 5th Tier quantum of 19,109 Pz (6.5% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 5th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 5 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Pure]] (P) |
| Function | [[Wards and Shields]], [[Walls and Barriers]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Forcecage (7-P-L-FRC)|Forcecage]] (7) · [[Hallow (5-V-L-HLL)|Hallow]] (5) · [[Wall of Stone (5-V-M-WS)|Wall of Stone]] (5) · [[Blade Barrier (6-V-L-BB)|Blade Barrier]] (6) · [[Fire Shield (4-V-L-FSR)|Fire Shield]] (4) · [[Resilient Sphere (4-P-L-RS)|Resilient Sphere]] (4) · [[Wall of Fire (4-V-M-WF)|Wall of Fire]] (4) · [[Wall of Ice (6-V-M-WI)|Wall of Ice]] (6).


---

## Tactical Assessment

Seals breaches, traps vehicles or creatures, and shields positions from all fire for ten minutes.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
