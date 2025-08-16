---
title: "Applications of Quantum Reservoir Computing (QRC) in High-Energy Physics"
excerpt: "Research Intern"
collection: experience
---

## Applications of Quantum Reservoir Computing (QRC) in High-Energy Physics  
**Research Intern**

---

## Role & Supervision
- Research Intern under Shalini Devendrababu, Fractal Analytics (Feb ’25)

## Aim
- Build hybrid quantum-classical workflows for collider anomaly detection and time-series forecasting, demonstrating quantum advantage and sustainability metrics. 

---

## Quantum-Classical Pipelines
- Anomaly Detection: Variational Autoencoder (VAE) or Quantum Autoencoder (QAE) compresses high-dimensional jet observables. Features are fed into a quantum reservoir
(static angle-embedding circuit ⊗ Pauli-basis measurements) with a classical one-class SVM readout.
– Achieved ROC-AUC 0.92 and 15–30% reduction in false positives under realistic NISQ noise (amplitude damping, T2 > 50 µs).
- Time-Series Forecasting: Hybrid QRC using QuantumReservoirPy on superconducting-qubit simulators predicts Global Market Price Series (GMPS). Ridge
regression readout on 8-qubit reservoir yields 20% lower RMSE vs. LSTM and ARIMA baselines.

---

## Performance & Sustainability
- Energy Consumption: ∼5.2 kWh per full pipeline run (quantum simulation + classical
readout), supporting scale-up planning.
- Carbon Footprint: Estimated 1.4 kg CO₂/month for continuous operation.
- Hardware Utilisation: Benchmarked qubit, shot, and memory requirements for modular, cloud-deployable QRC instances.

---

## Key Outcomes
- Demonstrated QRC’s superior feature-space separability and temporal memory with low training overhead.
- Quantified sustainability metrics to guide industrial-scale quantum integration.
- Open-source release of QuantumReservoirPy with tailored modules for anomaly
detection and time-series forecasting in HEP contexts.

