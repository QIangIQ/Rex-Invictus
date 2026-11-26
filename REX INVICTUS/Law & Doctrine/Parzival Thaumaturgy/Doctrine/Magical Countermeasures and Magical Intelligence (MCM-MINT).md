---
tags:
  - rex-invictus/magic-system
  - rex-invictus/doctrine
  - rex-invictus/electronic-warfare
  - source/rex-invictus
aliases:
  - MCM
  - MINT
  - Magical Countermeasures
  - Magical Intelligence
  - Auto-Counterspell Suite
  - MCCM
  - MCCCM
  - Magical Counter-Countermeasures
updated: 2026-11-16
---

**[[Magical Countermeasures and Magical Intelligence (MCM-MINT)]]** is the doctrine of finding, reading and defeating hostile workings in real time. MINT (magical intelligence) is the collection and analysis side: spectrometers and sensors classify every working in view. MCM (magical countermeasures) is the action side: counter-suites that unmake those workings before they close, and the counter-counter layers that each side stacks on top. It stands to [[Parzival Thaumaturgy]] as [[Electronic Warfare (EW)]] stands to radio. In the UOE every well-equipped element carries it: line troops, [[Ekdromoi]] and other special forces, and the Armoured Titans.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - Doctrine
    - [[Recast Tension and Combination Affinity]]
    - [[Combat Combination Analysis]]
    - **Magical Countermeasures and Magical Intelligence (MCM-MINT)** (this note)
    - [[Practical Magical Combat]]

---

## Physical basis

Two facts make MCM possible.

