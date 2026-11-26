---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/evocation
  - source/srd
aliases:
  - "2nd Tier Spell: Continual Flame"
  - "Continual Flame"
  - "2-V-M-CF"
registry_id: 2-V-M-CF
attribute_code: "2·Evo·None·None·Touch·Until dispelled"
incantation: "Hulixis"
tier: 2
school: Evocation
affinity: V
grade: M
pz_total: 5774.4
pz_quantum: 951.4
t_e: 3.80
updated: 2026-11-16
---

**Continual Flame** (`2-V-M-CF`) is a 2nd Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **5,774 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E 3.80 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Evocation]]
        - **Continual Flame** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-V-M-CF` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Evo·None·None·Touch·Until dispelled` |
| Incantation | *Hulixis* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | Touch |
| Area | single point or target |
| Duration | Until dispelled |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Ruby dust worth 50 gp, which the spell consumes |
| Ritual | no |
| Practitioner lineages | Cleric, Wizard |

### Mechanism

The field produces a torch-bright flame on an object that gives no heat and consumes no oxygen. It can be covered and still persists until dismantled.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| cold-flame ignition | `0.1` | 0.1 |
| upkeep: torch-equivalent field light 100 W, 24 h reference window | `100*86400/J` | 5,760 |
| Pattern cost | `0.01 × Q2 × (1 + 0.50)` | 14.3 |

| Quantity | Value |
|---|---|
| Effect energy | 0.1 Pz |
| Upkeep energy | 5,760 Pz (0.0667 Pz/s) |
| **Total draw** | **5,774 Pz** (8,661.6 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 6.07 |
| Energy-equivalent tier T_E | 3.80 |
| Handling points | 0.50 |
| Grade score | 1.40 → M |

**Handling flags:** costly material, consumed material.

**Assumptions:** Duration is open-ended; upkeep shown for a 24 h reference window at 100 W (0.0667 Pz/s); consumed ruby dust and ambient return assumed to carry the long tail.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Continual Flame (2-V-M-CF) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Until dispelled | 11 | `0000000010111` |

### Incantation

Spoken as **Hulixis** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihulixis* · T4: *Vihulixis* · T5: *Tihulixis* · T6: *Rihulixis* · T7: *Mihulixis* · T8: *Nihulixis* · T9: *Xyihulixis*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 2→9 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#66c299`.

![[Continual Flame (2-V-M-CF) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.956 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Until dispelled | 0.579 | 0.931 | `#00fff7` (526 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.792 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.15): swatch `#99c4a2`, measured lines at 0.201, 0.501, 0.579, 0.883. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.76. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·V·None`; the k4 to k6 lines (None, Touch, Until dispelled) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·V·None` |
| Standard spectrometer detection range | 7.60 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 1,247 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1b 1c 1d 1f` (Heat, Light, Life, Energy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 962 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 6.07 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 2nd Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Endures independently once set, which places it under the decay clause of ULMTU-XIII. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIII]] | Lex Impermanentiae | Long-lived patterns drift toward reversion unless refreshed from a source that satisfies ULMTU-I. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Light and Radiance]] |
| Element | [[Fire Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Faerie Fire (1-V-L-FF)|Faerie Fire]] (1) · [[Sacred Flame (0-V-L-SF)|Sacred Flame]] (0) · [[Flame Blade (2-V-L-FBA)|Flame Blade]] (2) · [[Galaxy Whirl (2-V-L-GWL)|Galaxy Whirl]] (2) · [[Moonbeam (2-V-M-MNB)|Moonbeam]] (2) · [[Scorching Ray (2-V-L-SR)|Scorching Ray]] (2) · [[Burning Hands (1-V-L-BH)|Burning Hands]] (1) · [[Daylight (3-V-L-DYL)|Daylight]] (3).


---

## Tactical Assessment

Permanent markers and lamps for bases, tunnels and ships without fuel, heat signature or oxygen draw.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
