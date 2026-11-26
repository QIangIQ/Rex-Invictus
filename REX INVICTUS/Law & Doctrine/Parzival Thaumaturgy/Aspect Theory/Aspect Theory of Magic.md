---
tags:
  - rex-invictus/magic-system
  - rex-invictus/aspect-theory
  - source/rex-invictus
aliases:
  - Aspect Theory
  - Ten Aspects
  - Warlock Aspects
updated: 2026-11-16
---

**[[Aspect Theory of Magic]]** describes every working as a point in a ten-dimensional space of paired qualities called aspects. Where the [[Spell Attribute Set]] says *what* a working does (tier, school, damage, area, range, duration), the aspects say *what it is made of*. The theory comes from the warlock research in *The Warlock's Spell Compendium* (The Gorilla of Destiny) and is the basis for derived damage types, [[Spell Evolution]] and the affinity penalty in [[Recast Tension and Combination Affinity]].

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - Aspect Theory
    - **Aspect Theory of Magic** (this note)
      - [[Aspect Interpolation and Derived Damage Types]]
      - [[Spell Evolution]]

---

## The ten aspects

Each axis has a positive pole (lower-case letter) and a negative pole (capital letter). A count of 2 on the negative pole is written as −2 on the shared axis.

| Axis | Positive (letter) | Negative (letter) |
|---|---|---|
| 1 | Beyond (a) | Within (A) |
| 2 | Heat (b) | Cold (B) |
| 3 | Light (c) | Dark (C) |
| 4 | Life (d) | Death (D) |
| 5 | Prodigious (e) | Diminutive (E) |
| 6 | Energy (f) | Potential (F) |
| 7 | Extraspection (g) | Introspection (G) |
| 8 | Flexibility (h) | Rigidity (H) |
| 9 | Hope (i) | Hopelessness (I) |
| 10 | Movement (j) | Stagnancy (J) |

In the source the aspects are written in a custom monoline script of straight strokes and quarter arcs, one glyph per letter, with the negative pole drawn as the positive glyph under an overbar. The registry writes them as letters.

## Rules

1. **Four slots.** An attribute value is built from exactly four aspect units; the absolute values sum to 4. Lightning is 2 Heat, Light and Movement (2b 1c 1j).
2. **Opposites cancel.** A positive and a negative unit on the same axis annihilate, so no value holds both poles of one axis.
3. **Values are whole.** Every stable value sits on a lattice point with whole counts. A point between lattice points is unstable and costs energy to hold ([[Aspect Interpolation and Derived Damage Types]]).
4. **Similarity is an angle.** Two values are compared by the cosine of the angle between their vectors (cos = 1 identical, 0 unrelated, below 0 opposed).

## Published compositions

The source prints four compositions in full: Lightning (2b 1c 1j), Necrotic (2D 2E), Cold (2B 2D) and Void (1B 2D 1E). It also prints the full six-row aspect blocks of the twelve Magic Missile and Eldritch Blast nodes in the Alnish evolution tree ([[Spell Evolution]]). No page lists the make-up of the other damage types, the schools, areas, ranges or durations.

## Registry compositions

### Damage types

The registry reconstructed the remaining damage types so that the interpolation rule reproduces every one of the 74 published rows of the source's interpolation tables (18 named types and 56 rows with free slots). Cold, Necrotic and Lightning are as published.

| Damage | Code | Aspects | Status |
|---|---|---|---|
| None | 1c 1d 1F 1J | Light, Life, Potential, Stagnancy | reconstructed |
| Acid | 1b 1D 2E | Heat, Death, 2× Diminutive | reconstructed |
| Bludgeoning | 1A 1H 2j | Within, Rigidity, 2× Movement | reconstructed |
| Cold | 2B 2D | 2× Cold, 2× Death | published |
| Fire | 1b 1c 1f 1j | Heat, Light, Energy, Movement | reconstructed |
| Force | 1a 1G 2j | Beyond, Introspection, 2× Movement | reconstructed |
| Lightning | 2b 1c 1j | 2× Heat, Light, Movement | published |
| Necrotic | 2D 2E | 2× Death, 2× Diminutive | published |
| Piercing | 1a 1B 1I 1j | Beyond, Cold, Hopelessness, Movement | reconstructed |
| Poison | 1A 1B 1D 1E | Within, Cold, Death, Diminutive | reconstructed |
| Psychic | 1C 1F 1G 1I | Dark, Potential, Introspection, Hopelessness | reconstructed |
| Radiant | 1b 1c 1d 1i | Heat, Light, Life, Hope | reconstructed |
| Slashing | 1B 1H 2j | Cold, Rigidity, 2× Movement | reconstructed |
| Thunder | 2b 1C 1j | 2× Heat, Dark, Movement | reconstructed |
| Radiation (RI) | 1b 1c 1D 1f | Heat, Light, Death, Energy | Rex Invictus addition |

The reconstruction is one solution that fits every published row; the source admits others. The Alnish tree suggests a second reading of Force (2j 1g 1h) for its damage row. The registry keeps the table above because it reproduces the published interpolation data, and treats the Alnish reading as a variant pattern of the same damage type.

### Schools

The source gives no school compositions. The registry assigns four units each under the same rules, chosen from the school's character. Composite (combinations) is the null vector because its make-up is that of its members.

| School | Code | Aspects |
|---|---|---|
| [[Abjuration]] | 1A 1H 1i 1J | Within, Rigidity, Hope, Stagnancy |
| [[Conjuration]] | 1a 1e 1F 1j | Beyond, Prodigious, Potential, Movement |
| [[Divination]] | 1a 1c 2g | Beyond, Light, 2× Extraspection |
| [[Enchantment]] | 1A 1G 1h 1i | Within, Introspection, Flexibility, Hope |
| [[Evocation]] | 1b 2f 1j | Heat, 2× Energy, Movement |
| [[Illusion]] | 1c 1G 2h | Light, Introspection, 2× Flexibility |
| [[Necromancy (School)\|Necromancy]] | 1A 1C 2D | Within, Dark, 2× Death |
| [[Transmutation]] | 1d 2h 1j | Life, 2× Flexibility, Movement |
| [[Pure]] | 2f 1H 1j | 2× Energy, Rigidity, Movement |
| [[Composite]] | 0 | null |

## Uses in the registry

- **Affinity vector.** A working's affinity vector is its school vector plus its damage vector. Every registry note prints it.
- **Combination penalty.** The cosine between two members' affinity vectors sets the link cost χ in a combination ([[Recast Tension and Combination Affinity]]). Contrasting members (cos below 0) pay half again.
- **Divine affinity.** A god's domain can be written as an aspect vector. A working whose vector points along the caster's [[Divine Affinity]] draws more easily; one that points against it pays the contrast penalty against the caster's own pattern.
- **Derived damage.** New damage types are lattice points reached by interpolating between two published types ([[Aspect Interpolation and Derived Damage Types]]).
- **Evolution.** Small changes to one aspect row under environmental pressure produce variant workings ([[Spell Evolution]]).

## ULMTU links

| Lex | Application |
|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IX]] Lex Correspondentiae | Aspects are the correspondences a pattern carries; like attracts like. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] Lex Interactionis | Opposed aspects interfere; this is the root of the contrast penalty. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] Lex Consequentiae | Holding a value off the lattice is unstable and its cost is paid in field energy. |

---

## Related

[[Aspect Interpolation and Derived Damage Types]] · [[Spell Evolution]] · [[Spell Attribute Set]] · [[Recast Tension and Combination Affinity]] · [[Warlocks]] · [[Divine Affinity]]
