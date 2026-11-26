---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-registry
  - spell/tier-2
  - spell/conjuration
  - source/srd
aliases:
  - "2nd Tier Spell: Find Steed"
  - "Find Steed"
  - "2-C-H-FS"
registry_id: 2-C-H-FS
attribute_code: "2·Con·None·None·30 feet·Instantaneous"
incantation: "Heusin"
tier: 2
school: Conjuration
affinity: C
grade: H
pz_total: 5602.4
pz_quantum: 951.4
t_e: 3.77
updated: 2026-11-16
---

**Find Steed** (`2-C-H-FS`) is a 2nd Tier working of the [[Conjuration]] school in [[Parzival Thaumaturgy]]. Source corpus spell (mechanics reference: System Reference Document 5.1). Its modelled draw is **5,602 Pz** against a slot quantum of 951 Pz, which puts its energy-equivalent tier at T_E 3.77 and its handling grade at **High**.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Registry]]
    - [[Tier 2 Workings]]
      - [[Conjuration]]
        - **Find Steed** (this note)

---

## Identification

| Field | Value |
|---|---|
| Registry tag | `2-C-H-FS` (see [[Spell Registry Identifier Standard]]) |
| Attribute code | `2·Con·None·None·30 feet·Instantaneous` |
| Incantation | *Heusin* |
| Affinity | C (Conjuration) |
| Source | SRD |

## Working Profile

| Attribute | Value |
|---|---|
| Tier | 2nd Tier |
| School | [[Conjuration]] |
| Casting time | 10 minutes |
| Range | 30 feet |
| Area | single point or target |
| Duration | Instantaneous |
| Components | spoken (incantation), somatic (glyph kata) |
| Ritual | no |
| Practitioner lineages | Paladin |

### Mechanism

The field builds a large spirit mount with an uplifted mind, a shared-working link to its rider and a telepathic bond out to 1.6 km.

---

## Energy Model

Computed under [[Parzival Energy Budget]] at ideal efficiency (η = 1). Constants come from [[Mana-Parzival Conversion]].

| Term | Formula | Pz |
|---|---|---|
| conjured body (warhorse form) | `10 Pz/kg * 540 kg` | 5,400 |
| autonomy endowment | `0.05 Pz/s * 3600 s (1 h reference)` | 180 |
| bond, cognition uplift, telepathy | `instant info` | 1.0 |
| Pattern cost | `0.01 × Q2 × (1 + 1.25)` | 21.4 |

| Quantity | Value |
|---|---|
| Effect energy | 5,581 Pz |
| Upkeep energy | 0 Pz (0 Pz/s) |
| **Total draw** | **5,602 Pz** (8,403.6 kJ) |
| Slot quantum Q2 | 951 Pz |
| Field gain (draw / quantum) | 5.89 |
| Energy-equivalent tier T_E | 3.77 |
| Handling points | 1.25 |
| Grade score | 2.14 → H |

**Handling flags:** fragile, long cast.

**Assumptions:** Warhorse 540 kg (1200 lb); 10 Pz/kg; autonomy 0.05 Pz/s booked over a 1 h reference; bond and uplift 1 Pz.

---

## Notation

### Glyph

Written as a 13-point glyph under [[Spell Writing (Glyph Notation)]], one layer per attribute with skip k equal to the attribute's place. Feature numbers come from the [[Glyph Key Tables]].

![[Find Steed (2-C-H-FS) glyph.svg]]

| Layer | Feature | Key | Binary |
|---|---|---|---|
| k1 Tier | 2 | 2 | `0000000000101` |
| k2 School | Conjuration | 1 | `0000000000011` |
| k3 Damage | None | 7 | `0000000001111` |
| k4 Area | None | 0 | `0000000000001` |
| k5 Range | 30 feet | 5 | `0000000001011` |
| k6 Duration | Instantaneous | 9 | `0000000010011` |

### Incantation

Spoken as **Heusin** under [[Spell Speech (Incantation)]] (sounds in [[Incantation Sound Tables]]).

Upcast forms: T3: *Liheusin* · T4: *Viheusin* · T5: *Tiheusin* · T6: *Riheusin* · T7: *Miheusin* · T8: *Niheusin* · T9: *Xyiheusin*.

### Somatic kata

Each stroke traces one chord from vertex a to vertex b (vertex 0 is top-right, numbered counter-clockwise; each chord runs k steps clockwise), layer by layer from k1 outward, under [[Somatic Notation (Gesture)]].

