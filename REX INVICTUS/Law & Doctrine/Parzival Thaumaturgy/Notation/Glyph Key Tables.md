---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-notation
aliases:
  - "Glyph Keys"
updated: 2026-11-16
---


**[[Glyph Key Tables]]** give the feature number and 13-bit binary for every value of every attribute used in [[Spell Writing (Glyph Notation)]]. Numbers are cyclically unique binary necklaces in ascending order with the all-zero string skipped. Source features keep the order of the corpus (ASCII sort, as in the Spell Saying Guide); Rex Invictus additions are appended after them so that source indices never move.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Writing (Glyph Notation)]]
    - **Glyph Key Tables** (this note)

---

## k1 Tier

| Key | Feature | Binary (n = 13) | Origin |
|---|---|---|---|
| 0 | Cantrip (Tier 0) | `0000000000001` | source |
| 1 | 1st Tier | `0000000000011` | source |
| 2 | 2nd Tier | `0000000000101` | source |
| 3 | 3rd Tier | `0000000000111` | source |
| 4 | 4th Tier | `0000000001001` | source |
| 5 | 5th Tier | `0000000001011` | source |
| 6 | 6th Tier | `0000000001101` | source |
| 7 | 7th Tier | `0000000001111` | source |
| 8 | 8th Tier | `0000000010001` | source |
| 9 | 9th Tier | `0000000010011` | source |
| 10 | 10th Tier | `0000000010101` | Rex Invictus |
| 11 | 11th Tier | `0000000010111` | Rex Invictus |
| 12 | 12th Tier | `0000000011001` | Rex Invictus |
| 13 | 13th Tier | `0000000011011` | Rex Invictus |
| 14 | 14th Tier | `0000000011101` | Rex Invictus |

## k2 School

| Key | Feature | Binary (n = 13) | Origin |
|---|---|---|---|
| 0 | Abjuration | `0000000000001` | source |
| 1 | Conjuration | `0000000000011` | source |
| 2 | Divination | `0000000000101` | source |
| 3 | Enchantment | `0000000000111` | source |
| 4 | Evocation | `0000000001001` | source |
| 5 | Illusion | `0000000001011` | source |
| 6 | Necromancy | `0000000001101` | source |
| 7 | Transmutation | `0000000001111` | source |
| 8 | Pure | `0000000010001` | Rex Invictus |
| 9 | Composite | `0000000010011` | Rex Invictus |

## k3 Damage

| Key | Feature | Binary (n = 13) | Origin |
|---|---|---|---|
| 0 | Acid | `0000000000001` | source |
| 1 | Bludgeoning | `0000000000011` | source |
| 2 | Cold | `0000000000101` | source |
| 3 | Fire | `0000000000111` | source |
| 4 | Force | `0000000001001` | source |
| 5 | Lightning | `0000000001011` | source |
| 6 | Necrotic | `0000000001101` | source |
| 7 | None | `0000000001111` | source |
| 8 | Piercing | `0000000010001` | source |
| 9 | Poison | `0000000010011` | source |
| 10 | Psychic | `0000000010101` | source |
| 11 | Radiant | `0000000010111` | source |
| 12 | Slashing | `0000000011001` | source |
| 13 | Thunder | `0000000011011` | source |
| 14 | Tarnish | `0000000011101` | Rex Invictus |
| 15 | Frost | `0000000011111` | Rex Invictus |
| 16 | Spark | `0000000100001` | Rex Invictus |
| 17 | Wither | `0000000100011` | Rex Invictus |
| 18 | Corrosive | `0000000100101` | Rex Invictus |
| 19 | Alkaline | `0000000100111` | Rex Invictus |
| 20 | Hydraulic | `0000000101001` | Rex Invictus |
| 21 | Venom | `0000000101011` | Rex Invictus |
| 22 | Spiritual | `0000000101101` | Rex Invictus |
| 23 | Stress | `0000000101111` | Rex Invictus |
| 24 | Tempest | `0000000110001` | Rex Invictus |
| 25 | Void | `0000000110011` | Rex Invictus |
| 26 | Ice | `0000000110101` | Rex Invictus |
| 27 | Storm | `0000000110111` | Rex Invictus |
| 28 | Vitriol | `0000000111001` | Rex Invictus |
| 29 | Psionic | `0000000111011` | Rex Invictus |
| 30 | Divine | `0000000111101` | Rex Invictus |
| 31 | Righteous | `0000000111111` | Rex Invictus |
| 32 | Radiation | `0000001000001` | Rex Invictus |

## k4 Area

