---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/transmutation
  - source/srd
aliases:
  - "2nd Tier Spell: Spike Growth"
  - "Spike Growth"
  - "2-T-L-SGI"
registry_id: 2-T-L-SGI
attribute_code: "2·Tra·None·cylinder (20)·150 feet·Up to 10 minutes"
incantation: "Hie’-Xénosinly"
tier: 2
school: Transmutation
affinity: T
grade: L
pz_total: 193.8
pz_quantum: 951.4
t_e: 0.41
updated: 2026-11-16
---

**Spike Growth** (`2-T-L-SGI`) is a 2nd Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **194 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E 0.41 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Transmutation]]
        - **Spike Growth** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-T-L-SGI` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Tra·None·cylinder (20)·150 feet·Up to 10 minutes` |
| Incantation | *Hie’-Xénosinly* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Transmutation]] |
| Casting time | 1 action |
| Range | 150 feet |
| Area | cylinder (20) |
| Duration | Up to 10 minutes (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Seven sharp thorns or seven small twigs, each sharpened to a point |
| Ritual | no |
| Practitioner lineages | Druid, Ranger |

### Mechanism

Soil in a 6 m radius is restructured into hardened spikes and thorns, masked to look natural, that pierce anything moving across it.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Reshaping ground into spikes | `3 Pz/kg * 0.5 kg/m^2 * 116.7 m^2` | 175 |
| Piercing injury to movers | `2d4=5 HP * 4 per 20 ft * 3 rounds * 4 creatures * 0.35 * 0.08` | 6.7 |
| Upkeep: Natural-look camouflage | `0.002 Pz/s * (116.7 m^3/1000) * 600 s` | 0.14 |
| Pattern cost | `0.01 × Q2 × (1 + 0.25)` | 11.9 |

| Quantity | Value |
|---|---|
| Effect energy | 182 Pz |
| Upkeep energy | 0.14 Pz (0.000234 Pz/s) |
| **Total draw** | **194 Pz** (290.7 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.204 |
| Energy-equivalent tier T_E | 0.41 |
| Handling points | 0.25 |
| Grade score | -0.55 → L |

**Handling flags:** concentration.

**Assumptions:** Spike layer 0.5 kg/m^2 of structured matter; each of 4 creatures moves 20 ft per round for 3 rounds; point-focused piercing.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Spike Growth (2-T-L-SGI) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | cylinder (20) | 18 | `0000000100101` |
| k5 Range | 150 feet | 4 | `0000000001001` |
| k6 Duration | Up to 10 minutes | 15 | `0000000011111` |

### Incantation

Spoken as **Hie’-Xénosinly** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihie’-Xénosinly* · T4: *Vihie’-Xénosinly* · T5: *Tihie’-Xénosinly* · T6: *Rihie’-Xénosinly* · T7: *Mihie’-Xénosinly* · T8: *Nihie’-Xénosinly* · T9: *Xyihie’-Xénosinly*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 2→11 5→1 | 3 |
| k5 Range | 0→8 3→11 | 2 |
| k6 Duration | 0→7 1→8 2→9 3→10 4→11 | 5 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#889f77`.

![[Spike Growth (2-T-L-SGI) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.796 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Up to 10 minutes | 0.789 | 0.841 | `#1e00ff` (463 nm eq.) | source grid |
| Area | cylinder (20) | 0.500 | 0.956 | `#00ff8b` (550 nm eq.) | source grid |
| Range | 150 feet | 0.235 | 0.999 | `#e3ff00` (629 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.23): swatch `#9b92a3`, measured lines at 0.201, 0.236, 0.501, 0.790, 0.876. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.29. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·T·None`; the k4 to k6 lines (cylinder (20), 150 feet, Up to 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·T·None` |
| Standard spectrometer detection range | 1.39 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 95.2 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 32.3 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (20.4% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Terrain and Matter Shaping]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Create or Destroy Water (1-T-L-CDW)|Create or Destroy Water]] (1) · [[Glue (1-T-L-GLU)|Glue]] (1) · [[Meld Into Stone (3-T-M-MIS)|Meld Into Stone]] (3) · [[Plant Growth (3-T-M-PG)|Plant Growth]] (3) · [[Purify Food and Drink (1-T-L-PFD)|Purify Food and Drink]] (1) · [[Control Water (4-T-H-CWN)|Control Water]] (4) · [[Druidcraft (0-T-L-DRD)|Druidcraft]] (0) · [[Fabricate (4-T-L-FBR)|Fabricate]] (4).


---

## Tactical Assessment

Area denial against infantry and soft-wheeled vehicles; turns a crossing or clearing into a slow, bleeding approach.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
