---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/necromancy
  - source/srd
aliases:
  - "2nd Tier Spell: Gentle Repose"
  - "Gentle Repose"
  - "2-N-H-GR"
registry_id: 2-N-H-GR
attribute_code: "2·Nec·None·None·Touch·10 days"
incantation: "Houlixy"
tier: 2
school: Necromancy
affinity: N
grade: H
pz_total: 4341.4
pz_quantum: 951.4
t_e: 3.52
updated: 2026-11-16
---

**Gentle Repose** (`2-N-H-GR`) is a 2nd Tier working of the [[Necromancy (School)|Necromancy]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **4,341 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E 3.52 and its handling grade at **High**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Necromancy (School)|Necromancy]]
        - **Gentle Repose** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-N-H-GR` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Nec·None·None·Touch·10 days` |
| Incantation | *Houlixy* |
| Affinity | N (Necromancy) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Necromancy (School)\|Necromancy]] |
| Casting time | 1 action |
| Range | Touch |
| Area | single point or target |
| Duration | 10 days |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A pinch of salt and one copper piece placed on each of the corpse's eyes, which must remain there for the duration |
| Ritual | yes |
| Practitioner lineages | Cleric, Wizard |

### Mechanism

Locks a corpse's biochemistry so it does not decay and cannot be animated, and stops the clock on later revival.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| biochemical stasis on remains | `0.005 Pz/s = 0.005 Pz/s * 864000 s` | 4,320 |
| Pattern cost | `0.01 × Q2 × (1 + 1.25)` | 21.4 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 4,320 Pz (0.005 Pz/s) |
| **Total draw** | **4,341 Pz** (6,512.1 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 4.56 |
| Energy-equivalent tier T_E | 3.52 |
| Handling points | 1.25 |
| Grade score | 2.01 → H |

**Handling flags:** ritual, fragile.

**Assumptions:** 10 days at enchantment rate on one body; a refrigeration equivalent (288 W heat leak) would cost about 1.7e5 Pz and is not used.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Gentle Repose (2-N-H-GR) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Necromancy | 6 | `0000000001101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | 10 days | 3 | `0000000000111` |

### Incantation

Spoken as **Houlixy** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihoulixy* · T4: *Vihoulixy* · T5: *Tihoulixy* · T6: *Rihoulixy* · T7: *Mihoulixy* · T8: *Nihoulixy* · T9: *Xyihoulixy*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 2→0 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 2→9 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#ad8873`.

![[Gentle Repose (2-N-H-GR) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Necromancy | 0.750 | 0.860 | `#0017ff` (475 nm eq.) | source grid |
| Duration | 10 days | 0.211 | 1.000 | `#fff500` (637 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.792 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.17): swatch `#8998a1`, measured lines at 0.204, 0.751, 0.883. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.64. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·N·None`; the k4 to k6 lines (None, Touch, 10 days) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·N·None` |
| Standard spectrometer detection range | 6.59 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 959 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Dark, 2x Death. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1D 1F 1J` (Within, Death, Potential, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 724 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 4.56 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 2nd Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Endures independently once set, which places it under the decay clause of ULMTU-XIII. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIII]] | Lex Impermanentiae | Long-lived patterns drift toward reversion unless refreshed from a source that satisfies ULMTU-I. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Necromancy school with aspect lean Within, Dark, 2x Death. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Necromancy (School)\|Necromancy]] |
| Affinity | [[Necromancy (School)\|Necromancy]] (N) |
| Function | [[Necromantic and Soul Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|High]] |

Similar workings: [[Animate Dead (3-N-M-AD)|Animate Dead]] (3) · [[Inflict Wounds (1-N-L-IW)|Inflict Wounds]] (1) · [[Speak with Dead (3-N-L-SDE)|Speak with Dead]] (3) · [[Vampiric Touch (3-N-L-VT)|Vampiric Touch]] (3) · [[Blight (4-N-L-BLG)|Blight]] (4) · [[Chill Touch (0-N-L-CT)|Chill Touch]] (0) · [[Beacon of Hope (3-A-L-BHA)|Beacon of Hope]] (3) · [[Charm Person (1-E-L-CP)|Charm Person]] (1).


---

## Tactical Assessment

Preserves fallen personnel for later revival or for intelligence and forensic work, and denies the bodies to enemy necromancers.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Necromancy (School)|Necromancy]] · [[Spell Breakdown Procedure]] · [[Parzival]]
