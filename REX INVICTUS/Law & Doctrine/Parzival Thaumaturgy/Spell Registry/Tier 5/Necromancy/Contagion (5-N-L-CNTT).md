---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/necromancy
  - source/srd
aliases:
  - "5th Tier Spell: Contagion"
  - "Contagion"
  - "5-N-L-CNTT"
registry_id: 5-N-L-CNTT
attribute_code: "5·Nec·None·None·Touch·7 days"
incantation: "Toulixei"
tier: 5
school: Necromancy
affinity: N
grade: L
pz_total: 240.1
pz_quantum: 19109.4
t_e: 0.62
updated: 2026-11-16
---

**Contagion** (`5-N-L-CNTT`) is a 5th Tier working of the [[Necromancy (School)|Necromancy]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **240 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 0.62 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Necromancy (School)|Necromancy]]
        - **Contagion** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-N-L-CNTT` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Nec·None·None·Touch·7 days` |
| Incantation | *Toulixei* |
| Affinity | N (Necromancy) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Necromancy (School)\|Necromancy]] |
| Casting time | 1 action |
| Range | Touch |
| Area | single point or target |
| Duration | 7 days |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Resistance check | constitution; on success: other |
| Delivery | aimed melee working |
| Practitioner lineages | Cleric, Druid |

### Mechanism

A touch implants and accelerates a disease agent until the body either clears it or the illness locks in for a week. Once established it runs as an ordinary disease and needs no further field support.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| pathogen seed (living matter 10 g) | `10*0.01` | 0.1 |
| systemic onset drive, 10 injury-equivalent necrotic by touch | `10*0.20*0.5` | 1.0 |
| upkeep: enchantment-class coupling over 3 rounds of onset | `0.005*1*18` | 0.09 |
| Pattern cost | `0.01 × Q5 × (1 + 0.25)` | 239 |

| Quantity | Value |
|---|---|
| Effect energy | 1.1 Pz |
| Upkeep energy | 0.09 Pz (0.005 Pz/s) |
| **Total draw** | **240 Pz** (360.1 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 0.0126 |
| Energy-equivalent tier T_E | 0.62 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** save or suck.

**Assumptions:** Pathogen mass 10 g; onset drive modeled as 10 HP-equivalent necrotic with touch F=0.5; 18 s of field coupling; afterward the disease is self-running.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Contagion (5-N-L-CNTT) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Necromancy | 6 | `0000000001101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | 7 days | 7 | `0000000001111` |

### Incantation

Spoken as **Toulixei** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Ritoulixei* · T7: *Mitoulixei* · T8: *Nitoulixei* · T9: *Xyitoulixei*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 2→0 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 2→9 3→10 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#2488a6`.

![[Contagion (5-N-L-CNTT) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| School | Necromancy | 0.750 | 0.969 | `#0017ff` (475 nm eq.) | source grid |
| Duration | 7 days | 0.421 | 0.997 | `#00ff1a` (574 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.930 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.15): swatch `#4dc6d1`, measured lines at 0.422, 0.501, 0.751, 0.883. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.38. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·N·None`; the k4 to k6 lines (None, Touch, 7 days) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·N·None` |
| Standard spectrometer detection range | 1.55 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 1,911 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Dark, 2x Death. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1D 1F 1J` (Within, Death, Potential, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 40.0 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 5th Tier quantum of 19,109 Pz (1.3% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Endures independently once set, which places it under the decay clause of ULMTU-XIII. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIII]] | Lex Impermanentiae | Long-lived patterns drift toward reversion unless refreshed from a source that satisfies ULMTU-I. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 5th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Necromancy school with aspect lean Within, Dark, 2x Death. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 5 Workings]] |
| School | [[Necromancy (School)\|Necromancy]] |
| Affinity | [[Necromancy (School)\|Necromancy]] (N) |
| Function | [[Necromantic and Soul Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Raise Dead (5-N-M-RD)|Raise Dead]] (5) · [[Blight (4-N-L-BLG)|Blight]] (4) · [[Circle of Death (6-N-L-CD)|Circle of Death]] (6) · [[Create Undead (6-N-L-CU)|Create Undead]] (6) · [[Harm (6-N-L-HRM)|Harm]] (6) · [[Magic Jar (6-N-H-MJ)|Magic Jar]] (6) · [[Animate Dead (3-N-M-AD)|Animate Dead]] (3) · [[Antilife Shell (5-A-L-ASI)|Antilife Shell]] (5).


---

## Tactical Assessment

A delayed incapacitation tool for assassination, interrogation or denying a key individual; the slow onset makes it poor for immediate battlefield effect.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Necromancy (School)|Necromancy]] · [[Spell Breakdown Procedure]] · [[Parzival]]
