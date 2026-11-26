---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/illusion
  - source/srd
aliases:
  - "4th Tier Spell: Hallucinatory Terrain"
  - "Hallucinatory Terrain"
  - "4-I-M-HT"
registry_id: 4-I-M-HT
attribute_code: "4·Ill·None·cube (150)·300 feet·24 hours"
incantation: "Vai’-Basphinl"
tier: 4
school: Illusion
affinity: I
grade: M
pz_total: 16602.3
pz_quantum: 7029.9
t_e: 4.86
updated: 2026-11-16
---

**Hallucinatory Terrain** (`4-I-M-HT`) is a 4th Tier working of the [[Illusion]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **16,602 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E 4.86 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Illusion]]
        - **Hallucinatory Terrain** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-I-M-HT` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Ill·None·cube (150)·300 feet·24 hours` |
| Incantation | *Vai’-Basphinl* |
| Affinity | I (Illusion) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Illusion]] |
| Casting time | 10 minutes |
| Range | 300 feet |
| Area | cube (150) |
| Duration | 24 hours |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A stone, a twig, and a bit of green plant |
| Ritual | no |
| Practitioner lineages | Bard, Druid, Warlock, Wizard |

### Mechanism

Overlays a 46 m cube of natural terrain with the sight, sound and smell of different terrain, leaving touch unchanged.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| terrain illusion | `0.002 Pz/s * 95569 m^3 / 1000 = 0.191139 Pz/s * 86400 s` | 16,514 |
| Pattern cost | `0.01 × Q4 × (1 + 0.25)` | 87.9 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 16,514 Pz (0.191 Pz/s) |
| **Total draw** | **16,602 Pz** (24,903.4 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 2.36 |
| Energy-equivalent tier T_E | 4.86 |
| Handling points | 0.25 |
| Grade score | 0.68 → M |

**Handling flags:** long cast.

**Assumptions:** Full 150 ft cube for 24 h at the illusion volume rate.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Hallucinatory Terrain (4-I-M-HT) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 4 | 4 | `0000000001001` |
| k2 School | Illusion | 5 | `0000000001011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | cube (150) | 8 | `0000000010001` |
| k5 Range | 300 feet | 6 | `0000000001101` |
| k6 Duration | 24 hours | 5 | `0000000001011` |

### Incantation

Spoken as **Vai’-Basphinl** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T5: *Tivai’-Basphinl* · T6: *Rivai’-Basphinl* · T7: *Mivai’-Basphinl* · T8: *Nivai’-Basphinl* · T9: *Xyivai’-Basphinl*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 3→2 | 2 |
| k2 School | 0→11 1→12 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 4→0 | 2 |
| k5 Range | 0→8 2→10 3→11 | 3 |
| k6 Duration | 0→7 1→8 3→10 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#55f332`.

![[Hallucinatory Terrain (4-I-M-HT) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| School | Illusion | 0.625 | 0.975 | `#00c5ff` (512 nm eq.) | source grid |
| Duration | 24 hours | 0.316 | 0.996 | `#76ff00` (605 nm eq.) | source grid |
| Area | cube (150) | 0.222 | 0.984 | `#f8ff00` (633 nm eq.) | source grid |
| Range | 300 feet | 0.353 | 0.999 | `#40ff00` (594 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.18): swatch `#9be3a0`, measured lines at 0.223, 0.316, 0.354, 0.401, 0.626. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.22. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·I·None`; the k4 to k6 lines (cube (150), 300 feet, 24 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·I·None` |
| Standard spectrometer detection range | 12.88 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 4,006 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Light, Introspection, 2x Flexibility. The working vector used by [[Recast Tension and Combination Affinity]] is `2c 1d 1F 1G 2h 1J` (2x Light, Life, Potential, Introspection, 2x Flexibility, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 2,767 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 2.36 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 4th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 4th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Illusion school with aspect lean Light, Introspection, 2x Flexibility. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 4 Workings]] |
| School | [[Illusion]] |
| Affinity | [[Illusion]] (I) |
| Function | [[Concealment and Illusion]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Greater Invisibility (4-I-L-GIE)|Greater Invisibility]] (4) · [[Illusory Geodesic Curve (3-I-L-IGC)|Illusory Geodesic Curve]] (3) · [[Major Image (3-I-L-MIJ)|Major Image]] (3) · [[Mislead (5-I-L-MSL)|Mislead]] (5) · [[Seeming (5-I-L-SMN)|Seeming]] (5) · [[Arcanist's Magic Aura (2-I-L-ASMA)|Arcanist's Magic Aura]] (2) · [[Blur (2-I-L-BLR)|Blur]] (2) · [[Cloak (2-I-L-CLK)|Cloak]] (2).


---

## Tactical Assessment

Large-scale camouflage: hides a road, fakes a swamp or masks a landing ground from visual reconnaissance for a day.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Illusion]] · [[Spell Breakdown Procedure]] · [[Parzival]]
