---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-6
  - spell/necromancy
  - source/srd
aliases:
  - "6th Tier Spell: Create Undead"
  - "Create Undead"
  - "6-N-L-CU"
registry_id: 6-N-L-CU
attribute_code: "6·Nec·None·None·10 feet·Instantaneous"
incantation: "Rouspul"
tier: 6
school: Necromancy
affinity: N
grade: L
pz_total: 16398.9
pz_quantum: 51944.6
t_e: 4.85
updated: 2026-11-16
---

**Create Undead** (`6-N-L-CU`) is a 6th Tier working of the [[Necromancy (School)|Necromancy]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **16,399 Pz** against a slot quantum of 51,945 Pz, which puts its energy-equivalent tier at T_E 4.85 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 6 Workings]]
      - [[Necromancy (School)|Necromancy]]
        - **Create Undead** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `6-N-L-CU` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `6·Nec·None·None·10 feet·Instantaneous` |
| Incantation | *Rouspul* |
| Affinity | N (Necromancy) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 6th Tier |
| School | [[Necromancy (School)\|Necromancy]] |
| Casting time | 1 minute |
| Range | 10 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: One clay pot filled with grave dirt, one clay pot filled with brackish water, and one 150 gp black onyx stone for each corpse |
| Ritual | no |
| Practitioner lineages | Cleric, Warlock, Wizard |

### Mechanism

At night the field restructures up to three humanoid corpses into ghouls bound to the caster for 24 hours. Control must be renewed before it lapses, after which the bodies act on their own.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| reanimate 3 corpses (semi-living restructuring) | `10*3*80` | 2,400 |
| upkeep: autonomy of 3 bound bodies for the 24 h control window | `0.05*3*86400` | 12,960 |
| Pattern cost | `0.01 × Q6 × (1 + 1.00)` | 1,039 |

| Quantity | Value |
|---|---|
| Effect energy | 2,400 Pz |
| Upkeep energy | 12,960 Pz (0.15 Pz/s) |
| **Total draw** | **16,399 Pz** (24,598.3 kJ) |
| Slot quantum Q6 | 51,945 Pz |
| Field gain (draw / quantum) | 0.316 |
| Energy-equivalent tier T_E | 4.85 |
| Handling points | 1.00 |
| Grade score | 0.42 → L |

**Handling flags:** costly material, multi target control, long cast.

**Assumptions:** Three 80 kg corpses at 10 Pz/kg; control upkeep 0.05 Pz/s each for 24 h; the animated bodies persist beyond that without field upkeep.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Create Undead (6-N-L-CU) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 6 | 6 | `0000000001101` |
| k2 School | Necromancy | 6 | `0000000001101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 10 feet | 1 | `0000000000011` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Rouspul** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T7: *Mirouspul* · T8: *Nirouspul* · T9: *Xyirouspul*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 3→2 | 3 |
| k2 School | 0→11 2→0 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 | 2 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#754f92`.

![[Create Undead (6-N-L-CU) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 6 | 0.600 | 1.000 | `#00ebff` (520 nm eq.) | source grid |
| School | Necromancy | 0.750 | 0.989 | `#0017ff` (475 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.835 | `#ff0028` (700 nm eq.) | source grid |
| Range | 10 feet | 0.059 | 0.864 | `#ff2700` (682 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.15): swatch `#5aa4ab`, measured lines at 0.004, 0.059, 0.601, 0.751. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.21. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `6·N·None`; the k4 to k6 lines (None, 10 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `6·N·None` |
| Standard spectrometer detection range | 12.81 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 2,597 Pz (0.05 × Q6) |
| Counter drawn cold (all six layers) | 5,194 Pz (0.10 × Q6) |
| Unravel after completion | 7,786 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Dark, 2x Death. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1D 1F 1J` (Within, Death, Potential, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 2,733 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 6th Tier quantum of 51,945 Pz (31.6% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 6th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Necromancy school with aspect lean Within, Dark, 2x Death. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 6 Workings]] |
| School | [[Necromancy (School)\|Necromancy]] |
| Affinity | [[Necromancy (School)\|Necromancy]] (N) |
| Function | [[Summoning and Conjured Creatures]], [[Necromantic and Soul Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Clone (8-N-L-CLN)|Clone]] (8) · [[Animate Dead (3-N-M-AD)|Animate Dead]] (3) · [[Circle of Death (6-N-L-CD)|Circle of Death]] (6) · [[Harm (6-N-L-HRM)|Harm]] (6) · [[Magic Jar (6-N-H-MJ)|Magic Jar]] (6) · [[Contagion (5-N-L-CNTT)|Contagion]] (5) · [[Finger of Death (7-N-L-FDN)|Finger of Death]] (7) · [[Raise Dead (5-N-M-RD)|Raise Dead]] (5).


---

## Tactical Assessment

Creates expendable shock troops or guards from battlefield dead, with a daily renewal burden and serious legal and moral restrictions in most polities.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 6 Workings]] · [[Necromancy (School)|Necromancy]] · [[Spell Breakdown Procedure]] · [[Parzival]]
