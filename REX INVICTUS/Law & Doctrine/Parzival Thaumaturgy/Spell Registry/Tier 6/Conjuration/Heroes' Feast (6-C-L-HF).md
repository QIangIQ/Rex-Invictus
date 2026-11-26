---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-6
  - spell/conjuration
  - source/srd
aliases:
  - "6th Tier Spell: Heroes' Feast"
  - "Heroes' Feast"
  - "6-C-L-HF"
registry_id: 6-C-L-HF
attribute_code: "6·Con·None·None·30 feet·Instantaneous"
incantation: "Reusin"
tier: 6
school: Conjuration
affinity: C
grade: L
pz_total: 7078.1
pz_quantum: 51944.6
t_e: 4.01
updated: 2026-11-16
---

**Heroes' Feast** (`6-C-L-HF`) is a 6th Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **7,078 Pz** against a slot quantum of 51,945 Pz, which puts its energy-equivalent tier at T_E 4.01 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 6 Workings]]
      - [[Conjuration]]
        - **Heroes' Feast** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `6-C-L-HF` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `6·Con·None·None·30 feet·Instantaneous` |
| Incantation | *Reusin* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 6th Tier |
| School | [[Conjuration]] |
| Casting time | 10 minutes |
| Range | 30 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A gem-encrusted bowl worth at least 1,000gp, which the spell consumes |
| Ritual | no |
| Practitioner lineages | Cleric, Druid |

### Mechanism

Conjures a meal for twelve that, once eaten over an hour, purges toxins and disease and grants a day of poison and fear immunity, firmer will and greater vitality.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| feast matter | `10 Pz/kg * 12 * 2 kg` | 240 |
| nutritional energy | `0.01*12*2000*4184/1500  [C3]` | 669 |
| vitality increase, 2d10=11 each | `0.30 Pz * 11 HP * 12` | 39.6 |
| disease and poison cure | `0.30 Pz * 10 HP-equivalent * 12` | 36.0 |
| 24 h immunities and resolve | `0.005 Pz/s * 12 * 86400 s` | 5,184 |
| Pattern cost | `0.01 × Q6 × (1 + 0.75)` | 909 |

| Quantity | Value |
|---|---|
| Effect energy | 6,169 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **7,078 Pz** (10,617.1 kJ) |
| Slot quantum Q6 | 51,945 Pz |
| Field gain (draw / quantum) | 0.136 |
| Energy-equivalent tier T_E | 4.01 |
| Handling points | 0.75 |
| Grade score | -0.25 → L |

Calibration applied: C3 (Borrowed sustenance), see [[Parzival Energy Budget#Registry calibration rules]].

**Handling flags:** costly material, consumed material, long cast.

**Assumptions:** 12 partakers, 2 kg food and 2000 kcal each; immunities at enchantment rate for 24 h paid at casting.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Heroes' Feast (6-C-L-HF) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 6 | 6 | `0000000001101` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Reusin** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T7: *Mireusin* · T8: *Nireusin* · T9: *Xyireusin*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 3→2 | 3 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#9da14e`.

![[Heroes' Feast (6-C-L-HF) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 6 | 0.600 | 1.000 | `#00ebff` (520 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.893 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.835 | `#ff0028` (700 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.954 | `#91ff00` (612 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.18): swatch `#bd9f70`, measured lines at 0.004, 0.126, 0.295, 0.601. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.85. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `6·C·None`; the k4 to k6 lines (None, 30 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `6·C·None` |
| Standard spectrometer detection range | 8.41 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 2,597 Pz (0.05 × Q6) |
| Counter drawn cold (all six layers) | 5,194 Pz (0.10 × Q6) |
| Unravel after completion | 5,194 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1,180 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 6th Tier quantum of 51,945 Pz (13.6% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
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
| Function | [[Healing and Restoration]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Mass Cure Wounds (5-C-L-MCW)|Mass Cure Wounds]] (5) · [[Heal (6-V-L-HEA)|Heal]] (6) · [[Greater Restoration (5-A-L-GRE)|Greater Restoration]] (5) · [[Mass Heal (9-C-L-MHS)|Mass Heal]] (9) · [[Raise Dead (5-N-M-RD)|Raise Dead]] (5) · [[Regenerate (7-T-L-RGN)|Regenerate]] (7) · [[Reincarnate (5-T-M-RNC)|Reincarnate]] (5) · [[Resurrection (7-N-L-RSR)|Resurrection]] (7).


---

## Tactical Assessment

A pre-mission preparation for a strike team facing chemical, biological or fear-based weapons.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 6 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
