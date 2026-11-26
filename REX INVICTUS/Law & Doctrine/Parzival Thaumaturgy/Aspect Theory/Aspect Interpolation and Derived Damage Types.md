---
tags:
  - rex-invictus/magic-system
  - rex-invictus/aspect-theory
  - source/rex-invictus
aliases:
  - Derived Damage Types
  - Interpolated Damage Types
  - Void Damage
updated: 2026-11-16
---

**[[Aspect Interpolation and Derived Damage Types]]** covers how new damage types are made by sliding between two existing ones in aspect space, and what that costs. It applies the rules of [[Aspect Theory of Magic]] and follows the method of *The Warlock's Spell Compendium*, chapter 2.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Aspect Theory of Magic]]
    - **Aspect Interpolation and Derived Damage Types** (this note)

---

## Method

1. **Path.** Take two damage vectors A and B. Points on the straight path between them are C = (1 − f)·A + f·B for 0 < f < 1.
2. **Nearest lattice point.** Round C to whole counts to get P. P must hold at most four units and must differ from A and from B.
3. **Projection.** Find the point on the path closest to P: f_P = (P − A)·(B − A) / |B − A|², and the distance d = |A + f_P·(B − A) − P|.
4. **Additional energy.** d is the work needed to pull the pattern from the path onto the lattice point. It stabilises the new type and adds no damage.
5. **Free slots.** When P holds fewer than four units, the rest are free slots the caster may fill with any aspect. Each filled slot adds to the energy (the source's second table).

A distance of zero means the path crosses the lattice exactly. Void, halfway between Cold and Necrotic, is the one published case: it needs no extra energy.

## Cost in Parzivals

The source's rule is that a working with an interpolated type must be cast at least ⌈d⌉ tiers higher: 0.82 needs one tier more, 1.3 needs two. In Parzival terms the working's pattern must sit on the quantum of tier T + ⌈d⌉ ([[Caster Capacity and Tiers]]).

| Term | Value |
|---|---|
| Tier needed | T + ⌈d⌉ |
| Pattern surcharge | 0.01 × (Q_{T+⌈d⌉} − Q_T) = 0.01 × Q_T × (e^⌈d⌉ − 1) |
| Field return ceiling | Q_{T+⌈d⌉} instead of Q_T |
| Damage | unchanged; dice are interpolated (n′ = (1 − f)n₁ + f·n₂, s′ likewise, rounded up) |

A Fireball recast as Storm (d = 0.60) must be held on the Tier 4 quantum: the pattern surcharge is 0.01 × 2,586 × 1.718 ≈ 44 Pz, and the caster must be able to reach Tier 4 at all. For a cantrip the surcharge is trivial; the tier floor is what bites.

## Named derived types

The vectors below are the lattice points the method gives with the registry compositions. The f and d values are the source's.

| Name | From | To | f | d | Aspects | cos(A, B) |
|---|---|---|---|---|---|---|
| Tarnish | None | Acid | 0.33 | 0.82 | Light, Diminutive, Potential, Stagnancy | −0.20 |
| Frost | None | Cold | 0.31 | 0.66 | Cold, Light, Potential, Stagnancy | −0.35 |
| Spark | None | Lightning | 0.40 | 0.63 | Heat, Light, Life, Potential | 0.00 |
| Wither | None | Necrotic | 0.31 | 0.66 | Light, Diminutive, Potential, Stagnancy | −0.35 |
| Corrosive | Acid | Bludgeoning | 0.33 | 0.82 | Heat, Death, Diminutive, Movement | 0.00 |
| Alkaline | Acid | Cold | 0.64 | 0.46 | Cold, 2× Death, Diminutive | 0.00 |
| Hydraulic | Acid | Force | 0.33 | 0.82 | Heat, Death, Diminutive, Movement | 0.00 |
| Venom | Acid | Piercing | 0.67 | 0.82 | Beyond, Diminutive, Hopelessness, Movement | −0.20 |
| Spiritual | Acid | Radiant | 0.60 | 0.63 | Heat, Light, Diminutive, Hope | 0.00 |
| Stress | Cold | Fire | 0.69 | 0.66 | Light, Death, Energy, Movement | −0.35 |
| Tempest | Cold | Lightning | 0.73 | 0.60 | Heat, Light, Death, Movement | −0.58 |
| **Void** | Cold | Necrotic | 0.50 | **0.00** | Cold, 2× Death, Diminutive | 0.50 |
| Ice | Cold | Slashing | 0.40 | 0.63 | 2× Cold, Death, Movement | 0.29 |
| Storm | Cold | Thunder | 0.73 | 0.60 | Heat, Dark, Death, Movement | −0.58 |
| Vitriol | Force | Poison | 0.67 | 0.82 | Cold, Death, Diminutive, Movement | −0.20 |
| Psionic | Lightning | Psychic | 0.67 | 0.82 | Heat, Potential, Introspection, Hopelessness | −0.20 |
| Divine | Necrotic | Radiant | 0.69 | 0.66 | Heat, Light, Diminutive, Hope | −0.35 |
| Righteous | Radiant | Slashing | 0.33 | 0.82 | Light, Life, Hope, Movement | −0.20 |

Some names share a lattice point (Tarnish and Wither; Corrosive and Hydraulic; Alkaline and Void; Spiritual and Divine). They are the same field pattern reached from different parents and differ only in the dice they carry. The source invites casters to rename them.

Radiation is a Rex Invictus addition (1b 1c 1D 1f) used for reactor and nuclear-adjacent workings. It is treated as a primary type in the registry.

Each derived type has its own sound in [[Incantation Sound Tables]] and its own glyph value after the source list in [[Glyph Key Tables]]. Workings that use them file under the matching element family (Frost and Ice under [[Cold and Ice Workings]], for example).

## Field rules

- **Resistance.** A target resistant or immune to either parent resists the derived type. Where precision matters, interpolate the resistance factor: r = (1 − f)·r₁ + f·r₂ with immunity 0 and resistance 0.5.
- **Wards.** A ward keyed to a parent type covers the derived type at the interpolated factor.
- **Spectrum.** A derived damage line sits at its own position on the damage scale ([[Spectral Key Tables]]), so a spectrometer trained only on the source types will misclassify it on first sight. MCM suites carry the derived lines ([[Magical Countermeasures and Magical Intelligence (MCM-MINT)]]).

## ULMTU links

| Lex | Application |
|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] Lex Limitationis | The stabilising energy is a real cost that buys no damage. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] Lex Consequentiae | A derived type cast without its tier floor collapses to the nearer parent. |

---

## Related

[[Aspect Theory of Magic]] · [[Spell Evolution]] · [[Spell Attribute Set]] · [[Parzival Energy Budget]] · [[Spell Families]]
