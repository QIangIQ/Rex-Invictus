---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/transmutation
  - source/srd
aliases:
  - "3rd Tier Spell: Meld Into Stone"
  - "Meld Into Stone"
  - "3-T-M-MIS"
registry_id: 3-T-M-MIS
attribute_code: "3·Tra·None·None·Touch·8 hours"
incantation: "Lielixiy"
tier: 3
school: Transmutation
affinity: T
grade: M
pz_total: 826.2
pz_quantum: 2586.2
t_e: 1.86
updated: 2026-11-16
---

**Meld Into Stone** (`3-T-M-MIS`) is a 3rd Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **826 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E 1.86 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Transmutation]]
        - **Meld Into Stone** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-T-M-MIS` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Tra·None·None·Touch·8 hours` |
| Incantation | *Lielixiy* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Transmutation]] |
| Casting time | 1 action |
| Range | Touch |
| Area | single point or target |
| Duration | 8 hours |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | yes |
| Practitioner lineages | Cleric |

### Mechanism

The field merges the caster and carried gear into a stone mass large enough to contain them, hiding them from ordinary senses for up to 8 hours. Breaking or reshaping the stone ejects and injures the occupant.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Phasing body into stone lattice | `3 Pz/kg * (0.08 m^3 * 2600 kg/m^3 = 208 kg)` | 624 |
| Holding the merged state (upkeep) | `0.005 Pz/s * 28800 s` | 144 |
| Pattern cost | `0.01 × Q3 × (1 + 1.25)` | 58.2 |

| Quantity | Value |
|---|---|
| Effect energy | 624 Pz |
| Upkeep energy | 144 Pz (0.005 Pz/s) |
| **Total draw** | **826 Pz** (1,239.3 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 0.319 |
| Energy-equivalent tier T_E | 1.86 |
| Handling points | 1.25 |
| Grade score | 0.68 → M |

**Handling flags:** ritual, fragile.

**Assumptions:** Body volume 0.08 m^3 of stone restructured; merged state held 8 hours.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Meld Into Stone (3-T-M-MIS) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | 8 hours | 8 | `0000000010001` |

### Incantation

Spoken as **Lielixiy** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vilielixiy* · T5: *Tilielixiy* · T6: *Rilielixiy* · T7: *Milielixiy* · T8: *Nilielixiy* · T9: *Xyilielixiy*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 4→11 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#6c8990`.

![[Meld Into Stone (3-T-M-MIS) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.848 | `#9600ff` (438 nm eq.) | source grid |
| Duration | 8 hours | 0.474 | 0.985 | `#00ff66` (558 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.844 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.20): swatch `#839dc2`, measured lines at 0.300, 0.474, 0.878. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.92. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·T·None`; the k4 to k6 lines (None, Touch, 8 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·T·None` |
| Standard spectrometer detection range | 2.87 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 287 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 138 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 3rd Tier quantum of 2,586 Pz (31.9% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Terrain and Matter Shaping]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Plant Growth (3-T-M-PG)|Plant Growth]] (3) · [[Control Water (4-T-H-CWN)|Control Water]] (4) · [[Fabricate (4-T-L-FBR)|Fabricate]] (4) · [[Freefall (4-T-L-FRF)|Freefall]] (4) · [[Spike Growth (2-T-L-SGI)|Spike Growth]] (2) · [[Stone Shape (4-T-M-SSO)|Stone Shape]] (4) · [[Arcane Redirection (3-A-L-AR)|Arcane Redirection]] (3) · [[Create Food and Water (3-C-L-CFW)|Create Food and Water]] (3).


---

## Tactical Assessment

A hide for scouts and stay-behind agents inside walls, cliffs and bunkers. The occupant is effectively blind and can be crushed by demolition.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
