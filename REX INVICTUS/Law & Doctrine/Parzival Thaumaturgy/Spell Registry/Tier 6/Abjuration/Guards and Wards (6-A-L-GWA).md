---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-6
  - spell/abjuration
  - source/srd
aliases:
  - "6th Tier Spell: Guards and Wards"
  - "Guards and Wards"
  - "6-A-L-GWA"
registry_id: 6-A-L-GWA
attribute_code: "6·Abj·None·cube (2500)·Touch·24 hours"
incantation: "Ra’-Boélixl"
tier: 6
school: Abjuration
affinity: A
grade: L
pz_total: 1528.5
pz_quantum: 51944.6
t_e: 2.47
updated: 2026-11-16
---

**Guards and Wards** (`6-A-L-GWA`) is a 6th Tier working of the [[Abjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **1,529 Pz** against a slot quantum of 51,945 Pz, which puts its energy-equivalent tier at T_E 2.47 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 6 Workings]]
      - [[Abjuration]]
        - **Guards and Wards** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `6-A-L-GWA` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `6·Abj·None·cube (2500)·Touch·24 hours` |
| Incantation | *Ra’-Boélixl* |
| Affinity | A (Abjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 6th Tier |
| School | [[Abjuration]] |
| Casting time | 10 minutes |
| Range | Touch |
| Area | cube (2500) |
| Duration | 24 hours |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Burning incense, a small measure of brimstone and oil, a knotted string, a small amount of umber hulk blood, and a small silver rod worth at least 10 gp |
| Ritual | no |
| Practitioner lineages | Bard, Wizard |

### Mechanism

Layers a building section of up to 232 m^2 with fog, misdirection, locked and disguised doors, webbed stairs and one extra ward effect for a day.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| corridor fog | `1 Pz/kg * 40% of 1416 m^3 * 0.0005 kg/m^3` | 0.283 |
| door locks absorption | `0.20 Pz * 10 doors * 50 HP` | 100 |
| stair webs | `3 Pz/kg * 2 stairwells * 5 kg` | 30.0 |
| web regrowth | `2 regrowths * 30 Pz` | 60.0 |
| two noxious clouds | `1 Pz/kg * 2 * 949 m^3 * 0.001 kg/m^3` | 1.9 |
| misdirection on intruders | `0.005 Pz/s * 4 intruders * 600 s` | 12.0 |
| fog replenishment | `10%/min of 0.283 kg / 60 = 0.000471947 Pz/s * 86400 s` | 40.8 |
| ward field and door illusions | `0.002 Pz/s * 1416 m^3 / 1000 = 0.00283168 Pz/s * 86400 s` | 245 |
| Pattern cost | `0.01 × Q6 × (1 + 1.00)` | 1,039 |

| Quantity | Value |
|---|---|
| Effect energy | 204 Pz |
| Upkeep energy | 285 Pz (0.0033 Pz/s) |
| **Total draw** | **1,529 Pz** (2,292.8 kJ) |
| Slot quantum Q6 | 51,945 Pz |
| Field gain (draw / quantum) | 0.0294 |
| Energy-equivalent tier T_E | 2.47 |
| Handling points | 1.00 |
| Grade score | 0.00 → L |

**Handling flags:** costly material, multi target control, long cast.

**Assumptions:** Full area at 20 ft height; 40% corridors; noxious clouds chosen as the extra effect; 10 doors, 2 stairwells, 4 intruders; 24 h upkeep.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Guards and Wards (6-A-L-GWA) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 6 | 6 | `0000000001101` |
| k2 School | Abjuration | 0 | `0000000000001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | cube (2500) | 11 | `0000000010111` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | 24 hours | 5 | `0000000001011` |

### Incantation

Spoken as **Ra’-Boélixl** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T7: *Mira’-Boélixl* · T8: *Nira’-Boélixl* · T9: *Xyira’-Boélixl*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 3→2 | 3 |
| k2 School | 0→11 | 1 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 1→10 2→11 4→0 | 4 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 3→10 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#7f9971`.

![[Guards and Wards (6-A-L-GWA) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 6 | 0.600 | 1.000 | `#00ebff` (520 nm eq.) | source grid |
| School | Abjuration | 0.000 | 0.835 | `#ff0028` (700 nm eq.) | source grid |
| Duration | 24 hours | 0.316 | 0.960 | `#76ff00` (605 nm eq.) | source grid |
| Area | cube (2500) | 0.306 | 0.958 | `#81ff00` (608 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.961 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.18): swatch `#939f9a`, measured lines at 0.007, 0.312, 0.601, 0.883. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.18. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `6·A·None`; the k4 to k6 lines (cube (2500), Touch, 24 hours) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `6·A·None` |
| Standard spectrometer detection range | 3.91 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 2,597 Pz (0.05 × Q6) |
| Counter drawn cold (all six layers) | 5,194 Pz (0.10 × Q6) |
| Unravel after completion | 5,252 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Rigidity, Hope, Stagnancy. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1H 1i 2J` (Within, Light, Life, Potential, Rigidity, Hope, 2x Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 255 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 6th Tier quantum of 51,945 Pz (2.9% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 6th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Abjuration school with aspect lean Within, Rigidity, Hope, Stagnancy. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 6 Workings]] |
| School | [[Abjuration]] |
| Affinity | [[Abjuration]] (A) |
| Function | [[Wards and Shields]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Globe of Invulnerability (6-A-L-GIO)|Globe of Invulnerability]] (6) · [[Death Ward (4-A-L-DW)|Death Ward]] (4) · [[Holy Aura (8-A-L-HA)|Holy Aura]] (8) · [[Mind Blank (8-A-L-MB)|Mind Blank]] (8) · [[Stoneskin (4-A-L-STN)|Stoneskin]] (4) · [[Bulwark (3-A-L-BLW)|Bulwark]] (3) · [[Forcecage (7-P-L-FRC)|Forcecage]] (7) · [[Glyph of Warding (3-A-H-GWY)|Glyph of Warding]] (3).


---

## Tactical Assessment

Converts a stronghold floor into a defensive maze that slows raiders long enough for a response; repeated daily for a year it becomes permanent.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 6 Workings]] · [[Abjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
