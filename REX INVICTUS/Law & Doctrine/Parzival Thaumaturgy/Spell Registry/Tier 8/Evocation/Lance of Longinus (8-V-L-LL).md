---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-8
  - spell/evocation
  - source/rex-invictus
aliases:
  - "8th Tier Spell: Lance of Longinus"
  - "Lance of Longinus"
  - "8-V-L-LL"
registry_id: 8-V-L-LL
attribute_code: "8·Evo·Radiant·None·120 feet·Instantaneous"
incantation: "Nunat-’mul"
tier: 8
school: Evocation
affinity: V
grade: L
pz_total: 154834.9
pz_quantum: 383821.6
t_e: 7.09
updated: 2026-11-16
---

**Lance of Longinus** (`8-V-L-LL`) is a 8th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Rex Invictus original working. Its modelled draw is **154,835 Pz** against a slot quantum of 383,822 Pz, which puts its energy-equivalent tier at T_E 7.09 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 8 Workings]]
      - [[Evocation]]
        - **Lance of Longinus** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `8-V-L-LL` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `8·Evo·Radiant·None·120 feet·Instantaneous` |
| Incantation | *Nunat-’mul* |
| Affinity | V (Evocation) |
| Source | Rex Invictus |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 8th Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 120 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: a sliver of iron from a spearhead |
| Ritual | no |
| Injury | 20d10 radiant (mean 110) |
| Injury by tier | T8: 20d10, T9: 22d10 |
| Delivery | aimed ranged working |
| Practitioner lineages | Cleric, Paladin, Wizard |

### Effect

A consecrated lance of light strikes one creature within range. It deals 20d10 radiant and 10d10 piercing injury, ignores ward absorption up to the strength of an eighth-tier ward stack, and the radiant part cannot be reduced by resistance.

### Mechanism

Concentrates field return into a narrow consecrated channel. Almost all of the draw goes to overriding wards and divine resistance (Lex Interactionis), and only a small fraction reaches the target as injury.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| radiant injury 110, ray | `110*0.5*0.5` | 27.5 |
| piercing injury 55, focused | `55*0.35*0.5` | 9.6 |
| ward override budget | `0.2 Pz/HP-eq * 750,000 ward capacity` | 150,000 |
| Pattern cost | `0.01 × Q8 × (1 + 0.25)` | 4,798 |

| Quantity | Value |
|---|---|
| Effect energy | 150,037 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **154,835 Pz** (232,252.3 kJ) |
| Slot quantum Q8 | 383,822 Pz |
| Field gain (draw / quantum) | 0.403 |
| Energy-equivalent tier T_E | 7.09 |
| Handling points | 0.25 |
| Grade score | -0.20 → L |

**Handling flags:** costly material.

**Assumptions:** Ward override sized to defeat a typical Tier-8 ward stack; without a stack to beat the lance costs little more than its injury terms.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Lance of Longinus (8-V-L-LL) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 8 | 8 | `0000000010001` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Radiant | 11 | `0000000010111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 120 feet | 3 | `0000000000111` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Nunat-’mul** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T9: *Xyinunat-’mul*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 4→3 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 4→1 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#665a95`.

![[Lance of Longinus (8-V-L-LL) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 8 | 0.800 | 1.000 | `#2900ff` (460 nm eq.) | source grid |
| Damage | Radiant | 0.786 | 1.000 | `#1900ff` (464 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.956 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.726 | `#ff0028` (700 nm eq.) | source grid |
| Range | 120 feet | 0.176 | 0.823 | `#ffc900` (647 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 5.19. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `8·V·Radiant`; the k4 to k6 lines (None, 120 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `8·V·Radiant` |
| Standard spectrometer detection range | 39.35 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 19,191 Pz (0.05 × Q8) |
| Counter drawn cold (all six layers) | 38,382 Pz (0.10 × Q8) |
| Unravel after completion | 38,382 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Heat, Light, Life, Hope and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `2b 1c 1d 2f 1i 1j` (2x Heat, Light, Life, 2x Energy, Hope, Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 25,806 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 8th Tier quantum of 383,822 Pz (40.3% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 8th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 8 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Precision Strikes]] |
| Element | [[Radiant Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Sunburst (8-V-L-SNBB)|Sunburst]] (8) · [[Arcane Sword (7-P-L-ASC)|Arcane Sword]] (7) · [[Dark Matter Sword (7-V-L-DMS)|Dark Matter Sword]] (7) · [[Branding Smite (2-V-L-BS)|Branding Smite]] (2) · [[Burst Radiation (6-V-L-BR)|Burst Radiation]] (6) · [[Chain Lightning (6-V-L-CLA)|Chain Lightning]] (6) · [[Feeblemind (8-E-L-FBL)|Feeblemind]] (8) · [[Sunbeam (6-V-L-SNB)|Sunbeam]] (6).


---

## Tactical Assessment

A killing working for armoured mages. It is far more efficient after a breaching primer has already opened the target's wards.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 8 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
