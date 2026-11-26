---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-4
  - spell/evocation
  - source/srd
aliases:
  - "4th Tier Spell: Resilient Sphere"
  - "Resilient Sphere"
  - "4-P-L-RS"
registry_id: 4-P-L-RS
attribute_code: "4·Evo·None·None·30 feet·Up to 1 minute"
incantation: "Vuusinse"
tier: 4
school: Evocation
affinity: P
grade: L
pz_total: 165.4
pz_quantum: 7029.9
t_e: 0.25
updated: 2026-11-16
---

**Resilient Sphere** (`4-P-L-RS`) is a 4th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **165 Pz** against a slot quantum of 7,030 Pz, which puts its energy-equivalent tier at T_E 0.25 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 4 Workings]]
      - [[Evocation]]
        - **Resilient Sphere** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `4-P-L-RS` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `4·Evo·None·None·30 feet·Up to 1 minute` |
| Incantation | *Vuusinse* |
| Affinity | P (Pure field construct) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 4th Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 30 feet |
| Area | single point or target |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A hemispherical piece of clear crystal and a matching hemispherical piece of gum arabic |
| Ritual | no |
| Resistance check | agility; on success: no effect |
| Practitioner lineages | Wizard |

### Mechanism

A closed force shell forms around a creature or object and blocks matter, energy and workings in both directions while letting air through.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| absorbed attacks on sphere, 30 points/round over 10 rounds | `0.20*30*10` | 60.0 |
| Pattern cost | `0.01 × Q4 × (1 + 0.50)` | 105 |

| Quantity | Value |
|---|---|
| Effect energy | 60.0 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **165 Pz** (248.2 kJ) |
| Slot quantum Q4 | 7,030 Pz |
| Field gain (draw / quantum) | 0.0235 |
| Energy-equivalent tier T_E | 0.25 |
| Handling points | 0.50 |
| Grade score | -0.50 → L |

**Handling flags:** concentration, save or suck.

**Assumptions:** Expected 30 points per round directed at the shell for 10 rounds.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Resilient Sphere (4-P-L-RS) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 4 | 4 | `0000000001001` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Vuusinse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T5: *Tivuusinse* · T6: *Rivuusinse* · T7: *Mivuusinse* · T8: *Nivuusinse* · T9: *Xyivuusinse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 3→2 | 2 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#24dd61`.

![[Resilient Sphere (4-P-L-RS) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 4 | 0.400 | 1.000 | `#00ff00` (580 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.995 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.960 | `#0074ff` (495 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.994 | `#91ff00` (612 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.22): swatch `#93eca6`, measured lines at 0.295, 0.401, 0.501, 0.685. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.22. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `4·V·None`; the k4 to k6 lines (None, 30 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `4·V·None` |
| Standard spectrometer detection range | 1.29 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 351 Pz (0.05 × Q4) |
| Counter drawn cold (all six layers) | 703 Pz (0.10 × Q4) |
| Unravel after completion | 703 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1b 1c 1d 1f` (Heat, Light, Life, Energy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 27.6 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 4th Tier quantum of 7,030 Pz (2.4% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 4th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 4 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Pure]] (P) |
| Function | [[Wards and Shields]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Fire Shield (4-V-L-FSR)|Fire Shield]] (4) · [[Hallow (5-V-L-HLL)|Hallow]] (5) · [[Wall of Force (5-P-L-WFL)|Wall of Force]] (5) · [[Death Ward (4-A-L-DW)|Death Ward]] (4) · [[Stoneskin (4-A-L-STN)|Stoneskin]] (4) · [[Bulwark (3-A-L-BLW)|Bulwark]] (3) · [[Forcecage (7-P-L-FRC)|Forcecage]] (7) · [[Glyph of Warding (3-A-H-GWY)|Glyph of Warding]] (3).


---

## Tactical Assessment

Isolates a single enemy from the fight or shelters an ally or device from fire for a minute.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 4 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
