---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-9
  - spell/necromancy
  - source/srd
aliases:
  - "9th Tier Spell: True Resurrection"
  - "True Resurrection"
  - "9-N-L-TR"
registry_id: 9-N-L-TR
attribute_code: "9·Nec·None·None·Touch·Instantaneous"
incantation: "Xyoulix"
tier: 9
school: Necromancy
affinity: N
grade: L
pz_total: 79088.4
pz_quantum: 1043335.3
t_e: 6.42
updated: 2026-11-16
---

**True Resurrection** (`9-N-L-TR`) is a 9th Tier working of the [[Necromancy (School)|Necromancy]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **79,088 Pz** against a slot quantum of 1.04 MPz Pz, which puts its energy-equivalent tier at T_E 6.42 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 9 Workings]]
      - [[Necromancy (School)|Necromancy]]
        - **True Resurrection** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `9-N-L-TR` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `9·Nec·None·None·Touch·Instantaneous` |
| Incantation | *Xyoulix* |
| Affinity | N (Necromancy) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 9th Tier |
| School | [[Necromancy (School)\|Necromancy]] |
| Casting time | 1 hour |
| Range | Touch |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: A sprinkle of holy water and diamonds worth at least 25,000gp, which the spell consumes |
| Ritual | no |
| Practitioner lineages | Cleric, Druid |

### Mechanism

A willing soul dead up to two centuries is re-anchored to a fully restored body, rebuilt from nothing if needed, with all disease, poison and curses removed.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Soul re-anchoring | `1e4 Pz * (9 - 3)` | 60,000 |
| Full restoration | `100 HP * 0.30` | 30.0 |
| New body if required | `10 Pz/kg * 80 kg` | 800 |
| Pattern cost | `0.01 × Q9 × (1 + 0.75)` | 18,258 |

| Quantity | Value |
|---|---|
| Effect energy | 60,830 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **79,088 Pz** (118,632.6 kJ) |
| Slot quantum Q9 | 1.04 MPz Pz |
| Field gain (draw / quantum) | 0.0758 |
| Energy-equivalent tier T_E | 6.42 |
| Handling points | 0.75 |
| Grade score | -0.25 → L |

**Handling flags:** costly material, consumed material, long cast.

**Assumptions:** Tier 9 soul constant; 100 HP restored; full new 80 kg body.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[True Resurrection (9-N-L-TR) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 9 | 9 | `0000000010011` |
| k2 School | Necromancy | 6 | `0000000001101` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Xyoulix** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 4→3 | 3 |
| k2 School | 0→11 2→0 3→1 | 3 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#8a06d7`.

![[True Resurrection (9-N-L-TR) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 9 | 0.900 | 1.000 | `#b600ff` (430 nm eq.) | source grid |
| School | Necromancy | 0.750 | 0.989 | `#0017ff` (475 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.667 | `#ff0028` (700 nm eq.) | source grid |
| Range | Touch | 0.882 | 1.000 | `#9b00ff` (435 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 4.90. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `9·N·None`; the k4 to k6 lines (None, Touch, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `9·N·None` |
| Standard spectrometer detection range | 28.12 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 52,167 Pz (0.05 × Q9) |
| Counter drawn cold (all six layers) | 104,334 Pz (0.10 × Q9) |
| Unravel after completion | 104,334 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Within, Dark, 2x Death. The working vector used by [[Recast Tension and Combination Affinity]] is `1A 1D 1F 1J` (Within, Death, Potential, Stagnancy).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 13,181 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 9th Tier quantum of 1.04 MPz Pz (7.6% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 9th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Necromancy school with aspect lean Within, Dark, 2x Death. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 9 Workings]] |
| School | [[Necromancy (School)\|Necromancy]] |
| Affinity | [[Necromancy (School)\|Necromancy]] (N) |
| Function | [[Healing and Restoration]], [[Necromantic and Soul Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Resurrection (7-N-L-RSR)|Resurrection]] (7) · [[Raise Dead (5-N-M-RD)|Raise Dead]] (5) · [[Clone (8-N-L-CLN)|Clone]] (8) · [[Finger of Death (7-N-L-FDN)|Finger of Death]] (7) · [[Mass Heal (9-C-L-MHS)|Mass Heal]] (9) · [[Power Word Kill (9-E-L-PWK)|Power Word Kill]] (9) · [[Time Stop (9-T-M-TSM)|Time Stop]] (9) · [[Circle of Death (6-N-L-CD)|Circle of Death]] (6).


---

## Tactical Assessment

Recovers irreplaceable personnel regardless of the state of the remains, at very high material cost.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 9 Workings]] · [[Necromancy (School)|Necromancy]] · [[Spell Breakdown Procedure]] · [[Parzival]]
