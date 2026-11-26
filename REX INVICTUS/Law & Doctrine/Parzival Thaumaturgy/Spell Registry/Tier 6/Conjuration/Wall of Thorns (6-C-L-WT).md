---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-6
  - spell/conjuration
  - source/srd
aliases:
  - "6th Tier Spell: Wall of Thorns"
  - "Wall of Thorns"
  - "6-C-L-WT"
registry_id: 6-C-L-WT
attribute_code: "6·Con·Piercing·line (60)·120 feet·Up to 10 minutes"
incantation: "Reix-Lemully"
tier: 6
school: Conjuration
affinity: C
grade: L
pz_total: 50899.3
pz_quantum: 51944.6
t_e: 5.98
updated: 2026-11-16
---

**Wall of Thorns** (`6-C-L-WT`) is a 6th Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **50,899 Pz** against a slot quantum of 51,945 Pz, which puts its energy-equivalent tier at T_E 5.98 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 6 Workings]]
      - [[Conjuration]]
        - **Wall of Thorns** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `6-C-L-WT` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `6·Con·Piercing·line (60)·120 feet·Up to 10 minutes` |
| Incantation | *Reix-Lemully* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 6th Tier |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | 120 feet |
| Area | line (60) |
| Duration | Up to 10 minutes (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A handful of thorns |
| Ritual | no |
| Injury | 7d8 piercing (mean 31.5) |
| Injury by tier | T6: 7d8, T7: 8d8, T8: 9d8, T9: 10d8 |
| Resistance check | agility; on success: half injury |
| Practitioner lineages | Druid |

### Mechanism

A dense hedge of living thorned brush, 18 m by 3 m by 1.5 m, grows instantly, blocking sight and tearing anyone forcing a way through.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Conjured living brush | `10 Pz/kg * 4248 kg (85.0 m^3 * 50 kg/m^3)` | 42,480 |
| Piercing on formation | `31.5 * 0.35 * 111 / 0.7` | 1,756 |
| Slashing on passage, 3 triggers | `31.5 * 0.40 * 111 / 0.7 * 3` | 6,020 |
| Pattern cost | `0.01 × Q6 × (1 + 0.25)` | 649 |

| Quantity | Value |
|---|---|
| Effect energy | 50,250 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **50,899 Pz** (76,349.0 kJ) |
| Slot quantum Q6 | 51,945 Pz |
| Field gain (draw / quantum) | 0.98 |
| Energy-equivalent tier T_E | 5.98 |
| Handling points | 0.25 |
| Grade score | 0.24 → L |

**Handling flags:** concentration.

**Assumptions:** Brush bulk density 50 kg/m^3; 7d8 = 31.5; 3 passage triggers.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Wall of Thorns (6-C-L-WT) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 6 | 6 | `0000000001101` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | Piercing | 8 | `0000000010001` |
| k4 Area | line (60) | 25 | `0000000110011` |
| k5 Range | 120 feet | 3 | `0000000000111` |
| k6 Duration | Up to 10 minutes | 15 | `0000000011111` |

### Incantation

Spoken as **Reix-Lemully** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T7: *Mireix-Lemully* · T8: *Nireix-Lemully* · T9: *Xyireix-Lemully*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 3→2 | 3 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 4→1 | 2 |
| k4 Area | 0→9 1→10 4→0 5→1 | 4 |
| k5 Range | 0→8 1→9 2→10 | 3 |
| k6 Duration | 0→7 1→8 2→9 3→10 4→11 | 5 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#549aac`.

![[Wall of Thorns (6-C-L-WT) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 6 | 0.600 | 1.000 | `#00ebff` (520 nm eq.) | source grid |
| Damage | Piercing | 0.571 | 1.000 | `#00ffec` (529 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.893 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Up to 10 minutes | 0.789 | 0.982 | `#1e00ff` (463 nm eq.) | source grid |
| Area | line (60) | 0.694 | 0.996 | `#0069ff` (492 nm eq.) | source grid |
| Range | 120 feet | 0.176 | 0.914 | `#ffc900` (647 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 4.71. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `6·C·Piercing`; the k4 to k6 lines (line (60), 120 feet, Up to 10 minutes) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `6·C·Piercing` |
| Standard spectrometer detection range | 22.56 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 2,597 Pz (0.05 × Q6) |
| Counter drawn cold (all six layers) | 5,194 Pz (0.10 × Q6) |
| Unravel after completion | 5,194 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Beyond, Cold, Hopelessness, Movement and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `2a 1B 1e 1F 1I 2j` (2x Beyond, Cold, Prodigious, Potential, Hopelessness, 2x Movement).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 8,483 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 6th Tier quantum of 51,945 Pz (98.0% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 6th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 6 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Walls and Barriers]], [[Area Destruction]] |
| Element | [[Piercing Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Insect Plague (5-C-L-IP)|Insect Plague]] (5) · [[Blade Barrier (6-V-L-BB)|Blade Barrier]] (6) · [[Wall of Ice (6-V-M-WI)|Wall of Ice]] (6) · [[Wall of Fire (4-V-M-WF)|Wall of Fire]] (4) · [[Cloudkill (5-C-L-CLD)|Cloudkill]] (5) · [[Magic Polarising Filter (Simplified) (5-C-L-MPFS)|Magic Polarising Filter (Simplified)]] (5) · [[Supersonic Omnidirectional Jet (5-C-M-SOJ)|Supersonic Omnidirectional Jet]] (5) · [[Wind Wall (3-V-L-WWN)|Wind Wall]] (3).


---

## Tactical Assessment

Obstacle belt against infantry; armoured vehicles push through but at reduced speed.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 6 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
