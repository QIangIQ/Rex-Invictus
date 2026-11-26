---
tags:
  - rex-invictus/magic-system
  - rex-invictus/parzival
  - source/rex-invictus
aliases:
  - Spell Energy Budget
  - Energy Model (Parzival)
updated: 2026-11-16
---

**[[Parzival Energy Budget]]** is the costing method used for every working in the [[Spell Registry]]. It turns what a working physically does into a draw in [[Parzival]] (Pz), using the constants of [[Mana-Parzival Conversion]], so that any working, standard or newly written, can be priced the same way.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - Foundations
    - [[Mana-Parzival Conversion]]
    - [[Thaumic Field Model]]
    - **Parzival Energy Budget** (this note)
    - [[Caster Capacity and Tiers]]

---

## The budget equation

**E_total = (E_effect + E_upkeep) / η + E_pattern**

| Term | Meaning |
|---|---|
| E_effect | Energy of what the working does once: injury, lift, heat, conjured mass, translocation |
| E_upkeep | Continuous power × maximum duration (concentration maximum counts) |
| η | Channel efficiency; 1 in the registry, lower in the field (see [[#Efficiency]]) |
| E_pattern | Cost of holding the working's pattern: **0.01 × Q_T × (1 + h)**, where h is the handling points |

The registry reports E_total at η = 1, the slot quantum Q_T, the field gain E_total / Q_T, and the energy-equivalent tier **T_E = 1 + ln(E_total / 350)**.

## Injury coefficients

Injury is priced through the fall anchor: 3.5 points from a 10 ft fall of an 80 kg body, 2,392 J, so **0.456 Pz per point** of blunt, whole-body injury. Other kinds are scaled by how much field energy each needs to do the same harm.

| Kind | κ (Pz per point) | Kind | κ (Pz per point) |
|---|---|---|---|
| Bludgeoning | 0.46 | Thunder | 0.60 |
| Slashing | 0.40 | Acid | 0.25 |
| Piercing | 0.35 | Poison | 0.05 |
| Force | 0.40 | Necrotic | 0.20 |
| Fire | 0.70 | Radiant | 0.50 |
| Cold | 0.90 | Psychic | 0.02 |
| Lightning | 0.30 | Radiation (RI) | 0.45 |

**Delivery factor F:** diffuse or whole-body 1.0; directed ray, bolt or touch on one target 0.5; weapon-like focused point (blade, arrow, single strike) 0.08. Average dice at the base tier and full (failed-resistance) injury are used.

- Single target: **E = injury × κ × F × number of strikes**
- Damage over time: × expected triggers (3 rounds unless the duration is shorter)
- Healing: **0.30 Pz** per point restored; temporary injury buffer: **0.20 Pz** per point

## Area geometry

Area workings use a point-source fluence model: the working must fill the exposure surface S at the edge of its area with the injury fluence that a Medium body (cross-section A_c = 0.7 m²) would take.

**E = injury × κ × S / A_c**

| Shape | Exposure surface S |
|---|---|
| Sphere radius r (and emanations) | 4πr² |
| Cone length l | 0.666·l² (solid angle 0.666 sr) |
| Cube side s | 4π(0.62s)² |
| Cylinder r, h | 2πrh + πr² |
| Line l × w | 2lw |

Because S grows with the square of size, large-area evocations run far over their tier curve. Fireball computes to about 13,100 Pz against a Tier 3 quantum of 2,586 Pz.

## Mechanical and physical terms

| Effect | Formula |
|---|---|
| Lift or move mass | m·g·h, ½mv², or force × distance (Earth g = 9.81 m/s²) |
| Hover or levitation upkeep | 0.02 × m·g per second |
| Translocation | 0.01 × m × 15 × d / 1500 Pz; plane boundary d_eff = 10⁶ m |
| Conjured matter | 1 Pz/kg fluids and gases, 3 Pz/kg structured solids, 10 Pz/kg living matter |
| Conjured creature | 10 Pz/kg body mass + 0.05 Pz/s autonomy upkeep |
| Heating or cooling | m·c·ΔT (water 4,186, air 1,005, stone 800, metal 450 J/kg·K) |
| Light | luminous power × time (a 20 ft torch-equivalent is about 100 W of field light) |
| Wards and buffs | 0.20 Pz × expected injury absorbed over the duration |
| Enchantment | 0.005 Pz/s per affected creature |
| Illusion | 0.002 Pz/s per 1,000 m³ of illusion volume |
| Divination | 0.001 Pz/s × (range in m / 10), capped by rule C2; one instant answer = 1 Pz |
| Soul work | 10⁴ Pz per tier above 3 (re-anchoring constant) plus healing terms |

The translocation rule reflects the Parzival's directional neutrality under [[Hecate]]: moving a body through a fold costs 1% of lifting it the same distance against the Parzival standard.

## Registry calibration rules

A few source workings produce nonsense under the raw rules. These eight rules fix them and are cited on each affected note.

| Rule | Name | Statement |
|---|---|---|
| C1 | Coterminous crossing | Crossing into a plane that lies on top of the material world (the ethereal border) uses d_eff = 10³ m. |
| C2 | Sympathetic link saturation | Under [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] a sensory link costs by distance only to 1 km; beyond that it rides on sympathy at 0.1 Pz/s. |
| C3 | Borrowed sustenance | Conjured food reverts within a day ([[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XIII]]), so its calories are charged at 1%. |
| C4 | Dormant patterns | A pattern that only waits for a trigger runs at 1% of its active rate. |
| C5 | Phasing | Matter shifted out of phase is displaced, not conjured: 10% of the structured-solid rate. |
| C6 | Illusion skin | Large terrain illusions are priced as a 0.1 m skin over the surface. |
| C7 | Domestic transmutation | Small sensory or thermal tricks act on about 1 kg. |
| C8 | Sub-injury dose | Area effects under 2 points of injury are priced as a dose on the creatures present. |

## Field gain

When E_total exceeds Q_T the working runs on field gain: its pattern sits in a deeper local minimum than its tier nominally allows, and the field returns more than the quantum ([[Thaumic Field Model]]). Gain is legal under ULMTU-IX while the pattern is held cleanly. Fatigue, jamming or a damaged glyph collapses the gain and the working fires at the quantum, which for Fireball means a burst about a fifth of its rated strength. When E_total is below Q_T the remainder bleeds off as light and heat.

## Efficiency

Real castings run at η < 1. The losses come from the [[Parzival]] definition and its theoretical notes.

| Loss | Typical η factor | Source |
|---|---|---|
| Channeling inefficiency (training, fatigue) | 0.6 to 0.95 | caster |
| Environmental interference | 0.5 to 1.0 | [[Electronic Warfare (EW)]], hostile counters, dead [[Ley lines]] |
| Divine domain mismatch | 0.3 to 1.0 | [[Divine Single Event Effects (DSEE)]], opposed [[Divine Affinity]] |
| Age and affinity offset | 0.8 to 1.3 | the definition assumes a 100-year-old being of neutral affinity |

Field practice multiplies them. A tired demigod at η = 0.5 pays double for everything.

## Handling points

Handling points raise the pattern cost and feed the grade in the [[Spell Registry Identifier Standard]].

| Flag | Points |
|---|---|
| Fragile (ends on injury or interception) | 1.0 |
| Independent multi-target control | 0.5 |
| Concentration, ritual, reaction cast, costly material, consumed material, incapacitating with no injury, casting time of a minute or more | 0.25 each |

## Worked example: Fireball

| Step | Value |
|---|---|
| Injury | 8 dice of 6, mean 28 |
| Surface | 4π(6.1 m)² = 467 m² |
| Effect | 28 × 0.70 × 467 / 0.7 = 13,076 Pz |
| Pattern | 0.01 × 2,586 = 25.9 Pz |
| Total | 13,101 Pz (19.7 MJ, about 4.7 kg of TNT) |
| T_E | 4.62, gain 5.07 |

---

## Related

[[Parzival Thaumaturgy]] · [[Mana-Parzival Conversion]] · [[Spell Breakdown Procedure]] · [[Recast Tension and Combination Affinity]] · [[Spell Registry]] · [[Parzival]]
