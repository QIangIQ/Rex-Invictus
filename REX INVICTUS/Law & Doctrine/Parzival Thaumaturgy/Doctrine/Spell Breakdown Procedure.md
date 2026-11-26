---
tags:
  - rex-invictus/magic-system
  - rex-invictus/doctrine
  - rex-invictus/spell-notation
  - source/rex-invictus
aliases:
  - Spell Breakdown
  - How to Profile a Working
  - Working Analysis Procedure
updated: 2026-11-16
---

**[[Spell Breakdown Procedure]]** is the standard method for taking any working, published or new, and producing its full registry profile: attributes, glyph, kata, incantation, spectrum, aspects, energy, identifier, ULMTU review and MINT/MCM profile. Every note in the [[Spell Registry]] was made this way, and a new working should be too.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - Doctrine
    - **Spell Breakdown Procedure** (this note)

---

## Step 1: Fix the six attributes

Write the working as Tier · School · Damage · Area · Range · Duration ([[Spell Attribute Set]]). Use the nearest value from the key tables. If no value fits, add one after its sorted neighbour and mark it as a Rex Invictus value.

- Tier: 0 to 14 ([[Caster Capacity and Tiers]]).
- School: one of the eight schools, or [[Pure]] for a bare force construct, or [[Composite]] for a combination.
- Damage: a source type, a derived type ([[Aspect Interpolation and Derived Damage Types]]) or None.

## Step 2: Write it

1. **Glyph.** Look up each attribute's key in [[Glyph Key Tables]], take its 13-bit pattern and draw layer k with chords k steps clockwise ([[Spell Writing (Glyph Notation)]]). If the six keys duplicate another working's, add the centre dots of its duplicate group.
2. **Kata.** Read the chords out as strokes from k1 outward ([[Somatic Notation (Gesture)]]).
3. **Incantation.** Join the sounds for tier, school and damage, then area, range and duration, from [[Incantation Sound Tables]] ([[Spell Speech (Incantation)]]). Duplicates take the registry homophone tail.
4. **Components.** Decide what the material focus anchors and whether it is costly ([[Spell Components]]).

## Step 3: Predict its light

Place each line at x = index / N on its attribute scale and give it brightness exp(−(x − T/10)² / 2) ([[Spectral Key Tables]], [[Arcane Spectroscopy]]). Blend for the swatch. Note the threat trigram (tier, school and damage lines). If a published plate exists, check every predicted line against it within ±0.008.

## Step 4: Place it in aspect space

Add the school vector and the damage vector to get the affinity vector ([[Aspect Theory of Magic]]). This vector sets its link costs in any combination.

## Step 5: Model the energy

Under [[Parzival Energy Budget]]:

1. List each physical term of the effect (damage by fluence, mass conjured, work done, heat, light, information) in Pz.
2. Add upkeep: power × maximum duration.
3. Apply the registry calibration rules C1 to C8 where they apply.
4. Add the pattern cost 0.01 × Q_T × (1 + h), where h is the sum of the handling points.
5. Total it, then compute T_E = 1 + ln(E / 350) and the field gain E / Q_T.

## Step 6: Grade and tag it

Score = clamp(0.5 × (T_E − T), −1, 3) + h. Grade L, M, H or X. Assign the shorthand and form the tag **Name (T-Affinity-Grade-Shorthand)**, the registry ID and the attribute code ([[Spell Registry Identifier Standard]]).

## Step 7: Review against the ULMTU

Check the working against the [[Universal Legum of Metaphysic-Thaumological Utilization]]. The usual questions:

| Lex | Question |
|---|---|
| I Fontis | Does it draw from the caster, a focus or a divine source? |
| III Limitationis | Is every term of its cost paid? |
| V Interactionis | Can it be countered, and by whom? |
| VIII Nexus | Does it open a link that can be traced or cut? |
| XI Consequentiae | What happens on misfire? |
| XVI Interdictorum | Does it exceed 100 MPz (T_E above about 13.6)? If so it needs the Répertoire. |

## Step 8: Write its MINT and MCM profile

Give the detection range r = 1 km × √(E / 100 Pz), the threat trigram, and the three counter costs (pre-loaded 0.05 × Q_T, cold 0.10 × Q_T, unravel cold plus 20% of remaining upkeep) ([[Magical Countermeasures and Magical Intelligence (MCM-MINT)]]).

## Step 9: File it

Place the note in its tier and school folder, and link it from its tier page, school page and families ([[Spell Families]]). Combinations go in the Combinations folder and are costed under [[Recast Tension and Combination Affinity]].

## Worked example: Fireball

| Step | Result |
|---|---|
| Attributes | 3 · Evocation · Fire · sphere (20) · 150 feet · Instantaneous |
| Glyph keys | 3, 4, 3, 30, 4, 9 |
| Incantation | *Luire-Sonosin* |
| Spectrum | lines at 0.300, 0.500, 0.286, 0.833, 0.235, 0.000; trigram 3·V·Fire; matches the published plate |
| Aspects | Evocation (1b 2f 1j) + Fire (1b 1c 1f 1j) |
| Energy | burst 28 × 0.70 × 467 m² / 0.7 m² = 13,076 Pz; pattern 25.9 Pz; total 13,101 Pz |
| Tier and grade | T_E 4.62, field gain 5.07, score 0.81, grade M |
| Tag | [[Fireball (3-V-M-FRB)]] |
| ULMTU | V (counterable); XI (fire spreads past the burst) |
| MCM | seen at about 11 km; pre-loaded counter 129 Pz, cold counter 259 Pz |

---

## Related

[[Spell Registry]] · [[Spell Attribute Set]] · [[Parzival Energy Budget]] · [[Spell Registry Identifier Standard]] · [[Spell Families]] · [[Combat Combination Analysis]]
