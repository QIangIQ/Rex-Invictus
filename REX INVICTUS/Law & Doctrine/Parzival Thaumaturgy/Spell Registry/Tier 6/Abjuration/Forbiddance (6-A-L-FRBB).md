---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-6
  - spell/abjuration
  - source/srd
aliases:
  - "6th Tier Spell: Forbiddance"
  - "Forbiddance"
  - "6-A-L-FRBB"
registry_id: 6-A-L-FRBB
attribute_code: "6·Abj·None·cube (40000)·Touch·24 hours"
incantation: "Ra’-Bielixl"
tier: 6
school: Abjuration
affinity: A
grade: L
pz_total: 14822.1
pz_quantum: 51944.6
t_e: 4.75
updated: 2026-11-16
---

**Forbiddance** (`6-A-L-FRBB`) is a 6th Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **14,822 Pz** against a slot quantum of 51,945 Pz, which puts its energy-equivalent tier at T_E 4.75 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 6 Workings]]
      - [[Abjuration]]
        - **Forbiddance** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `6-A-L-FRBB` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `6·Abj·None·cube (40000)·Touch·24 hours` |
| Incantation | *Ra’-Bielixl* |
| Affinity | A (Abjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 6th Tier |
| School | [[Abjuration]] |
| Casting time | 10 minutes |
| Range | Touch |
| Area | cube (40000) |
| Duration | 24 hours |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A sprinkling of holy water, rare incense, and powdered ruby worth at least 1,000 gp |
| Ritual | yes |
| Practitioner lineages | Cleric |

### Mechanism

A ward over up to 3,716 m^2 and 9 m high seals the volume against teleportation and planar entry and burns chosen kinds of creature that enter or linger.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| damage to chosen creature types, 5d10=27.5 | `27.5 HP * kappa_radiant 0.5 * F 1.0 * 1 target(s) * 3 trigger(s)` | 41.2 |
| planar crossing denial reserve | `0.01 * 80 kg * 15 * 1e6 m / 1500 (one blocked crossing)` | 8,000 |
| ward field maintenance | `0.002 Pz/s * 33980 m^3 / 1000 = 0.0679604 Pz/s * 86400 s` | 5,872 |
| Pattern cost | `0.01 × Q6 × (1 + 0.75)` | 909 |

| Quantity | Value |
|---|---|
| Effect energy | 8,041 Pz |
| Upkeep energy | 5,872 Pz (0.068 Pz/s) |
| **Total draw** | **14,822 Pz** (22,233.1 kJ) |
| Slot quantum Q6 | 51,945 Pz |
| Field gain (draw / quantum) | 0.285 |
| Energy-equivalent tier T_E | 4.75 |
| Handling points | 0.75 |
| Grade score | 0.12 → L |

**Handling flags:** ritual, costly material, long cast.

**Assumptions:** Full 40,000 ft^2 x 30 ft; 3 damage triggers on one target; one blocked plane crossing held in reserve; 24 h upkeep at the illusion-volume field rate.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Forbiddance (6-A-L-FRBB) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 6 | 6 | `0000000001101` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | cube (40000) | 14 | `0000000011101` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | 24 hours | 5 | `0000000001011` |

### Incantation

Spoken as **Ra’-Bielixl** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T7: *Mira’-Bielixl* · T8: *Nira’-Bielixl* · T9: *Xyira’-Bielixl*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 3→2 | 3 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 2→11 3→12 4→0 | 4 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 3→10 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#679a70`.

![[Forbiddance (6-A-L-FRBB) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 6 | 0.600 | 1.000 | `#00ebff` (520 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.835 | `#ff0028` (700 nm eq.) | source grid |
| Duration | 24 hours | 0.316 | 0.960 | `#76ff00` (605 nm eq.) | source grid |
| Area | cube (40000) | 0.389 | 0.978 | `#10ff00` (583 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.961 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.17): swatch `#8fa29c`, measured lines at 0.007, 0.316, 0.390, 0.601, 0.883. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.17. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `6·A·None`; the k4 to k6 lines (cube (40000), Touch, 24 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `6·A·None` |
| Standard spectrometer detection range | 12.17 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 2,597 Pz (0.05 × Q6) |
| Counter drawn cold (all six layers) | 5,194 Pz (0.10 × Q6) |
| Unravel after completion | 6,369 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 2,470 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 6th Tier quantum of 51,945 Pz (28.5% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 6th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 6 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Negation and Counterspell]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Globe of Invulnerability (6-A-L-GIO)|Globe of Invulnerability]] (6) · [[Antilife Shell (5-A-L-ASI)|Antilife Shell]] (5) · [[Dispel Evil and Good (5-A-L-DEGP)|Dispel Evil and Good]] (5) · [[Antimagic Field (8-A-L-AFT)|Antimagic Field]] (8) · [[Arcane Insulation (4-A-L-AI)|Arcane Insulation]] (4) · [[Banishment (4-A-M-BNS)|Banishment]] (4) · [[Mind Blank (8-A-L-MB)|Mind Blank]] (8) · [[Private Sanctum (4-A-L-PSI)|Private Sanctum]] (4).


---

## Tactical Assessment

Hardens a base, vault or command post against teleport raids and extraplanar incursion; daily recasting for a month makes it a permanent fixture.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 6 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
