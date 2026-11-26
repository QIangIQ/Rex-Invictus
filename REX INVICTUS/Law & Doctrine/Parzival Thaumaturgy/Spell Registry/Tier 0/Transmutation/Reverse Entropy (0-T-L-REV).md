---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-0
  - spell/transmutation
  - source/science-spellbook
aliases:
  - "Cantrip Spell: Reverse Entropy"
  - "0-T-L-REV"
  - "Reverse Entropy (Science)"
registry_id: 0-T-L-REV
attribute_code: "0·Tra·None·sphere (5)·Self·1 minute"
incantation: "Cie’-Supore"
tier: 0
school: Transmutation
affinity: T
grade: L
pz_total: 224.0
pz_quantum: 128.8
t_e: 0.55
updated: 2026-11-16
---

**Reverse Entropy** (`0-T-L-REV`) is a Cantrip (Tier 0) working of the [[Transmutation]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **224 Pz** against a slot quantum of 129 Pz, which puts its energy-equivalent tier at T_E 0.55 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 0 Workings]]
      - [[Transmutation]]
        - **Reverse Entropy** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `0-T-L-REV` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `0·Tra·None·sphere (5)·Self·1 minute` |
| Incantation | *Cie’-Supore* |
| Affinity | T (Transmutation) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | Cantrip (Tier 0) |
| School | [[Transmutation]] |
| Casting time | 1 Action |
| Range | Self |
| Area | sphere (5) |
| Duration | 1 minute |
| Components | none |
| Ritual | no |
| Practitioner lineages | Wizard, Druid, Sorcerer, Warlock |

### Mechanism

Restores order within 5 ft for a minute: broken things rejoin, mixtures separate, melt refreezes; all reverts at the end.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Entropy removed | `T dS for 1 kg ice at 273 K = 3.34e+05 J / 1500` | 223 |
| Pattern cost | `0.01 × Q0 × (1 + 0.00)` | 1.3 |

| Quantity | Value |
|---|---|
| Effect energy | 223 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **224 Pz** (335.9 kJ) |
| Slot quantum Q0 | 129 Pz |
| Field gain (draw / quantum) | 1.74 |
| Energy-equivalent tier T_E | 0.55 |
| Handling points | 0.00 |
| Grade score | 0.28 → L |

**Handling flags:** none.

**Assumptions:** Equivalent of refreezing 1 kg of melted ice: minimum work T x dS = 334 kJ (real thermodynamics).

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Reverse Entropy (0-T-L-REV) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 0 | 0 | `0000000000001` |
| k2 School | Transmutation | 7 | `0000000001111` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | sphere (5) | 34 | `0000001000101` |
| k5 Range | Self | 12 | `0000000011001` |
| k6 Duration | 1 minute | 1 | `0000000000011` |

### Incantation

Spoken as **Cie’-Supore** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T1: *Sicie’-Supore* · T2: *Hicie’-Supore* · T3: *Licie’-Supore* · T4: *Vicie’-Supore* · T5: *Ticie’-Supore* · T6: *Ricie’-Supore* · T7: *Micie’-Supore* · T8: *Nicie’-Supore* · T9: *Xyicie’-Supore*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 | 1 |
| k2 School | 0→11 1→12 2→0 3→1 | 4 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 2→11 6→2 | 3 |
| k5 Range | 0→8 3→11 4→12 | 3 |
| k6 Duration | 0→7 1→8 | 2 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#ba288c`.

![[Reverse Entropy (0-T-L-REV) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 0 | 0.000 | 1.000 | `#ff0028` (700 nm eq.) | source grid |
| School | Transmutation | 0.875 | 0.682 | `#9600ff` (438 nm eq.) | source grid |
| Duration | 1 minute | 0.105 | 0.994 | `#ff6300` (668 nm eq.) | source grid |
| Area | sphere (5) | 0.944 | 0.640 | `#f200ff` (417 nm eq.) | source grid |
| Range | Self | 0.706 | 0.779 | `#0058ff` (488 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 2.35. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `0·T·None`; the k4 to k6 lines (sphere (5), Self, 1 minute) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `0·T·None` |
| Standard spectrometer detection range | 1.50 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 6.4 Pz (0.05 × Q0) |
| Counter drawn cold (all six layers) | 12.9 Pz (0.10 × Q0) |
| Unravel after completion | 12.9 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Life, 2x Flexibility, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1c 2d 1F 2h` (Light, 2x Life, Potential, 2x Flexibility).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 37.3 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 1.74 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full Cantrip (Tier 0) pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at Cantrip (Tier 0) up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Transmutation school with aspect lean Life, 2x Flexibility, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 0 Workings]] |
| School | [[Transmutation]] |
| Affinity | [[Transmutation]] (T) |
| Function | [[Healing and Restoration]], [[Negation and Counterspell]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Shillelagh (0-T-L-SHLL)|Shillelagh]] (0) · [[Goodberry (1-T-L-GDB)|Goodberry]] (1) · [[Remove Curse (3-A-L-RC)|Remove Curse]] (3) · [[Arcane Die (0-C-L-ADC)|Arcane Die]] (0) · [[Hooke's Compelled Duel (0-E-L-HSCD)|Hooke's Compelled Duel]] (0) · [[Knock (2-T-L-KNC)|Knock]] (2) · [[Magic Weapon (2-T-L-MW)|Magic Weapon]] (2) · [[Spare the Dying (0-N-L-SD)|Spare the Dying]] (0).


---

## Tactical Assessment

Temporary field repair of equipment and evidence restoration.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 0 Workings]] · [[Transmutation]] · [[Spell Breakdown Procedure]] · [[Parzival]]
