---
tags:
  - rex-invictus/magic-system
  - rex-invictus/parzival
  - source/rex-invictus
aliases:
  - Quasi-Stable Magic Field
  - Theory of Magic Field
updated: 2026-11-16
---

**[[Thaumic Field Model]]** describes the medium every working draws on: a quasi-stable magic field that returns far more energy than a caster puts in, in discrete amounts. It is the physical basis of [[Parzival Thaumaturgy]], taken from the Theory of Magic model reproduced in *Arcane Spectroscopy* and the *Science of the Warlock Spell Compendium* ([[Source Texts (Theoretical Magic Corpus)]]), and recast in [[Parzival]] units.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - Foundations
    - [[Mana-Parzival Conversion]]
    - **Thaumic Field Model** (this note)
    - [[Parzival Energy Budget]]
    - [[Caster Capacity and Tiers]]

---

## The field equation

The source corpus writes the field's potential along an abstract coordinate x (the "position" of a working in attribute space) as

**E(x) = α·e^(−βx) − γ·e^(λx(1 − sin ωx)/2) + κx**

The first term is a decaying well that keeps low-energy workings bound; the second is a rippled, growing barrier whose sine term creates a ladder of local minima; the linear term tilts the whole landscape. The minima are where workings can sit stably, so energy is returned in steps. Rex Invictus reads each step as one tier and fixes the step ratio at *e* ([[Mana-Parzival Conversion#The fit]]).

| Symbol | Meaning in Rex Invictus |
|---|---|
| α, β | Depth and width of the ground well (cantrip floor) |
| γ, λ | Height and growth of the tier barrier; λ sets the e-fold per tier |
| ω | Spacing of the tier ladder |
| κ | Background tilt; varies with local [[Ley lines]] and [[Divine Affinity]] |
| x | Position in attribute space, set by the [[Spell Attribute Set]] |

## Workings as wave packets

A cast working is modelled as a two-dimensional Gaussian in (x, injury) space whose initial amplitude is its stored potential E_P0. As it travels, its width spreads as

**σ_x(t) = −v·λ0·t / R + λ0**, with λ0 = E_P0

where v is the working's speed and R its maximum range. The packet sheds its stored energy into three channels: retained potential ε0, kinetic εv and luminous εL, with **ε0 + εv + εL = 1**. The luminous share sets brightness, **L = εL · v · E_P0 / R**, which is why fast, short-range, high-tier workings glow brightest ([[Arcane Spectroscopy]]).

## Perturbation and return

The caster does not supply the working's energy. They supply a small perturbation (the input the corpus calls mana) that tips the field from one minimum into the next. The field then returns a quantum of energy proportional to the depth of that minimum. This is the mechanism behind the slot quantum Q_T: one tier of perturbation returns e times the energy of the tier below.

| Quantity | Caster supplies | Field returns |
|---|---|---|
| Cantrip | trivial | Q0 = 129 Pz |
| Tier 1 | 1 Mn of perturbation | Q1 = 350 Pz |
| Tier T | T Mn-steps | Q_T = 350·e^(T−1) Pz |

## Field tension

Every cast leaves the local field slightly stretched. The *Warlock Compendium* story of spell evolution describes a "taut" field in a pact dungeon that culled the brightest and fastest darts until a new form (Eldritch Blast) survived ([[Spell Evolution]]). Rex Invictus formalises this as recast tension: each recent working in the same field cell raises the cost of the next. See [[Recast Tension and Combination Affinity]].

## Interaction with the material world

- **Gravity and work:** in-world work uses local gravity (9.81 m/s² on Earth). The 15.00 m/s² of the Parzival definition is a reference standard only.
- **Interference:** two workings in the same region interfere like waves. In-phase patterns reinforce (combinations); anti-phase patterns cancel (counters). This is the physical basis of [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]].
- **Divine source:** a divine being's [[Divine Energy]] and [[Ichor]] deepen the minima they cast into, which is how [[Divine Affinity]] lowers effective cost. Mismatch produces the losses listed in [[Parzival Energy Budget#Efficiency]].

## ULMTU links

| Lex | Field-model reading |
|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] Lex Fontis | The field is the source; any sustained draw over 1 μPz/s is divine. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-II]] Lex Structurae | Stable minima are the ordered rules; the barrier between them is the unstable behaviour. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IX]] Lex Correspondentiae | A working must sit on a minimum (a valid pattern) to be returned energy. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-X]] Lex Aequilibrii | Field return is redistributed energy, not created energy. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIII]] Lex Impermanentiae | Packets spread and lose energy over time and range. |

---

## Related

[[Parzival Thaumaturgy]] · [[Mana-Parzival Conversion]] · [[Arcane Spectroscopy]] · [[Aspect Theory of Magic]] · [[Magic]] · [[Hecate]]
