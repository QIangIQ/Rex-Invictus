---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spectroscopy
aliases:
  - "Spectral Keys"
updated: 2026-11-16
---


**[[Spectral Key Tables]]** give the line position x (0 to 1), colour and equivalent wavelength of every attribute value under [[Arcane Spectroscopy]]. The rule was recovered by matching all 297 published profile plates: x = index / N over the source list, with the null value (no damage, no area, Instantaneous) first and the rest in ASCII order. Tier lines sit at x = T/10 and school lines at x = i/8. Applied to the 297 plates the rule predicts 1,322 of 1,326 lines within ±0.008, and every measured line is accounted for. Damage and area lines are absent when the value is null. Rex Invictus values that the source lists lack are placed half a step after their sorted neighbour, so source positions never move.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Arcane Spectroscopy]]
    - **Spectral Key Tables** (this note)

---

## Tier

| Tier | x | Colour |
|---|---|---|
| 0 | 0.000 | `#ff0028` |
| 1 | 0.100 | `#ff5d00` |
| 2 | 0.200 | `#ffea00` |
| 3 | 0.300 | `#8cff00` |
| 4 | 0.400 | `#00ff00` |
| 5 | 0.500 | `#00ff8b` |
| 6 | 0.600 | `#00ebff` |
| 7 | 0.700 | `#005eff` |
| 8 | 0.800 | `#2900ff` |
| 9 | 0.900 | `#b600ff` |
| 10 | 1.000 | `#ff00bf` |
| 11 | 1.000 | `#ff00bf` |
| 12 | 1.000 | `#ff00bf` |
| 13 | 1.000 | `#ff00bf` |
| 14 | 1.000 | `#ff00bf` |

Tiers above 10 share the x = 1.0 line and are told apart by luminosity.

## School

| School | x | Colour |
|---|---|---|
| Abjuration | 0.0000 | `#ff0028` |
| Conjuration | 0.1250 | `#ff8300` |
| Divination | 0.2500 | `#cdff00` |
| Enchantment | 0.3750 | `#20ff00` |
| Evocation | 0.5000 | `#00ff8b` |
| Illusion | 0.6250 | `#00c5ff` |
| Necromancy | 0.7500 | `#0017ff` |
| Transmutation | 0.8750 | `#9600ff` |
| Pure | 0.9375 | `#ed00ff` |
| Composite | 0.0625 | `#ff2d00` |

## Damage

| Feature | x | Colour | λ eq. (nm) | Basis |
|---|---|---|---|---|
| None | 0.000 | `#ff0028` | 700 | source |
| Acid | 0.071 | `#ff3700` | 679 | source |
| Alkaline | 0.107 | `#ff6800` | 668 | Rex Invictus |
| Bludgeoning | 0.143 | `#ff9900` | 657 | source |
| Cold | 0.214 | `#fffa00` | 636 | source |
| Corrosive | 0.250 | `#cdff00` | 625 | Rex Invictus |
| Divine | 0.250 | `#cdff00` | 625 | Rex Invictus |
| Fire | 0.286 | `#9cff00` | 614 | source |
| Force | 0.357 | `#3bff00` | 593 | source |
| Frost | 0.393 | `#0aff00` | 582 | Rex Invictus |
| Hydraulic | 0.393 | `#0aff00` | 582 | Rex Invictus |
| Ice | 0.393 | `#0aff00` | 582 | Rex Invictus |
| Lightning | 0.429 | `#00ff25` | 571 | source |
| Necrotic | 0.500 | `#00ff8b` | 550 | source |
| Piercing | 0.571 | `#00ffec` | 529 | source |
| Poison | 0.643 | `#00afff` | 507 | source |
| Psionic | 0.679 | `#007eff` | 496 | Rex Invictus |
| Psychic | 0.714 | `#004dff` | 486 | source |
| Radiant | 0.786 | `#1900ff` | 464 | source |
| Righteous | 0.821 | `#4a00ff` | 454 | Rex Invictus |
| Radiation | 0.821 | `#4a00ff` | 454 | Rex Invictus |
| Slashing | 0.857 | `#7b00ff` | 443 | source |
| Tarnish | 0.893 | `#ac00ff` | 432 | Rex Invictus |
| Spark | 0.893 | `#ac00ff` | 432 | Rex Invictus |
| Spiritual | 0.893 | `#ac00ff` | 432 | Rex Invictus |
| Stress | 0.893 | `#ac00ff` | 432 | Rex Invictus |
| Tempest | 0.893 | `#ac00ff` | 432 | Rex Invictus |
| Storm | 0.893 | `#ac00ff` | 432 | Rex Invictus |
| Thunder | 0.929 | `#dc00ff` | 421 | source |
| Wither | 0.964 | `#ff00f0` | 411 | Rex Invictus |
| Venom | 0.964 | `#ff00f0` | 411 | Rex Invictus |
| Void | 0.964 | `#ff00f0` | 411 | Rex Invictus |
| Vitriol | 0.964 | `#ff00f0` | 411 | Rex Invictus |

