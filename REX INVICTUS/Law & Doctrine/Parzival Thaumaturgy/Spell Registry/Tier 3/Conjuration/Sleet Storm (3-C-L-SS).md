---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-3
  - spell/conjuration
  - source/srd
aliases:
  - "3rd Tier Spell: Sleet Storm"
  - "Sleet Storm"
  - "3-C-L-SS"
registry_id: 3-C-L-SS
attribute_code: "3·Con·None·cylinder (40)·150 feet·Up to 1 minute"
incantation: "Le’-Xonosinse"
tier: 3
school: Conjuration
affinity: C
grade: L
pz_total: 3380.0
pz_quantum: 2586.2
t_e: 3.27
updated: 2026-11-16
---

**Sleet Storm** (`3-C-L-SS`) is a 3rd Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **3,380 Pz** against a slot quantum of 2,586 Pz, which puts its energy-equivalent tier at T_E 3.27 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 3 Workings]]
      - [[Conjuration]]
        - **Sleet Storm** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `3-C-L-SS` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `3·Con·None·cylinder (40)·150 feet·Up to 1 minute` |
| Incantation | *Le’-Xonosinse* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 3rd Tier |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | 150 feet |
| Area | cylinder (40) |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A pinch of dust and a few drops of water |
| Ritual | no |
| Practitioner lineages | Druid, Sorcerer, Wizard |

### Mechanism

Freezing precipitation fills a broad cylinder, obscuring vision, glazing the ground and dousing open flames.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| ice glaze 2 mm over r 40 ft, structured ice 3 Pz/kg | `3*917*0.002*pi*(40*ft)**2` | 2,569 |
| airborne sleet 1 min at 100 mm/h, 1 Pz/kg | `1*1000*(0.1/60)*pi*(40*ft)**2` | 778 |
| Pattern cost | `0.01 × Q3 × (1 + 0.25)` | 32.3 |

| Quantity | Value |
|---|---|
| Effect energy | 3,348 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **3,380 Pz** (5,069.9 kJ) |
| Slot quantum Q3 | 2,586 Pz |
| Field gain (draw / quantum) | 1.31 |
| Energy-equivalent tier T_E | 3.27 |
| Handling points | 0.25 |
| Grade score | 0.38 → L |

**Handling flags:** concentration.

**Assumptions:** Water formed near freezing so no cooling term; 2 mm glaze.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Sleet Storm (3-C-L-SS) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 3 | 3 | `0000000000111` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | cylinder (40) | 19 | `0000000100111` |
| k5 Range | 150 feet | 4 | `0000000001001` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Le’-Xonosinse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T4: *Vile’-Xonosinse* · T5: *Tile’-Xonosinse* · T6: *Rile’-Xonosinse* · T7: *Mile’-Xonosinse* · T8: *Nile’-Xonosinse* · T9: *Xyile’-Xonosinse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 | 3 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 2→11 5→1 | 4 |
| k5 Range | 0→8 3→11 | 2 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#7ecb53`.

![[Sleet Storm (3-C-L-SS) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 3 | 0.300 | 1.000 | `#8cff00` (610 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.985 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.929 | `#0074ff` (495 nm eq.) | source grid |
| Area | cylinder (40) | 0.528 | 0.974 | `#00ffb1` (542 nm eq.) | source grid |
| Range | 150 feet | 0.235 | 0.998 | `#e3ff00` (629 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.22): swatch `#cea76e`, measured lines at 0.126, 0.236, 0.300, 0.528, 0.685. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.53. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `3·C·None`; the k4 to k6 lines (cylinder (40), 150 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `3·C·None` |
| Standard spectrometer detection range | 5.81 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 129 Pz (0.05 × Q3) |
| Counter drawn cold (all six layers) | 259 Pz (0.10 × Q3) |
| Unravel after completion | 259 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 563 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 1.31 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 3rd Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 3rd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 3 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Terrain and Matter Shaping]] |
| Element | [[Cold and Ice Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Ice Storm (4-V-L-ISE)|Ice Storm]] (4) · [[Create Food and Water (3-C-L-CFW)|Create Food and Water]] (3) · [[Web (2-C-M-WEB)|Web]] (2) · [[Arcane Redirection (3-A-L-AR)|Arcane Redirection]] (3) · [[Entangle (1-C-M-ENT)|Entangle]] (1) · [[Entangle Spell Slots (3-E-L-ESS)|Entangle Spell Slots]] (3) · [[Grease (1-C-L-GRS)|Grease]] (1) · [[Meld Into Stone (3-T-M-MIS)|Meld Into Stone]] (3).


---

## Tactical Assessment

Area denial and concentration breaking; slows infantry and vehicles.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 3 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
