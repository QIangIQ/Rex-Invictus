---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-10
  - spell/conjuration
  - source/science-spellbook
aliases:
  - "10th Tier Spell: Supermassive Black Hole"
  - "10-C-X-SBH"
  - "Supermassive Black Hole (Science)"
registry_id: 10-C-X-SBH
attribute_code: "10·Con·Bludgeoning·sphere (5280)·10 miles·Until dispelled"
incantation: "Zyedeg-Saubaris"
tier: 10
school: Conjuration
affinity: C
grade: X
pz_total: 94633734636473.0
pz_quantum: 2836079.4
t_e: 27.32
updated: 2026-11-16
---

**Supermassive Black Hole** (`10-C-X-SBH`) is a 10th Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **94,633,734.64 MPz Pz** against a slot quantum of 2.84 MPz Pz, which puts its energy-equivalent tier at T_E 27.32 and its handling grade at **Extreme**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 10 Workings]]
      - [[Conjuration]]
        - **Supermassive Black Hole** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `10-C-X-SBH` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `10·Con·Bludgeoning·sphere (5280)·10 miles·Until dispelled` |
| Incantation | *Zyedeg-Saubaris* |
| Affinity | C (Conjuration) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 10th Tier |
| School | [[Conjuration]] |
| Casting time | 1 day (uninterupted) |
| Range | 10 miles |
| Area | sphere (5280) |
| Duration | Until dispelled |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: An Onyx orb at least 5 feet in radius, enscribed with the spell |
| Ritual | yes |
| Injury | 40d6 bludgeoning (mean 140) |
| Injury by tier | T10: 40d6, T11: 41d6, T12: 42d6 |
| Resistance check | agility; on success: half injury |
| Practitioner lineages | Wizard, Gods |

### Mechanism

After a day-long working, a lightless sphere 2 miles across appears, annihilating everything inside it, dragging creatures within 3 miles toward it and pelting those near its edge with inflowing debris.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Ground matter annihilated | `8.73e+09 m^3 x 2700 kg/m^3 x 3 Pz/kg` | 70,711,011.51 MPz |
| Air annihilated | `8.73e+09 m^3 x 1.2 kg/m^3 x 1 Pz/kg` | 10,475.71 MPz |
| Inflowing debris | `140 HP x 0.46 (bludgeoning) x S/A_c, S = sphere r=1700.8 m = 36350144.7 m^2 x 3` | 10,032.64 MPz |
| Air inflow consumed (upkeep) | `6.64e+09 kg/s x 1 Pz/kg x 3600 s` | 23,902,214.74 MPz |
| Pattern cost | `0.01 × Q10 × (1 + 0.50)` | 42,541 |

| Quantity | Value |
|---|---|
| Effect energy | 70,731,519.86 MPz Pz |
| Upkeep energy | 23,902,214.74 MPz Pz (6,639.50 MPz Pz/s) |
| **Total draw** | **94,633,734.64 MPz Pz** (141,950,601,954,709.4 kJ) |
| Slot quantum Q10 | 2.84 MPz Pz |
| Field gain (draw / quantum) | 3.34e+07 |
| Energy-equivalent tier T_E | 27.32 |
| Handling points | 0.50 |
| Grade score | 3.50 → X |

**Handling flags:** ritual, long cast.

**Assumptions:** Matter destroyed: half the sphere below ground (2.36e13 kg rock at 3 Pz/kg) and the upper half of air at 1 Pz/kg; debris 40d6 = 140 bludgeoning over the 300 ft band at the horizon, 3 triggers; air inflow at 340 m/s through the upper hemisphere destroyed at 1 Pz/kg for the 1 hour convention used for open durations. Real physics: a 1609 m Schwarzschild radius means 1.08e30 kg and a rest energy near 6.5e43 Pz; the author treats it as a magic approximation, so the described effects are costed instead.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Supermassive Black Hole (10-C-X-SBH) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 10 | 10 | `0000000010101` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | Bludgeoning | 1 | `0000000000011` |
| k4 Area | sphere (5280) | 42 | `0000001010101` |
| k5 Range | 10 miles | 17 | `0000000100011` |
| k6 Duration | Until dispelled | 11 | `0000000010111` |

### Incantation

Spoken as **Zyedeg-Saubaris** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 4→3 | 3 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 | 2 |
| k4 Area | 0→9 2→11 4→0 6→2 | 4 |
| k5 Range | 0→8 1→9 5→0 | 3 |
| k6 Duration | 0→7 1→8 2→9 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#cf6085`.

![[Supermassive Black Hole (10-C-X-SBH) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 10 | 1.000 | 1.000 | `#ff00bf` (400 nm eq.) | source grid |
| Damage | Bludgeoning | 0.143 | 0.693 | `#ff9900` (657 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.682 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Until dispelled | 0.579 | 0.915 | `#00fff7` (526 nm eq.) | source grid |
| Area | sphere (5280) | 0.958 | 0.999 | `#ff00f5` (412 nm eq.) | RI half-step |
| Range | 10 miles | 0.088 | 0.660 | `#ff4d00` (674 nm eq.) | RI half-step |

Relative luminosity scales with initial energy: log10(E) = 13.98. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `10·C·Bludgeoning`; the k4 to k6 lines (sphere (5280), 10 miles, Until dispelled) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `10·C·Bludgeoning` |
| Standard spectrometer detection range | 972,798.72 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 141,804 Pz (0.05 × Q10) |
| Counter drawn cold (all six layers) | 283,608 Pz (0.10 × Q10) |
| Unravel after completion | 4,780,443.23 MPz Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Within, Rigidity, 2x Movement and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1e 1F 1H 3j` (Prodigious, Potential, Rigidity, 3x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 15,772,289.11 MPz Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 33367801.86 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 10th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Endures independently once set, which places it under the decay clause of ULMTU-XIII. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIII]] | Lex Impermanentiae | Long-lived patterns drift toward reversion unless refreshed from a source that satisfies ULMTU-I. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVI]] | Lex Interdictorum | Exceeds 100 MPz; requires direct acknowledgement from the [[Répertoire du Savoir Athénien]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 10th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 10 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Area Destruction]] |
| Element | [[Bludgeoning Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Extreme]] |

Similar workings: [[Storm of Vengeance (9-C-M-SV)|Storm of Vengeance]] (9) · [[Supersonic Omnidirectional Jet (5-C-M-SOJ)|Supersonic Omnidirectional Jet]] (5) · [[Wormhole (9-P-L-WRM)|Wormhole]] (9) · [[Black Tentacles (4-C-L-BT)|Black Tentacles]] (4) · [[Incendiary Cloud (8-C-M-IC)|Incendiary Cloud]] (8) · [[Eruption (9-V-M-ERP)|Eruption]] (9) · [[Meteor Swarm (9-V-L-MST)|Meteor Swarm]] (9) · [[Starburst (9-A-L-STR)|Starburst]] (9).


---

## Tactical Assessment

Strategic area annihilation and a permanent barrier until removed; dangerous to the caster's own side within miles.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 10 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
