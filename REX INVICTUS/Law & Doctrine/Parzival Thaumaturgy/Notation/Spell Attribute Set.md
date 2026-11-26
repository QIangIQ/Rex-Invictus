---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-notation
  - source/rex-invictus
aliases:
  - Six Attributes
  - Attribute Code
updated: 2026-11-16
---

**[[Spell Attribute Set]]** is the list of six attributes that define a working in [[Parzival Thaumaturgy]]. Every notation in the system encodes the same six: the glyph, the incantation, the somatic kata, the spectral lines and the registry attribute code. Knowing any one of them recovers the others.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - Notation
    - **Spell Attribute Set** (this note)
    - [[Spell Writing (Glyph Notation)]]
    - [[Spell Speech (Incantation)]]
    - [[Somatic Notation (Gesture)]]
    - [[Spell Components]]
    - [[Spell Registry Identifier Standard]]

---

## The six attributes

| Place k | Attribute | Values | Source |
|---|---|---|---|
| 1 | Tier | 0 to 9 (corpus), 10 to 14 (Rex Invictus) | all corpus texts |
| 2 | School | eight schools, plus [[Pure]] and [[Composite]] | all corpus texts |
| 3 | Damage | 13 types plus None (corpus), 18 derived types and Radiation | Spell Writing Guide, Warlock Compendium |
| 4 | Area | None or shape (size in feet) | 2024 dictionary |
| 5 | Range | Self, Touch, distances, Sight, Special, Unlimited | all dictionaries |
| 6 | Duration | Instantaneous through Until dispelled, with concentration as "Up to" | Spell Saying Guide; planned third dictionary |

The order k = 1 to 6 is fixed. The 2024 dictionary and the non-damage chapter of the 2023 dictionary place Area at k = 4 and Range at k = 5. The damage chapter of the 2023 dictionary prints the two the other way round, but its own drawings use Area k = 4 and Range k = 5 in all 71 cases, so the printed labels are an error. The registry follows the drawings.

## Why six

The Spell Writing Guide needs n ≥ 2N + 1 points to draw N attributes without two layers sharing a chord length. The corpus used five attributes on 11 points; its author noted that a third dictionary would add duration "since that is required to distinguish most spells fully". Rex Invictus adds duration as k = 6 on **13 points** (2·6 + 1), which gives 632 unique codes per attribute.

Six attributes still leave 21 groups of workings with identical sets (for example Bane, Bless and Hideous Laughter). The published spectral plates show the same collisions, which confirms the plates encode exactly these attributes. Glyphs tell these apart with centre dots; spectrometers need context ([[Magical Countermeasures and Magical Intelligence (MCM-MINT)]]).

## Area vocabulary across editions

| Edition | Area values |
|---|---|
| 2022 guide | Cube, Line, Wall, Sphere, Circle, Cone, Cylinder, Square, Single-Target (ST), Multiple-Targets (MT), ST/MT, None, and more (19 in all) |
| 2023 dictionary | the 2022 list plus Wall/Square, Cone/Line, Cyl/Circle, Line/Cube |
| 2024 dictionary | None or shape with size, for example sphere (20), cube (5280) |

ST means Single-Target and MT Multiple-Targets; the 2022 guide's figure of Eldritch Blast labels its area "ST/MT". The registry uses the 2024 form.

## Attribute code

Each registry note carries the six values as an attribute code, for example Fireball: `3·Evo·Fire·sphere (20)·150 feet·Instantaneous`. The code is the long form of the registry tag described in [[Spell Registry Identifier Standard]].

---

## Related

[[Glyph Key Tables]] · [[Incantation Sound Tables]] · [[Spectral Key Tables]] · [[Aspect Theory of Magic]] · [[Spell Breakdown Procedure]]
