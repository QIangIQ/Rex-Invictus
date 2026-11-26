---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-8
  - spell/transmutation
  - source/srd
aliases:
  - "8th Tier Spell: Glibness"
  - "Glibness"
  - "8-T-L-GLB"
registry_id: 8-T-L-GLB
attribute_code: "8·Tra·None·None·Self·1 hour"
incantation: "Niepora"
tier: 8
school: Transmutation
affinity: T
grade: L
pz_total: 3856.2
pz_quantum: 383821.6
t_e: 3.40
updated: 2026-11-16
---

**Glibness** (`8-T-L-GLB`) is a 8th Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **3,856 Pz** against a slot quantum of 383,822 Pz, which puts its energy-equivalent tier at T_E 3.40 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 8 Workings]]
      - [[Transmutation]]
        - **Glibness** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `8-T-L-GLB` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `8·Tra·None·None·Self·1 hour` |
| Incantation | *Niepora* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 8th Tier |
| School | [[Transmutation]] |
| Casting time | 1 action |
| Range | Self |
| Area | single point or target |
| Duration | 1 hour |
| Components | spoken (incantation) |
| Ritual | no |
| Practitioner lineages | Bard, Warlock |

### Mechanism

Steadies the caster's speech so it is reliably persuasive and masks the caster's statements from truth-reading workings.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| persuasion field and truth-detection masking | `0.005 Pz/s = 0.005 Pz/s * 3600 s` | 18.0 |
| Pattern cost | `0.01 × Q8 × (1 + 0.00)` | 3,838 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 18.0 Pz (0.005 Pz/s) |
| **Total draw** | **3,856 Pz** (5,784.3 kJ) |
| Slot quantum Q8 | 383,822 Pz |
| Field gain (draw / quantum) | 0.01 |
| Energy-equivalent tier T_E | 3.40 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Enchantment rate on one subject for 1 hour; physical cost is small and the tier is set by complexity.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Glibness (8-T-L-GLB) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 8 | 8 | `0000000010001` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | 1 hour | 0 | `0000000000001` |

### Incantation

Spoken as **Niepora** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T9: *Xyiniepora*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 4→3 | 2 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 | 1 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#661dcb`.

![[Glibness (8-T-L-GLB) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 8 | 0.800 | 1.000 | `#2900ff` (460 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.997 | `#9600ff` (438 nm eq.) | source grid |
| Duration | 1 hour | 0.053 | 0.756 | `#ff1c00` (684 nm eq.) | source grid |
| Range | Self | 0.706 | 0.996 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.18): swatch `#437ed9`, measured lines at 0.053, 0.706, 0.801, 0.876. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.59. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `8·T·None`; the k4 to k6 lines (None, Self, 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `8·T·None` |
| Standard spectrometer detection range | 6.21 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 19,191 Pz (0.05 × Q8) |
| Counter drawn cold (all six layers) | 38,382 Pz (0.10 × Q8) |
| Unravel after completion | 38,386 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 643 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 8th Tier quantum of 383,822 Pz (1.0% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 8th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 8 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Negation and Counterspell]], [[Necromantic and Soul Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Antilife Shell (5-A-L-ASI)|Antilife Shell]] (5) · [[Antimagic Field (8-A-L-AFT)|Antimagic Field]] (8) · [[Clone (8-N-L-CLN)|Clone]] (8) · [[Disintegrate (6-P-L-DSN)|Disintegrate]] (6) · [[Mind Blank (8-A-L-MB)|Mind Blank]] (8) · [[Finger of Death (7-N-L-FDN)|Finger of Death]] (7) · [[Power Word Kill (9-E-L-PWK)|Power Word Kill]] (9) · [[Resurrection (7-N-L-RSR)|Resurrection]] (7).


---

## Tactical Assessment

Lets an agent pass interrogation, bluff checkpoints or negotiate under field-assisted lie detection for an hour.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 8 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
