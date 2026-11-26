---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spectroscopy
  - source/rex-invictus
aliases:
  - Spell Spectroscopy
  - Arcane Spectra
updated: 2026-11-16
---

**[[Arcane Spectroscopy]]** is the study of the light that workings emit. Every working sheds part of its energy as light, and the colours of that light encode its six attributes. The method comes from *Arcane Spectroscopy* (The Gorilla of Destiny, v3), whose published plates the registry has decoded, and it is the scientific basis of magical intelligence in [[Parzival Thaumaturgy]].

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - Spectroscopy
    - **Arcane Spectroscopy** (this note)
      - [[Spectral Key Tables]]
      - [[Arcane Spectrometer]]

---

## Physical basis

The source builds on real optics.

- **Emission spectra.** Excited electrons fall back to lower states and emit light at fixed wavelengths, so a gas shows a set of bright lines unique to it. Workings do the same: each attribute is a "state" of the field packet and emits its own line.
- **Diffraction.** Light passing a grating or a crystal lattice spreads by wavelength at angles given by **m·λ = d·sin θ**. Crystals repeat the pattern at each order m; a dense enough crystal shows exactly one repeat, which is what makes a crystal monocle possible.
- **Interference.** In-phase waves add and anti-phase waves cancel. The same rule governs combinations and counters ([[Thaumic Field Model#Interaction with the material world]]).
- **Stellar spectroscopy and redshift.** Stars are identified by their lines; motion shifts all lines by **z = Δλ/λ = v/c**. A working moving toward the observer is blueshifted, one moving away is redshifted. The source's Figure 2.4 shows a fireball shading from blue at the caster's hand, through its normal hue, to red as it recedes.

## Lines of a working

A working emits up to six lines, one per attribute. Their positions on a 0 to 1 scale were recovered from the 297 profile plates in the source:

**x = index / N** over the source list of that attribute, with the null value (no damage, no area, Instantaneous) first and the rest in ASCII order. Tier lines sit at **x = T/10**, school lines at **x = i/8**.

| Attribute | N | Null line |
|---|---|---|
| Tier | 10 | none (Tier 0 sits at x = 0) |
| School | 8 | none |
| Damage | 14 | absent when no damage |
| Area | 36 | absent when no area |
| Range | 17 | none |
| Duration | 19 | Instantaneous at x = 0 |

Applied to all 297 plates the rule predicts 1,322 of 1,326 lines within ±0.008 and accounts for every measured line. Full tables are in [[Spectral Key Tables]].

**Colour.** x maps through the gist_rainbow scale used by the source: x = 0 deep red, 0.25 orange-yellow, 0.5 mint green, 0.7 cyan, 0.88 blue-violet, 1.0 violet. The registry gives an equivalent wavelength of 700 − 300x nm.

**Brightness.** Each line's brightness falls off with its distance from the tier line: **h = h0 · exp(−(x − T/10)² / 2σ²)** with σ = 1. Lines near the tier line are brightest.

**Swatch.** The colour of the working's glow is the brightness-weighted blend of its lines. The source prints it above each plate.

## Luminosity

From the [[Thaumic Field Model]], **L = εL · v · E_P0 / R**. Brightness rises with initial energy and speed and falls with range. The source's Figure 3.1 plots log L against level: the spread climbs from about 10² to 3×10³ at level 1 to about 10⁴ to 3×10⁵ at level 9. Two consequences matter in the field:

- An accelerated working is much brighter than a thrown one. A railcannon bolt at 2,500 m/s would glow like a tracer if [[Cloak (2-I-L-CLK)|Cloak]] did not damp its εL ([[Magical Railcannon (SM-S-G-A-C)|Magical Railcannon]]).
- Long-range workings are dim for their energy, which is why scrying and sending are hard to spot.

## Identical spectra

Workings with the same six attributes have the same spectrum. The plates confirm seven such groups among the standard workings, for example Bane, Bless and Hideous Laughter, and Commune and Contact Other Plane. They are the same groups as the duplicate glyphs and homophones ([[Spell Writing (Glyph Notation)#Duplicate glyphs]]). A spectrometer cannot tell them apart without context.

## Coverage of the source plates

The plates run alphabetically from Acid Arrow to Tree Stride (297 workings). The last 22 standard workings, including Wall of Force and Wish, have no published plate; the registry computes theirs from the rule.

## Detection thresholds

| Observer | Threshold | Source |
|---|---|---|
| Unaided divine sense | a working of Tier 3 or more within a few hundred metres | Rex Invictus convention |
| Gaian-age [[Electronic Intelligence (ELINT)\|ELINT]] | sustained draw above 6 Pz/s | [[Ch20 - Rex Invictus XIII]] |
| Standard field spectrometer | r = 1 km × √(E / 100 Pz) | registry convention ([[Arcane Spectrometer]]) |
| Large arcane telescope | world-scale rituals at planetary distance | source section 5 |

A first-tier working cast in six seconds runs at about 58 Pz/s, ten times the ELINT threshold. Stealth casting therefore means slow casting, low tiers and emission damping.

## Applications

The source names three; Rex Invictus adds a fourth.

1. **Ritual monitoring.** Large rituals emit strongly, so observatories watch for world-scale curses.
2. **Battlefield aptitude.** Reading what a hostile caster is preparing, and how strong it is, from its glow.
3. **Arcane astronomy.** Pointing telescopes at stars and planets to learn whether they are magical, and to search for civilisations that use the field.
4. **Magical intelligence and countermeasures.** Automated spectrometers that classify and counter hostile workings in real time. See [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]].

## Instruments

| Instrument | Source description | Use |
|---|---|---|
| Diffraction grating or crystal | Spreads the light into its lines | Basic analysis; a skilled reader identifies a working in one or two minutes |
| Handheld spectrometer | Brass spyglass with a violet diffraction crystal in the objective | Field identification |
| Stained spectacles | Goggles with hinged red, green and blue filter discs | Isolating part of the spectrum |
| Crystal monocle | One-repeat dense crystal plus hinged filters; "the most advanced magic detection equipment" | Quick detection of distant workings |
| Large arcane telescope | Refractor on a pillar mount with a violet crystal assembly at the eyepiece | Astronomy and ritual watch |

Rex Invictus military versions are described in [[Arcane Spectrometer]].

## ULMTU links

| Lex | Application |
|---|---|
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-V]] Lex Interactionis | Spectral identification is the first step of every counter. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-IX]] Lex Correspondentiae | A working's lines are its pattern made visible. |
| [[Universal Legum of Metaphysic-Thaumological Utilization\|ULMTU-XVI]] Lex Interdictorum | Observatories watch for workings above 100 MPz. |

---

## Related

[[Spectral Key Tables]] · [[Arcane Spectrometer]] · [[Thaumic Field Model]] · [[Magical Countermeasures and Magical Intelligence (MCM-MINT)]] · [[Electronic Warfare (EW)]] · [[Scrying]]
