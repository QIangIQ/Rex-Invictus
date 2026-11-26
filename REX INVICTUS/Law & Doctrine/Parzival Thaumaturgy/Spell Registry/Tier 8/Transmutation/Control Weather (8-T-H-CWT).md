---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-8
  - spell/transmutation
  - source/srd
aliases:
  - "8th Tier Spell: Control Weather"
  - "Control Weather"
  - "8-T-H-CWT"
registry_id: 8-T-H-CWT
attribute_code: "8·Tra·None·None·Self·Up to 8 hours"
incantation: "Nieporos"
tier: 8
school: Transmutation
affinity: T
grade: H
pz_total: 7369229.5
pz_quantum: 383821.6
t_e: 10.95
updated: 2026-11-16
---

**Control Weather** (`8-T-H-CWT`) is a 8th Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **7.37 MPz Pz** against a slot quantum of 383,822 Pz, which puts its energy-equivalent tier at T_E 10.95 and its handling grade at **High**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 8 Workings]]
      - [[Transmutation]]
        - **Control Weather** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `8-T-H-CWT` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `8·Tra·None·None·Self·Up to 8 hours` |
| Incantation | *Nieporos* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 8th Tier |
| School | [[Transmutation]] |
| Casting time | 10 minutes |
| Range | Self |
| Area | single point or target |
| Duration | Up to 8 hours (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Burning incense and bits of earth and wood mixed in water |
| Ritual | no |
| Practitioner lineages | Cleric, Druid, Wizard |

### Mechanism

The field nudges regional precipitation, temperature and wind one stage at a time within 5 miles, steering existing atmospheric instabilities. Losing sight of the open sky ends it.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| one-stage shift: 5 K over 5 mi radius x 1 km air, catalytic leverage 1e-6 | `pi*(5*5280*ft)**2*1000*1.2*1005*5*1e-6/J` | 817,737 |
| upkeep: re-drive against relaxation (1 h time constant) for 8 h | `8*pi*(5*5280*ft)**2*1000*1.2*1005*5*1e-6/J` | 6.54 MPz |
| Pattern cost | `0.01 × Q8 × (1 + 1.50)` | 9,596 |

| Quantity | Value |
|---|---|
| Effect energy | 817,737 Pz |
| Upkeep energy | 6.54 MPz Pz (227 Pz/s) |
| **Total draw** | **7.37 MPz Pz** (11,053,844.2 kJ) |
| Slot quantum Q8 | 383,822 Pz |
| Field gain (draw / quantum) | 19.2 |
| Energy-equivalent tier T_E | 10.95 |
| Handling points | 1.50 |
| Grade score | 2.98 → H |

**Handling flags:** concentration, fragile, long cast.

**Assumptions:** Order-of-magnitude only. Full direct supply would be about 8.2e11 Pz; field assumed to act catalytically with leverage 1e-6; 1 h relaxation time so drive is renewed 8 times.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Control Weather (8-T-H-CWT) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 8 | 8 | `0000000010001` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Up to 8 hours | 18 | `0000000100101` |

### Incantation

Spoken as **Nieporos** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T9: *Xyinieporos*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 4→3 | 2 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 2→9 5→12 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#6d16ff`.

![[Control Weather (8-T-H-CWT) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 8 | 0.800 | 1.000 | `#2900ff` (460 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.997 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Up to 8 hours | 0.947 | 0.989 | `#f800ff` (416 nm eq.) | source grid |
| Range | Self | 0.706 | 0.996 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.15): swatch `#347af5`, measured lines at 0.706, 0.801, 0.876, 0.948. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 6.87. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `8·T·None`; the k4 to k6 lines (None, Self, Up to 8 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `8·T·None` |
| Standard spectrometer detection range | 271.46 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 19,191 Pz (0.05 × Q8) |
| Counter drawn cold (all six layers) | 38,382 Pz (0.10 × Q8) |
| Unravel after completion | 1.35 MPz Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1.23 MPz Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 19.20 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 8th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 8th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 8 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Terrain and Matter Shaping]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|High]] |

Similar workings: [[Alter Biome (9-T-X-AB)|Alter Biome]] (9) · [[Earthquake (8-V-M-ERT)|Earthquake]] (8) · [[Move Earth (6-T-M-ME)|Move Earth]] (6) · [[Passwall (5-T-L-PSS)|Passwall]] (5) · [[Animal Shapes (8-T-M-ASM)|Animal Shapes]] (8) · [[Control Water (4-T-H-CWN)|Control Water]] (4) · [[Fabricate (4-T-L-FBR)|Fabricate]] (4) · [[Freefall (4-T-L-FRF)|Freefall]] (4).


---

## Tactical Assessment

Shapes the operational weather for a theatre: grounding air assets, covering movements with fog or storms, or clearing skies for observation.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 8 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
