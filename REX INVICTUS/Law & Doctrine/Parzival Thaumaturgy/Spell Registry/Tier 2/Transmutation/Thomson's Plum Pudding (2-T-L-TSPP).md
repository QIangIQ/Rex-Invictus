---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/transmutation
  - source/science-spellbook
aliases:
  - "2nd Tier Spell: Thomson's Plum Pudding"
  - "2-T-L-TSPP"
  - "Thomson's Plum Pudding (Science)"
registry_id: 2-T-L-TSPP
attribute_code: "2·Tra·None·None·Touch·Instantaneous"
incantation: "Hielix"
tier: 2
school: Transmutation
affinity: T
grade: L
pz_total: 273.0
pz_quantum: 951.4
t_e: 0.75
updated: 2026-11-16
---

**Thomson's Plum Pudding** (`2-T-L-TSPP`) is a 2nd Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **273 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E 0.75 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Transmutation]]
        - **Thomson's Plum Pudding** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-T-L-TSPP` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Tra·None·None·Touch·Instantaneous` |
| Incantation | *Hielix* |
| Affinity | T (Transmutation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Transmutation]] |
| Casting time | 1 Action |
| Range | Touch |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Restoration | 1d4 restored (mean 2.5, modifier taken as +3) |
| Practitioner lineages | Druid |

### Mechanism

Produces 1d6+1 puddings studded with restorative berries; each heals a little and feeds a person for a day.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Puddings formed | `4.5 x 0.2 kg x 10 Pz/kg` | 9.0 |
| Healing content | `4.5 x 2.5 x 0.30 Pz` | 3.4 |
| Food energy | `4.5 x 8.37 MJ = 3.766e+07 J / 1500  *0.01 [C3]` | 251 |
| Pattern cost | `0.01 × Q2 × (1 + 0.00)` | 9.5 |

| Quantity | Value |
|---|---|
| Effect energy | 263 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **273 Pz** (409.5 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.287 |
| Energy-equivalent tier T_E | 0.75 |
| Handling points | 0.00 |
| Grade score | -0.62 → L |

Calibration applied: C3 (Borrowed sustenance), see [[Parzival Energy Budget#Registry calibration rules]].

**Handling flags:** none.

**Assumptions:** 4.5 puddings of 0.2 kg at 10 Pz/kg; healing 2.5 each at 0.30 Pz; food energy 2000 kcal (8.37 MJ) per pudding by real nutrition, which dominates.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Thomson's Plum Pudding (2-T-L-TSPP) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Hielix** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihielix* · T4: *Vihielix* · T5: *Tihielix* · T6: *Rihielix* · T7: *Mihielix* · T8: *Nihielix* · T9: *Xyihielix*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#d1417c`.

![[Thomson's Plum Pudding (2-T-L-TSPP) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.796 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.980 | `#ff0028` (700 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.792 | `#9b00ff` (435 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 2.44. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·T·None`; the k4 to k6 lines (None, Touch, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·T·None` |
| Standard spectrometer detection range | 1.65 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 95.1 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 45.5 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (28.7% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Summoning and Conjured Creatures]], [[Healing and Restoration]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Stinking Cloud (3-C-M-SCI)|Stinking Cloud]] (3) · [[Goodberry (1-T-L-GDB)|Goodberry]] (1) · [[Find Steed (2-C-H-FS)|Find Steed]] (2) · [[Giant Insect (4-T-H-GI)|Giant Insect]] (4) · [[Lesser Restoration (2-A-L-LR)|Lesser Restoration]] (2) · [[Prayer of Healing (2-V-L-PH)|Prayer of Healing]] (2) · [[Reverse Entropy (0-T-L-REV)|Reverse Entropy]] (0) · [[Spiritual Weapon (2-P-L-SW)|Spiritual Weapon]] (2).


---

## Tactical Assessment

Emergency rations and minor healing for a squad.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
