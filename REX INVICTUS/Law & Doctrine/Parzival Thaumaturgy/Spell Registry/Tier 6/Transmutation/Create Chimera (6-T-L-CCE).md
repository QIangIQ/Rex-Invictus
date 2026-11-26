---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-6
  - spell/transmutation
  - source/science-spellbook
aliases:
  - "6th Tier Spell: Create Chimera"
  - "6-T-L-CCE"
  - "Create Chimera (Science)"
registry_id: 6-T-L-CCE
attribute_code: "6·Tra·None·None·Touch·Instantaneous"
incantation: "Rielix"
tier: 6
school: Transmutation
affinity: T
grade: L
pz_total: 13038.9
pz_quantum: 51944.6
t_e: 4.62
updated: 2026-11-16
---

**Create Chimera** (`6-T-L-CCE`) is a 6th Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **13,039 Pz** against a slot quantum of 51,945 Pz, which puts its energy-equivalent tier at T_E 4.62 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 6 Workings]]
      - [[Transmutation]]
        - **Create Chimera** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `6-T-L-CCE` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `6·Tra·None·None·Touch·Instantaneous` |
| Incantation | *Rielix* |
| Affinity | T (Transmutation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 6th Tier |
| School | [[Transmutation]] |
| Casting time | 3 Hours |
| Range | Touch |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: At least two Beasts/Monstrosities to be combined, Silver Thread, Corundum Powder worth 500GP, Drying Oil |
| Ritual | yes |
| Resistance check | constitution; on success: no effect |
| Practitioner lineages | Druid, Warlock, Wizard |

### Mechanism

A three-hour ritual fuses two or more creatures into one loyal chimera with averaged traits.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Living matter restructured | `1200 kg x 10 Pz/kg` | 12,000 |
| Pattern cost | `0.01 × Q6 × (1 + 1.00)` | 1,039 |

| Quantity | Value |
|---|---|
| Effect energy | 12,000 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **13,039 Pz** (19,558.3 kJ) |
| Slot quantum Q6 | 51,945 Pz |
| Field gain (draw / quantum) | 0.251 |
| Energy-equivalent tier T_E | 4.62 |
| Handling points | 1.00 |
| Grade score | 0.31 → L |

**Handling flags:** ritual, costly material, consumed material, long cast.

**Assumptions:** Two large creatures of 700 and 500 kg rebuilt as living matter at 10 Pz/kg.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Create Chimera (6-T-L-CCE) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 6 | 6 | `0000000001101` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Rielix** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T7: *Mirielix* · T8: *Nirielix* · T9: *Xyirielix*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 3→2 | 3 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#863ecf`.

![[Create Chimera (6-T-L-CCE) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 6 | 0.600 | 1.000 | `#00ebff` (520 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.963 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.835 | `#ff0028` (700 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.961 | `#9b00ff` (435 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 4.12. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `6·T·None`; the k4 to k6 lines (None, Touch, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `6·T·None` |
| Standard spectrometer detection range | 11.42 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 2,597 Pz (0.05 × Q6) |
| Counter drawn cold (all six layers) | 5,194 Pz (0.10 × Q6) |
| Unravel after completion | 5,194 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 2,173 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 6th Tier quantum of 51,945 Pz (25.1% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Lex Interactionis | Can be resisted by the target; a large gap in Divine Power or a direct counter-affinity removes that chance. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 6th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 6 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Utility Workings]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Enhance Potion (5-T-L-EP)|Enhance Potion]] (5) · [[Sublimation (3-T-L-SBL)|Sublimation]] (3) · [[Weave Warp (9-T-L-WWA)|Weave Warp]] (9) · [[Disintegrate (6-P-L-DSN)|Disintegrate]] (6) · [[Flesh to Stone (6-T-L-FSE)|Flesh to Stone]] (6) · [[Magnetise (2-T-L-MGN)|Magnetise]] (2) · [[Momentum Transfer (2-T-L-MT)|Momentum Transfer]] (2) · [[Move Earth (6-T-M-ME)|Move Earth]] (6).


---

## Tactical Assessment

Bespoke war beasts for shock or guard duty.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 6 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
