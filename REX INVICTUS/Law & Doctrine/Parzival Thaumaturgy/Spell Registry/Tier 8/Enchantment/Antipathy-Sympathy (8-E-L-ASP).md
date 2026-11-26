---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-8
  - spell/enchantment
  - source/srd
aliases:
  - "8th Tier Spell: Antipathy/Sympathy"
  - "Antipathy/Sympathy"
  - "8-E-L-ASP"
registry_id: 8-E-L-ASP
attribute_code: "8·Enc·None·cube (200)·60 feet·10 days"
incantation: "No’-Baiwyny"
tier: 8
school: Enchantment
affinity: E
grade: L
pz_total: 91198.8
pz_quantum: 383821.6
t_e: 6.56
updated: 2026-11-16
---

**Antipathy/Sympathy** (`8-E-L-ASP`) is a 8th Tier working of the [[Enchantment]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **91,199 Pz** against a slot quantum of 383,822 Pz, which puts its energy-equivalent tier at T_E 6.56 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 8 Workings]]
      - [[Enchantment]]
        - **Antipathy/Sympathy** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `8-E-L-ASP` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `8·Enc·None·cube (200)·60 feet·10 days` |
| Incantation | *No’-Baiwyny* |
| Affinity | E (Enchantment) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 8th Tier |
| School | [[Enchantment]] |
| Casting time | 1 hour |
| Range | 60 feet |
| Area | cube (200) |
| Duration | 10 days |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Either a lump of alum soaked in vinegar for the antipathy effect or a drop of honey for the sympathy effect |
| Ritual | no |
| Practitioner lineages | Druid, Wizard |

### Mechanism

An object, creature or region up to 61 m across is given an aura that compels one designated kind of creature to flee from it or to approach and stay near it.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| instant information | `1 * 1 Pz` | 1.0 |
| aura upkeep | `0.005 Pz/s * 20 creature(s) * 864000 s` | 86,400 |
| Pattern cost | `0.01 × Q8 × (1 + 0.25)` | 4,798 |

| Quantity | Value |
|---|---|
| Effect energy | 1.0 Pz |
| Upkeep energy | 86,400 Pz (0.1 Pz/s) |
| **Total draw** | **91,199 Pz** (136,798.2 kJ) |
| Slot quantum Q8 | 383,822 Pz |
| Field gain (draw / quantum) | 0.238 |
| Energy-equivalent tier T_E | 6.56 |
| Handling points | 0.25 |
| Grade score | -0.47 → L |

**Handling flags:** long cast.

**Assumptions:** 20 affected creatures on average over 10 days at 0.005 Pz/s each.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Antipathy-Sympathy (8-E-L-ASP) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 8 | 8 | `0000000010001` |
| k2 School | Enchantment | 3 | `0000000000111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | cube (200) | 10 | `0000000010101` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | 10 days | 3 | `0000000000111` |

### Incantation

Spoken as **No’-Baiwyny** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T9: *Xyino’-Baiwyny*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 4→3 | 2 |
| k2 School | 0→11 1→12 2→0 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 2→11 4→0 | 3 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 1→8 2→9 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#5dc46d`.

![[Antipathy-Sympathy (8-E-L-ASP) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 8 | 0.800 | 1.000 | `#2900ff` (460 nm eq.) | source grid |
| School | Enchantment | 0.375 | 0.914 | `#20ff00` (588 nm eq.) | source grid |
| Duration | 10 days | 0.211 | 0.841 | `#fff500` (637 nm eq.) | source grid |
| Area | cube (200) | 0.278 | 0.873 | `#a7ff00` (617 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.978 | `#00fbff` (524 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.13): swatch `#87c6ad`, measured lines at 0.211, 0.278, 0.376, 0.589, 0.801. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.96. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `8·E·None`; the k4 to k6 lines (cube (200), 60 feet, 10 days) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `8·E·None` |
| Standard spectrometer detection range | 30.20 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 19,191 Pz (0.05 × Q8) |
| Counter drawn cold (all six layers) | 38,382 Pz (0.10 × Q8) |
| Unravel after completion | 55,662 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Introspection, Flexibility, Hope. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1c 1d 1F 1G 1h 1i 1J` (Within, Light, Life, Potential, Introspection, Flexibility, Hope, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 15,200 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 8th Tier quantum of 383,822 Pz (23.8% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Endures independently once set, which places it under the decay clause of ULMTU-XIII. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIII]] | Lex Impermanentiae | Long-lived patterns drift toward reversion unless refreshed from a source that satisfies ULMTU-I. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIV]] | Lex Voluntatis | Acts on the will of the subject and must leave it a resistance path. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 8th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Enchantment school with aspect lean Within, Introspection, Flexibility, Hope. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 8 Workings]] |
| School | [[Enchantment]] |
| Affinity | [[Enchantment]] (E) |
| Function | [[Mind and Will]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Dominate Monster (8-E-L-DMM)|Dominate Monster]] (8) · [[Feeblemind (8-E-L-FBL)|Feeblemind]] (8) · [[Power Word Stun (8-E-L-PWS)|Power Word Stun]] (8) · [[Power Word Kill (9-E-L-PWK)|Power Word Kill]] (9) · [[Gravitational Wave (8-V-L-GWV)|Gravitational Wave]] (8) · [[Irresistible Dance (6-E-L-ID)|Irresistible Dance]] (6) · [[Mass Suggestion (6-E-L-MSU)|Mass Suggestion]] (6) · [[Divine Word (7-V-L-DWV)|Divine Word]] (7).


---

## Tactical Assessment

Area denial against a specific species or faction, or a lure that holds enemy units at a chosen point for days.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 8 Workings]] · [[Enchantment]] · [[Spell Breakdown Procedure]] · [[Parzival]]
