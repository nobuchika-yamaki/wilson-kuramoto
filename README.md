README
Overview

This repository contains simulation code used in the study
“Absolute Time Limits of Interhemispheric Synchronization in Delayed Cortical Networks.”

We investigate delay-induced synchronization breakdown using:

a bilateral Wilson–Cowan population model (with intrinsic time constants)

a delayed phase-oscillator (Kuramoto-type) model

Both models are evaluated using an identical geometric breakdown criterion to isolate the role of internal dynamics versus phase geometry.

Models
1. Wilson–Cowan (WC) Model

Bilateral excitatory–inhibitory populations

Delayed interhemispheric coupling with stochastic delay (random walk)

Intrinsic time constants: τ_E = τ_I = 10 ms (unless stated otherwise)

2. Phase-Oscillator Model

Delay-coupled phase oscillators

No amplitude dynamics or intrinsic memory

Used as a control model

Synchronization Breakdown Criterion

Synchronization breakdown is defined as:

|φ_L − φ_R| > 1.8 rad


(≈100 degrees phase separation)

This criterion is applied identically to both models for direct comparison.

Key Quantities

τ_crit: critical communication delay at breakdown (ms)

f_L: driving frequency (Hz)

f_L × τ_crit: normalized phase measure

Main Findings (Summary)

τ_crit is approximately invariant across frequencies (5–40 Hz)

Phase-based scaling (f·τ = const) holds in the phase model but fails in WC

Synchronization breakdown is governed by an absolute temporal limit, not phase geometry

The critical delay reflects an emergent stability boundary of delayed E–I dynamics

Running the Simulations

Main script runs:

WC model

Phase model

Frequency sweep

Generates Figure 1 (τ_crit vs f, and f·τ_crit vs f)

Dependencies:

Python ≥ 3.9

NumPy

Matplotlib

Notes

Code prioritizes conceptual clarity and reproducibility over biophysical detail

Designed to extract theoretical limits, not to fit specific experimental datasets
