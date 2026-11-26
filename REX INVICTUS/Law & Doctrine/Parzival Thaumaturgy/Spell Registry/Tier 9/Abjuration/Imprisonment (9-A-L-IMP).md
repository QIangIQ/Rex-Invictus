---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-9
  - spell/abjuration
  - source/srd
aliases:
  - "9th Tier Spell: Imprisonment"
  - "Imprisonment"
  - "9-A-L-IMP"
registry_id: 9-A-L-IMP
attribute_code: "9·Abj·None·None·30 feet·Until dispelled"
incantation: "Xyausinis"
tier: 9
school: Abjuration
affinity: A
grade: L
pz_total: 86890.4
pz_quantum: 1043335.3
t_e: 6.51
updated: 2026-11-16
---

**Imprisonment** (`9-A-L-IMP`) is a 9th Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **86,890 Pz** against a slot quantum of 1.04 MPz Pz, which puts its energy-equivalent tier at T_E 6.51 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 9 Workings]]
      - [[Abjuration]]
        - **Imprisonment** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `9-A-L-IMP` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `9·Abj·None·None·30 feet·Until dispelled` |
| Incantation | *Xyausinis* |
| Affinity | A (Abjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 9th Tier |
| School | [[Abjuration]] |
| Casting time | 1 minute |
| Range | 30 feet |
| Area | single point or target |
| Duration | Until dispelled |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A vellum depiction or a carved statuette in the likeness of the target, and a special component that varies according to the version of the spell you choose, worth at least 500gp per Hit Die of the target |
| Ritual | no |
| Resistance check | will; on success: no effect |
| Practitioner lineages | Warlock, Wizard |

### Mechanism

The field seals one creature into a closed containment geometry, either a buried force shell, rooted chains, a pocket plane, a gemstone cell, or enforced sleep, and suspends its metabolism and aging. The binding persists until a release condition set at casting is met.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Plane-boundary translocation (hedged prison form) | `0.01 * 80 kg * 15 * 1e6 m / 1500` | 8,000 |
| Stasis anchor (soul-work constant, tiers above 3) | `1e4 Pz * (9 - 3)` | 60,000 |
| Containment ward absorption | `0.20 Pz * 1000 HP expected assault on the prison` | 200 |
| Sustaining hold, 24 h reference horizon (upkeep) | `0.005 Pz/s * 86400 s` | 432 |
| Pattern cost | `0.01 × Q9 × (1 + 0.75)` | 18,258 |

| Quantity | Value |
|---|---|
| Effect energy | 68,200 Pz |
| Upkeep energy | 432 Pz (0.005 Pz/s) |
| **Total draw** | **86,890 Pz** (130,335.6 kJ) |
| Slot quantum Q9 | 1.04 MPz Pz |
| Field gain (draw / quantum) | 0.0833 |
| Energy-equivalent tier T_E | 6.51 |
| Handling points | 0.75 |
| Grade score | -0.25 → L |

**Handling flags:** costly material, save or suck, long cast.

**Assumptions:** Order-of-magnitude model; costed on the pocket-plane form with one boundary crossing; stasis costed with the soul re-anchoring constant; indefinite duration costed over a 24 h reference horizon.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Imprisonment (9-A-L-IMP) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 9 | 9 | `0000000010011` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Until dispelled | 11 | `0000000010111` |

### Incantation

Spoken as **Xyausinis** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 4→3 | 3 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 2→9 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#898395`.

![[Imprisonment (9-A-L-IMP) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 9 | 0.900 | 1.000 | `#b600ff` (430 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.667 | `#ff0028` (700 nm eq.) | source grid |
| Duration | Until dispelled | 0.579 | 0.950 | `#00fff7` (526 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.832 | `#91ff00` (612 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.19): swatch `#8d7cab`, measured lines at 0.006, 0.295, 0.579, 0.901. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.94. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `9·A·None`; the k4 to k6 lines (None, 30 feet, Until dispelled) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `9·A·None` |
| Standard spectrometer detection range | 29.48 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 52,167 Pz (0.05 × Q9) |
| Counter drawn cold (all six layers) | 104,334 Pz (0.10 × Q9) |
| Unravel after completion | 104,420 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 14,482 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 9th Tier quantum of 1.04 MPz Pz (8.3% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Endures independently once set, which places it under the decay clause of ULMTU-XIII. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIII]] | Lex Impermanentiae | Long-lived patterns drift toward reversion unless refreshed from a source that satisfies ULMTU-I. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 9th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 9 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Teleportation and Planar Travel]], [[Summoning and Conjured Creatures]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Astral Projection (9-N-M-AP)|Astral Projection]] (9) · [[Gate (9-C-L-GAT)|Gate]] (9) · [[Magic Circle (3-A-L-MC)|Magic Circle]] (3) · [[Time Stop (9-T-M-TSM)|Time Stop]] (9) · [[Wish (9-C-L-WSH)|Wish]] (9) · [[Clone (8-N-L-CLN)|Clone]] (8) · [[Demiplane (8-C-L-DMP)|Demiplane]] (8) · [[Gravitational Wave (8-V-L-GWV)|Gravitational Wave]] (8).


---

## Tactical Assessment

Suited to permanent detention of high-value or uncontainable prisoners where conventional custody fails. The long casting and the target's resistance check limit it to captives already secured.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 9 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
