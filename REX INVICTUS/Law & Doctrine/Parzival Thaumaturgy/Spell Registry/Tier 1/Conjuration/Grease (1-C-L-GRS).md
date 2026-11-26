---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/conjuration
  - source/srd
aliases:
  - "1st Tier Spell: Grease"
  - "Grease"
  - "1-C-L-GRS"
registry_id: 1-C-L-GRS
attribute_code: "1·Con·None·cube (10)·60 feet·1 minute"
incantation: "Se’-Bewyne"
tier: 1
school: Conjuration
affinity: C
grade: L
pz_total: 11.9
pz_quantum: 350.0
t_e: -2.38
updated: 2026-11-16
---

**Grease** (`1-C-L-GRS`) is a 1st Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **11.9 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -2.38 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Conjuration]]
        - **Grease** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-C-L-GRS` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Con·None·cube (10)·60 feet·1 minute` |
| Incantation | *Se’-Bewyne* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | cube (10) |
| Duration | 1 minute |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A bit of pork rind or butter |
| Ritual | no |
| Resistance check | agility; on success: no effect |
| Practitioner lineages | Wizard |

### Mechanism

Coats a 3 m square of ground with a slick lubricant film that topples those standing on it.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| conjured lubricant film | `1 Pz/kg * (9.29 m^2 * 1 mm * 900 kg/m^3 = 8.36 kg)` | 8.4 |
| Pattern cost | `0.01 × Q1 × (1 + 0.00)` | 3.5 |

| Quantity | Value |
|---|---|
| Effect energy | 8.4 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **11.9 Pz** (17.8 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.0339 |
| Energy-equivalent tier T_E | -2.38 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Film thickness 1 mm, density 900 kg/m^3; no upkeep.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Grease (1-C-L-GRS) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | cube (10) | 5 | `0000000001011` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | 1 minute | 1 | `0000000000011` |

### Incantation

Spoken as **Se’-Bewyne** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hise’-Bewyne* · T3: *Lise’-Bewyne* · T4: *Vise’-Bewyne* · T5: *Tise’-Bewyne* · T6: *Rise’-Bewyne* · T7: *Mise’-Bewyne* · T8: *Nise’-Bewyne* · T9: *Xyise’-Bewyne*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 3→12 | 3 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#d08d2e`.

![[Grease (1-C-L-GRS) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Conjuration | 0.125 | 1.000 | `#ff8300` (662 nm eq.) | source grid |
| Duration | 1 minute | 0.105 | 1.000 | `#ff6300` (668 nm eq.) | source grid |
| Area | cube (10) | 0.139 | 0.999 | `#ff9300` (658 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.888 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.18): swatch `#e67044`, measured lines at 0.102, 0.124, 0.139, 0.589. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.07. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·C·None`; the k4 to k6 lines (cube (10), 60 feet, 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·C·None` |
| Standard spectrometer detection range | 0.34 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.0 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 2.0 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (3.4% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Terrain and Matter Shaping]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Entangle (1-C-M-ENT)|Entangle]] (1) · [[Summon Liquid (1-C-L-SL)|Summon Liquid]] (1) · [[Summon Metal (1-C-L-SM)|Summon Metal]] (1) · [[Web (2-C-M-WEB)|Web]] (2) · [[Create Food and Water (3-C-L-CFW)|Create Food and Water]] (3) · [[Create or Destroy Water (1-T-L-CDW)|Create or Destroy Water]] (1) · [[Entangled Attacks (1-E-L-EAT)|Entangled Attacks]] (1) · [[Glue (1-T-L-GLU)|Glue]] (1).


---

## Tactical Assessment

Cheap terrain denial on stairs, ramps and choke points, and an obstacle for wheeled or legged vehicles.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
