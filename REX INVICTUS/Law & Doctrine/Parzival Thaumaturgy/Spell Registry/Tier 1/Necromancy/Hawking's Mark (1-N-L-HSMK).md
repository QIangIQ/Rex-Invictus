---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/necromancy
  - source/science-spellbook
aliases:
  - "1st Tier Spell: Hawking's Mark"
  - "1-N-L-HSMK"
  - "Hawking's Mark (Science)"
registry_id: 1-N-L-HSMK
attribute_code: "1·Nec·None·None·30 feet·Until dispelled"
incantation: "Souusinis"
tier: 1
school: Necromancy
affinity: N
grade: L
pz_total: 4.7
pz_quantum: 350.0
t_e: -3.31
updated: 2026-11-16
---

**Hawking's Mark** (`1-N-L-HSMK`) is a 1st Tier working of the [[Necromancy (School)|Necromancy]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **4.7 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -3.31 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Necromancy (School)|Necromancy]]
        - **Hawking's Mark** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-N-L-HSMK` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Nec·None·None·30 feet·Until dispelled` |
| Incantation | *Souusinis* |
| Affinity | N (Necromancy) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Necromancy (School)\|Necromancy]] |
| Casting time | 1 Action |
| Range | 30 feet |
| Area | single point or target |
| Duration | Until dispelled |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 1 untyped (mean 0) |
| Injury by tier | T1: 1, T2: 1, T3: 1, T4: 1, T5: 1, T6: 1, T7: 1, T8: 1, T9: 1 |
| Resistance check | constitution; on success: no effect |
| Practitioner lineages | Wizard, Sorcerer, Cleric |

### Mechanism

Sets a slow siphon on a target that bleeds a sliver of vitality to the caster each round until it shakes the mark off.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Vitality drained | `1 HP x 0.2 (necrotic) x F 0.5 x 3 triggers` | 0.3 |
| Vitality returned to caster | `1 x 0.30 Pz x 3 rounds` | 0.9 |
| Pattern cost | `0.01 × Q1 × (1 + 0.00)` | 3.5 |

| Quantity | Value |
|---|---|
| Effect energy | 1.2 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **4.7 Pz** (7.1 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.0134 |
| Energy-equivalent tier T_E | -3.31 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** 1 unit of injury per round drained, necrotic rate with ray delivery F 0.5, and 1 unit healed to the caster at 0.30 Pz; 3 rounds expected before the target breaks free.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Hawking's Mark (1-N-L-HSMK) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Necromancy | 6 | `0000000001101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Until dispelled | 11 | `0000000010111` |

### Incantation

Spoken as **Souusinis** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisouusinis* · T3: *Lisouusinis* · T4: *Visouusinis* · T5: *Tisouusinis* · T6: *Risouusinis* · T7: *Misouusinis* · T8: *Nisouusinis* · T9: *Xyisouusinis*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 2→0 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 2→9 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#6ba073`.

![[Hawking's Mark (1-N-L-HSMK) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Necromancy | 0.750 | 0.810 | `#0017ff` (475 nm eq.) | source grid |
| Duration | Until dispelled | 0.579 | 0.892 | `#00fff7` (526 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.981 | `#91ff00` (612 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 0.67. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·N·None`; the k4 to k6 lines (None, 30 feet, Until dispelled) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·N·None` |
| Standard spectrometer detection range | 0.22 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.0 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Dark, 2x Death. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1D 1F 1J` (Within, Death, Potential, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 0.783 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (1.3% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Endures independently once set, which places it under the decay clause of ULMTU-XIII. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIII]] | Lex Impermanentiae | Long-lived patterns drift toward reversion unless refreshed from a source that satisfies ULMTU-I. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Necromancy school with aspect lean Within, Dark, 2x Death. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Necromancy (School)\|Necromancy]] |
| Affinity | [[Necromancy (School)\|Necromancy]] (N) |
| Function | [[Negation and Counterspell]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Blindness-Deafness (2-N-L-BD)|Blindness/Deafness]] (2) · [[Ray of Enfeeblement (2-N-L-RE)|Ray of Enfeeblement]] (2) · [[Hunter's Mark (1-D-L-HSM)|Hunter's Mark]] (1) · [[Mycelium Network (1-D-M-MN)|Mycelium Network]] (1) · [[Animal Messenger (2-E-L-AM)|Animal Messenger]] (2) · [[Arcane Die (0-C-L-ADC)|Arcane Die]] (0) · [[Arcane Lock (2-A-L-AL)|Arcane Lock]] (2) · [[Gust of Wind (2-V-M-GW)|Gust of Wind]] (2).


---

## Tactical Assessment

Attrition harassment that also sustains the caster; marginal in a firefight.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Necromancy (School)|Necromancy]] · [[Spell Breakdown Procedure]] · [[Parzival]]
