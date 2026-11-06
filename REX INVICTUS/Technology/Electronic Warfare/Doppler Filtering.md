---
aliases:
  - "Doppler processing"
  - "Moving Target Indication"
  - "MTI"
tags:
  - science
  - source/irl
updated: 2026-11-02
---
**[[Doppler Filtering]]** separates targets by the frequency shift their motion puts on the echo: *f*<sub>d</sub> = 2*v*/λ for radial speed *v*. Moving target indication (MTI) cancels stationary clutter between pulses, and pulse-Doppler radars use banks of filters (often FFTs) to measure velocity and reject ground and sea clutter.

Doppler filtering is why plain [[Chaff]] works poorly against modern radars: chaff slows quickly to wind speed, so its echo falls into the clutter notch while the aircraft moves on. See [[Radar Systems]] and [[Pulse Repetition Frequency (PRF)]].
