---
tags:
  - rex-invictus/magic-system
  - rex-invictus/doctrine
  - rex-invictus/spell-combination
  - source/rex-invictus
aliases:
  - Recast Tension
  - Combination Affinity
  - Link Cost
  - Repeat-Cast Penalty
updated: 2026-11-16
---

**[[Recast Tension and Combination Affinity]]** are the two rules that make a working cost more when it is repeated quickly or bound to an unlike working. Recast tension is the field's lag in relaxing after a pattern is drawn. Combination affinity is the extra work of holding two patterns together when their aspects disagree. Both are Rex Invictus rules built on the [[Thaumic Field Model]] and the [[Aspect Theory of Magic]], and both are used for every costing in [[Combat Combination Analysis]].

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - Doctrine
    - **Recast Tension and Combination Affinity** (this note)
    - [[Combat Combination Analysis]]
    - [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]]

---

## Recast tension

A working leaves the local field strained around its minimum. The strain relaxes with a time constant τ. A second working drawn into the strained field must first push the strain aside.

**R = (1 + ρ)^N_eff**, with ρ = 0.05 and **N_eff = Σ w · e^(−Δt/τ)** over earlier workings by the same caster, τ = 90 s.

| Earlier working | Weight w |
|---|---|
| The same working | 1.0 |
| Another working of the same school | 0.5 |
| A working of another school | 0.25 |

The charged cost of each cast is E × R. Some consequences:

- One working cast every 6 s settles at N_eff ≈ 14.5 and R ≈ 2.0. Spam doubles the price.
- Ten Misted Leaps 6 s apart cost 987 Pz instead of 825 Pz, a 20% premium ([[Haze Screen (ML)]]).
- After 5 minutes of rest N_eff has fallen to under 4% of its value; a caster who waits 90 s between casts pays only about 1.8% extra for a repeat.
- Mixing schools spreads the load: the weights are why a battle mage alternates between unlike workings when the clock allows.

The rule restates the source's experience that the same working cast many times in a row "gets harder", and gives it a decay time so that rest restores the caster's efficiency.

## Combination affinity

A combination binds two or more workings into one effect. Each pair that is bound together has a **link cost**:

**Λ = 0.01 · Q_max + χ · (E_a + E_b) / 2**

- Q_max is the quantum of the higher tier of the pair (the cost of a shared pattern frame).
- **χ = 0.30 × (1 − cos θ) / 2**, where cos θ is the cosine between the two members' affinity vectors (school plus damage, from [[Aspect Theory of Magic]]).
- **Contrast penalty.** When cos θ is below 0, χ is multiplied by 1.5.
- **Binder discount.** When one side of the link is a binder (a working that exists to hold others, such as [[Transfiguration Inheritance (2-T-L-TI)|Transfiguration Inheritance]] or [[Magic Link (1-P-L-MLK)|Magic Link]]), χ is halved.

| cos θ | χ | Example |
|---|---|---|
| 1.0 (identical) | 0.000 | two of the same working |
| 0.5 (kin) | 0.075 | Cold with Necrotic damage |
| 0 (unrelated) | 0.150 | Acid with Force damage |
| −0.58 (opposed) | 0.355 | Cold with Lightning damage |
| −1.0 (exact opposites) | 0.450 | maximum |

The combination's total is the sum of every member's charged cost (with tension) and every link cost:

**E_combo = Σ E_i × R_i + Σ Λ_link**

The energy-equivalent tier of the combination follows from the total, and the combination is registered as `X-T-code` with T the highest member tier ([[Spell Registry Identifier Standard#Combination tags]]).

## Design rules that follow

1. **Bind like with like.** Kin members (cos above 0.5) link for little more than the frame cost.
2. **Use a binder for unlike members.** It halves χ, and it lets members be cast as dormant patterns that wait for one release.
3. **Cast the expensive member last.** Tension is charged on the later casts, so put the cheap members first and the most expensive member where N_eff is still small, or space the casts.
4. **The binder is a single point of failure.** Countering it collapses every bound member ([[Magical Countermeasures and Magical Intelligence (MCM-MINT)#Counter-counter-counter (C3)]]).

## The three field tactics

The rule was first applied to three tactics already in field use.

| Tactic | Members | Draw | Notes |
|---|---|---|---|
| [[Haze Screen (ML)\|Haze Screen]] | Misted Leap | 83 Pz per leap; 987 Pz for ten leaps | Cheapest; cost is the haze, not the hop |
| [[Slipglue Field (SL-TI-GR-GL-GY)\|Slipglue Field]] | Summon Liquid, Transfiguration Inheritance, Grease, Glue, Geyser | 1,171 Pz | Most expensive; the Geyser contrasts with the binder (cos −0.32), and the binder halves that penalty |
| [[Skymark Flare (MM-LK-AL-LT-SK)\|Skymark Flare]] | Magic Missile, Magic Link, Alarm, Magelight, Skyward | 46 Pz; 233 Pz for six in a minute | Cheap per flare; tension dominates a battery shoot |

Full tables and the five later combinations are in [[Combat Combination Analysis]].

## ULMTU links

| Lex | Application |
|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-III]] Lex Limitationis | Tension and link costs are part of what a working costs. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] Lex Interactionis | Opposed aspects interfere, which is the contrast penalty. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] Lex Nexus | Binders and links are Nexus connections between patterns. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] Lex Consequentiae | Over-tensioned fields misfire. |

---

## Related

[[Combat Combination Analysis]] · [[Aspect Theory of Magic]] · [[Parzival Energy Budget]] · [[Thaumic Field Model]] · [[Linking and Triggers]] · [[Composite]]
