---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/conjuration
  - source/rex-invictus
aliases:
  - "1st Tier Spell: Summon Liquid"
  - "Summon Liquid"
  - "1-C-L-SL"
registry_id: 1-C-L-SL
attribute_code: "1·Con·None·None·30 feet·Instantaneous"
incantation: "Seusin"
tier: 1
school: Conjuration
affinity: C
grade: L
pz_total: 303.5
pz_quantum: 350.0
t_e: 0.86
updated: 2026-11-16
---

**Summon Liquid** (`1-C-L-SL`) is a 1st Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Rex Invictus original working. Its modelled draw is **304 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E 0.86 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Conjuration]]
        - **Summon Liquid** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-C-L-SL` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Con·None·None·30 feet·Instantaneous` |
| Incantation | *Seusin* |
| Affinity | C (Conjuration) |
| Source | Rex Invictus |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | 30 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Wizard, Sorcerer, Druid |

### Effect

Calls up to 300 kg of a common inert liquid (water, oil, or a chosen simple solution) at a point within range, as a pool or a held globe. Each tier above the first adds roughly e times the volume.

### Mechanism

Field return is spent directly as mass. The liquid is real matter and stays after the working ends.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| conjured inert liquid, 300 kg | `1 Pz/kg*300` | 300 |
| Pattern cost | `0.01 × Q1 × (1 + 0.00)` | 3.5 |

| Quantity | Value |
|---|---|
| Effect energy | 300 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **304 Pz** (455.2 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.867 |
| Energy-equivalent tier T_E | 0.86 |
| Handling points | 0.00 |
| Grade score | -0.07 → L |

**Handling flags:** none.

**Assumptions:** Inert fluid rate 1 Pz/kg; 300 kg at Tier 1 (near Q1 after pattern cost).

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Summon Liquid (1-C-L-SL) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Seusin** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hiseusin* · T3: *Liseusin* · T4: *Viseusin* · T5: *Tiseusin* · T6: *Riseusin* · T7: *Miseusin* · T8: *Niseusin* · T9: *Xyiseusin*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#e3770a`.

![[Summon Liquid (1-C-L-SL) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Conjuration | 0.125 | 1.000 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.995 | `#ff0028` (700 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.981 | `#91ff00` (612 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 2.48. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·C·None`; the k4 to k6 lines (None, 30 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·C·None` |
| Standard spectrometer detection range | 1.74 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.0 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 50.6 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (86.7% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Terrain and Matter Shaping]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Entangle (1-C-M-ENT)|Entangle]] (1) · [[Grease (1-C-L-GRS)|Grease]] (1) · [[Summon Metal (1-C-L-SM)|Summon Metal]] (1) · [[Web (2-C-M-WEB)|Web]] (2) · [[Create Food and Water (3-C-L-CFW)|Create Food and Water]] (3) · [[Create or Destroy Water (1-T-L-CDW)|Create or Destroy Water]] (1) · [[Entangled Attacks (1-E-L-EAT)|Entangled Attacks]] (1) · [[Glue (1-T-L-GLU)|Glue]] (1).


---

## Tactical Assessment

A base material for compound workings. Engineers use it to fill sandbags, flood a bunker floor or feed a binder that turns the fluid into something more useful.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
