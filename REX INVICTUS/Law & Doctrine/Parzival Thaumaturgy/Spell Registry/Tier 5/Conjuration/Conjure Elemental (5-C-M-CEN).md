---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/conjuration
  - source/srd
aliases:
  - "5th Tier Spell: Conjure Elemental"
  - "Conjure Elemental"
  - "5-C-M-CEN"
registry_id: 5-C-M-CEN
attribute_code: "5·Con·None·cube (10)·90 feet·Up to 1 hour"
incantation: "Te’-Beylarsi"
tier: 5
school: Conjuration
affinity: C
grade: M
pz_total: 20466.6
pz_quantum: 19109.4
t_e: 5.07
updated: 2026-11-16
---

**Conjure Elemental** (`5-C-M-CEN`) is a 5th Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **20,467 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 5.07 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Conjuration]]
        - **Conjure Elemental** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-C-M-CEN` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Con·None·cube (10)·90 feet·Up to 1 hour` |
| Incantation | *Te’-Beylarsi* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Conjuration]] |
| Casting time | 1 minute |
| Range | 90 feet |
| Area | cube (10) |
| Duration | Up to 1 hour (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Burning incense for air, soft clay for earth, sulfur and phosphorus for fire, or water and sand for water |
| Ritual | no |
| Practitioner lineages | Druid, Wizard |

### Mechanism

The field gathers air, earth, fire or water from a 10 ft cube of source material and binds it into a self-directing body that answers spoken orders. If the caster loses the link, the body persists for up to an hour under its own will.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| elemental body assembled from local element | `10*2000` | 20,000 |
| upkeep: autonomy of 1 creature for 1 h | `0.05*1*3600` | 180 |
| Pattern cost | `0.01 × Q5 × (1 + 0.50)` | 287 |

| Quantity | Value |
|---|---|
| Effect energy | 20,000 Pz |
| Upkeep energy | 180 Pz (0.05 Pz/s) |
| **Total draw** | **20,467 Pz** (30,700.0 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 1.07 |
| Energy-equivalent tier T_E | 5.07 |
| Handling points | 0.50 |
| Grade score | 0.53 → M |

**Handling flags:** concentration, long cast.

**Assumptions:** Representative elemental body 2000 kg (earth types heavier, air types lighter); body cost 10 Pz/kg; upkeep 0.05 Pz/s for full 1 h.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Conjure Elemental (5-C-M-CEN) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | cube (10) | 5 | `0000000001011` |
| k5 Range | 90 feet | 11 | `0000000010111` |
| k6 Duration | Up to 1 hour | 12 | `0000000011001` |

### Incantation

Spoken as **Te’-Beylarsi** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Rite’-Beylarsi* · T7: *Mite’-Beylarsi* · T8: *Nite’-Beylarsi* · T9: *Xyite’-Beylarsi*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 3→12 | 3 |
| k5 Range | 0→8 1→9 2→10 4→12 | 4 |
| k6 Duration | 0→7 3→10 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#62b484`.

![[Conjure Elemental (5-C-M-CEN) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.932 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Up to 1 hour | 0.632 | 0.991 | `#00c0ff` (511 nm eq.) | source grid |
| Area | cube (10) | 0.139 | 0.937 | `#ff9300` (658 nm eq.) | source grid |
| Range | 90 feet | 0.647 | 0.989 | `#00aaff` (506 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.15): swatch `#9cb98c`, measured lines at 0.124, 0.139, 0.501, 0.632, 0.648. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.31. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·C·None`; the k4 to k6 lines (cube (10), 90 feet, Up to 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·C·None` |
| Standard spectrometer detection range | 14.31 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 1,947 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 3,411 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 1.07 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 5th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 5th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 5 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Summoning and Conjured Creatures]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Conjure Fey (6-C-L-CFN)|Conjure Fey]] (6) · [[Conjure Magic Prism (4-C-L-CMPJ)|Conjure Magic Prism]] (4) · [[Conjure Minor Elementals (4-C-M-CME)|Conjure Minor Elementals]] (4) · [[Conjure Woodland Beings (4-C-L-CWB)|Conjure Woodland Beings]] (4) · [[Faithful Hound (4-C-L-FH)|Faithful Hound]] (4) · [[Guardian of Faith (4-C-L-GFA)|Guardian of Faith]] (4) · [[Instant Summons (6-C-L-ISS)|Instant Summons]] (6) · [[Magic Polarising Filter (4-C-L-MPF)|Magic Polarising Filter]] (4).


---

## Tactical Assessment

A field-raised heavy combatant usable as a breaching or blocking asset; loss of the caster link turns it into a hostile hazard, so doctrine pairs it with protected casters.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
