---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/transmutation
  - source/science-spellbook
aliases:
  - "3rd Tier Spell: Chemical Transition"
  - "3-T-L-CTE"
  - "Chemical Transition (Science)"
registry_id: 3-T-L-CTE
attribute_code: "3·Tra·None·None·Touch·Instantaneous"
incantation: "Lielix"
tier: 3
school: Transmutation
affinity: T
grade: L
pz_total: 372.1
pz_quantum: 2586.2
t_e: 1.06
updated: 2026-11-16
---

**Chemical Transition** (`3-T-L-CTE`) is a 3rd Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **372 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E 1.06 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Transmutation]]
        - **Chemical Transition** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-T-L-CTE` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Tra·None·None·Touch·Instantaneous` |
| Incantation | *Lielix* |
| Affinity | T (Transmutation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Transmutation]] |
| Casting time | 1 hour |
| Range | Touch |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A small vial of water |
| Ritual | yes |
| Practitioner lineages | Wizard, Sorcerer, Druid |

### Mechanism

Over an hour, rearranges the chemistry of a held potion into another of equal or lower grade.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Chemical rearrangement | `0.5 kg x 1 MJ/kg = 5e+05 J / 1500` | 333 |
| Pattern cost | `0.01 × Q3 × (1 + 0.50)` | 38.8 |

| Quantity | Value |
|---|---|
| Effect energy | 333 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **372 Pz** (558.2 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 0.144 |
| Energy-equivalent tier T_E | 1.06 |
| Handling points | 0.50 |
| Grade score | -0.47 → L |

**Handling flags:** ritual, long cast.

**Assumptions:** Potion 0.5 kg; reorganising its chemistry costs about 1 MJ/kg (partial bond rearrangement, real chemistry), so 0.5 MJ.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Chemical Transition (3-T-L-CTE) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Lielix** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vilielix* · T5: *Tilielix* · T6: *Rilielix* · T7: *Milielix* · T8: *Nilielix* · T9: *Xyilielix*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#af4580`.

![[Chemical Transition (3-T-L-CTE) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.848 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.956 | `#ff0028` (700 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.844 | `#9b00ff` (435 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 2.57. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·T·None`; the k4 to k6 lines (None, Touch, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·T·None` |
| Standard spectrometer detection range | 1.93 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 259 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 62.0 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 3rd Tier quantum of 2,586 Pz (14.4% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Transformation]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Gaseous Form (3-T-M-GF)|Gaseous Form]] (3) · [[Alter Self (2-T-L-AST)|Alter Self]] (2) · [[Enlarge-Reduce (2-T-M-ERL)|Enlarge/Reduce]] (2) · [[Polymorph (4-T-L-PLY)|Polymorph]] (4) · [[Arcane Redirection (3-A-L-AR)|Arcane Redirection]] (3) · [[Crystalise (1-T-L-CRY)|Crystalise]] (1) · [[Fourier Transform (3-E-L-FTU)|Fourier Transform]] (3) · [[Reduce Relative Velocity (1-T-L-RRV)|Reduce Relative Velocity]] (1).


---

## Tactical Assessment

Field logistics: converts surplus stores into the type a unit needs.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
