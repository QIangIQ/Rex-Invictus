---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/abjuration
  - source/srd
aliases:
  - "3rd Tier Spell: Magic Circle"
  - "Magic Circle"
  - "3-A-L-MC"
registry_id: 3-A-L-MC
attribute_code: "3·Abj·None·cylinder (10)·10 feet·1 hour"
incantation: "La’-Xespula"
tier: 3
school: Abjuration
affinity: A
grade: L
pz_total: 151.0
pz_quantum: 2586.2
t_e: 0.16
updated: 2026-11-16
---

**Magic Circle** (`3-A-L-MC`) is a 3rd Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **151 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E 0.16 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Abjuration]]
        - **Magic Circle** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-A-L-MC` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Abj·None·cylinder (10)·10 feet·1 hour` |
| Incantation | *La’-Xespula* |
| Affinity | A (Abjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Abjuration]] |
| Casting time | 1 minute |
| Range | 10 feet |
| Area | cylinder (10) |
| Duration | 1 hour |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Holy water or powdered silver and iron worth at least 100 gp, which the spell consumes |
| Ritual | no |
| Resistance check | presence; on success: other |
| Practitioner lineages | Cleric, Paladin, Warlock, Wizard |

### Mechanism

The field raises a 10 ft radius, 20 ft tall cylinder keyed to selected kinds of extraplanar or undead beings, blocking their entry, weakening their attacks across the boundary and shielding occupants from their control. It can be inverted to hold such a being inside.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Attack attenuation on bound kind (upkeep) | `0.20 Pz * (25% * 30 HP/round * 10 rounds) / 3600 s * 3600 s` | 15.0 |
| Boundary repulsion, 10 entry attempts (upkeep) | `0.5 * 80 kg * (5 m/s)^2 * 10 / 1500 / 3600 s * 3600 s` | 6.7 |
| Mental shielding of 4 occupants (upkeep) | `0.005 Pz/s * 4 * 3600 s` | 72.0 |
| Rune glow (upkeep) | `5 W / 1500 * 3600 s` | 12.0 |
| Pattern cost | `0.01 × Q3 × (1 + 0.75)` | 45.3 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 106 Pz (0.0294 Pz/s) |
| **Total draw** | **151 Pz** (226.4 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 0.0584 |
| Energy-equivalent tier T_E | 0.16 |
| Handling points | 0.75 |
| Grade score | -0.25 → L |

**Handling flags:** costly material, consumed material, long cast.

**Assumptions:** One 10-round assault at 30 per round with a quarter of hits lost; 10 attempts to push in at 5 m/s; 4 occupants shielded; 1 hour.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Magic Circle (3-A-L-MC) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | cylinder (10) | 17 | `0000000100011` |
| k5 Range | 10 feet | 1 | `0000000000011` |
| k6 Duration | 1 hour | 0 | `0000000000001` |

### Incantation

Spoken as **La’-Xespula** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vila’-Xespula* · T5: *Tila’-Xespula* · T6: *Rila’-Xespula* · T7: *Mila’-Xespula* · T8: *Nila’-Xespula* · T9: *Xyila’-Xespula*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 5→1 | 3 |
| k5 Range | 0→8 1→9 | 2 |
| k6 Duration | 0→7 | 1 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#b3751b`.

![[Magic Circle (3-A-L-MC) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.956 | `#ff0028` (700 nm eq.) | source grid |
| Duration | 1 hour | 0.053 | 0.970 | `#ff1c00` (684 nm eq.) | source grid |
| Area | cylinder (10) | 0.472 | 0.985 | `#00ff60` (558 nm eq.) | source grid |
| Range | 10 feet | 0.059 | 0.971 | `#ff2700` (682 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.19): swatch `#ec6c3f`, measured lines at 0.007, 0.057, 0.300, 0.473. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.18. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·A·None`; the k4 to k6 lines (cylinder (10), 10 feet, 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·A·None` |
| Standard spectrometer detection range | 1.23 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 280 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 25.2 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 3rd Tier quantum of 2,586 Pz (5.8% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Teleportation and Planar Travel]], [[Summoning and Conjured Creatures]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Banishment (4-A-M-BNS)|Banishment]] (4) · [[Animate Dead (3-N-M-AD)|Animate Dead]] (3) · [[Arcane Singularity (3-C-L-ASA)|Arcane Singularity]] (3) · [[Blink (3-T-L-BLN)|Blink]] (3) · [[Conjure Animals (3-C-M-CA)|Conjure Animals]] (3) · [[Imprisonment (9-A-L-IMP)|Imprisonment]] (9) · [[Pauli Exclusion Principle (5-A-L-PEP)|Pauli Exclusion Principle]] (5) · [[Phantom Steed (3-I-H-PSA)|Phantom Steed]] (3).


---

## Tactical Assessment

Forms a safe room against summoned or possessing entities, or a holding cell for a captured one. It offers no protection against ordinary troops.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
