---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-6
  - spell/evocation
  - source/srd
aliases:
  - "6th Tier Spell: Contingency"
  - "Contingency"
  - "6-V-L-CNTI"
registry_id: 6-V-L-CNTI
attribute_code: "6·Evo·None·None·Self·10 days"
incantation: "Rupory"
tier: 6
school: Evocation
affinity: V
grade: L
pz_total: 1490.7
pz_quantum: 51944.6
t_e: 2.45
updated: 2026-11-16
---

**Contingency** (`6-V-L-CNTI`) is a 6th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **1,491 Pz** against a slot quantum of 51,945 Pz, which puts its energy-equivalent tier at T_E 2.45 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 6 Workings]]
      - [[Evocation]]
        - **Contingency** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `6-V-L-CNTI` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `6·Evo·None·None·Self·10 days` |
| Incantation | *Rupory* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 6th Tier |
| School | [[Evocation]] |
| Casting time | 10 minutes |
| Range | Self |
| Area | single point or target |
| Duration | 10 days |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A statuette of yourself carved from ivory and decorated with gems worth at least 1,500 gp |
| Ritual | no |
| Practitioner lineages | Wizard |

### Mechanism

The caster seals a second working into a dormant pattern anchored to a carved statuette, with a sensing clause that releases it when a stated condition occurs. The stored working draws its own energy at casting.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| trigger sensor and release (instant info) | `1` | 1.0 |
| upkeep: stored-pattern leakage, 1% of Q5 over 10 days | `0.01*Q(5)` | 191 |
| Pattern cost | `0.01 × Q6 × (1 + 1.50)` | 1,299 |

| Quantity | Value |
|---|---|
| Effect energy | 1.0 Pz |
| Upkeep energy | 191 Pz (0.000221 Pz/s) |
| **Total draw** | **1,491 Pz** (2,236.1 kJ) |
| Slot quantum Q6 | 51,945 Pz |
| Field gain (draw / quantum) | 0.0287 |
| Energy-equivalent tier T_E | 2.45 |
| Handling points | 1.50 |
| Grade score | 0.50 → L |

**Handling flags:** costly material, fragile, long cast.

**Assumptions:** Contingent working is paid separately; storage leakage taken as 1% of Q5 over 864000 s; release sensor 1 Pz.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Contingency (6-V-L-CNTI) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 6 | 6 | `0000000001101` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | 10 days | 3 | `0000000000111` |

### Incantation

Spoken as **Rupory** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T7: *Mirupory* · T8: *Nirupory* · T9: *Xyirupory*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 3→2 | 3 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 2→9 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#3ccda5`.

![[Contingency (6-V-L-CNTI) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 6 | 0.600 | 1.000 | `#00ebff` (520 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.995 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | 10 days | 0.211 | 0.927 | `#fff500` (637 nm eq.) | source grid |
| Range | Self | 0.706 | 0.994 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.15): swatch `#70e4b7`, measured lines at 0.211, 0.501, 0.601, 0.706. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.17. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `6·V·None`; the k4 to k6 lines (None, Self, 10 days) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `6·V·None` |
| Standard spectrometer detection range | 3.86 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 2,597 Pz (0.05 × Q6) |
| Counter drawn cold (all six layers) | 5,194 Pz (0.10 × Q6) |
| Unravel after completion | 5,233 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1b 1c 1d 1f` (Heat, Light, Life, Energy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 248 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 6th Tier quantum of 51,945 Pz (2.9% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Endures independently once set, which places it under the decay clause of ULMTU-XIII. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIII]] | Lex Impermanentiae | Long-lived patterns drift toward reversion unless refreshed from a source that satisfies ULMTU-I. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 6th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 6 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Linking and Triggers]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Delayed Blast Fireball (7-V-M-DBF)|Delayed Blast Fireball]] (7) · [[Programmed Illusion (6-I-L-PI)|Programmed Illusion]] (6) · [[Symbol (7-A-H-SYM)|Symbol]] (7) · [[Telepathic Bond (5-D-L-TB)|Telepathic Bond]] (5) · [[Absolute Zero (6-V-L-AZ)|Absolute Zero]] (6) · [[Blade Barrier (6-V-L-BB)|Blade Barrier]] (6) · [[Burst Radiation (6-V-L-BR)|Burst Radiation]] (6) · [[Chain Lightning (6-V-L-CLA)|Chain Lightning]] (6).


---

## Tactical Assessment

Provides automatic emergency responses such as a protective or escape working that fires on a set condition, which suits pilots, couriers and high-value personnel.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 6 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
