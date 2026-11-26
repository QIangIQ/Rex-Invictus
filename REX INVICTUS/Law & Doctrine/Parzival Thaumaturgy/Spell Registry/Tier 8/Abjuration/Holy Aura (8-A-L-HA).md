---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-8
  - spell/abjuration
  - source/srd
aliases:
  - "8th Tier Spell: Holy Aura"
  - "Holy Aura"
  - "8-A-L-HA"
registry_id: 8-A-L-HA
attribute_code: "8·Abj·None·sphere (30)·Self·Up to 1 minute"
incantation: "Na’-Sorporse"
tier: 8
school: Abjuration
affinity: A
grade: L
pz_total: 5813.5
pz_quantum: 383821.6
t_e: 3.81
updated: 2026-11-16
---

**Holy Aura** (`8-A-L-HA`) is a 8th Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **5,813 Pz** against a slot quantum of 383,822 Pz, which puts its energy-equivalent tier at T_E 3.81 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 8 Workings]]
      - [[Abjuration]]
        - **Holy Aura** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `8-A-L-HA` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `8·Abj·None·sphere (30)·Self·Up to 1 minute` |
| Incantation | *Na’-Sorporse* |
| Affinity | A (Abjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 8th Tier |
| School | [[Abjuration]] |
| Casting time | 1 action |
| Range | Self |
| Area | sphere (30) |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A tiny reliquary worth at least 1,000gp containing a sacred relic, such as a scrap of cloth from a saint's robe or a piece of parchment from a religious text |
| Ritual | no |
| Practitioner lineages | Cleric |

### Mechanism

Spreads a 9 m radius radiance that strengthens chosen allies' resistance and makes them harder to hit, and blinds undead or fiendish attackers with flashes.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| ally evasion absorption | `0.20 Pz * (6 allies * 10 rounds * 10 HP/round * 25% avoided = 150 HP)` | 30.0 |
| blinding flashes | `3 * 10 kJ / 1500` | 20.0 |
| blindness holds | `0.005 Pz/s * 60 s * 3` | 0.9 |
| radiance and ally glow | `(112.5 W aura + 6 * 3.125 W glow) / 1500 = 0.0875 Pz/s * 60 s` | 5.2 |
| Pattern cost | `0.01 × Q8 × (1 + 0.50)` | 5,757 |

| Quantity | Value |
|---|---|
| Effect energy | 50.9 Pz |
| Upkeep energy | 5.2 Pz (0.0875 Pz/s) |
| **Total draw** | **5,813 Pz** (8,720.2 kJ) |
| Slot quantum Q8 | 383,822 Pz |
| Field gain (draw / quantum) | 0.0151 |
| Energy-equivalent tier T_E | 3.81 |
| Handling points | 0.50 |
| Grade score | -0.50 → L |

**Handling flags:** concentration, costly material.

**Assumptions:** 6 allies, 10 rounds, 25% of incoming injury avoided; 3 flashes of 10 kJ; dim radiance 112.5 W.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Holy Aura (8-A-L-HA) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 8 | 8 | `0000000010001` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (30) | 31 | `0000000111111` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Na’-Sorporse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T9: *Xyina’-Sorporse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 4→3 | 2 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 2→11 3→12 4→0 5→1 | 6 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#4b2bdd`.

![[Holy Aura (8-A-L-HA) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 8 | 0.800 | 1.000 | `#2900ff` (460 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.726 | `#ff0028` (700 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.993 | `#0074ff` (495 nm eq.) | source grid |
| Area | sphere (30) | 0.861 | 0.998 | `#8000ff` (442 nm eq.) | source grid |
| Range | Self | 0.706 | 0.996 | `#0058ff` (488 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.18): swatch `#4390c6`, measured lines at 0.006, 0.685, 0.706, 0.801, 0.862. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.76. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `8·A·None`; the k4 to k6 lines (sphere (30), Self, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `8·A·None` |
| Standard spectrometer detection range | 7.62 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 19,191 Pz (0.05 × Q8) |
| Counter drawn cold (all six layers) | 38,382 Pz (0.10 × Q8) |
| Unravel after completion | 38,383 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 969 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 8th Tier quantum of 383,822 Pz (1.5% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 8th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 8 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Wards and Shields]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Mind Blank (8-A-L-MB)|Mind Blank]] (8) · [[Globe of Invulnerability (6-A-L-GIO)|Globe of Invulnerability]] (6) · [[Guards and Wards (6-A-L-GWA)|Guards and Wards]] (6) · [[Forcecage (7-P-L-FRC)|Forcecage]] (7) · [[Wish (9-C-L-WSH)|Wish]] (9) · [[Antimagic Field (8-A-L-AFT)|Antimagic Field]] (8) · [[Death Ward (4-A-L-DW)|Death Ward]] (4) · [[Medic's Tent (8-A-L-MSTI)|Medic's Tent]] (8).


---

## Tactical Assessment

Protects a squad in a close fight against undead or demonic forces for one minute.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 8 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
