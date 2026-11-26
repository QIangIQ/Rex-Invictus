---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-7
  - spell/transmutation
  - source/srd
aliases:
  - "7th Tier Spell: Regenerate"
  - "Regenerate"
  - "7-T-L-RGN"
registry_id: 7-T-L-RGN
attribute_code: "7·Tra·None·None·Touch·1 hour"
incantation: "Mielixa"
tier: 7
school: Transmutation
affinity: T
grade: L
pz_total: 2074.9
pz_quantum: 141200.1
t_e: 2.78
updated: 2026-11-16
---

**Regenerate** (`7-T-L-RGN`) is a 7th Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **2,075 Pz** against a slot quantum of 141,200 Pz, which puts its energy-equivalent tier at T_E 2.78 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 7 Workings]]
      - [[Transmutation]]
        - **Regenerate** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `7-T-L-RGN` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `7·Tra·None·None·Touch·1 hour` |
| Incantation | *Mielixa* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 7th Tier |
| School | [[Transmutation]] |
| Casting time | 1 minute |
| Range | Touch |
| Area | single point or target |
| Duration | 1 hour |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A prayer wheel and holy water |
| Ritual | no |
| Restoration | 4d8 + 15 restored (mean 33, modifier taken as +3) |
| Practitioner lineages | Bard, Cleric, Druid |

### Mechanism

Touch delivery drives accelerated tissue regeneration, restoring injuries and rebuilding lost limbs over minutes.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| immediate healing 4d8+15 (33) | `0.30*33` | 9.9 |
| regrow one major limb, 12 kg living tissue | `10*12` | 120 |
| [upkeep] 1 point per round for 1 h (600 points) | `0.30*600` | 180 |
| Pattern cost | `0.01 × Q7 × (1 + 0.25)` | 1,765 |

| Quantity | Value |
|---|---|
| Effect energy | 130 Pz |
| Upkeep energy | 180 Pz (0.05 Pz/s) |
| **Total draw** | **2,075 Pz** (3,112.4 kJ) |
| Slot quantum Q7 | 141,200 Pz |
| Field gain (draw / quantum) | 0.0147 |
| Energy-equivalent tier T_E | 2.78 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** long cast.

**Assumptions:** One limb of 12 kg regrown; 600 rounds of 1 point each.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Regenerate (7-T-L-RGN) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 7 | 7 | `0000000001111` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | 1 hour | 0 | `0000000000001` |

### Incantation

Spoken as **Mielixa** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T8: *Nimielixa* · T9: *Xyimielixa*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 3→2 | 4 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 | 1 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#861ec8`.

![[Regenerate (7-T-L-RGN) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 7 | 0.700 | 1.000 | `#005eff` (490 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.985 | `#9600ff` (438 nm eq.) | source grid |
| Duration | 1 hour | 0.053 | 0.811 | `#ff1c00` (684 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.984 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.21): swatch `#4d7ad6`, measured lines at 0.053, 0.701, 0.878. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.32. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `7·T·None`; the k4 to k6 lines (None, Touch, 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `7·T·None` |
| Standard spectrometer detection range | 4.56 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 7,060 Pz (0.05 × Q7) |
| Counter drawn cold (all six layers) | 14,120 Pz (0.10 × Q7) |
| Unravel after completion | 14,156 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 346 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 7th Tier quantum of 141,200 Pz (1.5% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 7th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 7 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Healing and Restoration]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Reincarnate (5-T-M-RNC)|Reincarnate]] (5) · [[Resurrection (7-N-L-RSR)|Resurrection]] (7) · [[Time Stop (9-T-M-TSM)|Time Stop]] (9) · [[Heal (6-V-L-HEA)|Heal]] (6) · [[Heroes' Feast (6-C-L-HF)|Heroes' Feast]] (6) · [[Etherealness (7-T-L-ETH)|Etherealness]] (7) · [[Greater Restoration (5-A-L-GRE)|Greater Restoration]] (5) · [[Mass Cure Wounds (5-C-L-MCW)|Mass Cure Wounds]] (5).


---

## Tactical Assessment

Returns maimed personnel to full function without prosthetics.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 7 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
