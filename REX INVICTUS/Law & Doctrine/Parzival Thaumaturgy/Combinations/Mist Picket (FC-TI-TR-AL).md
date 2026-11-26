---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-combination
  - source/rex-invictus
aliases:
  - "Mist Picket"
  - "Anti-Missile Mist Array"
registry_id: "X-6-FC-TI-TR-AL"
pz_total: 5800
updated: 2026-11-16
---

**Mist Picket** (`FC-TI-TR-AL`) is a defensive combination against conventional guided missiles and artillery. A three-dimensional array of mist, bound with tripwires and an alarm, detects any object large enough to disturb it and releases a pre-drawn personal defence stack. The concept is the author's (16 November 2026); the costing follows [[Recast Tension and Combination Affinity]] with estimates where a member has no registry entry. The worked threat is an air-launched anti-tank missile of the Hellfire class.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Combat Combination Analysis]]
    - **Mist Picket** (this note)

---

## The concept

1. Lay a 3D array of [[Fog Cloud (1-C-L-FC)|mist]] around the position, with [[Tripwire (0-A-L-TRP)|Tripwire]] and a wide-area [[Alarm (1-A-L-ALR)|Alarm]] bound into it by [[Transfiguration Inheritance (2-T-L-TI)|Transfiguration Inheritance]].
2. Anything of sufficient size that passes through the mist trips the array and sounds the alarm.
3. The alarm releases a [[Haste (3-T-L-HST)|Haste]] bound to the mage's own eyes, so they perceive the incoming round at inhuman speed.
4. The mage then:
   - thickens the air (Solidify);
   - raises earth for cover;
   - stacks [[Arcane Ward (1-A-L-AW)|Arcane Ward]], [[Shield (1-P-L-SHL)|Shield]] and [[Mage Armor (1-P-L-MA)|Mage Armor]] against fragments;
   - transfigures into stone ([[Flesh to Stone (6-T-L-FSE)|Flesh to Stone]], cast on themself);
   - fires a [[Blast (1-V-L-BLS)|Blast]] to disperse the missile.

All of this assumes the munition is purely conventional. A round blessed or guided with Dionysian, Hephaestian, Apollonian, Artemisian, Poseidonian, Shinto or other divine support is a counter-countermeasure, and the picket must be rebuilt against it (see below).

## The threat

