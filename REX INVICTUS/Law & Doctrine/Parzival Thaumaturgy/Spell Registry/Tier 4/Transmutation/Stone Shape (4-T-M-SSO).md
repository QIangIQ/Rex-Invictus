---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/transmutation
  - source/srd
aliases:
  - "4th Tier Spell: Stone Shape"
  - "Stone Shape"
  - "4-T-M-SSO"
registry_id: 4-T-M-SSO
attribute_code: "4·Tra·None·None·Touch·Instantaneous"
incantation: "Vielix"
tier: 4
school: Transmutation
affinity: T
grade: M
pz_total: 27680.3
pz_quantum: 7029.9
t_e: 5.37
updated: 2026-11-16
---

**Stone Shape** (`4-T-M-SSO`) is a 4th Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **27,680 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E 5.37 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Transmutation]]
        - **Stone Shape** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-T-M-SSO` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Tra·None·None·Touch·Instantaneous` |
| Incantation | *Vielix* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Transmutation]] |
| Casting time | 1 action |
| Range | Touch |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Soft clay, to be crudely worked into the desired shape for the stone object |
| Ritual | no |
| Practitioner lineages | Cleric, Druid, Wizard |

### Mechanism

Stone up to 1.5 m in any dimension is made plastic and re-formed into a chosen shape with up to two hinges and a latch.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Reshaping stone section | `3 Pz/kg * 9203 kg (3.54 m^3 * 2600 kg/m^3)` | 27,610 |
| Pattern cost | `0.01 × Q4 × (1 + 0.00)` | 70.3 |

| Quantity | Value |
|---|---|
| Effect energy | 27,610 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **27,680 Pz** (41,520.4 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 3.94 |
| Energy-equivalent tier T_E | 5.37 |
| Handling points | 0.00 |
| Grade score | 0.69 → M |

**Handling flags:** none.

**Assumptions:** Maximum 5 ft cube of granite at 2600 kg/m^3; typical uses involve much less mass.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Stone Shape (4-T-M-SSO) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 4 | 4 | `0000000001001` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Vielix** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T5: *Tivielix* · T6: *Rivielix* · T7: *Mivielix* · T8: *Nivielix* · T9: *Xyivielix*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 3→2 | 2 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#884484`.

![[Stone Shape (4-T-M-SSO) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.893 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.923 | `#ff0028` (700 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.890 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.23): swatch `#7a88c0`, measured lines at 0.004, 0.401, 0.878. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.44. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·T·None`; the k4 to k6 lines (None, Touch, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·T·None` |
| Standard spectrometer detection range | 16.64 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 703 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 4,613 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 3.94 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 4th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 4th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 4 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Terrain and Matter Shaping]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Control Water (4-T-H-CWN)|Control Water]] (4) · [[Fabricate (4-T-L-FBR)|Fabricate]] (4) · [[Freefall (4-T-L-FRF)|Freefall]] (4) · [[Meld Into Stone (3-T-M-MIS)|Meld Into Stone]] (3) · [[Passwall (5-T-L-PSS)|Passwall]] (5) · [[Plant Growth (3-T-M-PG)|Plant Growth]] (3) · [[Ice Storm (4-V-L-ISE)|Ice Storm]] (4) · [[Move Earth (6-T-M-ME)|Move Earth]] (6).


---

## Tactical Assessment

Breaching thin masonry, sealing doors and crafting improvised fittings during urban or bunker operations.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
