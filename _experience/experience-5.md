---
title: "Energy Demand Forecasting Using Quantum Machine Learning"
excerpt: ""
collection: experience
---

## Energy Demand Forecasting Using Quantum Machine Learning 

---

## Role & Supervision
- Research Intern under Dr. Corey O’Meara, E.ON Digital Technology & Womanium Quantum (Dec ’24)

---

## Project Aim
- Accurately forecast short- and medium-term electricity demand using hybrid quantum–classical pipelines on utility time-series data.

---

## Data & Preprocessing
- Dataset: 10,000+ hourly load profiles (real E.ON data + synthetic series modelling seasonality, holidays, weather).
- Rolling-window split: 80% train / 20% test to preserve temporal order.
- Features: Loads at t–1…t–24, one-hot hour/day encodings, ambient temperature.
- Standardisation: z-score normalisation using training-set statistics.

---

## Models

### Quantum Reservoir Computing (QRC)
- **Encoder**: Angle embedding of 24-lag inputs into four qubits via RX/RZ rotations.  
- **Reservoir**: 3 layers of random single-qubit rotations + CZ entanglers (circuit depth = 3).  
- **Feature extraction**: Pauli-Z expectations on four qubits × 5 virtual nodes (σ = 0.01).  
- **Readout**: Ridge regression (α = 10⁻⁴) on 20-dim feature vectors.  
- **Backend**: Qiskit Aer QASM simulator, 4096 shots per measurement.  

### Quantum-Enhanced Gaussian Process (QGP)
- **Kernel**: Fidelity \( k(x, x′) = |\langle 0 | U†(x′)U(x) | 0 \rangle|² \) on 3-qubit feature map.  
- **Regression**: Exact GP regression using quantum-computed Gram matrix + RBF prior.  
- **Backend**: Qiskit Aer statevector simulator for kernel matrix.  

### Classical Baselines
- **LSTM**: PyTorch model, 2×50-unit layers, Adam (lr = 5×10⁻⁴), dropout = 0.2, early stopping.  
- **ARIMA(5,1,2)**: Parameter selection via AIC.  
- **Gaussian Process**: Scikit-learn GP with RBF kernel and α = 1×10⁻⁶.  


---

## Results (Test RMSE)
- QRC: 3.40% of peak demand
- QGP: 3.22% (15% lower than LSTM’s 3.75%)
- LSTM: 3.75%
- ARIMA: 4.10%
- Temporal Detail: Q-models reduce peak-hour RMSE by 18%, better capturing load ramps.

---

## Architecture Benchmarking

| Model | Qubits | Depth | RMSE (%) | Training Time |
|-------|--------|-------|----------|---------------|
| QRC   | 4      | 3     | 3.40     | 12 min        |
| QGP   | 3      | –     | 3.22     | 8 min         |
| LSTM  | –      | –     | 3.75     | 20 min        |
| ARIMA | –      | –     | 4.10     | 2 min         |

---

## Industry Engagement & Delivery
- Workshops & demos delivered to E.ON R&D teams, including live QRC visualisations.
- Provided Jupyter notebooks integrating Qiskit/Pennylane pipelines and classical comparisons.
- Contributed to joint technical reports; incorporated feedback from five data-science mentors to refine hyperparameters and deployment considerations.

---

## Sustainability & Scalability
- Energy footprint: ~5.2 kWh per full pipeline run (quantum simulation + readout).
- Carbon estimate: 1.4 kg CO₂/month under continuous forecasting.
- Scalability plan: Evaluate cloud-based quantum simulator services and emerging NISQ hardware for real-time grid forecasting.

---

## Conclusion & Next Steps
- Quantum–classical models demonstrate robust RMSE improvements and superior temporal pattern learning.
- Future work: Extend QRC to 8–16 qubits, incorporate real-time weather forecasts, and benchmark on early-access quantum hardware for live operational trials.



