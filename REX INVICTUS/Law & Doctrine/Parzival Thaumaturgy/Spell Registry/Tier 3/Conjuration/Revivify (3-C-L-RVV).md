---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/conjuration
  - source/srd
aliases:
  - "3rd Tier Spell: Revivify"
  - "Revivify"
  - "3-C-L-RVV"
registry_id: 3-C-L-RVV
attribute_code: "3·Con·None·None·Touch·Instantaneous"
incantation: "Lelix"
tier: 3
school: Conjuration
affinity: C
grade: L
pz_total: 40.1
pz_quantum: 2586.2
t_e: -1.17
updated: 2026-11-16
---

**Revivify** (`3-C-L-RVV`) is a 3rd Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **40.1 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E -1.17 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Conjuration]]
        - **Revivify** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-C-L-RVV` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Con·None·None·Touch·Instantaneous` |
| Incantation | *Lelix* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | Touch |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Diamonds worth 300gp, which the spell consumes |
| Ritual | no |
| Practitioner lineages | Cleric, Paladin |

### Mechanism

Within a minute of death the field restarts the body and holds the not-yet-departed soul in place.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| soul re-anchoring, 0 tiers above 3 | `1e4*0` | 0 |
| return at 1 point | `0.30*1` | 0.3 |
| cardiac and neural restart, instant | `1` | 1.0 |
| Pattern cost | `0.01 × Q3 × (1 + 0.50)` | 38.8 |

| Quantity | Value |
|---|---|
| Effect energy | 1.3 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **40.1 Pz** (60.1 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 0.0155 |
| Energy-equivalent tier T_E | -1.17 |
| Handling points | 0.50 |
| Grade score | -0.50 → L |

**Handling flags:** costly material, consumed material.

**Assumptions:** Tier 3 gives no soul re-anchoring term; cost is restart plus 1 point of healing.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Revivify (3-C-L-RVV) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Lelix** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vilelix* · T5: *Tilelix* · T6: *Rilelix* · T7: *Milelix* · T8: *Nilelix* · T9: *Xyilelix*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#ca6542`.

![[Revivify (3-C-L-RVV) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.985 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.956 | `#ff0028` (700 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.844 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.22): swatch `#d77a64`, measured lines at 0.004, 0.126, 0.300, 0.883. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 1.60. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·C·None`; the k4 to k6 lines (None, Touch, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·C·None` |
| Standard spectrometer detection range | 0.63 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 259 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 6.7 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 3rd Tier quantum of 2,586 Pz (1.6% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Healing and Restoration]], [[Necromantic and Soul Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Raise Dead (5-N-M-RD)|Raise Dead]] (5) · [[Stinking Cloud (3-C-M-SCI)|Stinking Cloud]] (3) · [[Animate Dead (3-N-M-AD)|Animate Dead]] (3) · [[Beacon of Hope (3-A-L-BHA)|Beacon of Hope]] (3) · [[Mass Cure Wounds (5-C-L-MCW)|Mass Cure Wounds]] (5) · [[Mass Healing Word (3-V-L-MHW)|Mass Healing Word]] (3) · [[Remove Curse (3-A-L-RC)|Remove Curse]] (3) · [[Resurrection (7-N-L-RSR)|Resurrection]] (7).


---

## Tactical Assessment

A front-line resuscitation tool for combat medics.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
