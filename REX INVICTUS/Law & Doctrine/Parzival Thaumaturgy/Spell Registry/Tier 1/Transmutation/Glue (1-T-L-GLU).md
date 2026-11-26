---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/transmutation
  - source/rex-invictus
aliases:
  - "1st Tier Spell: Glue"
  - "Glue"
  - "1-T-L-GLU"
registry_id: 1-T-L-GLU
attribute_code: "1·Tra·None·None·30 feet·1 hour"
incantation: "Sieusina"
tier: 1
school: Transmutation
affinity: T
grade: L
pz_total: 21.6
pz_quantum: 350.0
t_e: -1.79
updated: 2026-11-16
---

**Glue** (`1-T-L-GLU`) is a 1st Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Rex Invictus original working. Its modelled draw is **21.6 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -1.79 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Transmutation]]
        - **Glue** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-T-L-GLU` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Tra·None·None·30 feet·1 hour` |
| Incantation | *Sieusina* |
| Affinity | T (Transmutation) |
| Source | Rex Invictus |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Transmutation]] |
| Casting time | 1 action |
| Range | 30 feet |
| Area | single point or target |
| Duration | 1 hour |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: a pinch of tree resin |
| Ritual | no |
| Resistance check | strength; on success: no effect |
| Practitioner lineages | Wizard, Sorcerer, Artificer |

### Effect

Turns a surface or a body of liquid up to a 10 foot square (or 100 kg of liquid) into a strong adhesive for one hour. A creature that steps in must pass a strength check or be stuck in place.

### Mechanism

Raises the surface energy and cohesion of the target matter so that it bonds to anything in contact. The bond is a held pattern, so it fades when the hour ends (Lex Impermanentiae).

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| adhesive imprint, 100 kg of liquid | `0.1 Pz/kg*100` | 10.0 |
| [upkeep] bond held for 1 h | `0.002 Pz/s*3600` | 7.2 |
| Pattern cost | `0.01 × Q1 × (1 + 0.25)` | 4.4 |

| Quantity | Value |
|---|---|
| Effect energy | 10.0 Pz |
| Upkeep energy | 7.2 Pz (0.002 Pz/s) |
| **Total draw** | **21.6 Pz** (32.4 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.0616 |
| Energy-equivalent tier T_E | -1.79 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** save or suck.

**Assumptions:** 0.1 Pz/kg property imprint; low upkeep for the held bond.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Glue (1-T-L-GLU) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | 1 hour | 0 | `0000000000001` |

### Incantation

Spoken as **Sieusina** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisieusina* · T3: *Lisieusina* · T4: *Visieusina* · T5: *Tisieusina* · T6: *Risieusina* · T7: *Misieusina* · T8: *Nisieusina* · T9: *Xyisieusina*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 | 1 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#cd6332`.

![[Glue (1-T-L-GLU) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.741 | `#9600ff` (438 nm eq.) | source grid |
| Duration | 1 hour | 0.053 | 0.999 | `#ff1c00` (684 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.981 | `#91ff00` (612 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 1.33. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·T·None`; the k4 to k6 lines (None, 30 feet, 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·T·None` |
| Standard spectrometer detection range | 0.46 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 36.4 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 3.6 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (6.2% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Terrain and Matter Shaping]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Create or Destroy Water (1-T-L-CDW)|Create or Destroy Water]] (1) · [[Purify Food and Drink (1-T-L-PFD)|Purify Food and Drink]] (1) · [[Druidcraft (0-T-L-DRD)|Druidcraft]] (0) · [[Mending (0-T-L-MND)|Mending]] (0) · [[Prestidigitation (0-T-L-PRS)|Prestidigitation]] (0) · [[Reflective Coating (0-T-L-RCF)|Reflective Coating]] (0) · [[Sharpen (0-T-L-SHR)|Sharpen]] (0) · [[Spike Growth (2-T-L-SGI)|Spike Growth]] (2).


---

## Tactical Assessment

Pins infantry in a breach or glues a door shut. Inside a binder it lets a conjured fluid stick to walls and vehicles before a second property is released.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
