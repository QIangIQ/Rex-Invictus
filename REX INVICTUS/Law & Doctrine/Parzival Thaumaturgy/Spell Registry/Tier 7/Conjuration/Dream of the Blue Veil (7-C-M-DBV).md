---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-7
  - spell/conjuration
  - source/rex-invictus
aliases:
  - "7th Tier Spell: Dream of the Blue Veil"
  - "Dream of the Blue Veil"
  - "7-C-M-DBV"
registry_id: 7-C-M-DBV
attribute_code: "7·Con·None·None·20 feet·6 hours"
incantation: "Mebanba"
tier: 7
school: Conjuration
affinity: C
grade: M
pz_total: 76502.0
pz_quantum: 141200.1
t_e: 6.39
updated: 2026-11-16
---

**Dream of the Blue Veil** (`7-C-M-DBV`) is a 7th Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Rex Invictus original working. Its modelled draw is **76,502 Pz** against a slot quantum of 141,200 Pz, which puts its energy-equivalent tier at T_E 6.39 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 7 Workings]]
      - [[Conjuration]]
        - **Dream of the Blue Veil** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `7-C-M-DBV` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `7·Con·None·None·20 feet·6 hours` |
| Incantation | *Mebanba* |
| Affinity | C (Conjuration) |
| Source | Rex Invictus |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 7th Tier |
| School | [[Conjuration]] |
| Casting time | 10 minutes |
| Range | 20 feet |
| Area | single point or target |
| Duration | 6 hours |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: a magic item or a willing creature from the destination world |
| Ritual | no |
| Practitioner lineages | Bard, Sorcerer, Warlock, Wizard |

### Effect

The caster and up to eight willing creatures fall into a shared trance and wake on another world of the same material plane, one the caster has a token or a native from. Any target who takes injury, or who is intercepted by a being of equal or greater power, drops out of the transfer. If the caster takes injury, no one is carried.

### Mechanism

Carries the sleepers along the Mist from one world to another without crossing a plane boundary. The transfer is held by the caster's trance, which is why any injury breaks it.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| translocation, 9 bodies, interworld jump | `0.01*720*15*1e6/1500` | 72,000 |
| [upkeep] shared trance, 9 bodies, 6 h | `0.005*9*21600` | 972 |
| Pattern cost | `0.01 × Q7 × (1 + 1.50)` | 3,530 |

| Quantity | Value |
|---|---|
| Effect energy | 72,000 Pz |
| Upkeep energy | 972 Pz (0.045 Pz/s) |
| **Total draw** | **76,502 Pz** (114,753.0 kJ) |
| Slot quantum Q7 | 141,200 Pz |
| Field gain (draw / quantum) | 0.542 |
| Energy-equivalent tier T_E | 6.39 |
| Handling points | 1.50 |
| Grade score | 1.19 → M |

**Handling flags:** costly material, fragile, long cast.

**Assumptions:** Interworld distance priced like a plane boundary (1e6 m); 80 kg per traveller; trance hold at the enchantment rate.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Dream of the Blue Veil (7-C-M-DBV) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 7 | 7 | `0000000001111` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 20 feet | 19 | `0000000100111` |
| k6 Duration | 6 hours | 21 | `0000000101011` |

### Incantation

Spoken as **Mebanba** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T8: *Nimebanba* · T9: *Xyimebanba*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 3→2 | 4 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 5→0 | 4 |
| k6 Duration | 0→7 1→8 3→10 5→12 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#69b744`.

![[Dream of the Blue Veil (7-C-M-DBV) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 7 | 0.700 | 1.000 | `#005eff` (490 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.848 | `#ff8300` (662 nm eq.) | source grid |
| Duration | 6 hours | 0.395 | 0.954 | `#05ff00` (582 nm eq.) | RI half-step |
| Range | 20 feet | 0.265 | 0.910 | `#bdff00` (621 nm eq.) | RI half-step |

Relative luminosity scales with initial energy: log10(E) = 4.88. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `7·C·None`; the k4 to k6 lines (None, 20 feet, 6 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `7·C·None` |
| Standard spectrometer detection range | 27.66 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 7,060 Pz (0.05 × Q7) |
| Counter drawn cold (all six layers) | 14,120 Pz (0.10 × Q7) |
| Unravel after completion | 14,314 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 12,750 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 7th Tier quantum of 141,200 Pz (54.2% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 7th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 7 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Teleportation and Planar Travel]], [[Concealment and Illusion]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Magnificent Mansion (7-C-M-MMN)|Magnificent Mansion]] (7) · [[Plane Shift (7-C-L-PSN)|Plane Shift]] (7) · [[Teleport (7-C-L-TLP)|Teleport]] (7) · [[Demiplane (8-C-L-DMP)|Demiplane]] (8) · [[Maze (8-C-L-MAZ)|Maze]] (8) · [[Misted Leap (2-C-L-ML)|Misted Leap]] (2) · [[Transport via Plants (6-C-L-TP)|Transport via Plants]] (6) · [[Word of Recall (6-C-L-WR)|Word of Recall]] (6).


---

## Tactical Assessment

Strategic insertion and evacuation between worlds. Its fragility makes it a rear-area working that needs guarded casters.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 7 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
