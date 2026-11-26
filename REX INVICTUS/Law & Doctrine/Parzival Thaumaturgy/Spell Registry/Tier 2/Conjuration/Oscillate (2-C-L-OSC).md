---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/conjuration
  - source/science-spellbook
aliases:
  - "2nd Tier Spell: Oscillate"
  - "2-C-L-OSC"
  - "Oscillate (Science)"
registry_id: 2-C-L-OSC
attribute_code: "2·Con·None·None·Touch·Up to 1 minute or until the target moves"
incantation: "Helixbel"
tier: 2
school: Conjuration
affinity: C
grade: L
pz_total: 22.1
pz_quantum: 951.4
t_e: -1.76
updated: 2026-11-16
---

**Oscillate** (`2-C-L-OSC`) is a 2nd Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell ([[Science Spellbook Registry|The Science Spellbook]]). Its modelled draw is **22.1 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E -1.76 and its handling grade at **Low**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Conjuration]]
        - **Oscillate** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-C-L-OSC` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Con·None·None·Touch·Up to 1 minute or until the target moves` |
| Incantation | *Helixbel* |
| Affinity | C (Conjuration) |
| Source | Science Spellbook |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Conjuration]] |
| Casting time | 1 Bonus Action |
| Range | Touch |
| Area | single point or target |
| Duration | Up to 1 minute or until the target moves (concentration) |
| Components | somatic (glyph kata), material focus. Material: A spring |
| Ritual | no |
| Practitioner lineages | Wizard, Sorcerer |

### Mechanism

Lets a willing creature flip once per round between its position and a second point within 30 ft.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| Position flips (upkeep) | `10 x 0.01 x 80 kg x 15 x 9.144 m / 1500` | 0.732 |
| Pattern cost | `0.01 × Q2 × (1 + 1.25)` | 21.4 |

| Quantity | Value |
|---|---|
| Effect energy | 0 Pz |
| Upkeep energy | 0.732 Pz (0.0122 Pz/s) |
| **Total draw** | **22.1 Pz** (33.2 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 0.0233 |
| Energy-equivalent tier T_E | -1.76 |
| Handling points | 1.25 |
| Grade score | 0.25 → L |

**Handling flags:** concentration, fragile.

**Assumptions:** Ten jumps of 9.144 m for an 80 kg creature by the translocation rule.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Oscillate (2-C-L-OSC) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | Touch | 15 | `0000000011111` |
| k6 Duration | Up to 1 minute or until the target moves | 22 | `0000000101101` |

### Incantation

Spoken as **Helixbel** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Lihelixbel* · T4: *Vihelixbel* · T5: *Tihelixbel* · T6: *Rihelixbel* · T7: *Mihelixbel* · T8: *Nihelixbel* · T9: *Xyihelixbel*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 2→10 3→11 4→12 | 5 |
| k6 Duration | 0→7 2→9 3→10 5→12 | 4 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#ac7774`.

![[Oscillate (2-C-L-OSC) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.997 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Up to 1 minute or until the target moves | 0.711 | 0.878 | `#0053ff` (487 nm eq.) | RI half-step |
| Range | Touch | 0.882 | 0.792 | `#9b00ff` (435 nm eq.) | source grid |

Relative luminosity scales with initial energy: log10(E) = 1.35. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·C·None`; the k4 to k6 lines (None, Touch, Up to 1 minute or until the target moves) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·C·None` |
| Standard spectrometer detection range | 0.47 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 95.3 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 3.7 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Draw sits inside the 2nd Tier quantum of 951 Pz (2.3% of it). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | Lex Persistens Ontologica | Held by the caster's attention; the effect ceases without that support. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Lex Consequentiae | Breaks under injury or interruption; a broken cast can misfire. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVIII]] | Lex Curvae Magisterii | Mastery runs from access at 2nd Tier up through upcasting; see [[Caster Capacity and Tiers]]. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIX]] | Lex Specialisationis Thematicae | Specialised under the Conjuration school with aspect lean Beyond, Prodigious, Potential, Movement. |

---

## Classification

| Classifier | Browse |
|---|---|
| Tier | [[Tier 2 Workings]] |
| School | [[Conjuration]] |
| Affinity | [[Conjuration]] (C) |
| Function | [[Negation and Counterspell]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|Low]] |

Similar workings: [[Animal Messenger (2-E-L-AM)|Animal Messenger]] (2) · [[Arcane Die (0-C-L-ADC)|Arcane Die]] (0) · [[Arcane Lock (2-A-L-AL)|Arcane Lock]] (2) · [[Blindness-Deafness (2-N-L-BD)|Blindness/Deafness]] (2) · [[Gust of Wind (2-V-M-GW)|Gust of Wind]] (2) · [[Knock (2-T-L-KNC)|Knock]] (2) · [[Magic Weapon (2-T-L-MW)|Magic Weapon]] (2) · [[Ray of Enfeeblement (2-N-L-RE)|Ray of Enfeeblement]] (2).


---

## Tactical Assessment

Peek-and-shoot from cover, or holding two positions at once.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
