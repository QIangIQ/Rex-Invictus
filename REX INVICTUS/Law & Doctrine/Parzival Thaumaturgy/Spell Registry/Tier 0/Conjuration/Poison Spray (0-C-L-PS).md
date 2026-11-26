---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-0
  - spell/conjuration
  - source/srd
aliases:
  - "Cantrip Spell: Poison Spray"
  - "Poison Spray"
  - "0-C-L-PS"
registry_id: 0-C-L-PS
attribute_code: "0·Con·Poison·None·10 feet·Instantaneous"
incantation: "Cenis-’spul"
tier: 0
school: Conjuration
affinity: C
grade: L
pz_total: 1.5
pz_quantum: 128.8
t_e: -4.48
updated: 2026-11-16
---

**Poison Spray** (`0-C-L-PS`) is a Cantrip (Tier 0) working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **1.5 Pz** against a slot quantum of 129 Pz, which puts its energy-equivalent tier at T_E -4.48 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 0 Workings]]
      - [[Conjuration]]
        - **Poison Spray** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `0-C-L-PS` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `0·Con·Poison·None·10 feet·Instantaneous` |
| Incantation | *Cenis-’spul* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | Cantrip (Tier 0) |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | 10 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 1d12 poison (mean 6.5) |
| Injury by caster maturity bands | T1: 1d12, T5: 2d12, T11: 3d12, T17: 4d12 |
| Resistance check | constitution; on success: no effect |
| Practitioner lineages | Sorcerer, Warlock, Wizard, Druid |

### Mechanism

The palm vents a short burst of conjured toxic aerosol at a single nearby target.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| 1d12 poison (6.5) directed at one target | `6.5*0.05*0.5` | 0.163 |
| toxic gas puff, 0.01 kg inert-fluid matter | `1*0.01` | 0.01 |
| Pattern cost | `0.01 × Q0 × (1 + 0.00)` | 1.3 |

| Quantity | Value |
|---|---|
| Effect energy | 0.172 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **1.5 Pz** (2.2 kJ) |
| Slot quantum Q0 | 129 Pz |
| Field gain (draw / quantum) | 0.0113 |
| Energy-equivalent tier T_E | -4.48 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Base 1d12 average 6.5; directed delivery F 0.5; gas mass 10 g.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Poison Spray (0-C-L-PS) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 0 | 0 | `0000000000001` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | Poison | 9 | `0000000010011` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 10 feet | 1 | `0000000000011` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Cenis-’spul** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T1: *Sicenis-’spul* · T2: *Hicenis-’spul* · T3: *Licenis-’spul* · T4: *Vicenis-’spul* · T5: *Ticenis-’spul* · T6: *Ricenis-’spul* · T7: *Micenis-’spul* · T8: *Nicenis-’spul* · T9: *Xyicenis-’spul*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 | 1 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 4→1 | 3 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 | 2 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#d3403b`.

![[Poison Spray (0-C-L-PS) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 0 | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| Damage | Poison | 0.643 | 0.813 | `#00afff` (507 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.992 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| Range | 10 feet | 0.059 | 0.998 | `#ff2700` (682 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.21): swatch `#db563d`, measured lines at 0.005, 0.059, 0.126, 0.643. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 0.16. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `0·C·Poison`; the k4 to k6 lines (None, 10 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `0·C·Poison` |
| Standard spectrometer detection range | 0.12 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 6.4 Pz (0.05 × Q0) |
| Counter drawn cold (all six layers) | 12.9 Pz (0.10 × Q0) |
| Unravel after completion | 12.9 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Within, Cold, Death, Diminutive and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1B 1D 1F 1j` (Cold, Death, Potential, Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 0.243 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the Cantrip (Tier 0) quantum of 129 Pz (1.1% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at Cantrip (Tier 0) up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 0 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Precision Strikes]] |
| Element | [[Poison Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Radiation Poisoning (0-V-L-RP)|Radiation Poisoning]] (0) · [[Acid Splash (0-C-L-AS)|Acid Splash]] (0) · [[Produce Flame (0-C-L-PF)|Produce Flame]] (0) · [[Chill Touch (0-N-L-CT)|Chill Touch]] (0) · [[Eldritch Blast (0-P-L-EB)|Eldritch Blast]] (0) · [[Fire Bolt (0-V-L-FB)|Fire Bolt]] (0) · [[Flaming Sphere (2-C-L-FSA)|Flaming Sphere]] (2) · [[Ray of Frost (0-V-L-RF)|Ray of Frost]] (0).


---

## Tactical Assessment

A close-range irritant with negligible effect on protected or sealed troops.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 0 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
