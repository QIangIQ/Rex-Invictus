---
tags:
  - rex-invictus/magic-system
  - rex-invictus/parzival
  - source/rex-invictus
updated: 2026-11-16
aliases:
  - Mana to Parzival Ratio
  - Slot Quantum
---

**[[Mana-Parzival Conversion]]** fixes how the loosely defined "mana" of the [[Source Texts (Theoretical Magic Corpus)|Theoretical Magic corpus]] converts into the [[Parzival]] (Pz), the defined unit of magical energy in the Rex Invictus setting. It is the first step of [[Parzival Thaumaturgy]] and every other note in that system depends on it.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - Foundations
    - **Mana-Parzival Conversion** (this note)
    - [[Thaumic Field Model]]
    - [[Parzival Energy Budget]]
    - [[Caster Capacity and Tiers]]

---

## The Problem

The [[Parzival]] is defined: 1 Pz is the work of lifting 10 kg through 10 m under the standard gravity of 15.00 m/s², which is 1,500 J, performed by a standard divine being of 100 years of age and neutral [[Divine Affinity]] at ideal efficiency.

Mana, as the source corpus uses it, has no unit. The corpus measures spells in discrete levels (cantrip, then 1 to 9) and states only two quantitative things about the energy behind them:

1. **The quasi-stable field.** A caster gives a small perturbation to a quasi-stable magic field, and the field returns a far larger amount of energy in discrete amounts. The returned energy is related exponentially to the energy put in ([[Thaumic Field Model]], from *Arcane Spectroscopy* section 2.2).
2. **Luminosity tracks initial energy.** A travelling spell bleeds part of its stored potential energy as light, with luminosity L = ε_L · v · E_P0 / R. Spells of higher level are brighter because their initial energy grows exponentially with level ([[Arcane Spectroscopy]], equations 9 to 18 and figure 3.1).

So the corpus gives a shape (exponential in level) and no scale. The conversion below supplies the scale by measuring what spells physically do.

---

## Method

Three independent anchors were used, then the exponential was fitted.

### Anchor 1: the injury constant (κ)

