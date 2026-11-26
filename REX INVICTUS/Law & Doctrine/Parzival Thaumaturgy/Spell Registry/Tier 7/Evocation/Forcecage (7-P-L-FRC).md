---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-7
  - spell/evocation
  - source/srd
aliases:
  - "7th Tier Spell: Forcecage"
  - "Forcecage"
  - "7-P-L-FRC"
registry_id: 7-P-L-FRC
attribute_code: "7·Evo·None·cube (20)·100 feet·1 hour"
incantation: "Mu’-Bospona"
tier: 7
school: Evocation
affinity: P
grade: L
pz_total: 10478.8
pz_quantum: 141200.1
t_e: 4.40
updated: 2026-11-16
---

**Forcecage** (`7-P-L-FRC`) is a 7th Tier working of the [[Evocation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **10,479 Pz** against a slot quantum of 141,200 Pz, which puts its energy-equivalent tier at T_E 4.40 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 7 Workings]]
      - [[Evocation]]
        - **Forcecage** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `7-P-L-FRC` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `7·Evo·None·cube (20)·100 feet·1 hour` |
| Incantation | *Mu’-Bospona* |
| Affinity | P (Pure field construct) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 7th Tier |
| School | [[Evocation]] |
| Casting time | 1 action |
| Range | 100 feet |
| Area | cube (20) |
| Duration | 1 hour |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Ruby dust worth 1,500 gp |
| Ritual | no |
| Practitioner lineages | Bard, Warlock, Wizard |

### Mechanism

Raises an invisible cube of force, either a barred cage or a sealed box, that also extends into the ethereal layer and resists teleport escape.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| containment absorption | `0.20 Pz * (30 HP/round * 60 rounds = 1800 HP)` | 360 |
| planar escape denial reserve | `0.01 * 80 kg * 15 * 1e6 m / 1500 (one blocked crossing)` | 8,000 |
| displacement of partial occupants | `0.5 * 80 kg * 9.81 * 3 m / 1500` | 0.785 |
| Pattern cost | `0.01 × Q7 × (1 + 0.50)` | 2,118 |

| Quantity | Value |
|---|---|
| Effect energy | 8,361 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **10,479 Pz** (15,718.2 kJ) |
| Slot quantum Q7 | 141,200 Pz |
| Field gain (draw / quantum) | 0.0742 |
| Energy-equivalent tier T_E | 4.40 |
| Handling points | 0.50 |
| Grade score | -0.50 → L |

**Handling flags:** costly material, save or suck.

**Assumptions:** Trapped creature assaults the walls at 30 injury points per round for 10% of the hour; one teleport escape blocked; push of 80 kg over 3 m with friction 0.5.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Forcecage (7-P-L-FRC) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 7 | 7 | `0000000001111` |
| k2 School | Evocation | 4 | `0000000001001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | cube (20) | 9 | `0000000010011` |
| k5 Range | 100 feet | 2 | `0000000000101` |
| k6 Duration | 1 hour | 0 | `0000000000001` |

### Incantation

Spoken as **Mu’-Bospona** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T8: *Nimu’-Bospona* · T9: *Xyimu’-Bospona*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 2→1 3→2 | 4 |
| k2 School | 0→11 3→1 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 4→0 | 3 |
| k5 Range | 0→8 2→10 | 2 |
| k6 Duration | 0→7 | 1 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#859956`.

![[Forcecage (7-P-L-FRC) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 7 | 0.700 | 1.000 | `#005eff` (490 nm eq.) | source grid |
| School | Evocation | 0.500 | 0.980 | `#00ff8b` (550 nm eq.) | source grid |
| Duration | 1 hour | 0.053 | 0.811 | `#ff1c00` (684 nm eq.) | source grid |
| Area | cube (20) | 0.250 | 0.904 | `#cdff00` (625 nm eq.) | source grid |
| Range | 100 feet | 0.118 | 0.844 | `#ff7800` (665 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.17): swatch `#8cb996`, measured lines at 0.053, 0.118, 0.251, 0.501, 0.701. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.02. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `7·V·None`; the k4 to k6 lines (cube (20), 100 feet, 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `7·V·None` |
| Standard spectrometer detection range | 10.24 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 7,060 Pz (0.05 × Q7) |
| Counter drawn cold (all six layers) | 14,120 Pz (0.10 × Q7) |
| Unravel after completion | 14,120 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Heat, 2x Energy, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1b 1c 1d 1f` (Heat, Light, Life, Energy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1,746 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 7th Tier quantum of 141,200 Pz (7.4% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 7th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Evocation school with aspect lean Heat, 2x Energy, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 7 Workings]] |
| School | [[Evocation]] |
| Affinity | [[Pure]] (P) |
| Function | [[Wards and Shields]], [[Walls and Barriers]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Wall of Force (5-P-L-WFL)|Wall of Force]] (5) · [[Blade Barrier (6-V-L-BB)|Blade Barrier]] (6) · [[Wall of Ice (6-V-M-WI)|Wall of Ice]] (6) · [[Hallow (5-V-L-HLL)|Hallow]] (5) · [[Wall of Stone (5-V-M-WS)|Wall of Stone]] (5) · [[Fire Shield (4-V-L-FSR)|Fire Shield]] (4) · [[Globe of Invulnerability (6-A-L-GIO)|Globe of Invulnerability]] (6) · [[Guards and Wards (6-A-L-GWA)|Guards and Wards]] (6).


---

## Tactical Assessment

Instant detention for a dangerous target or an instant bunker against incoming fire; it cannot be removed by ordinary dispelling.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 7 Workings]] · [[Evocation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