## Duration

| Feature | x | Colour | λ eq. (nm) | Basis |
|---|---|---|---|---|
| Instantaneous | 0.000 | `#ff0028` | 700 | source |
| 1 day | 0.026 | `#ff0008` | 692 | Rex Invictus |
| 1 hour | 0.053 | `#ff1c00` | 684 | source |
| 1 hour or until dispelled | 0.079 | `#ff4200` | 676 | Rex Invictus |
| 1 minute | 0.105 | `#ff6300` | 668 | source |
| 1 round | 0.158 | `#ffae00` | 653 | source |
| 10 days | 0.211 | `#fff500` | 637 | source |
| 10 minutes | 0.263 | `#bdff00` | 621 | source |
| 24 hours | 0.316 | `#76ff00` | 605 | source |
| 30 days | 0.368 | `#2bff00` | 589 | source |
| 6 hours | 0.395 | `#05ff00` | 582 | Rex Invictus |
| 7 days | 0.421 | `#00ff1a` | 574 | source |
| 8 hours | 0.474 | `#00ff66` | 558 | source |
| Special | 0.526 | `#00ffac` | 542 | source |
| Until dispelled | 0.579 | `#00fff7` | 526 | source |
| Up to 1 hour | 0.632 | `#00c0ff` | 511 | source |
| Up to 1 minute | 0.684 | `#0074ff` | 495 | source |
| Up to 1 minute or until the target moves | 0.711 | `#0053ff` | 487 | Rex Invictus |
| Up to 1 round | 0.737 | `#002dff` | 479 | source |
| Up to 10 minutes | 0.789 | `#1e00ff` | 463 | source |
| Up to 2 hours | 0.842 | `#6500ff` | 447 | source |
| Up to 24 hours | 0.895 | `#b100ff` | 432 | source |
| Up to 8 hours | 0.947 | `#f800ff` | 416 | source |
| until the beginning of your next turn | 0.974 | `#ff00df` | 408 | Rex Invictus |
| until the end of your turn | 0.974 | `#ff00df` | 408 | Rex Invictus |
| until the end of your turn or a spell is cast through the prism | 0.974 | `#ff00df` | 408 | Rex Invictus |
| until used or short rest | 0.974 | `#ff00df` | 408 | Rex Invictus |

## Area