1. **Workings announce themselves while forming.** A kata is traced from k1 outward ([[Somatic Notation (Gesture)]]), and each finished layer already glows on its line ([[Arcane Spectroscopy]]). The tier, school and damage lines (the **threat trigram**) are visible about one second into a four- to five-second cast.
2. **Patterns cancel in anti-phase.** A working sits on a field minimum defined by its six attributes. An anti-phase copy of the same pattern, cast into the same cell before the working closes, interferes destructively and both collapse ([[Thaumic Field Model#Interaction with the material world]]). This is the mechanism behind Counterspell and Dispel Magic, under [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]].

A counter does not have to match the working's energy, only its pattern. That is why it is cheap.

| Counter | Cost | Time |
|---|---|---|
| Pre-loaded trigram, last three layers drawn on demand | 0.05 × Q_T of the target | 0.3 to 0.6 s |
| Cold counter, all six layers drawn | 0.10 × Q_T | 1.5 to 3 s |
| Unravel after the working closes | cold counter + 20% of its remaining upkeep | 2 to 4 s |

Every registry note lists these three numbers in its MINT and MCM profile.

## MINT: magical intelligence

| Stage | Means | Product |
|---|---|---|
| Collection | [[Arcane Spectrometer\|Arcane spectrometers]], Mana Sensing, [[Electronic Intelligence (ELINT)\|ELINT]] receivers, trained observers reading kata | Lines, brightness, Doppler shift, bearing |
| Processing | Trigram match, then full six-line match against the [[Spell Registry]] | Working identity, tier, energy, speed, heading |
| Fusion | Bearings from several apertures; cumulative draw per caster | Caster position, caster tier, remaining reservoir estimate ([[Caster Capacity and Tiers]]) |
| Dissemination | Fire-control net, marker flares | Targets for guns and casters ([[Skymark Flare (MM-LK-AL-LT-SK)\|Skymark Flare]]) |

MINT also watches the slow signals: long-range links (a scrying or sending thread is a steady low-rate emitter), dormant patterns (wards and glyphs leak at 1% of their active rate) and ritual build-ups. A [[Periscope Eye (AE-LK-CK-SK)|Periscope Eye]]'s link thread is a classic MINT target.

## MCM: the counter ladder

Each side can add a layer on top of the other's. The layers are named by how many "counters" deep they sit: MCM (C1), MCCM (C2, magical counter-countermeasures), MCCCM (C3) and so on. The MINT structures that feed them are built the same way, and most workings and combinations need hours of analysis to settle where they sit on the ladder.

### Counter (C1, MCM)

The defender's suite reads the hostile trigram and fires an anti-phase pattern. Without a match it can fall back on an opposed working (fire against ice), which must match the hostile energy and so costs far more. To be fast, the suite keeps a **rotating ring of pre-drawn trigrams**: partial glyphs for the most likely threats, held dormant and cycled through ready positions like the chambers of a revolver. When a trigram matches, the suite only has to draw k4 to k6 and release. A ready trigram costs dormant upkeep at 1% of its active rate (rule C4 of [[Parzival Energy Budget#Registry calibration rules]]).

### Counter-counter (C2, MCCM)

The attacker protects the working against C1.

| Measure | How it works | Cost to attacker |
|---|---|---|
| Layer scramble | Draw k4 to k6 first and the trigram last, so the suite cannot classify early | +0.5 handling points; higher misfire risk |
| False trigram | A zero-energy ghost layer that matches a different working | 0.01 × Q_T |
| Emission damping | [[Cloak (2-I-L-CLK)\|Cloak]] the forming pattern | Cloak's draw plus a pattern link |
| Compressed kata | The attacker's own pre-drawn trigram, so the working closes in under a second | dormant upkeep |
| Pattern shield | A reaction ward on the working itself that absorbs the first counter | a [[Shield (1-P-L-SHL)\|Shield]] or [[Bulwark (3-A-L-BLW)\|Bulwark]] |
| Decoys | Glowing figures that bait the ring ([[Ghost Battery (SIM-LT-CK-ML)\|Ghost Battery]]) | about 200 Pz |
| Masked working behind a decoy | Illusion and Cloak hide the real circle while a decoy Fireball forms in view; a counter spent on the decoy is wasted | the decoy's draw plus Cloak; the defender needs an extra dispel to catch the real one |

Rotating the glyph frame gains nothing: the codes are rotation-invariant by design ([[Spell Writing (Glyph Notation)#Principle]]).

### Counter-counter-counter (C3, MCCCM)

The defender answers C2.

| Measure | Defeats | Price |
|---|---|---|
| Full-match gating (wait for all six lines) | False trigrams and decoys | Adds 0.4 s; fast workings may close first |
| Consistency check (brightness, Doppler and range must agree with the claimed working) | Ghost layers and light-only decoys | Processing only |
| Multi-aperture triangulation | Emission damping (a damped working still shows at release from a second angle) | More sensors |
| Saturation counter (counter every candidate trigram at once) | Layer scramble | Ring size × pre-loaded counter cost |
| Counter-shield breaker (a short dispel ahead of the counter) | Pattern shields | One extra counter |
| Binder hunting | Combinations: counter the binder and every bound member falls apart | One counter on the binder's tier |

### C4 and beyond

Past three layers the contest becomes a race of volume and reservoir. The attacker's best tool is saturation: more simultaneous workings than the defender's ring has ready chambers. The defender's best tool is depth: a bigger ring and a faster refill. Exchange ratios decide who wins.

| Exchange | Attacker spends | Defender spends |
|---|---|---|
| Fireball versus a pre-loaded counter | 13,101 Pz | 129 Pz |
| Fireball cast cold versus a ring that lacks its trigram | 13,101 Pz | 259 Pz, if the counter closes in time |
| Railcannon bolt (kinetic) versus any counter | 730 Pz | a counter only stops it before release; afterwards it is physical |
| Six-flare battery shoot | 233 Pz | 6 counters at 47 Pz |
| Anti-Mage Primer, binder countered in flight | 1,838 Pz lost | 48 Pz |

Two lessons follow. Counters are cheap against evocations, so defenders with good MCM make massed evocation a poor trade. Kinetic workings such as the [[Magical Railcannon (SM-S-G-A-C)|Magical Railcannon]] are counterable only before release, which makes them the attacker's answer to strong MCM.

## Equipment by echelon (UOE)

| Element | MINT | MCM ring | Notes |
|---|---|---|---|
| Line infantry of well-equipped units | Helmet spectrometer, squad net | 6 trigrams per squad | Covers the common Tier 0 to 3 threats |
| Special forces ([[Ekdromoi]] and similar) | Personal spectrometer, crystal monocle with filter sets | 12 trigrams per operator | Adds emission damping on their own workings |
| Command posts | Multi-aperture arrays | 24 to 48 trigrams | Feeds fire control and counter-battery |
| Armoured Titans | Multi-aperture suite, continuous tracking | 64 trigrams or more, refilled by a dedicated glyph engine | One of the twenty-plus layered protections alongside divine runic, sigil and cantic wards |

Gaian-age forces have ELINT that can sense field draw (the 6 Pz/s threshold in [[Ch20 - Rex Invictus XIII]]) but cannot read attributes. They detect magic; they cannot counter it. That gap is one of the UOE's largest advantages.

## Doctrine notes

- **Cast slow or cast fast.** Below ELINT and spectrometer thresholds, slow low-tier casting goes unseen. Above them, only speed (compressed kata) or volume beats a ring.
- **Hit the ring, then the target.** Decoys and cheap cantrips drain ready chambers before the real working goes.
- **Prefer kinetic and physical effects against strong MCM.** Once an effect is matter or momentum, a counter no longer helps.
- **Bind late.** In combinations the binder is the single point of failure; cast it last and release in the same second.
- **Read before you counter.** The hardest part is identifying the working before the projectile leaves; a counter fired at a decoy feeds the enemy's plan ([[Practical Magical Combat#The counterplay chain]]).
- **Protect the observers.** A suite without MINT is blind; spectrometers are priority targets.

## ULMTU links

| Lex | Application |
|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] Lex Interactionis | All counters rest on the requirement that magic can be opposed; a large gap in [[Divine Power]] removes the option. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-VIII]] Lex Nexus | Link threads are detectable and can be cut. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XI]] Lex Consequentiae | Layer scrambles and compressed kata raise misfire risk. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XII]] Lex Reversibilitatis | Unravelling a completed working needs far greater knowledge or power than the caster's; this is why low-tier workings such as Magic Missile weaken in high-tier combat. |

---

## Related

[[Practical Magical Combat]] · [[Arcane Spectrometer]] · [[Arcane Spectroscopy]] · [[Negation and Counterspell]] · [[Combat Combination Analysis]] · [[Electronic Warfare (EW)]] · [[Divine Single Event Effects (DSEE)]]