| Layer | Strokes | Count |
|---|---|---|
| k1 Tier | 0→12 2→1 | 2 |
| k2 School | 0→11 1→12 | 2 |
| k3 Damage | 0→10 1→11 2→12 3→0 | 4 |
| k4 Area | 0→9 | 1 |
| k5 Range | 0→8 1→9 3→11 | 3 |
| k6 Duration | 0→7 1→8 4→11 | 3 |

### Spectral signature

Line positions follow the rule recovered from the published plates in [[Arcane Spectroscopy]] (see [[Spectral Key Tables]]). Blended swatch colour: `#e39b09`.

![[Find Steed (2-C-H-FS) spectrum.svg]]

| Line | Feature | x | Brightness | Colour | Basis |
|---|---|---|---|---|---|
| Tier | 2 | 0.200 | 1.000 | `#ffea00` (640 nm eq.) | source grid |
| School | Conjuration | 0.125 | 0.997 | `#ff8300` (662 nm eq.) | source grid |
| Duration | Instantaneous | 0.000 | 0.980 | `#ff0028` (700 nm eq.) | source grid |
| Range | 30 feet | 0.294 | 0.996 | `#91ff00` (612 nm eq.) | source grid |

Published plate (Arcane Spectroscopy, printed p.17): swatch `#fb7c42`, measured lines at 0.004, 0.126, 0.201, 0.295. Every predicted line falls on a measured one within ±0.008.

Relative luminosity scales with initial energy: log10(E) = 3.75. Stationary castings show only the rest lines; a travelling working shifts them by v/c and brightens with speed.

### MINT and MCM profile

Under [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] a field [[Arcane Spectrometer]] classifies this working from its k1 to k3 lines. Its threat trigram is `2·C·None`; the k4 to k6 lines (None, 30 feet, Instantaneous) refine it to a registry match.

| Quantity | Value |
|---|---|
| Threat trigram (k1·k2·k3) | `2·C·None` |
| Standard spectrometer detection range | 7.48 km (r = 1 km × √(E/100 Pz)) |
| Counter with pre-loaded trigram | 47.6 Pz (0.05 × Q2) |
| Counter drawn cold (all six layers) | 95.1 Pz (0.10 × Q2) |
| Unravel after completion | 95.1 Pz (cold counter + 20% of remaining upkeep) |

### Aspect vector

Under [[Aspect Theory of Magic]] the damage aspect is Light, Life, Potential, Stagnancy and the school lean is Beyond, Prodigious, Potential, Movement. The working vector used by [[Recast Tension and Combination Affinity]] is `1a 1c 1d 1e 2F` (Beyond, Light, Life, Prodigious, 2x Potential).

---

## ULMTU Compliance

Assessed against the [[Universal Legum of Metaphysic-Thaumological Utilization]].

| Lex | Name | Application |
|---|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] | Lex Fontis | Mean draw over one 6 s cast is 934 Pz/s, far above the 1 μPz/s divine floor, so the working is classed as divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] | Lex Limitationis | Physical output is 5.89 times the tier quantum. The excess is field gain from pattern alignment and is legal only while the caster holds the full 2nd Tier pattern; a degraded pattern falls back to the quantum. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VII]] | Lex Methodi | Has a fixed, repeatable procedure (ritual or extended casting). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Lex Nexus | Operates through a connection (spatial fold, plane link or sympathetic thread). |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] | Lex Aequilibrii | Matter or motion it creates is paid for by field return; it redistributes energy and creates nothing for free. |
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
| Function | [[Summoning and Conjured Creatures]] |
| Grade | [[Spell Registry Identifier Standard#Grade\|High]] |

Similar workings: [[Temporary Magic Prism (2-C-L-TMP)|Temporary Magic Prism]] (2) · [[Arcane Singularity (3-C-L-ASA)|Arcane Singularity]] (3) · [[Conjure Animals (3-C-M-CA)|Conjure Animals]] (3) · [[Find Familiar (1-C-H-FFN)|Find Familiar]] (1) · [[Stinking Cloud (3-C-M-SCI)|Stinking Cloud]] (3) · [[Unseen Servant (1-C-M-US)|Unseen Servant]] (1) · [[Arcane Die (0-C-L-ADC)|Arcane Die]] (0) · [[Conjure Magic Prism (4-C-L-CMPJ)|Conjure Magic Prism]] (4).


---

## Tactical Assessment

Provides a loyal, resummonable mount that shares the rider's protective workings; for far-future forces it serves as a self-repairing all-terrain carrier where vehicles cannot be fuelled.

---

## Related

[[Parzival Thaumaturgy]] · [[Spell Registry]] · [[Tier 2 Workings]] · [[Conjuration]] · [[Spell Breakdown Procedure]] · [[Parzival]]
