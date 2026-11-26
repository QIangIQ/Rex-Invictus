---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-6
  - spell/evocation
  - source/science-spellbook
aliases:
  - "6th Tier Spell: Absolute Zero"
  - "6-V-L-AZ"
  - "Absolute Zero (Science)"
registry_id: 6-V-L-AZ
attribute_code: "6·Evo·Cold·sphere (30)·60 feet·1 round"
incantation: "Rulod-Sorwyni"
tier: 6
school: Evocation
affinity: V
grade: L
pz_total: 110862.5
pz_quantum: 51944.6
t_e: 6.76
updated: 2026-11-16
---

**Absolute Zero** (`6-V-L-AZ`) is a 6th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **110,863 Pz** against a slot quantum of 51,945 Pz, which puts its energy-equivalent tier at T_E 6.76 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 6 Workings]]
      - [[Evocation]]
        - **Absolute Zero** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `6-V-L-AZ` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `6·Evo·Cold·sphere (30)·60 feet·1 round` |
| Incantation | *Rulod-Sorwyni* |
| Affinity | V (Evocation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 6th Tier |
| School | [[Evocation]] |
| Casting time | 1 Bonus Action |
| Range | 60 feet |
| Area | sphere (30) |
| Duration | 1 round |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 7d6 cold (mean 24.5) |
| Injury by tier | T6: 7d6, T7: 7d6, T8: 7d6, T9: 7d6 |
| Resistance check | constitution; on success: half injury |
| Practitioner lineages | Wizard, Sorcerer, Warlock |

### Mechanism

The field drains heat from a 30 ft sphere fast enough to freeze standing liquids, quench combustion and lock exposed bodies rigid for a few seconds.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Cold injury, 30 ft sphere | `24.5 HP x 0.9 (cold) x S/A_c, S = sphere r=9.144 m = 1050.7 m^2` | 33,097 |
| Air chilled to freezing | `air mass 1.2 kg/m^3 x 3203 m^3: 3843.07 kg x 1005 J/kgK x 30 K / 1500` | 77,246 |
| Pattern cost | `0.01 × Q6 × (1 + 0.00)` | 519 |

| Quantity | Value |
|---|---|
| Effect energy | 110,343 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **110,863 Pz** (166,293.8 kJ) |
| Slot quantum Q6 | 51,945 Pz |
| Field gain (draw / quantum) | 2.13 |
| Energy-equivalent tier T_E | 6.76 |
| Handling points | 0.00 |
| Grade score | 0.38 → L |

**Handling flags:** none.

**Assumptions:** Cold injury 7d6 = 24.5 at full exposure over a 30 ft sphere; 3843 kg of air in the sphere chilled by 30 K so liquids freeze; extracted heat is dumped outside the sphere at no further cost; true cooling toward 0 K would cost far more and is outside the described effect.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Absolute Zero (6-V-L-AZ) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 6 | 6 | `0000000001101` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Cold | 2 | `0000000000101` |
| k4 Area | sphere (30) | 31 | `0000000111111` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | 1 round | 2 | `0000000000101` |

### Incantation

Spoken as **Rulod-Sorwyni** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T7: *Mirulod-Sorwyni* · T8: *Nirulod-Sorwyni* · T9: *Xyirulod-Sorwyni*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 3→2 | 3 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 2→12 | 2 |
| k4 Area | 0→9 1→10 2→11 3→12 4→0 5→1 | 6 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 2→9 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#66c29a`.

![[Absolute Zero (6-V-L-AZ) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 6 | 0.600 | 1.000 | `#00ebff` (520 nm eq.) | source grid |
| Damage | Cold | 0.214 | 0.928 | `#fffa00` (636 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.995 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | 1 round | 0.158 | 0.907 | `#ffae00` (653 nm eq.) | source grid |
| Area | sphere (30) | 0.861 | 0.966 | `#8000ff` (442 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 1.000 | `#00fbff` (524 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 5.04. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `6·V·Cold`; the k4 to k6 lines (sphere (30), 60 feet, 1 round) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `6·V·Cold` |
| Standard spectrometer detection range | 33.30 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 2,597 Pz (0.05 × Q6) |
| Counter drawn cold (all six layers) | 5,194 Pz (0.10 × Q6) |
| Unravel after completion | 5,194 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is 2x Cold, 2x Death and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1B 2D 2f 1j` (Cold, 2x Death, 2x Energy, Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 18,477 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 2.13 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 6th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 6th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 6 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Area Destruction]] |
| Element | [[Cold and Ice Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Freezing Sphere (6-V-M-FSZ)|Freezing Sphere]] (6) · [[Wall of Ice (6-V-M-WI)|Wall of Ice]] (6) · [[Cone of Cold (5-V-L-CC)|Cone of Cold]] (5) · [[Ice Storm (4-V-L-ISE)|Ice Storm]] (4) · [[Blade Barrier (6-V-L-BB)|Blade Barrier]] (6) · [[Burst Radiation (6-V-L-BR)|Burst Radiation]] (6) · [[Sunbeam (6-V-L-SNB)|Sunbeam]] (6) · [[Delayed Blast Fireball (7-V-M-DBF)|Delayed Blast Fireball]] (7).


---

## Tactical Assessment

Breaks an assault wave or a vehicle column for one round and doubles as instant fire suppression on burning hulls and fuel spills.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 6 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
