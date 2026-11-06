---
aliases:
  - "Single-Event Latch-up (SEL)"
  - "Single-Event Gate Rupture (SEGR)"
  - "Single-Event Burnout (SEB)"
  - "soft error"
  - "Single-Event Upset (SEU)"
tags:
  - science
  - source/irl
updated: 2026-11-02
---
**[[Destructive Single-Event Effects]]** and their non-destructive cousins are failures caused by a single ionizing particle. See [[Single Event Effects (SEE)]] for the overview.

- **Single-event upset (SEU), or soft error.** A strike flips a [[Semiconductor Devices|memory bit]] or latch. No lasting damage; fixed by error-correcting codes, scrubbing and triple modular redundancy.
- **Single-event latch-up (SEL).** The strike triggers a parasitic thyristor in CMOS, creating a low-resistance path from supply to ground. The part can burn out unless power is cycled quickly.
- **Single-event burnout (SEB).** In power MOSFETs and bipolar transistors, a strike starts runaway current that destroys the device.
- **Single-event gate rupture (SEGR).** In power MOSFETs, a heavy ion breaks down the gate oxide.

Hardening uses SOI processes, guard rings, current limiting and derating ([[Radiation Hardening]]).
