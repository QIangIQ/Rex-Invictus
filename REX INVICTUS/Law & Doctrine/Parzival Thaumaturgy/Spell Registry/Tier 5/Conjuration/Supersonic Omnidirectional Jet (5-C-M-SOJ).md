---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/conjuration
  - source/science-spellbook
aliases:
  - "5th Tier Spell: Supersonic Omnidirectional Jet"
  - "5-C-M-SOJ"
  - "Supersonic Omnidirectional Jet (Science)"
registry_id: 5-C-M-SOJ
attribute_code: "5·Con·Bludgeoning·sphere (30)·60 feet·Instantaneous"
incantation: "Tedeg-Sorwyn"
tier: 5
school: Conjuration
affinity: C
grade: M
pz_total: 91696.8
pz_quantum: 19109.4
t_e: 6.57
updated: 2026-11-16
---

**Supersonic Omnidirectional Jet** (`5-C-M-SOJ`) is a 5th Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **91,697 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 6.57 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Conjuration]]
        - **Supersonic Omnidirectional Jet** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-C-M-SOJ` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Con·Bludgeoning·sphere (30)·60 feet·Instantaneous` |
| Incantation | *Tedeg-Sorwyn* |
| Affinity | C (Conjuration) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Conjuration]] |
| Casting time | 1 Action |
| Range | 60 feet |
| Area | sphere (30) |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Water |
| Ritual | no |
| Injury | 3d8 bludgeoning (mean 13.5) |
| Injury by tier | T5: 3d8, T6: 4d8, T7: 5d8, T8: 6d8, T9: 7d8 |
| Resistance check | constitution; on success: half injury |
| Practitioner lineages | Wizard |

### Mechanism

Conjures a 5 ft sphere of water and blasts it outward at supersonic speed to 30 ft, battering and chilling everything exposed.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Water conjured | `1853 kg x 1 Pz/kg` | 1,853 |
| Supersonic water jet | `0.5 x 1853 kg x (340 m/s)^2 = 1.071e+08 J / 1500` | 71,415 |
| Chilling spray | `13.5 HP x 0.9 (cold) x S/A_c, S = sphere r=9.144 m = 1050.7 m^2` | 18,237 |
| Pattern cost | `0.01 × Q5 × (1 + 0.00)` | 191 |

| Quantity | Value |
|---|---|
| Effect energy | 91,506 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **91,697 Pz** (137,545.3 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 4.8 |
| Energy-equivalent tier T_E | 6.57 |
| Handling points | 0.00 |
| Grade score | 0.78 → M |

**Handling flags:** none.

**Assumptions:** Water sphere 5 ft diameter (1853 kg) at 1 Pz/kg; kinetic energy of the water at 340 m/s (real physics, replaces the impact term); cold 3d8 = 13.5 over a 30 ft sphere.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Supersonic Omnidirectional Jet (5-C-M-SOJ) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | Bludgeoning | 1 | `0000000000011` |
| k4 Area | sphere (30) | 31 | `0000000111111` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Tedeg-Sorwyn** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Ritedeg-Sorwyn* · T7: *Mitedeg-Sorwyn* · T8: *Nitedeg-Sorwyn* · T9: *Xyitedeg-Sorwyn*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 | 2 |
| k4 Area | 0→9 1→10 2→11 3→12 4→0 5→1 | 6 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#908775`.

![[Supersonic Omnidirectional Jet (5-C-M-SOJ) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| Damage | Bludgeoning | 0.143 | 0.938 | `#ff9900` (657 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.932 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.882 | `#ff0028` (700 nm eq.) | source grid |
| Area | sphere (30) | 0.861 | 0.937 | `#8000ff` (442 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.996 | `#00fbff` (524 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 4.96. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·C·Bludgeoning`; the k4 to k6 lines (sphere (30), 60 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·C·Bludgeoning` |
| Standard spectrometer detection range | 30.28 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 1,911 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Within, Rigidity, 2x Movement and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1e 1F 1H 3j` (Prodigious, Potential, Rigidity, 3x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 15,283 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 4.80 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 5th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
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
| Function | [[Area Destruction]] |
| Element | [[Bludgeoning Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Black Tentacles (4-C-L-BT)|Black Tentacles]] (4) · [[Control Water (4-T-H-CWN)|Control Water]] (4) · [[Ice Storm (4-V-L-ISE)|Ice Storm]] (4) · [[Cloudkill (5-C-L-CLD)|Cloudkill]] (5) · [[Insect Plague (5-C-L-IP)|Insect Plague]] (5) · [[Wind Wall (3-V-L-WWN)|Wind Wall]] (3) · [[Geyser (2-V-L-GYS)|Geyser]] (2) · [[Guardian of Faith (4-C-L-GFA)|Guardian of Faith]] (4).


---

## Tactical Assessment

Clears a room or deck and puts out fires in the same action.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
