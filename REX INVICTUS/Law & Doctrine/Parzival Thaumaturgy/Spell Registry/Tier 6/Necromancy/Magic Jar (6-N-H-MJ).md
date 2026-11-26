---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-6
  - spell/necromancy
  - source/srd
aliases:
  - "6th Tier Spell: Magic Jar"
  - "Magic Jar"
  - "6-N-H-MJ"
registry_id: 6-N-H-MJ
attribute_code: "6·Nec·None·None·Self·Until dispelled"
incantation: "Rouporis"
tier: 6
school: Necromancy
affinity: N
grade: H
pz_total: 31860.5
pz_quantum: 51944.6
t_e: 5.51
updated: 2026-11-16
---

**Magic Jar** (`6-N-H-MJ`) is a 6th Tier working of the [[Necromancy (School)|Necromancy]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **31,860 Pz** against a slot quantum of 51,945 Pz, which puts its energy-equivalent tier at T_E 5.51 and its handling grade at **High**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 6 Workings]]
      - [[Necromancy (School)|Necromancy]]
        - **Magic Jar** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `6-N-H-MJ` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `6·Nec·None·None·Self·Until dispelled` |
| Incantation | *Rouporis* |
| Affinity | N (Necromancy) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 6th Tier |
| School | [[Necromancy (School)\|Necromancy]] |
| Casting time | 1 minute |
| Range | Self |
| Area | single point or target |
| Duration | Until dispelled |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A gem, crystal, reliquary, or some other ornamental container worth at least 500 gp |
| Ritual | no |
| Resistance check | presence; on success: other |
| Practitioner lineages | Wizard |

### Mechanism

The field moves the caster's soul into a prepared container and from there into a nearby humanoid host, parking the host's soul in the container. Destroying the container or the host can kill either party.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Soul transfer into container (soul-work constant) | `1e4 Pz * (6 - 3)` | 30,000 |
| Possession swap (instant info) | `instant info = 1 Pz` | 1.0 |
| Host body control, 24 h reference horizon (upkeep) | `0.005 Pz/s * 86400 s` | 432 |
| Pattern cost | `0.01 × Q6 × (1 + 1.75)` | 1,428 |

| Quantity | Value |
|---|---|
| Effect energy | 30,000 Pz |
| Upkeep energy | 432 Pz (0.005 Pz/s) |
| **Total draw** | **31,860 Pz** (47,790.7 kJ) |
| Slot quantum Q6 | 51,945 Pz |
| Field gain (draw / quantum) | 0.613 |
| Energy-equivalent tier T_E | 5.51 |
| Handling points | 1.75 |
| Grade score | 1.51 → H |

**Handling flags:** costly material, consumed material, fragile, long cast.

**Assumptions:** One soul re-anchoring at 3 tiers above 3; possession held over a 24 h reference horizon; container lost when the effect ends.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Magic Jar (6-N-H-MJ) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 6 | 6 | `0000000001101` |
| k2 School | Necromancy | 6 | `0000000001101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Until dispelled | 11 | `0000000010111` |

### Incantation

Spoken as **Rouporis** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T7: *Mirouporis* · T8: *Nirouporis* · T9: *Xyirouporis*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 3→2 | 3 |
| k2 School | 0→11 2→0 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 2→9 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#0096fc`.

![[Magic Jar (6-N-H-MJ) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 6 | 0.600 | 1.000 | `#00ebff` (520 nm eq.) | source grid |
| School | Necromancy | 0.750 | 0.989 | `#0017ff` (475 nm eq.) | source grid |
| Duration | Until dispelled | 0.579 | 1.000 | `#00fff7` (526 nm eq.) | source grid |
| Range | Self | 0.706 | 0.994 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.19): swatch `#29d5dc`, measured lines at 0.580, 0.600, 0.706, 0.751. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.50. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `6·N·None`; the k4 to k6 lines (None, Self, Until dispelled) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `6·N·None` |
| Standard spectrometer detection range | 17.85 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 2,597 Pz (0.05 × Q6) |
| Counter drawn cold (all six layers) | 5,194 Pz (0.10 × Q6) |
| Unravel after completion | 5,281 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Dark, 2x Death. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1D 1F 1J` (Within, Death, Potential, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 5,310 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 6th Tier quantum of 51,945 Pz (61.3% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Endures independently once set, which places it under the decay clause of ULMTU-XIII. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIII]] | Lex Impermanentiae | Long-lived patterns drift toward reversion unless refreshed from a source that satisfies ULMTU-I. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 6th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Necromancy school with aspect lean Within, Dark, 2x Death. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 6 Workings]] |
| School | [[Necromancy (School)\|Necromancy]] |
| Affinity | [[Necromancy (School)\|Necromancy]] (N) |
| Function | [[Transformation]], [[Necromantic and Soul Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|High]] |

Similar workings: [[Circle of Death (6-N-L-CD)|Circle of Death]] (6) · [[Create Undead (6-N-L-CU)|Create Undead]] (6) · [[Harm (6-N-L-HRM)|Harm]] (6) · [[Contagion (5-N-L-CNTT)|Contagion]] (5) · [[Finger of Death (7-N-L-FDN)|Finger of Death]] (7) · [[Raise Dead (5-N-M-RD)|Raise Dead]] (5) · [[Resurrection (7-N-L-RSR)|Resurrection]] (7) · [[Blight (4-N-L-BLG)|Blight]] (4).


---

## Tactical Assessment

Enables covert takeover of a guard, officer or courier for infiltration. The caster's own body lies helpless meanwhile and the 100 ft tether limits range.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 6 Workings]] · [[Necromancy (School)|Necromancy]] · [[Spell Breakdown Procedure]] · [[Parzival]]
