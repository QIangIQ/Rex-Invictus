---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/pure
  - source/rex-invictus
aliases:
  - "1st Tier Spell: Magic Link"
  - "Magic Link"
  - "1-P-L-MLK"
registry_id: 1-P-L-MLK
attribute_code: "1·Pur·None·None·Touch·1 hour"
incantation: "Seulixa"
tier: 1
school: Pure
affinity: P
grade: L
pz_total: 8.1
pz_quantum: 350.0
t_e: -2.77
updated: 2026-11-16
---

**Magic Link** (`1-P-L-MLK`) is a 1st Tier working of the [[Pure]] school in [[Parzival Thaumaturgy]]. Rex Invictus original working. Its modelled draw is **8.1 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -2.77 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Pure]]
        - **Magic Link** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-P-L-MLK` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Pur·None·None·Touch·1 hour` |
| Incantation | *Seulixa* |
| Affinity | P (Pure field construct) |
| Source | Rex Invictus |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Pure]] |
| Casting time | 1 bonus action |
| Range | Touch |
| Area | single point or target |
| Duration | 1 hour |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Wizard, Sorcerer, Warlock |

### Effect

Creates a field thread between two workings or between a working and an object. When the first working ends, triggers or strikes, the second is released through the thread.

### Mechanism

A raw field thread with no school bias. It is the simplest form of Lex Nexus: a recorded connection that passes a release signal from one pattern to another.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| thread formation | `instant info` | 1.0 |
| [upkeep] thread hold, 1 h | `0.001 Pz/s*3600` | 3.6 |
| Pattern cost | `0.01 × Q1 × (1 + 0.00)` | 3.5 |

| Quantity | Value |
|---|---|
| Effect energy | 1.0 Pz |
| Upkeep energy | 3.6 Pz (0.001 Pz/s) |
| **Total draw** | **8.1 Pz** (12.1 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.0231 |
| Energy-equivalent tier T_E | -2.77 |
| Handling points | 0.00 |
| Grade score | -1.00 → L |

**Handling flags:** none.

**Assumptions:** Thread is informational; 0.001 Pz/s hold.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Magic Link (1-P-L-MLK) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Pure | 8 | `0000000010001` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | 1 hour | 0 | `0000000000001` |

### Incantation

Spoken as **Seulixa** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hiseulixa* · T3: *Liseulixa* · T4: *Viseulixa* · T5: *Tiseulixa* · T6: *Riseulixa* · T7: *Miseulixa* · T8: *Niseulixa* · T9: *Xyiseulixa*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 4→2 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 | 1 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#e5236a`.

![[Magic Link (1-P-L-MLK) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Pure | 0.938 | 0.704 | `#ed00ff` (419 nm eq.) | RI half-step |
| Duration | 1 hour | 0.053 | 0.999 | `#ff1c00` (684 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.736 | `#9b00ff` (435 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 0.91. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·P·None`; the k4 to k6 lines (None, Touch, 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·P·None` |
| Standard spectrometer detection range | 0.28 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.7 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is 2x Energy, Rigidity, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 1d 1f 1H` (Light, Life, Energy, Rigidity).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 1.3 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (2.3% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Pure school with aspect lean 2x Energy, Rigidity, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Pure]] |
| Affinity | [[Pure]] (P) |
| Function | [[Linking and Triggers]], [[Divination and Sensing]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Alarm (1-A-L-ALR)|Alarm]] (1) · [[Comprehend Languages (1-D-L-CL)|Comprehend Languages]] (1) · [[Detect Evil and Good (1-D-L-DEG)|Detect Evil and Good]] (1) · [[Detect Habitat (1-D-L-DH)|Detect Habitat]] (1) · [[Detect Magic (1-D-L-DMT)|Detect Magic]] (1) · [[Detect Poison and Disease (1-D-L-DPD)|Detect Poison and Disease]] (1) · [[Expectation Values (1-D-L-EV)|Expectation Values]] (1) · [[Focusing Lens (1-V-L-FLC)|Focusing Lens]] (1).


---

## Tactical Assessment

Lets a projectile carry a second working to the target, or lets one cast set off a chain of prepared effects at once.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Pure]] · [[Spell Breakdown Procedure]] · [[Parzival]]
