---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/transmutation
  - source/srd
aliases:
  - "2nd Tier Spell: Heat Metal"
  - "Heat Metal"
  - "2-T-M-HM"
registry_id: 2-T-M-HM
attribute_code: "2·Tra·Fire·None·60 feet·Up to 1 minute"
incantation: "Hieire-’wynse"
tier: 2
school: Transmutation
affinity: T
grade: M
pz_total: 6232.0
pz_quantum: 951.4
t_e: 3.88
updated: 2026-11-16
---

**Heat Metal** (`2-T-M-HM`) is a 2nd Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **6,232 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E 3.88 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Transmutation]]
        - **Heat Metal** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-T-M-HM` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Tra·Fire·None·60 feet·Up to 1 minute` |
| Incantation | *Hieire-’wynse* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Transmutation]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | single point or target |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A piece of iron and a flame |
| Ritual | no |
| Injury | 2d8 fire (mean 9) |
| Injury by tier | T2: 2d8, T3: 3d8, T4: 4d8, T5: 5d8, T6: 6d8, T7: 7d8, T8: 8d8, T9: 9d8 |
| Resistance check | constitution; on success: other |
| Practitioner lineages | Bard, Druid |

### Mechanism

Heats a manufactured metal object to red heat and keeps it there, burning anyone touching or wearing it.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| heating armor to red heat | `25 kg * 450 J/kgK * 600 K / 1500` | 4,500 |
| contact burns, 2d8=9 | `9 HP * kappa_fire 0.7 * F 0.5 * 1 target(s) * 3 trigger(s)` | 9.4 |
| hold against radiative loss | `5.67e-8 * 0.8 * 1.5 m^2 * (893^4 - 293^4) W / 1500 = 28.5112 Pz/s * 60 s` | 1,711 |
| Pattern cost | `0.01 × Q2 × (1 + 0.25)` | 11.9 |

| Quantity | Value |
|---|---|
| Effect energy | 4,509 Pz |
| Upkeep energy | 1,711 Pz (28.5 Pz/s) |
| **Total draw** | **6,232 Pz** (9,348.0 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 6.55 |
| Energy-equivalent tier T_E | 3.88 |
| Handling points | 0.25 |
| Grade score | 1.19 → M |

**Handling flags:** concentration.

**Assumptions:** Target 25 kg of steel armour heated by 600 K and held for 1 minute (emissivity 0.8, 1.5 m^2); 3 burn triggers at F 0.5.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Heat Metal (2-T-M-HM) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | Fire | 3 | `0000000000111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Hieire-’wynse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihieire-’wynse* · T4: *Vihieire-’wynse* · T5: *Tihieire-’wynse* · T6: *Rihieire-’wynse* · T7: *Mihieire-’wynse* · T8: *Nihieire-’wynse* · T9: *Xyihieire-’wynse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 | 3 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#72b290`.

![[Heat Metal (2-T-M-HM) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| Damage | Fire | 0.286 | 0.996 | `#9cff00` (614 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.796 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.889 | `#0074ff` (495 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.927 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.18): swatch `#93a7a8`, measured lines at 0.201, 0.286, 0.589, 0.685, 0.876. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.79. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·T·Fire`; the k4 to k6 lines (None, 60 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·T·Fire` |
| Standard spectrometer detection range | 7.89 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 437 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Energy, Movement and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1b 1c 1d 1f 2h 2j` (Heat, Light, Life, Energy, 2x Flexibility, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1,039 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 6.55 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 2nd Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
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
| Function | [[Precision Strikes]] |
| Element | [[Fire Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Flame Blade (2-V-L-FBA)|Flame Blade]] (2) · [[Flaming Sphere (2-C-L-FSA)|Flaming Sphere]] (2) · [[Scorching Ray (2-V-L-SR)|Scorching Ray]] (2) · [[Focusing Lens (1-V-L-FLC)|Focusing Lens]] (1) · [[Hellish Rebuke (1-V-L-HR)|Hellish Rebuke]] (1) · [[Cool Metal (2-T-L-CM)|Cool Metal]] (2) · [[Fire Bolt (0-V-L-FB)|Fire Bolt]] (0) · [[Produce Flame (0-C-L-PF)|Produce Flame]] (0).


---

## Tactical Assessment

Defeats armoured infantry, renders weapons unusable and heats vehicle hulls or hatches; a strong counter to powered armour.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
