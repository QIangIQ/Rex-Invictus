---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/transmutation
  - source/science-spellbook
aliases:
  - "4th Tier Spell: Planetary Rings"
  - "4-P-L-PR"
  - "Planetary Rings (Science)"
registry_id: 4-P-L-PR
attribute_code: "4·Tra·Force·sphere (5)·Self·10 minutes"
incantation: "Vieton-Supors"
tier: 4
school: Transmutation
affinity: P
grade: L
pz_total: 507.5
pz_quantum: 7029.9
t_e: 1.37
updated: 2026-11-16
---

**Planetary Rings** (`4-P-L-PR`) is a 4th Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **507 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E 1.37 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Transmutation]]
        - **Planetary Rings** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-P-L-PR` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Tra·Force·sphere (5)·Self·10 minutes` |
| Incantation | *Vieton-Supors* |
| Affinity | P (Pure field construct) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Transmutation]] |
| Casting time | 1 Action |
| Range | Self |
| Area | sphere (5) |
| Duration | 10 minutes |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A ring |
| Ritual | no |
| Injury | 3d6 force (mean 10.5) |
| Injury by tier | T4: 3d6, T5: 3d6, T6: 3d6, T7: 3d6, T8: 3d6, T9: 3d6 |
| Resistance check | strength; on success: half injury |
| Delivery | aimed ranged working |
| Practitioner lineages | Wizard, Sorcerer |

### Mechanism

Three rings of orbiting debris circle the caster, battering anyone who lingers close and each able to be hurled once at a target.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Debris rings conjured | `15 kg x 3 Pz/kg` | 45.0 |
| Orbital motion | `0.5 x 15 kg x (10 m/s)^2 = 750 J / 1500` | 0.5 |
| Ring launches | `10.5 HP x 0.4 (force) x F 0.5 x 3 targets/projectiles` | 6.3 |
| Debris aura | `7 HP x 0.4 (force) x S/A_c, S = sphere r=1.524 m = 29.2 m^2 x 3` | 350 |
| Pattern cost | `0.01 × Q4 × (1 + 0.50)` | 105 |

| Quantity | Value |
|---|---|
| Effect energy | 402 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **507 Pz** (761.2 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 0.0722 |
| Energy-equivalent tier T_E | 1.37 |
| Handling points | 0.50 |
| Grade score | -0.50 → L |

**Handling flags:** multi target control.

**Assumptions:** Rings 5 kg each at 3 Pz/kg orbiting at 10 m/s; each launch 3d6 = 10.5 force ray F 0.5; aura 2d6 = 7 force over a 5 ft sphere, 3 triggers.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Planetary Rings (4-P-L-PR) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 4 | 4 | `0000000001001` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | Force | 4 | `0000000001001` |
| k4 Area | sphere (5) | 34 | `0000001000101` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | 10 minutes | 4 | `0000000001001` |

### Incantation

Spoken as **Vieton-Supors** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T5: *Tivieton-Supors* · T6: *Rivieton-Supors* · T7: *Mivieton-Supors* · T8: *Nivieton-Supors* · T9: *Xyivieton-Supors*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 3→2 | 2 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 3→0 | 2 |
| k4 Area | 0→9 2→11 6→2 | 3 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 3→10 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#679479`.

![[Planetary Rings (4-P-L-PR) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| Damage | Force | 0.357 | 0.999 | `#3bff00` (593 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.893 | `#9600ff` (438 nm eq.) | source grid |
| Duration | 10 minutes | 0.263 | 0.991 | `#bdff00` (621 nm eq.) | source grid |
| Area | sphere (5) | 0.944 | 0.862 | `#f200ff` (417 nm eq.) | source grid |
| Range | Self | 0.706 | 0.954 | `#0058ff` (488 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 2.71. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·T·Force`; the k4 to k6 lines (sphere (5), Self, 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·T·Force` |
| Standard spectrometer detection range | 2.25 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 703 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Beyond, Introspection, 2x Movement and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1d 1G 2h 3j` (Beyond, Life, Introspection, 2x Flexibility, 3x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 84.6 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 4th Tier quantum of 7,030 Pz (7.2% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 4th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 4 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Pure]] (P) |
| Function | [[Area Destruction]] |
| Element | [[Force Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Disintegrate (6-P-L-DSN)|Disintegrate]] (6) · [[Sonic Boom (3-P-L-SBN)|Sonic Boom]] (3) · [[Turbulent Gas (3-P-L-TG)|Turbulent Gas]] (3) · [[Bohr's Model (2-P-L-BSM)|Bohr's Model]] (2) · [[Control Water (4-T-H-CWN)|Control Water]] (4) · [[Tidal Force (4-P-L-TF)|Tidal Force]] (4) · [[Black Tentacles (4-C-L-BT)|Black Tentacles]] (4) · [[Dimension Door (4-P-L-DD)|Dimension Door]] (4).


---

## Tactical Assessment

Close defence plus three ranged shots for a forward caster.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
