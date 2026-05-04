# Cognitive Load Theory: Information-Theoretic Compression Routing

**Authors:** Research Stack Team  
**Date:** April 2026  
**Domain:** TTM Layer A (Compression/Routing)  
**OTOM Version:** 2.2

---

## Abstract

This paper presents the foundational routing engine for the OTOM framework. Every input byte sequence is evaluated across five load dimensions, enabling optimal compression routing through information-theoretic analysis.

---

## 1. Introduction

The Cognitive Load Theory (CLT) provides the mathematical foundation for routing decisions in the OTOM framework. It extends Sweller's cognitive load theory into the information-theoretic domain, treating compression as a cognitive process performed by computational agents.

---

## 2. Core Equations

### 2.1 Intrinsic Load (Shannon Entropy)

$$L_I(x) = -\sum p(b|x) \log_2 p(b|x)$$

The irreducible complexity of input sequence $x$, measured as Shannon entropy of its byte distribution.

### 2.2 Extraneous Load (Suboptimal Policy Cost)

$$L_E(x) = \text{BPB}(x, w_{\text{prior}}) - \text{BPB}^*(x)$$

The cost of using a suboptimal routing policy versus the optimal achievable.

### 2.3 Germane Load (Learning Effort)

$$L_G(x,t) = \sum \gamma^s \cdot \Delta L_E(x_s, t+1)$$

Productive learning effort that improves future routing decisions.

### 2.4 Routing Load (Decision Cost)

$$L_R(x) = \sum c_j \cdot \mathbb{1}[f_j] + \sum \log_2|M_l|$$

Classification cost plus decision tree traversal cost.

### 2.5 Memory Load (Storage Burden)

$$L_M(x) = \log_2|E| + \alpha \cdot \mathbb{1}[\text{hit}] + \beta + \lambda \cdot \frac{|E|}{|E_{\text{max}}|}$$

Engram storage, retrieval, and update burden.

### 2.6 Total Load

$$L_{\text{total}} = \lambda_I \cdot \hat{l}_I + \lambda_E \cdot \hat{l}_E - \lambda_G \cdot \hat{l}_G + \lambda_R \cdot \hat{l}_R + \lambda_M \cdot \hat{l}_M$$

---

## 3. 9D Feature Vector

| Dimension | Symbol | Description |
|-----------|--------|-------------|
| 1 | byteEntropy | Shannon entropy of byte distribution |
| 2 | repetitionRate | Frequency of repeated sequences |
| 3 | dictPotential | Dictionary compression opportunity |
| 4 | periodicityLag1 | First-order periodicity measure |
| 5 | residualSparsity | Sparsity after transformation |
| 6 | matchDensity | Density of matching contexts |
| 7 | longestMatch | Length of longest repeated sequence |
| 8 | bitplaneBias | Correlation across bit planes |
| 9 | bestStrideCorr | Best stride correlation |

---

## 4. Mixture-of-Experts Predictor

$$P_w(x_i) = \sum_j w_j \cdot P_{m_j}(x_i | x_{<i})$$

Weighted ensemble prediction across expert models $m_j$.

---

## 5. Implementation

**Location:** `core/intrinsic/specs/COGNITIVE_LOAD_FUNCTIONS_SPEC.md`

**Lean 4 Module:** `CognitiveLoad.lean` (TODO: Create)

---

## 6. References

- Sweller, J. (1988). Cognitive load during problem solving.
- Shannon, C.E. (1948). A mathematical theory of communication.
- Research Stack, OTOM Ontology v2.2.