| Property | Hellfire-class missile |
|---|---|
| Mass | about 49 kg |
| Speed | about 425 m/s (Mach 1.3) |
| Kinetic energy | about 4.4 MJ, **2,950 Pz** |
| Warhead | about 9 kg tandem shaped charge, roughly 9 kg TNT equivalent: about 38 MJ, **25,100 Pz** |
| Guidance | semi-active laser (needs a designator's spot) or millimetre-wave radar |

## The timing problem

| Picket radius | Warning time at 425 m/s |
|---|---|
| 150 m | 0.35 s |
| 100 m | 0.24 s |
| 50 m | 0.12 s |

A cold working takes seconds to draw, and even a pre-loaded trigram needs 0.3 to 0.6 s to finish ([[Magical Countermeasures and Magical Intelligence (MCM-MINT)#Physical basis]]). The mage cannot cast the stack after the alarm sounds. Every member must already be fully drawn and held dormant in the binder, then released together by the tripwire in a few hundredths of a second. Haste on the eyes does not buy casting time. It buys perception, so the mage can aim the Blast and judge whether to drop into stone.

## Why standoff matters most

- **Wards do not stop the jet.** A shaped-charge jet's fluence is far above the areal strength of Arcane Ward, Mage Armor, Shield and Bulwark. This is the same Munroe effect the [[Anti-Mage Primer (SP-TI-MM-DM-SH-AC-BL-AL)|Anti-Mage Primer]] uses to breach ward stacks. A direct hit goes through the personal stack.
- **Distance kills the jet.** A shaped charge set off far from its target loses its jet within a few metres. The decisive move is to make the warhead go off early, well out from the mage.
- **Blast at distance is survivable.** For about 9 kg TNT equivalent, scaled distance at 20 m is about 9.6 m/kg^⅓ (light overpressure), and at 5 m it is about 2.4 (severe). At 20 m the stone form, thickened air and wards handle the fragments.

A lateral shove of 10 m in the last 0.12 s needs about 167 m/s of sideways velocity on 49 kg, about 450 Pz. A [[Blast (1-V-L-BLS)|Blast]] (about 900 Pz) that overpressures the fuze or the seeker at standoff does the job more reliably.

## Bonus against guidance

Thick mist scatters a laser designator's spot, so a semi-active laser round may lose its target before it reaches the picket. Millimetre-wave radar sees through fog, so radar-guided rounds are unaffected.

## Cost breakdown

Members held dormant in one binder. Solidify and Summon Earth have no registry entry; their figures are estimates (Solidify: 136 kg of air in a 3 m sphere at 3 Pz/kg; Summon Earth: about 1.5 t of local soil reshaped at 0.3 Pz/kg and raised 1 m).

| Member | Role | Pz |
|---|---|---|
| Fog Cloud array, threat sector only (about 1/8 of a 150 m hemisphere, 17 Tier-3 clouds, 1 hour) | sensing medium and laser screen | about 2,500 |
| Tripwire and Alarm, inherited into the mist | trigger | about 40 |
| Transfiguration Inheritance and links | binds everything to one release | about 350 |
| Haste (eyes) | perception | 51 |
| Solidify (estimate) | fragment drag | about 410 |
| Summon Earth (estimate) | cover | about 460 |
| Arcane Ward, Shield, Mage Armor | fragment layers | 32 |
| Flesh to Stone, self | last-ditch hardening | 1,020 |
| Blast | early detonation of the round | 904 |
| **Total** | | **about 5,800 to 6,000** |

A full 150 m hemisphere of mist instead of one sector raises the array to about 20,000 Pz. Prepared over several minutes, recast tension is negligible; the binder's dormant hold costs 1% of active rates.

| Comparison | Pz |
|---|---|
| Sector picket and stack | about 6,000 |
| The missile's warhead | about 25,100 |
| Tier 3 reservoir | 9,427 |
| Tier 5 reservoir | 52,212 |

A Tier 3 mage can stand one sector picket and survive one missile. A second missile inside the hour finds the stack spent. Saturation beats the picket the same way it beats a counter ring.

## A cheaper variant: mined mist

Bind the Blast into the mist itself, so the cloud the round passes through detonates on the tripwire, 150 m out. The engagement no longer depends on the mage's reaction or aim, and the personal stack becomes a backup. The cost moves from one Blast to one Blast per tripped cloud, held dormant at 1%.

## Counter-countermeasures

| Divine support on the munition | Effect on the picket |
|---|---|
| Hephaestian forging | Casing and fuze resist Blast and dispel; standoff detonation fails |
| Apollonian guidance | Sight-based seeking ignores the mist; the laser-screen bonus is lost |
| Artemisian blessing | The round hunts its mark; lateral pushes are corrected |
| Dionysian, Poseidonian, Shinto and other patrons | Domain-specific effects, judged case by case under ULMTU-V |

Against such rounds the mage needs a counter on the blessing itself (MCCM) before the conventional defences work. See [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]].

## ULMTU notes

| Lex | Application |
|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IV]] | The dormant stack must be supported for as long as it waits. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] | Divine blessing on a munition can place it beyond the picket's counters. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] | Mist, tripwire, alarm and stack share one Nexus through the binder. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] | Releasing a large dormant stack in one instant carries backlash risk. |

## Related

[[Combat Combination Analysis]] · [[Practical Magical Combat]] · [[Slipglue Field (SL-TI-GR-GL-GY)]] · [[Haze Screen (ML)]] · [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]]
