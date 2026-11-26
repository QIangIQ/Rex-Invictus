---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/conjuration
  - source/srd
aliases:
  - "2nd Tier Spell: Web"
  - "Web"
  - "2-C-M-WEB"
registry_id: 2-C-M-WEB
attribute_code: "2·Con·None·cube (20)·60 feet·Up to 1 hour"
incantation: "He’-Bowynsi"
tier: 2
school: Conjuration
affinity: C
grade: M
pz_total: 703.4
pz_quantum: 951.4
t_e: 1.70
updated: 2026-11-16
---

**Web** (`2-C-M-WEB`) is a 2nd Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **703 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E 1.70 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Conjuration]]
        - **Web** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-C-M-WEB` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Con·None·cube (20)·60 feet·Up to 1 hour` |
| Incantation | *He’-Bowynsi* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | cube (20) |
| Duration | Up to 1 hour (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A bit of spiderweb |
| Ritual | no |
| Practitioner lineages | Sorcerer, Wizard |

### Mechanism

Thick adhesive webbing fills a 6 m cube, anchoring between surfaces and holding fast anything that enters.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Conjured webbing | `3 Pz/kg * 227 kg (227 m^3 * 1 kg/m^3)` | 680 |
| Pattern cost | `0.01 × Q2 × (1 + 1.50)` | 23.8 |

| Quantity | Value |
|---|---|
| Effect energy | 680 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **703 Pz** (1,055.1 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.739 |
| Energy-equivalent tier T_E | 1.70 |
| Handling points | 1.50 |
| Grade score | 1.35 → M |

**Handling flags:** concentration, fragile, save or suck.

**Assumptions:** Web density 1 kg/m^3 of structured fibre.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Web (2-C-M-WEB) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | cube (20) | 9 | `0000000010011` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Up to 1 hour | 12 | `0000000011001` |

### Incantation

Spoken as **He’-Bowynsi** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihe’-Bowynsi* · T4: *Vihe’-Bowynsi* · T5: *Tihe’-Bowynsi* · T6: *Rihe’-Bowynsi* · T7: *Mihe’-Bowynsi* · T8: *Nihe’-Bowynsi* · T9: *Xyihe’-Bowynsi*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 4→0 | 3 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 3→10 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#93d460`.

![[Web (2-C-M-WEB) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.997 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Up to 1 hour | 0.632 | 0.911 | `#00c0ff` (511 nm eq.) | source grid |
| Area | cube (20) | 0.250 | 0.999 | `#cdff00` (625 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.927 | `#00fbff` (524 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 2.85. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·C·None`; the k4 to k6 lines (cube (20), 60 feet, Up to 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·C·None` |
| Standard spectrometer detection range | 2.65 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 95.1 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 117 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (73.9% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Terrain and Matter Shaping]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Create Food and Water (3-C-L-CFW)|Create Food and Water]] (3) · [[Entangle (1-C-M-ENT)|Entangle]] (1) · [[Grease (1-C-L-GRS)|Grease]] (1) · [[Sleet Storm (3-C-L-SS)|Sleet Storm]] (3) · [[Summon Liquid (1-C-L-SL)|Summon Liquid]] (1) · [[Summon Metal (1-C-L-SM)|Summon Metal]] (1) · [[Geyser (2-V-L-GYS)|Geyser]] (2) · [[Spike Growth (2-T-L-SGI)|Spike Growth]] (2).


---

## Tactical Assessment

Cheap immobilisation of infantry in corridors; it burns away quickly.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
