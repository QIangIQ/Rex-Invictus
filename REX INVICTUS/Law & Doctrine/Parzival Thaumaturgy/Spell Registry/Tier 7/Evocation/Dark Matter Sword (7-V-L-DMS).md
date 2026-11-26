---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-7
  - spell/evocation
  - source/science-spellbook
aliases:
  - "7th Tier Spell: Dark Matter Sword"
  - "7-V-L-DMS"
  - "Dark Matter Sword (Science)"
registry_id: 7-V-L-DMS
attribute_code: "7·Evo·Piercing·None·Self·1 hour"
incantation: "Muix-’pora"
tier: 7
school: Evocation
affinity: V
grade: L
pz_total: 2832.3
pz_quantum: 141200.1
t_e: 3.09
updated: 2026-11-16
---

**Dark Matter Sword** (`7-V-L-DMS`) is a 7th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **2,832 Pz** against a slot quantum of 141,200 Pz, which puts its energy-equivalent tier at T_E 3.09 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 7 Workings]]
      - [[Evocation]]
        - **Dark Matter Sword** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `7-V-L-DMS` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `7·Evo·Piercing·None·Self·1 hour` |
| Incantation | *Muix-’pora* |
| Affinity | V (Evocation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 7th Tier |
| School | [[Evocation]] |
| Casting time | 1 Bonus Action |
| Range | Self |
| Area | single point or target |
| Duration | 1 hour |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Injury | 6d8 piercing (mean 27) |
| Injury by tier | T7: 6d8, T8: 6d8, T9: 6d8 |
| Delivery | aimed melee working |
| Practitioner lineages | Wizard, Sorcerer, Warlock, Ranger |

### Mechanism

Forms an invisible short blade of exotic matter that strikes hard and does not reveal a hidden wielder.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Exotic blade conjured | `1 kg x 3 Pz/kg` | 3.0 |
| Blade strikes (upkeep) | `27 HP x 0.35 (piercing) x F 0.08 x 7 targets/projectiles` | 5.3 |
| Pattern cost | `0.01 × Q7 × (1 + 1.00)` | 2,824 |

| Quantity | Value |
|---|---|
| Effect energy | 3.0 Pz |
| Upkeep energy | 5.3 Pz (0.00147 Pz/s) |
| **Total draw** | **2,832 Pz** (4,248.4 kJ) |
| Slot quantum Q7 | 141,200 Pz |
| Field gain (draw / quantum) | 0.0201 |
| Energy-equivalent tier T_E | 3.09 |
| Handling points | 1.00 |
| Grade score | 0.00 → L |

**Handling flags:** fragile.

**Assumptions:** Blade 1 kg structured solid; 6d8 = 27 piercing per hit, weapon point F 0.08; 7 hits expected in one engagement during the hour.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Dark Matter Sword (7-V-L-DMS) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 7 | 7 | `0000000001111` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | Piercing | 8 | `0000000010001` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | 1 hour | 0 | `0000000000001` |

### Incantation

Spoken as **Muix-’pora** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T8: *Nimuix-’pora* · T9: *Xyimuix-’pora*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 3→2 | 4 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 4→1 | 2 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 | 1 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#2b93b8`.

![[Dark Matter Sword (7-V-L-DMS) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 7 | 0.700 | 1.000 | `#005eff` (490 nm eq.) | source grid |
| Damage | Piercing | 0.571 | 0.992 | `#00ffec` (529 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.980 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | 1 hour | 0.053 | 0.811 | `#ff1c00` (684 nm eq.) | source grid |
| Range | Self | 0.706 | 1.000 | `#0058ff` (488 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 3.45. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `7·V·Piercing`; the k4 to k6 lines (None, Self, 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `7·V·Piercing` |
| Standard spectrometer detection range | 5.32 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 7,060 Pz (0.05 × Q7) |
| Counter drawn cold (all six layers) | 14,120 Pz (0.10 × Q7) |
| Unravel after completion | 14,121 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Beyond, Cold, Hopelessness, Movement and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 2f 1I 2j` (Beyond, 2x Energy, Hopelessness, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 472 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 7th Tier quantum of 141,200 Pz (2.0% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 7th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 7 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Precision Strikes]] |
| Element | [[Piercing Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Arcane Sword (7-P-L-ASC)|Arcane Sword]] (7) · [[Chain Lightning (6-V-L-CLA)|Chain Lightning]] (6) · [[Faithful Hound (4-C-L-FH)|Faithful Hound]] (4) · [[Lance of Longinus (8-V-L-LL)|Lance of Longinus]] (8) · [[Finger of Death (7-N-L-FDN)|Finger of Death]] (7) · [[Feeblemind (8-E-L-FBL)|Feeblemind]] (8) · [[Harm (6-N-L-HRM)|Harm]] (6) · [[Wall of Thorns (6-C-L-WT)|Wall of Thorns]] (6).


---

## Tactical Assessment

Assassination and close protection weapon for concealed operatives.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 7 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