| Feature | x | Colour | λ eq. (nm) | Basis |
|---|---|---|---|---|
| None | 0.000 | `#ff0028` | 700 | source |
| cone (15) | 0.028 | `#ff0003` | 692 | source |
| cone (30) | 0.056 | `#ff2200` | 683 | source |
| cone (40) | 0.083 | `#ff4800` | 675 | source |
| cone (60) | 0.111 | `#ff6e00` | 667 | source |
| cube (10) | 0.139 | `#ff9300` | 658 | source |
| cube (100) | 0.167 | `#ffb900` | 650 | source |
| cube (15) | 0.194 | `#ffdf00` | 642 | source |
| cube (150) | 0.222 | `#f8ff00` | 633 | source |
| cube (20) | 0.250 | `#cdff00` | 625 | source |
| cube (200) | 0.278 | `#a7ff00` | 617 | source |
| cube (2500) | 0.306 | `#81ff00` | 608 | source |
| cube (30) | 0.333 | `#5bff00` | 600 | source |
| cube (40) | 0.361 | `#36ff00` | 592 | source |
| cube (40000) | 0.389 | `#10ff00` | 583 | source |
| cube (5) | 0.417 | `#00ff15` | 575 | source |
| cube (5280) | 0.444 | `#00ff3b` | 567 | source |
| cylinder (10) | 0.472 | `#00ff60` | 558 | source |
| cylinder (15) | 0.486 | `#00ff76` | 554 | Rex Invictus |
| cylinder (20) | 0.500 | `#00ff8b` | 550 | source |
| cylinder (30) | 0.514 | `#00ff9b` | 546 | Rex Invictus |
| cylinder (40) | 0.528 | `#00ffb1` | 542 | source |
| cylinder (5) | 0.556 | `#00ffd7` | 533 | source |
| cylinder (50) | 0.583 | `#00fffc` | 525 | source |
| cylinder (5280) | 0.597 | `#00f1ff` | 521 | Rex Invictus |
| cylinder (60) | 0.611 | `#00dbff` | 517 | source |
| line (100) | 0.639 | `#00b5ff` | 508 | source |
| line (50) | 0.667 | `#008fff` | 500 | source |
| line (60) | 0.694 | `#0069ff` | 492 | source |
| line (90) | 0.722 | `#0043ff` | 483 | source |
| sphere (10) | 0.750 | `#0017ff` | 475 | source |
| sphere (100) | 0.778 | `#0e00ff` | 467 | source |
| sphere (120) | 0.792 | `#1e00ff` | 462 | Rex Invictus |
| sphere (15) | 0.806 | `#3400ff` | 458 | source |
| sphere (150) | 0.819 | `#4400ff` | 454 | Rex Invictus |
| sphere (20) | 0.833 | `#5a00ff` | 450 | source |
| sphere (30) | 0.861 | `#8000ff` | 442 | source |
| sphere (300) | 0.875 | `#9600ff` | 438 | Rex Invictus |
| sphere (360) | 0.889 | `#a600ff` | 433 | source |
| sphere (40) | 0.917 | `#cc00ff` | 425 | source |
| sphere (5) | 0.944 | `#f200ff` | 417 | source |
| sphere (5280) | 0.958 | `#ff00f5` | 412 | Rex Invictus |
| sphere (60) | 0.972 | `#ff00e5` | 408 | source |

## Range

| Feature | x | Colour | λ eq. (nm) | Basis |
|---|---|---|---|---|
| 1 mile | 0.000 | `#ff0028` | 700 | source |
| 10 feet | 0.059 | `#ff2700` | 682 | source |
| 10 miles | 0.088 | `#ff4d00` | 674 | Rex Invictus |
| 100 feet | 0.118 | `#ff7800` | 665 | source |
| 120 feet | 0.176 | `#ffc900` | 647 | source |
| 15 feet | 0.206 | `#ffef00` | 638 | Rex Invictus |
| 150 feet | 0.235 | `#e3ff00` | 629 | source |
| 20 feet | 0.265 | `#bdff00` | 621 | Rex Invictus |
| 30 feet | 0.294 | `#91ff00` | 612 | source |
| 300 feet | 0.353 | `#40ff00` | 594 | source |
| 5 feet | 0.412 | `#00ff10` | 576 | source |
| 500 feet | 0.471 | `#00ff60` | 559 | source |
| 500 miles | 0.529 | `#00ffb1` | 541 | source |
| 60 feet | 0.588 | `#00fbff` | 524 | source |
| 90 feet | 0.647 | `#00aaff` | 506 | source |
| Self | 0.706 | `#0058ff` | 488 | source |
| Sight | 0.765 | `#0007ff` | 471 | source |
| Special | 0.824 | `#4a00ff` | 453 | source |
| Touch | 0.882 | `#9b00ff` | 435 | source |
| Unlimited | 0.941 | `#ed00ff` | 418 | source |

## Related

[[Arcane Spectroscopy]] · [[Arcane Spectrometer]] · [[Glyph Key Tables]]
