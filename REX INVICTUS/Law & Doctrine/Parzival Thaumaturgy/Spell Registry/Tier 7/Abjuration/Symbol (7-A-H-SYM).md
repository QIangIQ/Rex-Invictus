---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-7
  - spell/abjuration
  - source/srd
aliases:
  - "7th Tier Spell: Symbol"
  - "Symbol"
  - "7-A-H-SYM"
registry_id: 7-A-H-SYM
attribute_code: "7·Abj·None·cube (10)·Touch·Until dispelled"
incantation: "Ma’-Belixis"
tier: 7
school: Abjuration
affinity: A
grade: H
pz_total: 202426.0
pz_quantum: 141200.1
t_e: 7.36
updated: 2026-11-16
---

**Symbol** (`7-A-H-SYM`) is a 7th Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **202,426 Pz** against a slot quantum of 141,200 Pz, which puts its energy-equivalent tier at T_E 7.36 and its handling grade at **High**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 7 Workings]]
      - [[Abjuration]]
        - **Symbol** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `7-A-H-SYM` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `7·Abj·None·cube (10)·Touch·Until dispelled` |
| Incantation | *Ma’-Belixis* |
| Affinity | A (Abjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 7th Tier |
| School | [[Abjuration]] |
| Casting time | 1 minute |
| Range | Touch |
| Area | cube (10) |
| Duration | Until dispelled |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Mercury, phosphorus, and powdered diamond and opal with a total value of at least 1,000 gp, which the spell consumes |
| Ritual | no |
| Practitioner lineages | Bard, Cleric, Wizard |

### Mechanism

A near-invisible glyph lies dormant on a surface or inside an object until its trigger condition is met, then fills an 18 m sphere with one chosen effect for ten minutes.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Death glyph, 3 triggers | `55 HP * 0.20 * 4203 m^2 / 0.7 * 3` | 198,100 |
| Upkeep: Dim glow 60 ft for 10 min | `100 W * (60/20)^2 * 0.25 * 600 s / 1500` | 90.0 |
| Pattern cost | `0.01 × Q7 × (1 + 2.00)` | 4,236 |

| Quantity | Value |
|---|---|
| Effect energy | 198,100 Pz |
| Upkeep energy | 90.0 Pz (0.15 Pz/s) |
| **Total draw** | **202,426 Pz** (303,639.0 kJ) |
| Slot quantum Q7 | 141,200 Pz |
| Field gain (draw / quantum) | 1.43 |
| Energy-equivalent tier T_E | 7.36 |
| Handling points | 2.00 |
| Grade score | 2.18 → H |

**Handling flags:** costly material, consumed material, fragile, save or suck, long cast.

**Assumptions:** Death option modeled (10d10 = 55); dormant period treated as passive storage at zero power; 3 triggers.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Symbol (7-A-H-SYM) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 7 | 7 | `0000000001111` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | cube (10) | 5 | `0000000001011` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Until dispelled | 11 | `0000000010111` |

### Incantation

Spoken as **Ma’-Belixis** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T8: *Nima’-Belixis* · T9: *Xyima’-Belixis*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 3→2 | 4 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 3→12 | 3 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 2→9 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#7b66a9`.

![[Symbol (7-A-H-SYM) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 7 | 0.700 | 1.000 | `#005eff` (490 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.783 | `#ff0028` (700 nm eq.) | source grid |
| Duration | Until dispelled | 0.579 | 0.993 | `#00fff7` (526 nm eq.) | source grid |
| Area | cube (10) | 0.139 | 0.854 | `#ff9300` (658 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.984 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.23): swatch `#6892ae`, measured lines at 0.007, 0.140, 0.579, 0.701, 0.883. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 5.31. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `7·A·None`; the k4 to k6 lines (cube (10), Touch, Until dispelled) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `7·A·None` |
| Standard spectrometer detection range | 44.99 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 7,060 Pz (0.05 × Q7) |
| Counter drawn cold (all six layers) | 14,120 Pz (0.10 × Q7) |
| Unravel after completion | 14,138 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 33,738 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 1.43 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 7th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Endures independently once set, which places it under the decay clause of ULMTU-XIII. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIII]] | Lex Impermanentiae | Long-lived patterns drift toward reversion unless refreshed from a source that satisfies ULMTU-I. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 7th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 7 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Linking and Triggers]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|High]] |

Similar workings: [[Delayed Blast Fireball (7-V-M-DBF)|Delayed Blast Fireball]] (7) · [[Contingency (6-V-L-CNTI)|Contingency]] (6) · [[Programmed Illusion (6-I-L-PI)|Programmed Illusion]] (6) · [[Glyph of Warding (3-A-H-GWY)|Glyph of Warding]] (3) · [[Telepathic Bond (5-D-L-TB)|Telepathic Bond]] (5) · [[Antimagic Field (8-A-L-AFT)|Antimagic Field]] (8) · [[Forbiddance (6-A-L-FRBB)|Forbiddance]] (6) · [[Globe of Invulnerability (6-A-L-GIO)|Globe of Invulnerability]] (6).


---

## Tactical Assessment

A long-duration trap for vaults, archives and choke points, with selective triggers that spare authorised personnel.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 7 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
