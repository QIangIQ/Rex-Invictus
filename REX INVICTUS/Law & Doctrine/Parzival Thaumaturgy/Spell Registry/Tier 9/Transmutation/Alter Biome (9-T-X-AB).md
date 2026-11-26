---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-9
  - spell/transmutation
  - source/science-spellbook
aliases:
  - "9th Tier Spell: Alter Biome"
  - "9-T-X-AB"
  - "Alter Biome (Science)"
registry_id: 9-T-X-AB
attribute_code: "9·Tra·None·cylinder (5280)·Touch·Until dispelled"
incantation: "Xyie’-Xailixis"
tier: 9
school: Transmutation
affinity: T
grade: X
pz_total: 812907385.9
pz_quantum: 1043335.3
t_e: 15.66
updated: 2026-11-16
---

**Alter Biome** (`9-T-X-AB`) is a 9th Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **812.91 MPz Pz** against a slot quantum of 1.04 MPz Pz, which puts its energy-equivalent tier at T_E 15.66 and its handling grade at **Extreme**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 9 Workings]]
      - [[Transmutation]]
        - **Alter Biome** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `9-T-X-AB` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `9·Tra·None·cylinder (5280)·Touch·Until dispelled` |
| Incantation | *Xyie’-Xailixis* |
| Affinity | T (Transmutation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 9th Tier |
| School | [[Transmutation]] |
| Casting time | 1 hour |
| Range | Touch |
| Area | cylinder (5280) |
| Duration | Until dispelled |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A small amount of soil or plantlife from the new biome |
| Ritual | yes |
| Practitioner lineages | Wizard, Sorcerer, Druid |

### Mechanism

A one-hour working rewrites ground cover, topsoil and relief across a disc 1 mile in radius and binds the result with a standing land ward that keeps local climate in the new regime.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Living ground cover conjured | `8.14e+06 m^2 x 2 kg/m^2 x 10 Pz/kg` | 162.73 MPz |
| Topsoil restructured | `8.14e+06 m^2 x 0.05 m x 1500 kg/m^3 x 1 Pz/kg` | 610.25 MPz |
| Relief raised | `m*g*h: 6.1e+09 kg x 9.81 x 1 m / 1500` | 39.91 MPz |
| Pattern cost | `0.01 × Q9 × (1 + 0.50)` | 15,650 |

| Quantity | Value |
|---|---|
| Effect energy | 812.89 MPz Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **812.91 MPz Pz** (1,219,361,078.8 kJ) |
| Slot quantum Q9 | 1.04 MPz Pz |
| Field gain (draw / quantum) | 779 |
| Energy-equivalent tier T_E | 15.66 |
| Handling points | 0.50 |
| Grade score | 3.50 → X |

**Handling flags:** ritual, long cast.

**Assumptions:** Disc radius 1609 m (8.13e6 m^2); new standing biomass 2 kg/m^2 at 10 Pz/kg; topsoil reworked to 5 cm depth (1500 kg/m^3) at 1 Pz/kg; mean relief change 1 m over half the area; climate is held by the permanent ward, which draws its own return and is not charged to this casting, so upkeep is 0.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Alter Biome (9-T-X-AB) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 9 | 9 | `0000000010011` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | cylinder (5280) | 38 | `0000001001101` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Until dispelled | 11 | `0000000010111` |

### Incantation

Spoken as **Xyie’-Xailixis** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 4→3 | 3 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 2→11 3→12 6→2 | 4 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 2→9 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#6360fd`.

![[Alter Biome (9-T-X-AB) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 9 | 0.900 | 1.000 | `#b600ff` (430 nm eq.) | source grid |
| School | Transmutation | 0.875 | 1.000 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Until dispelled | 0.579 | 0.950 | `#00fff7` (526 nm eq.) | source grid |
| Area | cylinder (5280) | 0.597 | 0.955 | `#00f1ff` (521 nm eq.) | RI half-step |
| Range | Touch | 0.882 | 1.000 | `#9b00ff` (435 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 8.91. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `9·T·None`; the k4 to k6 lines (cylinder (5280), Touch, Until dispelled) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `9·T·None` |
| Standard spectrometer detection range | 2,851.15 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 52,167 Pz (0.05 × Q9) |
| Counter drawn cold (all six layers) | 104,334 Pz (0.10 × Q9) |
| Unravel after completion | 104,334 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 135.48 MPz Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 779.14 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 9th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Endures independently once set, which places it under the decay clause of ULMTU-XIII. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIII]] | Lex Impermanentiae | Long-lived patterns drift toward reversion unless refreshed from a source that satisfies ULMTU-I. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVI]] | Lex Interdictorum | Exceeds 100 MPz; requires direct acknowledgement from the [[Répertoire du Savoir Athénien]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 9th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 9 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Terrain and Matter Shaping]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Extreme]] |

Similar workings: [[Control Weather (8-T-H-CWT)|Control Weather]] (8) · [[Earthquake (8-V-M-ERT)|Earthquake]] (8) · [[Move Earth (6-T-M-ME)|Move Earth]] (6) · [[Passwall (5-T-L-PSS)|Passwall]] (5) · [[Shapechange (9-T-L-SHP)|Shapechange]] (9) · [[Time Stop (9-T-M-TSM)|Time Stop]] (9) · [[True Polymorph (9-T-L-TPU)|True Polymorph]] (9) · [[Weave Warp (9-T-L-WWA)|Weave Warp]] (9).


---

## Tactical Assessment

Strategic terraforming: turns approach routes into swamp or tundra, creates forest cover for concealment, or makes a desert airfield on short notice.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 9 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
