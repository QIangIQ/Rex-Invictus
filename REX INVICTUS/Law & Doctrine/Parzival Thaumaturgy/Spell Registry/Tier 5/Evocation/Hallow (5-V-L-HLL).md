---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/evocation
  - source/srd
aliases:
  - "5th Tier Spell: Hallow"
  - "Hallow"
  - "5-V-L-HLL"
registry_id: 5-V-L-HLL
attribute_code: "5·Evo·None·sphere (60)·Touch·Until dispelled"
incantation: "Tu’-Silixis"
tier: 5
school: Evocation
affinity: V
grade: L
pz_total: 9083.6
pz_quantum: 19109.4
t_e: 4.26
updated: 2026-11-16
---

**Hallow** (`5-V-L-HLL`) is a 5th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **9,084 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 4.26 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Evocation]]
        - **Hallow** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-V-L-HLL` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Evo·None·sphere (60)·Touch·Until dispelled` |
| Incantation | *Tu’-Silixis* |
| Affinity | V (Evocation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Evocation]] |
| Casting time | 24 hours |
| Range | Touch |
| Area | sphere (60) |
| Duration | Until dispelled |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Herbs, oils, and incense worth at least 1,000 gp, which the spell consumes |
| Ritual | no |
| Resistance check | presence; on success: no effect |
| Practitioner lineages | Cleric |

### Mechanism

Consecrates an 18 m radius area that bars chosen outsider and undead types and supports one bound effect such as courage, darkness, light or silence.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| exclusion repulsion | `3 * 0.5 * 80 kg * (5 m/s)^2 / 1500` | 2.0 |
| consecration field | `0.002 Pz/s * 25620 m^3 / 1000 = 0.051241 Pz/s * 86400 s` | 4,427 |
| bound effect (courage, 10 creatures) | `0.005 Pz/s * 10 = 0.05 Pz/s * 86400 s` | 4,320 |
| Pattern cost | `0.01 × Q5 × (1 + 0.75)` | 334 |

| Quantity | Value |
|---|---|
| Effect energy | 2.0 Pz |
| Upkeep energy | 8,747 Pz (0.101 Pz/s) |
| **Total draw** | **9,084 Pz** (13,625.5 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 0.475 |
| Energy-equivalent tier T_E | 4.26 |
| Handling points | 0.75 |
| Grade score | 0.38 → L |

**Handling flags:** costly material, consumed material, long cast.

**Assumptions:** Indefinite duration: upkeep booked over a 24 h reference period; courage chosen as the bound effect for 10 creatures; 3 intrusions repelled.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Hallow (5-V-L-HLL) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (60) | 35 | `0000001000111` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Until dispelled | 11 | `0000000010111` |

### Incantation

Spoken as **Tu’-Silixis** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Ritu’-Silixis* · T7: *Mitu’-Silixis* · T8: *Nitu’-Silixis* · T9: *Xyitu’-Silixis*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 2→11 6→2 | 4 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 2→9 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#4d9ec8`.

![[Hallow (5-V-L-HLL) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| School | Evocation | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Until dispelled | 0.579 | 0.997 | `#00fff7` (526 nm eq.) | source grid |
| Area | sphere (60) | 0.972 | 0.894 | `#ff00e5` (408 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.930 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.18): swatch `#6fd4c8`, measured lines at 0.501, 0.580, 0.883, 0.973. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.96. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·V·None`; the k4 to k6 lines (sphere (60), Touch, Until dispelled) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·V·None` |
| Standard spectrometer detection range | 9.53 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 3,660 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1b 1c 1d 1f` (Heat, Light, Life, Energy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1,514 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 5th Tier quantum of 19,109 Pz (47.5% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Endures independently once set, which places it under the decay clause of ULMTU-XIII. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIII]] | Lex Impermanentiae | Long-lived patterns drift toward reversion unless refreshed from a source that satisfies ULMTU-I. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 5th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 5 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Evocation]] (V) |
| Function | [[Wards and Shields]], [[Teleportation and Planar Travel]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Wall of Force (5-P-L-WFL)|Wall of Force]] (5) · [[Fire Shield (4-V-L-FSR)|Fire Shield]] (4) · [[Resilient Sphere (4-P-L-RS)|Resilient Sphere]] (4) · [[Forcecage (7-P-L-FRC)|Forcecage]] (7) · [[Teleportation Circle (5-C-M-TC)|Teleportation Circle]] (5) · [[Tree Stride (5-C-L-TSE)|Tree Stride]] (5) · [[Wish (9-C-L-WSH)|Wish]] (9) · [[Banishment (4-A-M-BNS)|Banishment]] (4).


---

## Tactical Assessment

A durable defensive installation for temples, bases and burial grounds against possession, fear and extraplanar intrusion.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
