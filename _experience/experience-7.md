---
title: "K-Block Group Algebra (K-BGA)"
excerpt: "Research Intern"
collection: experience
---

## K-Block Group Algebra (K-BGA)  
**Research Intern**

---

## Role & Supervision
- Research Intern under Dr. Kishor Bharti, ASTAR Singapore (May '24)

---

## Project Objective
- Develop theoretical foundations for generalising quantum two-block group algebra (2-BGA) codes to arbitrary k-block constructions, extending beyond the current two-block limitation to enable more flexible quantum LDPC code design.

---

## Theoretical Framework Development

### Mathematical Generalisation
- **K-Block CSS Construction**: Extended the 2-BGA ansatz from 2×2 to k×k block matrices:  
  - \( H_X = (A_1, A_2, ..., A_k) \)  
  - \( H_Z^T = (B_1^T, B_2^T, ..., B_k^T, -A_1^T, -A_2^T, ..., -A_k^T)^T \)  
- **Group Algebra Integration**: Formulated matrices as \( A_i = L(a_i), B = R(b) \) with \( a_i, b \in F[G] \), preserving CSS orthogonality through left-right matrix commutation properties.

### Dimension Analysis
- **Generalised Dimension Formula**:  
  \( k = n(k-1) - \text{rank}(H_X) - \text{rank}(H_Z) + \text{rank}(H_X H_Z^T) \)  
- **Rank Defect Extension**: Analysed how rank defect parameters \( \delta_i \) generalise from 2-BGA to k-BGA case, identifying conditions where \( \delta_i = 0 \) for semisimple group algebras.

### Code Equivalence Framework
- **Extended Symmetries**: Generalised Theorem 6 equivalence relations to the k-block case, incorporating:  
  - Group automorphisms: \( LP[\varphi(a_1),...,\varphi(a_k), \varphi(b_1),...,\varphi(b_k)] \)  
  - Multi-conjugation: \( LP[\alpha_1^{-1}a_1\alpha_1,..., \beta_1^{-1}b_1\beta_1,...] \)  
  - Block permutations: Additional \( k! \) symmetries from block reordering  
- **Connectivity Analysis**: Extended double-coset decomposition theory to multi-block support group intersections.

### Parameter Bound Analysis
- **Distance Bounds**:  
  - Lower: \( d \geq d_S\sqrt{k} \) (conjectured scaling with block number)  
  - Upper: \( d \leq \min(|G_{a_i}|) \) where \( G_{a_i} \) are support groups  
- **Rate Analysis**: Theoretical rate scaling \( R \approx \frac{k-1}{k} \) for large \( k \), approaching unity asymptotically.

---

## Implementation Challenges Identified
- **Computational Complexity**: Block matrix operations scale as \( O(k^2|G|^2) \), requiring efficient sparse representations.  
- **Optimization Landscape**: k-BGA parameter space grows exponentially, necessitating heuristic search methods.  
- **Commutation Constraints**: Ensuring CSS orthogonality becomes increasingly restrictive with larger k.  

---

## Preliminary Theoretical Results
- **Proof of Concept**: Demonstrated mathematical consistency of \( k=3 \) case through explicit construction.  
- **Specialisation Recovery**: Verified that \( k=2 \) case reduces exactly to known 2-BGA theory.  
- **Connection to Existing Constructions**: Showed k-BGA codes include generalised hypergraph-product codes as special cases when support groups satisfy certain intersection properties.  

---

## Open Questions and Future Directions
- **Distance Scaling**: Actual asymptotic behaviour of \( d \) vs. \( n \) for \( k>2 \) remains unresolved – requires extensive numerical investigation.  
- **Optimal k Selection**: Trade-offs between rate improvement and implementation complexity need empirical study.  
- **Decoding Algorithms**: Iterative decoding strategies for k-BGA codes require development and analysis.  

---

## Technical Contributions
- **Algorithmic Framework**: Designed systematic enumeration procedure for inequivalent k-BGA codes using extended GAP computational tools.  
- **Parameter Space Analysis**: Characterised feasible regions in \( (n,k,d,k_{blocks}) \) parameter space.  
- **Bounds Derivation**: Established theoretical performance limits connecting k-BGA codes to classical group-algebra code theory.  

---

## Project Status and Limitations
- **Theoretical Foundation**: Successfully established mathematical framework and consistency proofs.  
- **Incomplete Numerical Analysis**: Time constraints prevented comprehensive enumeration of \( k>2 \) examples.  
- **Future Implementation**: Framework ready for systematic computational exploration of parameter space.  

---

## Research Impact
- **Foundation for Future Work**: Created theoretical infrastructure enabling systematic study of multi-block quantum LDPC constructions.  
- **Bridging Theory**: Connected group algebra methods with modern quantum LDPC code theory.  
- **Algorithmic Contributions**: Developed computational approaches for exploring quantum code parameter spaces.  

---

## Recommendation
This preliminary theoretical framework provides solid mathematical foundations for k-BGA codes. Future research should focus on computational enumeration of small examples (\( k=3,4 \)) and numerical validation of predicted scaling behaviours to establish practical utility of the generalised construction.