| Key | Feature | Binary (n = 13) | Origin |
|---|---|---|---|
| 0 | None | `0000000000001` | source |
| 1 | cone (15) | `0000000000011` | source |
| 2 | cone (30) | `0000000000101` | source |
| 3 | cone (40) | `0000000000111` | source |
| 4 | cone (60) | `0000000001001` | source |
| 5 | cube (10) | `0000000001011` | source |
| 6 | cube (100) | `0000000001101` | source |
| 7 | cube (15) | `0000000001111` | source |
| 8 | cube (150) | `0000000010001` | source |
| 9 | cube (20) | `0000000010011` | source |
| 10 | cube (200) | `0000000010101` | source |
| 11 | cube (2500) | `0000000010111` | source |
| 12 | cube (30) | `0000000011001` | source |
| 13 | cube (40) | `0000000011011` | source |
| 14 | cube (40000) | `0000000011101` | source |
| 15 | cube (5) | `0000000011111` | source |
| 16 | cube (5280) | `0000000100001` | source |
| 17 | cylinder (10) | `0000000100011` | source |
| 18 | cylinder (20) | `0000000100101` | source |
| 19 | cylinder (40) | `0000000100111` | source |
| 20 | cylinder (5) | `0000000101001` | source |
| 21 | cylinder (50) | `0000000101011` | source |
| 22 | cylinder (60) | `0000000101101` | source |
| 23 | line (100) | `0000000101111` | source |
| 24 | line (50) | `0000000110001` | source |
| 25 | line (60) | `0000000110011` | source |
| 26 | line (90) | `0000000110101` | source |
| 27 | sphere (10) | `0000000110111` | source |
| 28 | sphere (100) | `0000000111001` | source |
| 29 | sphere (15) | `0000000111011` | source |
| 30 | sphere (20) | `0000000111101` | source |
| 31 | sphere (30) | `0000000111111` | source |
| 32 | sphere (360) | `0000001000001` | source |
| 33 | sphere (40) | `0000001000011` | source |
| 34 | sphere (5) | `0000001000101` | source |
| 35 | sphere (60) | `0000001000111` | source |
| 36 | cylinder (15) | `0000001001001` | Rex Invictus |
| 37 | cylinder (30) | `0000001001011` | Rex Invictus |
| 38 | cylinder (5280) | `0000001001101` | Rex Invictus |
| 39 | sphere (120) | `0000001001111` | Rex Invictus |
| 40 | sphere (150) | `0000001010001` | Rex Invictus |
| 41 | sphere (300) | `0000001010011` | Rex Invictus |
| 42 | sphere (5280) | `0000001010101` | Rex Invictus |

## k5 Range

| Key | Feature | Binary (n = 13) | Origin |
|---|---|---|---|
| 0 | 1 mile | `0000000000001` | source |
| 1 | 10 feet | `0000000000011` | source |
| 2 | 100 feet | `0000000000101` | source |
| 3 | 120 feet | `0000000000111` | source |
| 4 | 150 feet | `0000000001001` | source |
| 5 | 30 feet | `0000000001011` | source |
| 6 | 300 feet | `0000000001101` | source |
| 7 | 5 feet | `0000000001111` | source |
| 8 | 500 feet | `0000000010001` | source |
| 9 | 500 miles | `0000000010011` | source |
| 10 | 60 feet | `0000000010101` | source |
| 11 | 90 feet | `0000000010111` | source |
| 12 | Self | `0000000011001` | source |
| 13 | Sight | `0000000011011` | source |
| 14 | Special | `0000000011101` | source |
| 15 | Touch | `0000000011111` | source |
| 16 | Unlimited | `0000000100001` | source |
| 17 | 10 miles | `0000000100011` | Rex Invictus |
| 18 | 15 feet | `0000000100101` | Rex Invictus |
| 19 | 20 feet | `0000000100111` | Rex Invictus |

## k6 Duration

| Key | Feature | Binary (n = 13) | Origin |
|---|---|---|---|
| 0 | 1 hour | `0000000000001` | source |
| 1 | 1 minute | `0000000000011` | source |
| 2 | 1 round | `0000000000101` | source |
| 3 | 10 days | `0000000000111` | source |
| 4 | 10 minutes | `0000000001001` | source |
| 5 | 24 hours | `0000000001011` | source |
| 6 | 30 days | `0000000001101` | source |
| 7 | 7 days | `0000000001111` | source |
| 8 | 8 hours | `0000000010001` | source |
| 9 | Instantaneous | `0000000010011` | source |
| 10 | Special | `0000000010101` | source |
| 11 | Until dispelled | `0000000010111` | source |
| 12 | Up to 1 hour | `0000000011001` | source |
| 13 | Up to 1 minute | `0000000011011` | source |
| 14 | Up to 1 round | `0000000011101` | source |
| 15 | Up to 10 minutes | `0000000011111` | source |
| 16 | Up to 2 hours | `0000000100001` | source |
| 17 | Up to 24 hours | `0000000100011` | source |
| 18 | Up to 8 hours | `0000000100101` | source |
| 19 | 1 day | `0000000100111` | Rex Invictus |
| 20 | 1 hour or until dispelled | `0000000101001` | Rex Invictus |
| 21 | 6 hours | `0000000101011` | Rex Invictus |
| 22 | Up to 1 minute or until the target moves | `0000000101101` | Rex Invictus |
| 23 | until the beginning of your next turn | `0000000101111` | Rex Invictus |
| 24 | until the end of your turn | `0000000110001` | Rex Invictus |
| 25 | until the end of your turn or a spell is cast through the prism | `0000000110011` | Rex Invictus |
| 26 | until used or short rest | `0000000110101` | Rex Invictus |

## Related

[[Spell Writing (Glyph Notation)]] · [[Spell Attribute Set]] · [[Incantation Sound Tables]]