The corpus never states how much energy one point of injury costs. The cleanest physical anchor in the source rules is falling injury: a fall of 10 ft (3.048 m) inflicts an average of 3.5 points of injury. An 80 kg humanoid falling that distance arrives with 80 × 9.81 × 3.048 = 2,392 J. That gives **683 J per point of blunt, whole-body injury, or 0.456 Pz per point**. Every damage coefficient in [[Parzival Energy Budget#Injury coefficients|the injury table]] is scaled from this value.

### Anchor 2: benchmark workings

Workings whose physical output can be computed directly, at η = 1 and Earth gravity:

| Benchmark (source level) | Physical model | Energy | Pz |
|---|---|---|---|
| Mage Hand (0), one lift | 4.5 kg raised 9.1 m | 0.41 kJ | 0.27 |
| Burning Hands (1) | 10.5 injury, fire, 15 ft cone fluence | 213 kJ | 142 |
| Feather Fall (1), two bodies | 160 kg held at 3 m/s descent | 4.7 kW | 3.1 Pz/s |
| Shatter (2) | 13.5 injury, thunder, 10 ft sphere fluence | 2.0 MJ | 1,350 |
| Fireball (3) | 28 injury, fire, 20 ft sphere fluence | 19.2 MJ (≈4.6 kg TNT) | 12,800 |
| Cone of Cold (5) | 36 injury, cold, 60 ft cone fluence | 12 MJ | 8,000 |
| Move Earth (6), one reshaping | 2.9 × 10⁶ kg of soil moved 6 m | 171 MJ | 114,000 |
| Meteor Swarm (9) | 4 × 40 ft spheres, 70 fire + 70 blunt injury | 1.27 GJ | 845,000 |

The fluence model for area workings is explained in [[Parzival Energy Budget#Area geometry]].

### Anchor 3: a canon observation

In [[Ch20 - Rex Invictus XIII]], [[Ione]]'s augur reports his [[Hexenlaufgerät Erweiterte Thaumaturgische Bewegungsplattform für Runische Vorfeldkonstruktion und Kontinuierliche Glyphenvernetzungseinheit (Tochter des Elysium Serienstandard–Variante IX Beta-Null Mk.CLVI|Hexenlaufgerät]] array at 5 Pz/s while it carries him and [[Iane]] down a mountainside. Two armoured bodies (about 160 kg) descending at a held rate need m · g · v of braking power: at 3 m/s that is 4.7 kW, or **3.1 Pz/s**, the same order as the canon reading. The remaining 1.9 Pz/s is the array's own pattern upkeep. The conversion therefore agrees with the one number the manuscript already prints.

### The fit

A log-linear fit of the benchmark energies against source level, excluding cantrips (whose output is capped by tactical design), gives a growth factor of 2.62 per level, within 4 percent of *e*. The corpus says the field return is exponential, so the base was fixed at *e* and only the scale was fitted.

---

## The Conversion

> **1 Mana Unit (1 Mn) is the field return of one first-tier working: 1 Mn = 350 Pz = 525 kJ.**
>
> A tier-T working is supplied by a **Slot Quantum** of **Q_T = 350 Pz · e^(T−1)**, so each tier carries *e* (about 2.718) times the energy of the tier below it.

Mana in the corpus is the caster's *input*; the Parzival measures the field's *return*. The relation between them is the exponential of the [[Thaumic Field Model]], so there is no single fixed ratio across all tiers. The practical statements are:

- **Headline ratio:** 1 Mn ≡ 350 Pz (a first-tier quantum).
- **Per tier:** spending tier-T mana yields Q_T Pz, which equals 350 · e^(T−1) Pz.
- **Marginal ratio:** one more tier of input multiplies the return by *e*.

### Slot Quantum table

| Tier | Q_T (Pz) | Energy | TNT equivalent | Burst power over 6 s |
|---|---|---|---|---|
| 0 (cantrip) | 129 | 0.19 MJ | 0.05 kg | 21 Pz/s |
| 1 | 350 | 0.53 MJ | 0.13 kg | 58 Pz/s |
| 2 | 951 | 1.43 MJ | 0.34 kg | 159 Pz/s |
| 3 | 2,586 | 3.88 MJ | 0.93 kg | 431 Pz/s |
| 4 | 7,030 | 10.5 MJ | 2.5 kg | 1,172 Pz/s |
| 5 | 19,109 | 28.7 MJ | 6.9 kg | 3,185 Pz/s |
| 6 | 51,945 | 77.9 MJ | 18.6 kg | 8,657 Pz/s |
| 7 | 141,200 | 212 MJ | 51 kg | 23,533 Pz/s |
| 8 | 383,822 | 576 MJ | 138 kg | 63,970 Pz/s |
| 9 | 1,043,335 | 1.57 GJ | 374 kg | 173,889 Pz/s |
| 10 | 2,836,079 | 4.25 GJ | 1.0 t | 472,680 Pz/s |
| 11 | 7.71 MPz | 11.6 GJ | 2.8 t | |
| 12 | 20.96 MPz | 31.4 GJ | 7.5 t | |
| 13 | 56.96 MPz | 85.4 GJ | 20 t | |
| 14 | 154.8 MPz | 232 GJ | 56 t | |

Tiers above 9 are a Rex Invictus extension. The corpus already contains a "10th level" working (*Supermassive Black Hole* in the [[Science Spellbook Registry|Science Spellbook]]), so the scale is continued rather than capped.

### Energy-equivalent tier

Any working with a computed energy E can be placed on the scale:

**T_E = 1 + ln(E / 350 Pz)**

T_E is used by the [[Spell Registry Identifier Standard]] to grade how hard a spell runs against its nominal tier. Fireball, for example, computes to T_E ≈ 4.6 while being a third-tier working. It draws about five times its own quantum, which matches its long reputation as an over-curve evocation. In-field this is explained by Evocation's high field gain on the Heat aspect ([[Aspect Theory of Magic]]).

---

## Assumptions

1. The field return is exponential in tier, as both [[Thaumic Field Model|the field model]] and the [[Arcane Spectroscopy|luminosity data]] state. The base *e* comes from fitting, not from the corpus.
2. Benchmarks are taken at ideal efficiency (η = 1) as the [[Parzival]] definition requires. Real castings pay the losses listed in [[Parzival Energy Budget#Efficiency]].
3. Earth gravity (9.81 m/s²) is used for in-world work. The 15.00 m/s² in the Parzival definition is the reference standard only, and its joule value (1,500 J) is what converts.
4. Injury is converted through the falling-injury anchor. Weapon-like focused delivery couples far better and is handled by the delivery factor in [[Parzival Energy Budget]].
5. A spell's tier is kept equal to its source level so the registry stays one-to-one with the corpus. T_E records where its physics actually sits.

---

## Consequences for existing law

- **[[Universal Legum of Metaphysic-Thaumological Utilization|ULMTU-I]] (Lex Fontis):** the divine floor of 1 μPz/s is about 1.5 mW. A cantrip quantum spread over a full day still runs at 1.5 mPz/s, a thousand times above the floor, so every registered working is unambiguously divine.
- **[[Universal Legum of Metaphysic-Thaumological Utilization|ULMTU-XVI]] (Lex Interdictorum):** the 100 MegaParzival ceiling sits between Q13 (57 MPz) and Q14 (155 MPz). In tier terms the ceiling is T ≈ 13.56, so **any tier-14 working requires direct acknowledgement from the [[Répertoire du Savoir Athénien]]**. The law's wording "MegaParzival-Seconds" is read here as a total of 100 MPz (energy), since Pz is already an energy unit. If the author intends Pz·s literally, the ceiling becomes time-weighted and should be revisited.
- **[[Universal Legum of Metaphysic-Thaumological Utilization|ULMTU-III]] (Lex Limitationis):** the caster pays the quantum of the tier the working is cast at. A working whose physical output exceeds its quantum (Fireball, Heat Metal) runs on field gain from pattern alignment (ULMTU-IX) and falls back to the quantum when the pattern degrades; one whose output is below it bleeds the remainder as luminosity and heat. See [[Parzival Energy Budget#Field gain]].
- **Detection:** the Gaian-age [[Electronic Intelligence (ELINT)|ELINT]] threshold of 6 Pz/s in [[Ch20 - Rex Invictus XIII]] is far below any combat burst (a first-tier working cast in six seconds runs at 58 Pz/s), so stealth casting is a discipline of slow, low-rate workings. See [[Arcane Spectroscopy#Detection thresholds]] and [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]].

---

## Related

[[Parzival Thaumaturgy]] · [[Parzival]] · [[Thaumic Field Model]] · [[Parzival Energy Budget]] · [[Caster Capacity and Tiers]] · [[Arcane Spectroscopy]] · [[Hecate]] · [[Mana Crystal]] · [[Divine Power]]
