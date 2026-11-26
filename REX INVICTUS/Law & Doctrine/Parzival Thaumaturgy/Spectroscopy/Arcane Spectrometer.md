---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spectroscopy
  - rex-invictus/equipment
  - source/rex-invictus
aliases:
  - Arcane Spectrometers
  - Spectrometer (Arcane)
updated: 2026-11-16
---

**[[Arcane Spectrometer]]** is the instrument that splits a working's light into its lines and reads its attributes. It begins as the scholar's brass spyglass of [[Arcane Spectroscopy]] and ends, in the UOE, as an automatic sensor in every well-equipped unit's kit that drives the counter suites of [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]].

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Arcane Spectroscopy]]
    - **Arcane Spectrometer** (this note)

---

## How it works

1. **Collect.** An objective (lens or telescope) gathers the working's light.
2. **Disperse.** A diffraction crystal spreads the light by wavelength (m·λ = d·sin θ). A dense crystal shows one clean repeat.
3. **Locate.** The instrument measures each line's position on the 0 to 1 scale, its brightness and its Doppler shift.
4. **Decode.** Positions are matched against the [[Spectral Key Tables]]: the tier and school lines first, then damage, then area, range and duration.
5. **Estimate.** Brightness and distance give luminosity, and luminosity gives energy and so T_E ([[Parzival Energy Budget]]). Shift gives speed and heading.

A trained scholar does this by eye in one or two minutes. A military unit does it in a tenth of a second.

## Generations

| Generation | Form | Time to identify | Users |
|---|---|---|---|
| Scholar's spyglass | Brass tube with a violet crystal | 1 to 2 min | Universities, observatories |
| Stained spectacles and crystal monocle | Worn, with hinged filters | 10 to 30 s | Hunters of hostile casters, battle mages |
| Gaian-age detector | Electronic sensor tuned to field emission, often bolted to ELINT kit | 1 to 5 s, energy only, no attributes | Modern armies ([[Electronic Intelligence (ELINT)\|ELINT]] platforms) |
| UOE field spectrometer | Helmet or weapon-mounted crystal array with a glyph engine | 0.1 s to a three-line trigram, 0.5 s to a full match | Line troops of well-equipped units |
| UOE suite spectrometer | Multi-aperture array on vehicles, [[Ekdromoi]] kit and Titans | Continuous, many tracks | Armoured Titans, special forces, command posts |

## Standard field spectrometer

| Property | Value |
|---|---|
| Detection range | r = 1 km × √(E / 100 Pz); Fireball about 11 km, Magic Missile about 250 m |
| Line resolution | ±0.003 in x, enough to separate every source feature |
| Doppler resolution | 10 m/s |
| Trigram classification | k1 to k3 (tier, school, damage) in 0.1 s |
| Full match | all six lines in 0.5 s, then registry lookup |
| Power | under 0.01 Pz/s; it reads light and draws almost nothing |

The range rule follows the inverse-square fall of light. It is a registry convention; real ranges depend on weather, background light and the working's speed and emission damping.

## Limits

- **Identical spectra.** Workings with the same six attributes cannot be told apart by light alone ([[Arcane Spectroscopy#Identical spectra]]).
- **Emission damping.** [[Cloak (2-I-L-CLK)|Cloak]] and similar workings suppress εL; a damped working may be seen only at release.
- **Decoys.** Light without the k3 to k6 lines of a real working is a decoy ([[Ghost Battery (SIM-LT-CK-ML)|Ghost Battery]]).
- **Saturation.** A bright working near the sensor washes out dimmer lines; suites use filters like the source's stained spectacles to cut it.

## ULMTU links

| Lex | Application |
|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-I]] Lex Fontis | The instrument draws far under the divine floor and is not itself a working. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] Lex Interactionis | Identification is the first step of every counter. |

---

## Related

[[Arcane Spectroscopy]] · [[Spectral Key Tables]] · [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] · [[Electronic Warfare (EW)]] · [[Mana Crystal]]
