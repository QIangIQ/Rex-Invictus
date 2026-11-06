---
aliases:
  - "LFM"
  - "Chirp"
  - "Modulation Scheme"
  - "Modulation Type"
tags:
  - science
  - source/irl
updated: 2026-11-02
---
**[[Linear Frequency Modulation (LFM)]]**, or a chirp, sweeps a pulse's frequency linearly across a bandwidth *B* during the pulse width τ. It is the most common [[Pulse Compression]] waveform because it is easy to generate and tolerant of Doppler shift. Its drawback is range-Doppler coupling: a moving target appears slightly displaced in range. Sidelobes are usually reduced with amplitude weighting (such as Hamming windows) on receive.

The other main family is [[Phase Modulation (PM)]], such as [[Phase Modulation (PM)|BPSK]] Barker codes. Matching a received chirp to its replica is the job of the [[Matched Filter]].
