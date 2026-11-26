---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-6
  - spell/conjuration
  - source/srd
aliases:
  - "6th Tier Spell: Instant Summons"
  - "Instant Summons"
  - "6-C-L-ISS"
registry_id: 6-C-L-ISS
attribute_code: "6·Con·None·None·Touch·Until dispelled"
incantation: "Relixis"
tier: 6
school: Conjuration
affinity: C
grade: L
pz_total: 1493.5
pz_quantum: 51944.6
t_e: 2.45
updated: 2026-11-16
---

**Instant Summons** (`6-C-L-ISS`) is a 6th Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **1,493 Pz** against a slot quantum of 51,945 Pz, which puts its energy-equivalent tier at T_E 2.45 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 6 Workings]]
      - [[Conjuration]]
        - **Instant Summons** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `6-C-L-ISS` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `6·Con·None·None·Touch·Until dispelled` |
| Incantation | *Relixis* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 6th Tier |
| School | [[Conjuration]] |
| Casting time | 1 minute |
| Range | Touch |
| Area | single point or target |
| Duration | Until dispelled |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A sapphire worth 1,000 gp |
| Ritual | yes |
| Practitioner lineages | Wizard |

### Mechanism

The field binds a resonant tag on a small object to a matched crystal; crushing the crystal pulls the object to the holder's hand from any distance. If someone else holds it, the link returns their identity and position instead.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Mark and name inscription (instant info) | `instant info = 1 Pz` | 1.0 |
| Recall translocation, one plane boundary | `0.01 * 4.536 kg * 15 * 1e6 m / 1500` | 454 |
| Pattern cost | `0.01 × Q6 × (1 + 1.00)` | 1,039 |

| Quantity | Value |
|---|---|
| Effect energy | 455 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **1,493 Pz** (2,240.2 kJ) |
| Slot quantum Q6 | 51,945 Pz |
| Field gain (draw / quantum) | 0.0288 |
| Energy-equivalent tier T_E | 2.45 |
| Handling points | 1.00 |
| Grade score | 0.00 → L |

**Handling flags:** ritual, costly material, consumed material, long cast.

**Assumptions:** Object at the 10 lb maximum; recall priced as one plane boundary crossing for the worst case; mark itself passive with no upkeep.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Instant Summons (6-C-L-ISS) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 6 | 6 | `0000000001101` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Until dispelled | 11 | `0000000010111` |

### Incantation

Spoken as **Relixis** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T7: *Mirelixis* · T8: *Nirelixis* · T9: *Xyirelixis*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 3→2 | 3 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 2→9 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#619dc1`.

![[Instant Summons (6-C-L-ISS) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 6 | 0.600 | 1.000 | `#00ebff` (520 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.893 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Until dispelled | 0.579 | 1.000 | `#00fff7` (526 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.961 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.19): swatch `#89a6a0`, measured lines at 0.126, 0.580, 0.600, 0.883. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.17. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `6·C·None`; the k4 to k6 lines (None, Touch, Until dispelled) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `6·C·None` |
| Standard spectrometer detection range | 3.86 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 2,597 Pz (0.05 × Q6) |
| Counter drawn cold (all six layers) | 5,194 Pz (0.10 × Q6) |
| Unravel after completion | 5,194 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 249 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 6th Tier quantum of 51,945 Pz (2.9% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Endures independently once set, which places it under the decay clause of ULMTU-XIII. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIII]] | Lex Impermanentiae | Long-lived patterns drift toward reversion unless refreshed from a source that satisfies ULMTU-I. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 6th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 6 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Summoning and Conjured Creatures]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Conjure Fey (6-C-L-CFN)|Conjure Fey]] (6) · [[Planar Ally (6-C-L-PA)|Planar Ally]] (6) · [[Conjure Celestial (7-C-L-CCN)|Conjure Celestial]] (7) · [[Conjure Elemental (5-C-M-CEN)|Conjure Elemental]] (5) · [[Conjure Magic Prism (4-C-L-CMPJ)|Conjure Magic Prism]] (4) · [[Conjure Minor Elementals (4-C-M-CME)|Conjure Minor Elementals]] (4) · [[Conjure Woodland Beings (4-C-L-CWB)|Conjure Woodland Beings]] (4) · [[Create Undead (6-N-L-CU)|Create Undead]] (6).


---

## Tactical Assessment

Guarantees access to a key device, code book or weapon wherever it is stored, and acts as a tripwire that reveals who has taken it. One crystal per object limits use to critical items.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 6 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
