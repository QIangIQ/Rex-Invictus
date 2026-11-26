---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-5
  - spell/transmutation
  - source/srd
aliases:
  - "5th Tier Spell: Reincarnate"
  - "Reincarnate"
  - "5-T-M-RNC"
registry_id: 5-T-M-RNC
attribute_code: "5·Tra·None·None·Touch·Instantaneous"
incantation: "Tielix"
tier: 5
school: Transmutation
affinity: T
grade: M
pz_total: 21134.4
pz_quantum: 19109.4
t_e: 5.10
updated: 2026-11-16
---

**Reincarnate** (`5-T-M-RNC`) is a 5th Tier working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **21,134 Pz** against a slot quantum of 19,109 Pz, which puts its energy-equivalent tier at T_E 5.10 and its handling grade at **Medium**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 5 Workings]]
      - [[Transmutation]]
        - **Reincarnate** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `5-T-M-RNC` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `5·Tra·None·None·Touch·Instantaneous` |
| Incantation | *Tielix* |
| Affinity | T (Transmutation) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 5th Tier |
| School | [[Transmutation]] |
| Casting time | 1 hour |
| Range | Touch |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata), material focus. Material: Rare oils and unguents worth at least 1,000 gp, which the spell consumes |
| Ritual | no |
| Practitioner lineages | Druid |

### Mechanism

A new adult body of a random lineage is grown from a fragment and the dead person's soul is drawn into it.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| soul re-anchoring, 2 tiers above 3 | `1e4*(5-3)` | 20,000 |
| new adult body, 80 kg living matter | `10*80` | 800 |
| Pattern cost | `0.01 × Q5 × (1 + 0.75)` | 334 |

| Quantity | Value |
|---|---|
| Effect energy | 20,800 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **21,134 Pz** (31,701.6 kJ) |
| Slot quantum Q5 | 19,109 Pz |
| Field gain (draw / quantum) | 1.11 |
| Energy-equivalent tier T_E | 5.10 |
| Handling points | 0.75 |
| Grade score | 0.80 → M |

**Handling flags:** costly material, consumed material, long cast.

**Assumptions:** New body 80 kg at 10 Pz/kg; soul constant as for raising.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Reincarnate (5-T-M-RNC) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 5 | 5 | `0000000001011` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Tielix** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T6: *Ritielix* · T7: *Mitielix* · T8: *Nitielix* · T9: *Xyitielix*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]]. This attribute set is shared with other workings, so the glyph carries 1 centre dot(s) to tell it apart.

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 1→0 3→2 | 3 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#8744ad`.

![[Reincarnate (5-T-M-RNC) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 5 | 0.500 | 1.000 | `#00ff8b` (550 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.932 | `#9600ff` (438 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.882 | `#ff0028` (700 nm eq.) | source grid |
| Range | Touch | 0.882 | 0.930 | `#9b00ff` (435 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.21): swatch `#678bcd`, measured lines at 0.004, 0.501, 0.878. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 4.32. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `5·T·None`; the k4 to k6 lines (None, Touch, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `5·T·None` |
| Standard spectrometer detection range | 14.54 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 955 Pz (0.05 × Q5) |
| Counter drawn cold (all six layers) | 1,911 Pz (0.10 × Q5) |
| Unravel after completion | 1,911 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 3,522 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 1.11 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 5th Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XV]] | Lex Reciprocitatis Moralis | Soul and death work returns consequence on the caster in proportion to use. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 5th Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 5 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Healing and Restoration]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Medium]] |

Similar workings: [[Greater Restoration (5-A-L-GRE)|Greater Restoration]] (5) · [[Mass Cure Wounds (5-C-L-MCW)|Mass Cure Wounds]] (5) · [[Raise Dead (5-N-M-RD)|Raise Dead]] (5) · [[Regenerate (7-T-L-RGN)|Regenerate]] (7) · [[Heal (6-V-L-HEA)|Heal]] (6) · [[Heroes' Feast (6-C-L-HF)|Heroes' Feast]] (6) · [[Thomson's Plum Pudding (2-T-L-TSPP)|Thomson's Plum Pudding]] (2) · [[Animate Objects (5-T-L-AO)|Animate Objects]] (5).


---

## Tactical Assessment

Recovery of personnel whose bodies were destroyed, at the price of a changed physiology.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 5 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
