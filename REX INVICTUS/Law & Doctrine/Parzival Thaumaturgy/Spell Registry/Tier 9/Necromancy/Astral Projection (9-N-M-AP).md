---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-9
  - spell/necromancy
  - source/srd
aliases:
  - "9th Tier Spell: Astral Projection"
  - "Astral Projection"
  - "9-N-M-AP"
registry_id: 9-N-M-AP
attribute_code: "9·Nec·None·None·10 feet·Special"
incantation: "Xyouspulyl"
tier: 9
school: Necromancy
affinity: N
grade: M
pz_total: 462995.7
pz_quantum: 1043335.3
t_e: 8.19
updated: 2026-11-16
---

**Astral Projection** (`9-N-M-AP`) is a 9th Tier working of the [[Necromancy (School)|Necromancy]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **462,996 Pz** against a slot quantum of 1.04 MPz Pz, which puts its energy-equivalent tier at T_E 8.19 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 9 Workings]]
      - [[Necromancy (School)|Necromancy]]
        - **Astral Projection** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `9-N-M-AP` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `9·Nec·None·None·10 feet·Special` |
| Incantation | *Xyouspulyl* |
| Affinity | N (Necromancy) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 9th Tier |
| School | [[Necromancy (School)\|Necromancy]] |
| Casting time | 1 hour |
| Range | 10 feet |
| Area | single point or target |
| Duration | Special |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: For each creature you affect with this spell, you must provide one jacinth worth at least 1,000gp and one ornately carved bar of silver worth at least 100gp, all of which the spell consumes |
| Ritual | no |
| Practitioner lineages | Cleric, Warlock, Wizard |

### Mechanism

The caster and up to eight companions shift their minds into the astral domain, leaving bodies in suspended animation tethered by a cord that carries them to any new plane entered.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| astral departure | `0.01 * 80 kg * 15 m/s^2 * 1e+06 m / 1500 * 9` | 72,000 |
| return transport along tether | `0.01 * 80 kg * 15 m/s^2 * 1e+06 m / 1500 * 9` | 72,000 |
| suspended animation of bodies | `9 bodies * 80 W * 604800 s / 1500` | 290,304 |
| Pattern cost | `0.01 × Q9 × (1 + 1.75)` | 28,692 |

| Quantity | Value |
|---|---|
| Effect energy | 144,000 Pz |
| Upkeep energy | 290,304 Pz (0.48 Pz/s) |
| **Total draw** | **462,996 Pz** (694,493.6 kJ) |
| Slot quantum Q9 | 1.04 MPz Pz |
| Field gain (draw / quantum) | 0.444 |
| Energy-equivalent tier T_E | 8.19 |
| Handling points | 1.75 |
| Grade score | 1.34 → M |

**Handling flags:** costly material, consumed material, fragile, long cast.

**Assumptions:** 9 travellers at 80 kg; one boundary each way; bodies held at 80 W each for an assumed 7 days.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Astral Projection (9-N-M-AP) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 9 | 9 | `0000000010011` |
| k2 School | Necromancy | 6 | `0000000001101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 10 feet | 1 | `0000000000011` |
| k6 Duration | Special | 10 | `0000000010101` |

### Incantation

Spoken as **Xyouspulyl** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 4→3 | 3 |
| k2 School | 0→11 2→0 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 | 2 |
| k6 Duration | 0→7 2→9 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#634fb8`.

![[Astral Projection (9-N-M-AP) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 9 | 0.900 | 1.000 | `#b600ff` (430 nm eq.) | source grid |
| School | Necromancy | 0.750 | 0.989 | `#0017ff` (475 nm eq.) | source grid |
| Duration | Special | 0.526 | 0.933 | `#00ffac` (542 nm eq.) | source grid |
| Range | 10 feet | 0.059 | 0.702 | `#ff2700` (682 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.13): swatch `#4b8dcf`, measured lines at 0.060, 0.527, 0.751, 0.901. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 5.67. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `9·N·None`; the k4 to k6 lines (None, 10 feet, Special) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `9·N·None` |
| Standard spectrometer detection range | 68.04 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 52,167 Pz (0.05 × Q9) |
| Counter drawn cold (all six layers) | 104,334 Pz (0.10 × Q9) |
| Unravel after completion | 162,394 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Dark, 2x Death. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1D 1F 1J` (Within, Death, Potential, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 77,166 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 9th Tier quantum of 1.04 MPz Pz (44.4% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Endures independently once set, which places it under the decay clause of ULMTU-XIII. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIII]] | Lex Impermanentiae | Long-lived patterns drift toward reversion unless refreshed from a source that satisfies ULMTU-I. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 9th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Necromancy school with aspect lean Within, Dark, 2x Death. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 9 Workings]] |
| School | [[Necromancy (School)\|Necromancy]] |
| Affinity | [[Necromancy (School)\|Necromancy]] (N) |
| Function | [[Teleportation and Planar Travel]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Gate (9-C-L-GAT)|Gate]] (9) · [[Imprisonment (9-A-L-IMP)|Imprisonment]] (9) · [[Wish (9-C-L-WSH)|Wish]] (9) · [[Demiplane (8-C-L-DMP)|Demiplane]] (8) · [[Maze (8-C-L-MAZ)|Maze]] (8) · [[Dream of the Blue Veil (7-C-M-DBV)|Dream of the Blue Veil]] (7) · [[Etherealness (7-T-L-ETH)|Etherealness]] (7) · [[Magnificent Mansion (7-C-M-MMN)|Magnificent Mansion]] (7).


---

## Tactical Assessment

Long-range planar reconnaissance with low risk to the physical body, and a route into other planes for small teams.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 9 Workings]] · [[Necromancy (School)|Necromancy]] · [[Spell Breakdown Procedure]] · [[Parzival]]
