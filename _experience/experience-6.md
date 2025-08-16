---
title: "Reinforcement Learning for Dynamical Quantum Error Correction"
excerpt: "Research Intern"
collection: experience
---

## Role & Supervision
- Research Intern under Dr. Kishor Bharti, ASTAR Singapore (July '24)

## Aim
- Develop adaptive quantum error correction using reinforcement learning agents to optimise syndrome detection and recovery operations under non-Markovian noise environments.

---

## Technical Framework
- **Custom RL Environment:** Built an OpenAI Gym-compatible quantum simulator modelling [] Steane code with spatiotemporally correlated Pauli noise.
- **State Space:** 128-dimensional vector encoding syndrome history, noise correlations, and logical state fidelity estimates via Choi–Choi-Jamiolkowski representation.
- **Action Space:** 64 discrete recovery operations including X/Z Pauli corrections, syndrome measurements, and adaptive waiting periods.
- **Algorithms:** Deep Deterministic Policy Gradient (DDPG) with experience replay and target networks; Deep Q-Network (DQN) with ε-greedy exploration.

---

## Strategic Codes Implementation
- **Spatio-Temporal Framework:** Implemented dynamic stabiliser scheduling, adapting to noise correlation lengths τ ∈ timesteps.
- **Noise Models:** Correlated amplitude damping (T₁ = 100 μs), dephasing (T₂ = 80 μs), and crosstalk with nearest-neighbour coupling strength g = 0.02.
- **Code Distance:** Evaluated on distance-3 codes with seven physical qubits encoding one logical qubit.

---

## Simulation & Training
- **Training:** 5×10⁴ episodes over 200 hours GPU time (NVIDIA A100), batch size 256, learning rate 3×10⁻⁴.
- **Validation:** 10⁴ Monte Carlo trajectories with 20-50 correction cycles per episode.
- **Benchmarks:** Static majority-vote decoder, lookup-table decoder, and minimum-weight perfect matching (MWPM).

---
## Performance Results
- **Logical Fidelity:** RL-adaptive QEC achieved 0.94 ± 0.02 average fidelity vs. 0.76 ± 0.04 for the static MWPM decoder.
- **Threshold Improvement:** Effective error threshold increased from 8.2×10⁻⁴ (static) to 1.4×10⁻³ (RL-adaptive), representing 71% improvement.
- **Syndrome Detection Efficiency:** RL agent reduced average syndrome measurements by 35% while maintaining >90% error detection accuracy.
- **Non-Markovian Robustness:** Sustained >85% fidelity under noise autocorrelation times τ = 30, where traditional decoders dropped to <50%.

---

## Algorithm Benchmarking

| Method        | Avg. Fidelity   | Training Time | Inference Time | Memory Usage |
|---------------|-----------------|---------------|----------------|--------------|
| **DDPG**      | 0.94 ± 0.02     | 180 hrs       | 45 μs          | 2.1 GB       |
| **DQN**       | 0.91 ± 0.03     | 210 hrs       | 52 μs          | 1.8 GB       |
| **Static MWPM** | 0.76 ± 0.04   | –             | 12 μs          | 50 MB        |


---
## Key Technical Achievements

- **Convergence**: DDPG converged to a stable policy after 3.2×10⁴ episodes with a 98.5% success rate on validation episodes.  
- **Generalisation**: Trained agents transferred successfully to 15% different noise environments without retraining.  
- **Real-Time Capability**: Policy inference averaged 45 μs per decision, meeting sub-100 μs requirements for feedback control.

--- 

## Hardware Integration

- Collaborated with ASTAR quantum testbed team to design FPGA-compatible policy deployment.  
- Validated RL policies on a 5-qubit superconducting processor, achieving 89% of simulated performance.  
- Developed a real-time syndrome processing pipeline with <50 μs latency.

---

## Publications & Impact

- Contributed to internal ASTAR technical report: *"Adaptive QEC for Near-Term Quantum Processors."*  
- Presented findings to 12+ researchers across the ASTAR quantum computing division.  
- Results informed the design of Singapore's next-generation quantum error correction testbed.

---

## Conclusion & Future Directions

- Demonstrated **25% improvement** in logical error rates and **35% reduction** in measurement overhead using RL-adaptive strategies.  
- Established framework for real-time deployment on current and near-term quantum hardware platforms.  
- **Next phase**: Scale to [] colour codes and integrate with the full quantum computing stack for fault-tolerant operation demonstration.  
