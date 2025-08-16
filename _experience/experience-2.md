---
title: "Designing Compact Thermal and Pressure-Stabilised Cavity for Portable Atomic Clocks"
excerpt: "Summer Intern"
collection: experience
---

## Project Role & Supervision
- Research Intern under Prof. Douglas Murray Barrett, National University of Singapore (May ’24)
- Goal: Develop a passively stable optical reference cavity suitable for use in field-deployable atomic clocks

## Research Aim & Objective
- Design and characterise a miniature Fabry-Pérot cavity with active temperature and pressure stabilisation
- Quantify resonance frequency sensitivity to ambient temperature and pressure variations.
- Implement a dual-laser locking scheme: one laser locked to an atomic transition for drift monitoring, another locked to the cavity for frequency reference.

---

## Theoretical Background
- Resonance f = c ∕ (2 n L) for cavity refractive index n and length L; drifts arise from ∂n∕∂T,
∂n∕∂p, and thermal expansion α
- Fractional frequency shift due to temperature: ∂f∕f = –(1⁄n ∂n∕∂T + α) ΔT
- Fractional shift due to pressure: ∂f∕f = –(1⁄n ∂n∕∂p) Δp

---

## Experimental Setup
- **Test cavities**: 3 cm Zerodur, 10 cm quartz, 1.5 cm quartz—each monitored using an 852nm Cs-referenced laser and wide-band EOM sideband locking
- **Temperature control**: PID-regulated TECs with thermistor feedback
- **Pressure control**: vacuum chamber sealing and airtight acrylic enclosure  

---

## Procedure & Measurements
- Monitored free-spectral-range drift by tracking sideband resonance frequency over time
- Correlated short-term fluctuations with ambient temperature changes; measured ∂f∕∂T of quartz cavity
- Sealed cavity to suppress pressure-induced drifts; observed remaining temperature-dependent variations.
- Long-term drift (~200 MHz∕day) attributed to epoxy ageing and quartz creep

---

## Key Findings
- Unstabilized cavities drifted by 8–17 MHz/day; temperature sensitivity far exceeded theoretical α = 5.5 × 10⁻⁷ K⁻¹ due to epoxy layers (effective α ≈ 2.8 × 10⁻⁶ K⁻¹)
- Pressure-sealed cavity eliminated rapid pressure-induced shifts; residual drift dominated by temperature and material ageing.g
- Dual-laser locking successfully tracked cavity resonance variations, enabling post-correction of portable laser frequencies.

---

## Conclusions & Future Work
- Combined thermal and pressure stabilisation yields a robust, compact cavity suitable for portable clock applications.
- **Future studies:** Explore alternative low‐α adhesives, extend monitoring durations to characterise ageing trends, and integrate active pressure control for fully closed-loop stabilisation
