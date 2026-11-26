---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/conjuration
  - source/srd
aliases:
  - "5th Tier Spell: Mass Cure Wounds"
  - "Mass Cure Wounds"
  - "5-C-L-MCW"
registry_id: 5-C-L-MCW
attribute_code: "5·Con·None·sphere (30)·60 feet·Instantaneous"
incantation: "Te’-Sorwyn"
tier: 5
school: Conjuration
affinity: C
grade: L
pz_total: 220.8
pz_quantum: 19109.4
t_e: 0.54
updated: 2026-11-16
---

**Mass Cure Wounds** (`5-C-L-MCW`) is a 5th Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **221 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 0.54 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Conjuration]]
        - **Mass Cure Wounds** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-C-L-MCW` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Con·None·sphere (30)·60 feet·Instantaneous` |
| Incantation | *Te’-Sorwyn* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | sphere (30) |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Restoration | 3d8 + MOD restored (mean 16.5, modifier taken as +3) |
| Practitioner lineages | Bard, Cleric, Druid |

### Mechanism

A pulse of restorative energy from a chosen point repairs injuries in up to six creatures within a 30 ft radius. It has no effect on the undead or constructs.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Healing, 6 targets | `6 * (13.5 + 3) HP * 0.30` | 29.7 |
| Pattern cost | `0.01 × Q5 × (1 + 0.00)` | 191 |

| Quantity | Value |
|---|---|
| Effect energy | 29.7 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **221 Pz** (331.2 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 0.0116 |
| Energy-equivalent tier T_E | 0.54 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** 3d8 = 13.5 plus an ability bonus of 3 per target; six targets.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Mass Cure Wounds (5-C-L-MCW) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (30) | 31 | `0000000111111` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Te’-Sorwyn** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Rite’-Sorwyn* · T7: *Mite’-Sorwyn* · T8: *Nite’-Sorwyn* · T9: *Xyite’-Sorwyn*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 2→11 3→12 4→0 5→1 | 6 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#7a848c`.

![[Mass Cure Wounds (5-C-L-MCW) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.932 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.882 | `#ff0028` (700 nm eq.) | source grid |
| Area | sphere (30) | 0.861 | 0.937 | `#8000ff` (442 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.996 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.20): swatch `#a9a581`, measured lines at 0.004, 0.126, 0.501, 0.589, 0.862. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.34. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·C·None`; the k4 to k6 lines (sphere (30), 60 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·C·None` |
| Standard spectrometer detection range | 1.49 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 1,911 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 36.8 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 5th Tier quantum of 19,109 Pz (1.2% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 5th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 5 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Healing and Restoration]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Heroes' Feast (6-C-L-HF)|Heroes' Feast]] (6) · [[Greater Restoration (5-A-L-GRE)|Greater Restoration]] (5) · [[Raise Dead (5-N-M-RD)|Raise Dead]] (5) · [[Reincarnate (5-T-M-RNC)|Reincarnate]] (5) · [[Revivify (3-C-L-RVV)|Revivify]] (3) · [[Stinking Cloud (3-C-M-SCI)|Stinking Cloud]] (3) · [[Heal (6-V-L-HEA)|Heal]] (6) · [[Cloudkill (5-C-L-CLD)|Cloudkill]] (5).


---

## Tactical Assessment

A casualty-clearing tool for a squad after an engagement or a blast. Wounded must be grouped together.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
