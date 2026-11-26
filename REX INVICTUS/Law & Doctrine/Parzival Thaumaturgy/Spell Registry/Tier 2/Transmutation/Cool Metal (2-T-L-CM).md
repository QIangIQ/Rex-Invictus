---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/transmutation
  - source/science-spellbook
aliases:
  - "2nd Tier Spell: Cool Metal"
  - "2-T-L-CM"
  - "Cool Metal (Science)"
registry_id: 2-T-L-CM
attribute_code: "2·Tra·Cold·None·60 feet·Up to 1 minute"
incantation: "Hielod-’wynse"
tier: 2
school: Transmutation
affinity: T
grade: L
pz_total: 121.5
pz_quantum: 951.4
t_e: -0.06
updated: 2026-11-16
---

**Cool Metal** (`2-T-L-CM`) is a 2nd Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **122 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E -0.06 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Transmutation]]
        - **Cool Metal** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-T-L-CM` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Tra·Cold·None·60 feet·Up to 1 minute` |
| Incantation | *Hielod-’wynse* |
| Affinity | T (Transmutation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Transmutation]] |
| Casting time | 1 Action |
| Range | 60 feet |
| Area | single point or target |
| Duration | Up to 1 minute (concentration) |
| Components | none |
| Ritual | no |
| Injury | 2d10 cold (mean 11) |
| Injury by tier | T2: 2d10, T3: 2d10, T4: 2d10, T5: 2d10, T6: 2d10, T7: 2d10, T8: 2d10, T9: 2d10 |
| Resistance check | constitution; on success: no effect |
| Practitioner lineages | Wizard, Sorcerer |

### Mechanism

Pulls heat from a manufactured metal object until it sits far below freezing, burning anyone holding it and wiping its magnetism.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Metal chilled | `steel object: 5 kg x 450 J/kgK x 60 K / 1500` | 90.0 |
| Contact cold injury | `11 HP x 0.9 (cold) x F 0.5 x 3 triggers` | 14.8 |
| Heat leak held off (upkeep) | `120 W x 60 s = 7200 J / 1500` | 4.8 |
| Pattern cost | `0.01 × Q2 × (1 + 0.25)` | 11.9 |

| Quantity | Value |
|---|---|
| Effect energy | 105 Pz |
| Upkeep energy | 4.8 Pz (0.08 Pz/s) |
| **Total draw** | **122 Pz** (182.3 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.128 |
| Energy-equivalent tier T_E | -0.06 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** concentration.

**Assumptions:** Object 5 kg steel cooled by 60 K; heat leak 120 W for 1 minute; contact cold 2d10 = 11 per touch, hand contact F 0.5, 3 contacts.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Cool Metal (2-T-L-CM) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | Cold | 2 | `0000000000101` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Hielod-’wynse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihielod-’wynse* · T4: *Vihielod-’wynse* · T5: *Tihielod-’wynse* · T6: *Rihielod-’wynse* · T7: *Mihielod-’wynse* · T8: *Nihielod-’wynse* · T9: *Xyihielod-’wynse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 2→12 | 2 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#88b190`.

![[Cool Metal (2-T-L-CM) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| Damage | Cold | 0.214 | 1.000 | `#fffa00` (636 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.796 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.889 | `#0074ff` (495 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.927 | `#00fbff` (524 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 2.08. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·T·Cold`; the k4 to k6 lines (None, 60 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·T·Cold` |
| Standard spectrometer detection range | 1.10 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 96.1 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is 2x Cold, 2x Death and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `2B 1D 2h 1j` (2x Cold, Death, 2x Flexibility, Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 20.3 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (12.8% of it). |
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
| Element | [[Cold and Ice Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Chill Touch (0-N-L-CT)|Chill Touch]] (0) · [[Heat Metal (2-T-M-HM)|Heat Metal]] (2) · [[Ray of Frost (0-V-L-RF)|Ray of Frost]] (0) · [[Acid Arrow (2-V-L-AA)|Acid Arrow]] (2) · [[Branding Smite (2-V-L-BS)|Branding Smite]] (2) · [[Flame Blade (2-V-L-FBA)|Flame Blade]] (2) · [[Flaming Sphere (2-C-L-FSA)|Flaming Sphere]] (2) · [[Scorching Ray (2-V-L-SR)|Scorching Ray]] (2).


---

## Tactical Assessment

Disarms soldiers by making weapons painful to hold and degrades magnetic sensors and locks.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
