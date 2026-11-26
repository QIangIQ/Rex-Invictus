---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/illusion
  - source/srd
aliases:
  - "2nd Tier Spell: Magic Mouth"
  - "Magic Mouth"
  - "2-I-L-MMG"
registry_id: 2-I-L-MMG
attribute_code: "2·Ill·None·None·30 feet·Until dispelled"
incantation: "Haiusinis"
tier: 2
school: Illusion
affinity: I
grade: L
pz_total: 99.0
pz_quantum: 951.4
t_e: -0.26
updated: 2026-11-16
---

**Magic Mouth** (`2-I-L-MMG`) is a 2nd Tier working of the [[Illusion]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **99.0 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E -0.26 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Illusion]]
        - **Magic Mouth** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-I-L-MMG` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Ill·None·None·30 feet·Until dispelled` |
| Incantation | *Haiusinis* |
| Affinity | I (Illusion) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Illusion]] |
| Casting time | 1 minute |
| Range | 30 feet |
| Area | single point or target |
| Duration | Until dispelled |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A honeycomb and jade dust of at least 10 inches, the spell consumes |
| Ritual | yes |
| Practitioner lineages | Bard, Wizard |

### Mechanism

The field stores a short spoken message on an object and replays it in the caster's voice when a visual or audible condition occurs within 30 ft. It can trigger once or repeatedly.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Message recording (instant info) | `instant info = 1 Pz` | 1.0 |
| Playback acoustic output | `1 W * 10 s / 1500` | 0.00667 |
| Trigger watch, 30 ft, 24 h reference horizon (upkeep) | `0.001 Pz/s * (9.144 m / 10) * 86400 s` | 79.0 |
| Pattern cost | `0.01 × Q2 × (1 + 1.00)` | 19.0 |

| Quantity | Value |
|---|---|
| Effect energy | 1.0 Pz |
| Upkeep energy | 79.0 Pz (0.000914 Pz/s) |
| **Total draw** | **99.0 Pz** (148.6 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.104 |
| Energy-equivalent tier T_E | -0.26 |
| Handling points | 1.00 |
| Grade score | 0.00 → L |

**Handling flags:** ritual, costly material, consumed material, long cast.

**Assumptions:** Message of 25 words played as 10 s at 1 W; trigger sensing held over a 24 h reference horizon; material listed in the record is garbled, assumed 10 gp and consumed.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Magic Mouth (2-I-L-MMG) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Illusion | 5 | `0000000001011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Until dispelled | 11 | `0000000010111` |

### Incantation

Spoken as **Haiusinis** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihaiusinis* · T4: *Vihaiusinis* · T5: *Tihaiusinis* · T6: *Rihaiusinis* · T7: *Mihaiusinis* · T8: *Nihaiusinis* · T9: *Xyihaiusinis*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 1→12 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 2→9 4→11 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#68eb78`.

![[Magic Mouth (2-I-L-MMG) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Illusion | 0.625 | 0.914 | `#00c5ff` (512 nm eq.) | source grid |
| Duration | Until dispelled | 0.579 | 0.931 | `#00fff7` (526 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.996 | `#91ff00` (612 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.20): swatch `#9dcd97`, measured lines at 0.201, 0.295, 0.579, 0.626. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 2.00. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·I·None`; the k4 to k6 lines (None, 30 feet, Until dispelled) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·I·None` |
| Standard spectrometer detection range | 1.00 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 111 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Light, Introspection, 2x Flexibility. The working vector used by [[Recast Tension and Combination Affinity]] is `2c 1d 1F 1G 2h 1J` (2x Light, Life, Potential, Introspection, 2x Flexibility, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 16.5 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (10.4% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Endures independently once set, which places it under the decay clause of ULMTU-XIII. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIII]] | Lex Impermanentiae | Long-lived patterns drift toward reversion unless refreshed from a source that satisfies ULMTU-I. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Illusion school with aspect lean Light, Introspection, 2x Flexibility. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Illusion]] |
| Affinity | [[Illusion]] (I) |
| Function | [[Linking and Triggers]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Transfiguration Inheritance (2-T-L-TI)|Transfiguration Inheritance]] (2) · [[Alarm (1-A-L-ALR)|Alarm]] (1) · [[Glyph of Warding (3-A-H-GWY)|Glyph of Warding]] (3) · [[Magic Link (1-P-L-MLK)|Magic Link]] (1) · [[Arcanist's Magic Aura (2-I-L-ASMA)|Arcanist's Magic Aura]] (2) · [[Blur (2-I-L-BLR)|Blur]] (2) · [[Cloak (2-I-L-CLK)|Cloak]] (2) · [[Invisibility (2-I-L-INV)|Invisibility]] (2).


---

## Tactical Assessment

Serves as a voice tripwire, a recorded warning at a perimeter or a dead drop for short messages. It provides no remote alert to its maker.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Illusion]] · [[Spell Breakdown Procedure]] · [[Parzival]]
