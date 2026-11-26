---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/necromancy
  - source/srd
aliases:
  - "5th Tier Spell: Raise Dead"
  - "Raise Dead"
  - "5-N-M-RD"
registry_id: 5-N-M-RD
attribute_code: "5·Nec·None·None·Touch·Instantaneous"
incantation: "Toulix"
tier: 5
school: Necromancy
affinity: N
grade: M
pz_total: 20341.7
pz_quantum: 19109.4
t_e: 5.06
updated: 2026-11-16
---

**Raise Dead** (`5-N-M-RD`) is a 5th Tier working of the [[Necromancy (School)|Necromancy]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **20,342 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 5.06 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Necromancy (School)|Necromancy]]
        - **Raise Dead** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-N-M-RD` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Nec·None·None·Touch·Instantaneous` |
| Incantation | *Toulix* |
| Affinity | N (Necromancy) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Necromancy (School)\|Necromancy]] |
| Casting time | 1 hour |
| Range | Touch |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A diamond worth at least 500gp, which the spell consumes |
| Ritual | no |
| Practitioner lineages | Bard, Cleric, Paladin |

### Mechanism

The working recalls a willing soul into a body dead under ten days, closing fatal wounds and clearing ordinary toxins and infection.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| soul re-anchoring, 2 tiers above 3 | `1e4*(5-3)` | 20,000 |
| wound closure, ~20 points equivalent | `0.30*20` | 6.0 |
| return at 1 point | `0.30*1` | 0.3 |
| neutralise poisons and disease | `1` | 1.0 |
| Pattern cost | `0.01 × Q5 × (1 + 0.75)` | 334 |

| Quantity | Value |
|---|---|
| Effect energy | 20,007 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **20,342 Pz** (30,512.6 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 1.06 |
| Energy-equivalent tier T_E | 5.06 |
| Handling points | 0.75 |
| Grade score | 0.78 → M |

**Handling flags:** costly material, consumed material, long cast.

**Assumptions:** Fatal wounds equal to 20 points; soul constant 1e4 Pz per tier above 3.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Raise Dead (5-N-M-RD) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Necromancy | 6 | `0000000001101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Toulix** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Ritoulix* · T7: *Mitoulix* · T8: *Nitoulix* · T9: *Xyitoulix*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 2→0 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#6149ae`.

![[Raise Dead (5-N-M-RD) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| School | Necromancy | 0.750 | 0.969 | `#0017ff` (475 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.882 | `#ff0028` (700 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.930 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.21): swatch `#4dacc8`, measured lines at 0.004, 0.501, 0.751, 0.883. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.31. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·N·None`; the k4 to k6 lines (None, Touch, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·N·None` |
| Standard spectrometer detection range | 14.26 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 1,911 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Dark, 2x Death. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1D 1F 1J` (Within, Death, Potential, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 3,390 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 1.06 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 5th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 5th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Necromancy school with aspect lean Within, Dark, 2x Death. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 5 Workings]] |
| School | [[Necromancy (School)\|Necromancy]] |
| Affinity | [[Necromancy (School)\|Necromancy]] (N) |
| Function | [[Healing and Restoration]], [[Necromantic and Soul Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Resurrection (7-N-L-RSR)|Resurrection]] (7) · [[Contagion (5-N-L-CNTT)|Contagion]] (5) · [[Revivify (3-C-L-RVV)|Revivify]] (3) · [[True Resurrection (9-N-L-TR)|True Resurrection]] (9) · [[Blight (4-N-L-BLG)|Blight]] (4) · [[Circle of Death (6-N-L-CD)|Circle of Death]] (6) · [[Create Undead (6-N-L-CU)|Create Undead]] (6) · [[Harm (6-N-L-HRM)|Harm]] (6).


---

## Tactical Assessment

Recovers key personnel lost in action when the body is intact, though recovery is weakened for several days.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Necromancy (School)|Necromancy]] · [[Spell Breakdown Procedure]] · [[Parzival]]
