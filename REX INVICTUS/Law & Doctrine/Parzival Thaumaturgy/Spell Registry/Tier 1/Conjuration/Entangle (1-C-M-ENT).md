---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/conjuration
  - source/srd
aliases:
  - "1st Tier Spell: Entangle"
  - "Entangle"
  - "1-C-M-ENT"
registry_id: 1-C-M-ENT
attribute_code: "1·Con·None·cube (20)·90 feet·Up to 1 minute"
incantation: "Se’-Boylarse"
tier: 1
school: Conjuration
affinity: C
grade: M
pz_total: 748.5
pz_quantum: 350.0
t_e: 1.76
updated: 2026-11-16
---

**Entangle** (`1-C-M-ENT`) is a 1st Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **748 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E 1.76 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Conjuration]]
        - **Entangle** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-C-M-ENT` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Con·None·cube (20)·90 feet·Up to 1 minute` |
| Incantation | *Se’-Boylarse* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | 90 feet |
| Area | cube (20) |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Resistance check | strength; on success: no effect |
| Practitioner lineages | Druid |

### Mechanism

The field grows grasping weeds over a 20 ft square, slowing movement and binding those caught until they break free.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| vine biomass 2 kg/m2 over 20 ft square | `10*2*(20*ft)**2` | 743 |
| Pattern cost | `0.01 × Q1 × (1 + 0.50)` | 5.2 |

| Quantity | Value |
|---|---|
| Effect energy | 743 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **748 Pz** (1,122.7 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 2.14 |
| Energy-equivalent tier T_E | 1.76 |
| Handling points | 0.50 |
| Grade score | 0.88 → M |

**Handling flags:** concentration, save or suck.

**Assumptions:** Biomass 2 kg/m2 at 10 Pz/kg.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Entangle (1-C-M-ENT) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | cube (20) | 9 | `0000000010011` |
| k5 Range | 90 feet | 11 | `0000000010111` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Se’-Boylarse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hise’-Boylarse* · T3: *Lise’-Boylarse* · T4: *Vise’-Boylarse* · T5: *Tise’-Boylarse* · T6: *Rise’-Boylarse* · T7: *Mise’-Boylarse* · T8: *Nise’-Boylarse* · T9: *Xyise’-Boylarse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 4→0 | 3 |
| k5 Range | 0→8 1→9 2→10 4→12 | 4 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#97995c`.

![[Entangle (1-C-M-ENT) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Conjuration | 0.125 | 1.000 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.843 | `#0074ff` (495 nm eq.) | source grid |
| Area | cube (20) | 0.250 | 0.989 | `#cdff00` (625 nm eq.) | source grid |
| Range | 90 feet | 0.647 | 0.861 | `#00aaff` (506 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.16): swatch `#c58461`, measured lines at 0.101, 0.126, 0.251, 0.648, 0.685. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.87. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·C·None`; the k4 to k6 lines (cube (20), 90 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·C·None` |
| Standard spectrometer detection range | 2.74 km (r = 1 km × √(E/100 Pz)) |
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
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 125 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 2.14 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 1st Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
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
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Grease (1-C-L-GRS)|Grease]] (1) · [[Summon Liquid (1-C-L-SL)|Summon Liquid]] (1) · [[Summon Metal (1-C-L-SM)|Summon Metal]] (1) · [[Web (2-C-M-WEB)|Web]] (2) · [[Create Food and Water (3-C-L-CFW)|Create Food and Water]] (3) · [[Create or Destroy Water (1-T-L-CDW)|Create or Destroy Water]] (1) · [[Entangled Attacks (1-E-L-EAT)|Entangled Attacks]] (1) · [[Glue (1-T-L-GLU)|Glue]] (1).


---

## Tactical Assessment

Area denial against infantry for a minute; ineffective against vehicles.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
