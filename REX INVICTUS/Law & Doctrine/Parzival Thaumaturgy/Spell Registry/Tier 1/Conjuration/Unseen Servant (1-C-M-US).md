---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-1
  - spell/conjuration
  - source/srd
aliases:
  - "1st Tier Spell: Unseen Servant"
  - "Unseen Servant"
  - "1-C-M-US"
registry_id: 1-C-M-US
attribute_code: "1·Con·None·None·60 feet·1 hour"
incantation: "Sewyna"
tier: 1
school: Conjuration
affinity: C
grade: M
pz_total: 236.9
pz_quantum: 350.0
t_e: 0.61
updated: 2026-11-16
---

**Unseen Servant** (`1-C-M-US`) is a 1st Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **237 Pz** against a slot quantum of 350 Pz, which puts its energy-equivalent tier at T_E 0.61 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 1 Workings]]
      - [[Conjuration]]
        - **Unseen Servant** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `1-C-M-US` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `1·Con·None·None·60 feet·1 hour` |
| Incantation | *Sewyna* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 1st Tier |
| School | [[Conjuration]] |
| Casting time | 1 action |
| Range | 60 feet |
| Area | single point or target |
| Duration | 1 hour |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A piece of string and a bit of wood |
| Ritual | yes |
| Practitioner lineages | Bard, Warlock, Wizard |

### Mechanism

An invisible, weak force agent carries out simple manual tasks within 18 m of the caster for an hour.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Force agent formed | `instant set-up = 1 Pz` | 1.0 |
| Upkeep: Agent autonomy | `0.05 Pz/s * 3600 s` | 180 |
| Upkeep: Chores at 20 W | `20 W * 3600 s / 1500` | 48.0 |
| Pattern cost | `0.01 × Q1 × (1 + 1.25)` | 7.9 |

| Quantity | Value |
|---|---|
| Effect energy | 1.0 Pz |
| Upkeep energy | 228 Pz (0.0633 Pz/s) |
| **Total draw** | **237 Pz** (355.3 kJ) |
| Slot quantum Q1 | 350 Pz |
| Field gain (draw / quantum) | 0.677 |
| Energy-equivalent tier T_E | 0.61 |
| Handling points | 1.25 |
| Grade score | 1.05 → M |

**Handling flags:** ritual, fragile.

**Assumptions:** 20 W mean mechanical output (strength 2); 1 h.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Unseen Servant (1-C-M-US) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 1 | 1 | `0000000000011` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 60 feet | 10 | `0000000010101` |
| k6 Duration | 1 hour | 0 | `0000000000001` |

### Incantation

Spoken as **Sewyna** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T2: *Hisewyna* · T3: *Lisewyna* · T4: *Visewyna* · T5: *Tisewyna* · T6: *Risewyna* · T7: *Misewyna* · T8: *Nisewyna* · T9: *Xyisewyna*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 | 2 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 2→10 4→12 | 3 |
| k6 Duration | 0→7 | 1 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#c47a3a`.

![[Unseen Servant (1-C-M-US) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 1 | 0.100 | 1.000 | `#ff5d00` (670 nm eq.) | source grid |
| School | Conjuration | 0.125 | 1.000 | `#ff8300` (662 nm eq.) | source grid |
| Duration | 1 hour | 0.053 | 0.999 | `#ff1c00` (684 nm eq.) | source grid |
| Range | 60 feet | 0.588 | 0.888 | `#00fbff` (524 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 2.37. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `1·C·None`; the k4 to k6 lines (None, 60 feet, 1 hour) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `1·C·None` |
| Standard spectrometer detection range | 1.54 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 17.5 Pz (0.05 × Q1) |
| Counter drawn cold (all six layers) | 35.0 Pz (0.10 × Q1) |
| Unravel after completion | 80.6 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 39.5 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 1st Tier quantum of 350 Pz (67.7% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 1st Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 1 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Summoning and Conjured Creatures]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Find Familiar (1-C-H-FFN)|Find Familiar]] (1) · [[Arcane Die (0-C-L-ADC)|Arcane Die]] (0) · [[Find Steed (2-C-H-FS)|Find Steed]] (2) · [[Quantum Familiar (0-C-L-QF)|Quantum Familiar]] (0) · [[Temporary Magic Prism (2-C-L-TMP)|Temporary Magic Prism]] (2) · [[Arcane Singularity (3-C-L-ASA)|Arcane Singularity]] (3) · [[Conjure Animals (3-C-M-CA)|Conjure Animals]] (3) · [[Stinking Cloud (3-C-M-SCI)|Stinking Cloud]] (3).


---

## Tactical Assessment

Camp logistics, triggering mechanisms at a distance and probing for pressure traps.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 1 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
