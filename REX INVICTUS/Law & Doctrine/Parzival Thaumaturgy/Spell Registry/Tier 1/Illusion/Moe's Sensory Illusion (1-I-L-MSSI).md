---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/illusion
  - source/science-spellbook
aliases:
  - "1st Tier Spell: Moe's Sensory Illusion"
  - "1-I-L-MSSI"
  - "Moe's Sensory Illusion (Science)"
registry_id: 1-I-L-MSSI
attribute_code: "1·Ill·None·None·30 feet·Up to 1 minute"
incantation: "Saiusinse"
tier: 1
school: Illusion
affinity: I
grade: L
pz_total: 4.7
pz_quantum: 350.0
t_e: -3.32
updated: 2026-11-16
---

**Moe's Sensory Illusion** (`1-I-L-MSSI`) is a 1st Tier working of the [[Illusion]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **4.7 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E -3.32 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Illusion]]
        - **Moe's Sensory Illusion** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-I-L-MSSI` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Ill·None·None·30 feet·Up to 1 minute` |
| Incantation | *Saiusinse* |
| Affinity | I (Illusion) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Illusion]] |
| Casting time | 1 Action |
| Range | 30 feet |
| Area | single point or target |
| Duration | Up to 1 minute (concentration) |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Some rotten food |
| Ritual | no |
| Practitioner lineages | Wizard, Sorcerer, Druid, Cleric |

### Mechanism

Feeds one creature a false sensation such as nausea, a smell, a texture, a temperature, a colour cast or a brief sound.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Sensory override (upkeep) | `enchantment rate: 0.005 Pz/s x 60 s` | 0.3 |
| Pattern cost | `0.01 × Q1 × (1 + 0.25)` | 4.4 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 0.3 Pz (0.005 Pz/s) |
| **Total draw** | **4.7 Pz** (7.0 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.0134 |
| Energy-equivalent tier T_E | -3.32 |
| Handling points | 0.25 |
| Grade score | -0.75 → L |

**Handling flags:** concentration.

**Assumptions:** Enchantment rate on one creature for 1 minute.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Moe's Sensory Illusion (1-I-L-MSSI) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Illusion | 5 | `0000000001011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Up to 1 minute | 13 | `0000000011011` |

### Incantation

Spoken as **Saiusinse** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisaiusinse* · T3: *Lisaiusinse* · T4: *Visaiusinse* · T5: *Tisaiusinse* · T6: *Risaiusinse* · T7: *Misaiusinse* · T8: *Nisaiusinse* · T9: *Xyisaiusinse*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 1→12 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 3→10 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#6ba576`.

![[Moe's Sensory Illusion (1-I-L-MSSI) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Illusion | 0.625 | 0.871 | `#00c5ff` (512 nm eq.) | source grid |
| Duration | Up to 1 minute | 0.684 | 0.843 | `#0074ff` (495 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.981 | `#91ff00` (612 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 0.67. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·I·None`; the k4 to k6 lines (None, 30 feet, Up to 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·I·None` |
| Standard spectrometer detection range | 0.22 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 35.1 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Light, Introspection, 2x Flexibility. The working vector used by [[Recast Tension and Combination Affinity]] is `2c 1d 1F 1G 2h 1J` (2x Light, Life, Potential, Introspection, 2x Flexibility, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 0.779 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (1.3% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Illusion school with aspect lean Light, Introspection, 2x Flexibility. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Illusion]] |
| Affinity | [[Illusion]] (I) |
| Function | [[Concealment and Illusion]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Alter Difraction Pattern (1-I-L-ADP)|Alter Difraction Pattern]] (1) · [[Disguise Self (1-I-L-DS)|Disguise Self]] (1) · [[Illusory Script (1-I-L-IS)|Illusory Script]] (1) · [[One Way Mirror (1-I-L-OWM)|One Way Mirror]] (1) · [[Silent Image (1-I-L-SI)|Silent Image]] (1) · [[Arcanist's Magic Aura (2-I-L-ASMA)|Arcanist's Magic Aura]] (2) · [[Blur (2-I-L-BLR)|Blur]] (2) · [[Cloak (2-I-L-CLK)|Cloak]] (2).


---

## Tactical Assessment

Distraction and misdirection of sentries.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Illusion]] · [[Spell Breakdown Procedure]] · [[Parzival]]
