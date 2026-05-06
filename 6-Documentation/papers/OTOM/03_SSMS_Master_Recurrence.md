# SSMS Master Recurrence: State Space Model Synthesis

**Authors:** Research Stack Team
**Date:** April 2026
**Domain:** TTM Layer A (Compression/Routing) + Recurrence
**OTOM Version:** 2.2

**References:** See [00_Master_References.md](00_Master_References.md) for complete source mapping

---

## Abstract

The SSMS (State Space Model Synthesis) Master Recurrence provides the unified evolution equation for all agent states in the OTOM framework. It combines selective state space mechanisms with structured evolution rules. The recurrence is now extended with geometric structure folding (Torus-Menger-Horn) for state space navigation and Mass Number gates for transition admissibility.

---

## 1. Introduction

The Master Recurrence unifies all temporal evolution in OTOM through a single equation that governs agent state transitions across the manifold.

---

## 2. The Master Equation

$$S_{t+1} = \text{MLGRU}(\text{Gossip}(\text{Prune}(\text{Stabilize}(\text{Score}_{\Sigma+NK}(\text{Expand}(S_t))))))$$

### 2.1 Components

| Component | Function |
|-----------|----------|
| **Expand** | Generate candidate successor states |
| **Score** | Evaluate candidates using Σ+NK coupling |
| **Stabilize** | Apply conservation constraints |
| **Prune** | Remove unstable trajectories |
| **Gossip** | Share state across agents |
| **MLGRU** | Update via multi-layer gated recurrence |

---

## 3. Unified Manifold-Blit Equation

For manifold-space shortcuts:

$$\mathcal{M}_{t+1} = \text{Blit}_{\text{manifold}}(\mathcal{M}_t, \Delta_{\text{field}})$$

---

## 4. Implementation

**Lean 4 Modules:**
- `SSMS.lean` — Core state space mechanics
- `SSMS_nD.lean` — N-dimensional extension
- `MasterEquation.lean` — Formal verification
- `MLGRU.lean` — Recurrence implementation

---

## 5. Theoretical Properties

- **Conservation:** Energy and information invariants preserved
- **Convergence:** Guaranteed under ACI conditions
- **Completeness:** All valid states reachable

---

## 6. References

- Gu, A., & Dao, T. (2023). Mamba: Linear-time sequence modeling.
- Research Stack, OTOM Ontology v2.2.
