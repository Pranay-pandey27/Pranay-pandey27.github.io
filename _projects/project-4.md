---
title: "Variational Quantum Eigensolver for Molecular Ground State Calculation"
collection: projects
---

# Purpose
Implementation of the **Variational Quantum Eigensolver (VQE)** for quantum chemistry applications, specifically calculating **ground state energies of molecules** using quantum algorithms.

---

# Key Components

### Three Implementation Stages
1. **Basic VQE** – H₂ molecule with STO-3G basis set  
2. **Advanced VQE** – Attempted LiH molecule with cc-pVDZ basis *(encountered memory limitations)*  
3. **Production VQE** – H₂ with realistic noise models and error mitigation  

---

# Technical Features
- **Framework:** Qiskit Nature for molecular simulation  
- **Ansatz Circuits:** EfficientSU2 and UCCSD variational forms  
- **Hardware Simulation:** FakeManila backend with noise models  
- **Error Mitigation:** Complete measurement error mitigation  
- **Optimisation:** SLSQP optimiser with convergence tracking  
- **Visualisation:** Energy convergence plots and qubit expectation values  

---

# Results
- **Ground State Energy:** Successfully calculated H₂ energy (~ **-0.52 Hartree**)  
- **Quantum Advantage:** Demonstrated VQE's capability over classical methods  
- **Convergence Analysis:** Visualised optimisation progress and parameter evolution  

---

# Summary
This project demonstrates a **complete quantum chemistry workflow**:
- From molecular setup → to energy calculation  
- With **realistic hardware constraints**, noise models, and error mitigation  

It highlights VQE’s potential as a **practical near-term quantum algorithm** for quantum chemistry.
