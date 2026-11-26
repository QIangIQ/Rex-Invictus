---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/transmutation
  - source/srd
aliases:
  - "5th Tier Spell: Awaken"
  - "Awaken"
  - "5-T-H-AWK"
registry_id: 5-T-H-AWK
attribute_code: "5·Tra·None·None·Touch·Instantaneous"
incantation: "Tielix"
tier: 5
school: Transmutation
affinity: T
grade: H
pz_total: 15499.5
pz_quantum: 19109.4
t_e: 4.79
updated: 2026-11-16
---

**Awaken** (`5-T-H-AWK`) is a 5th Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **15,500 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 4.79 and its handling grade at **High**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Transmutation]]
        - **Awaken** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-T-H-AWK` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Tra·None·None·Touch·Instantaneous` |
| Incantation | *Tielix* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Transmutation]] |
| Casting time | 8 hours |
| Range | Touch |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: An agate worth at least 1,000 gp, which the spell consumes |
| Ritual | no |
| Practitioner lineages | Bard, Druid |

### Mechanism

Over eight hours the caster builds a reasoning nervous system into a beast or plant, which gains speech and, for plants, motion and senses, and is bonded to the caster for 30 days.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| neural growth | `1.4 kg neural tissue * 10 Pz/kg` | 14.0 |
| motile restructuring (plant case) | `200 kg (10% of 2000 kg) * 10 Pz/kg` | 2,000 |
| bonding upkeep | `0.005 Pz/s * 2592000 s` | 12,960 |
| Pattern cost | `0.01 × Q5 × (1 + 1.75)` | 526 |

| Quantity | Value |
|---|---|
| Effect energy | 2,014 Pz |
| Upkeep energy | 12,960 Pz (0.005 Pz/s) |
| **Total draw** | **15,500 Pz** (23,249.3 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 0.811 |
| Energy-equivalent tier T_E | 4.79 |
| Handling points | 1.75 |
| Grade score | 1.65 → H |

**Handling flags:** costly material, consumed material, fragile, long cast.

**Assumptions:** Huge plant case 2000 kg with 10% restructured; 1.4 kg neural tissue; bond held for 30 days at 0.005 Pz/s.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Awaken (5-T-H-AWK) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Tielix** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Ritielix* · T7: *Mitielix* · T8: *Nitielix* · T9: *Xyitielix*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#8744ad`.

![[Awaken (5-T-H-AWK) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.932 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.882 | `#ff0028` (700 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.930 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.13): swatch `#678bcd`, measured lines at 0.004, 0.501, 0.878. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.19. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·T·None`; the k4 to k6 lines (None, Touch, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·T·None` |
| Standard spectrometer detection range | 12.45 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 4,503 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 2,583 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 5th Tier quantum of 19,109 Pz (81.1% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 5th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 5 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Mind and Will]], [[Divination and Sensing]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|High]] |

Similar workings: [[Suspend Motion (4-T-L-SMS)|Suspend Motion]] (4) · [[Plagarise (4-E-L-PLG)|Plagarise]] (4) · [[Divine Word (7-V-L-DWV)|Divine Word]] (7) · [[Spirit Guardians (3-C-M-SGR)|Spirit Guardians]] (3) · [[Arcane Hand (5-P-L-AH)|Arcane Hand]] (5) · [[Commune (5-D-L-CMMM)|Commune]] (5) · [[Commune With Nature (5-D-L-CN)|Commune With Nature]] (5) · [[Contact Other Plane (5-D-L-COP)|Contact Other Plane]] (5).


---

## Tactical Assessment

Creates loyal sentries and guides from local fauna or trees, including large mobile plant guardians.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
