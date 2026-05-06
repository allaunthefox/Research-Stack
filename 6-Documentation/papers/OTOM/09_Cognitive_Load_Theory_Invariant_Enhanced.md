# Cognitive Load Theory: Invariant Enhanced

**Authors:** Research Stack Team
**Date:** May 2026
**Domain:** TTM Layer A (Compression/Routing) + Cognitive Load Theory
**Purpose:** Extend Cognitive Load Theory with invariant preservation

**References:** See [00_Master_References.md](00_Master_References.md) for complete source mapping

---

## Abstract

This paper presents the invariant-enhanced routing engine for the OTOM framework. The original Cognitive Load Theory (CLT) is extended to incorporate invariant preservation, trajectory quality, and convergence inhibition as fundamental load dimensions. Every input byte sequence is now evaluated across eight load dimensions, enabling optimal compression routing through information-theoretic analysis with invariant-aware decision making.

---

## 1. Introduction

The original Cognitive Load Theory provided the mathematical foundation for routing decisions in the OTOM framework, treating compression as a cognitive process. This revision integrates the GCL Invariant Theory framework, recognizing that compression decisions must preserve critical invariants, maintain trajectory quality, and respect convergence inhibition constraints.

**Key insight:** Cognitive load is not merely about compression efficiency—it is about **invariant-aware compression** that preserves the meaningful structure of the data while achieving optimal compression.

---

## 2. Core Equations (Invariant-Enhanced)

### 2.1 Intrinsic Load (Shannon Entropy)

$$L_I(x) = -\sum p(b|x) \log_2 p(b|x)$$

The irreducible complexity of input sequence $x$, measured as Shannon entropy of its byte distribution.

**Status:** Unchanged from original CLT.

---

### 2.2 Extraneous Load (Suboptimal Policy Cost)

$$L_E(x) = \text{BPB}(x, w_{\text{prior}}) - \text{BPB}^*(x)$$

The cost of using a suboptimal routing policy versus the optimal achievable.

**Status:** Unchanged from original CLT.

---

### 2.3 Germane Load (Learning Effort)

$$L_G(x,t) = \sum \gamma^s \cdot \Delta L_E(x_s, t+1)$$

Productive learning effort that improves future routing decisions.

**Status:** Unchanged from original CLT.

---

### 2.4 Routing Load (Decision Cost)

$$L_R(x) = \sum c_j \cdot \mathbb{1}[f_j] + \sum \log_2|M_l|$$

Classification cost plus decision tree traversal cost.

**Status:** Unchanged from original CLT.

---

### 2.5 Memory Load (Storage Burden)

$$L_M(x) = \log_2|E| + \alpha \cdot \mathbb{1}[\text{hit}] + \beta + \lambda \cdot \frac{|E|}{|E_{\text{max}}|}$$

Engram storage, retrieval, and update burden.

**Status:** Unchanged from original CLT.

---

### 2.6 Invariant Preservation Load (NEW)

$$L_{\text{inv}}(x, \mathcal{I}) = \sum_{i \in \mathcal{I}} w_i \cdot \mathbb{1}[\text{broken}(i, x)] \cdot \text{severity}(i)$$

The cost of breaking invariants during compression.

**Components:**
- $\mathcal{I}$: Set of critical invariants to preserve
- $w_i$: Weight of invariant $i$ (importance)
- $\mathbb{1}[\text{broken}(i, x)]$: Indicator if invariant $i$ is broken by compression of $x$
- $\text{severity}(i)$: Severity of breaking invariant $i$ (1 = minor, ∞ = critical)

**Invariants to preserve:**
- **Structural invariants:** Periodicity, symmetry, hierarchical structure
- **Semantic invariants:** Meaning-preserving transformations
- **Statistical invariants:** Distribution moments, correlation structure
- **Topological invariants:** Connectivity, genus, homology groups
- **Causal invariants:** Temporal ordering, dependency structure

**Special case:** Critical invariants have $\text{severity}(i) = \infty$, making $L_{\text{inv}} = \infty$ if broken, forcing rejection of compression path.

---

### 2.7 Trajectory Quality Load (NEW)

$$L_{\text{traj}}(x, \gamma) = \frac{\Sigma(\gamma)}{\Sigma_{\text{optimal}}} - 1$$

The cost of suboptimal trajectory quality through the compression manifold.

**Components:**
- $\gamma$: Compression trajectory (sequence of routing decisions)
- $\Sigma(\gamma) = \int_0^T \sqrt{g_{ij} \dot{x}^i \dot{x}^j}\, dt$: Trajectory length through manifold
- $\Sigma_{\text{optimal}}$: Optimal trajectory length (geodesic)

**Interpretation:**
- $L_{\text{traj}} = 0$: Optimal geodesic path
- $L_{\text{traj}} > 0$: Suboptimal path (longer than necessary)
- $L_{\text{traj}} \gg 0$: Highly inefficient path

**Connection to GCL:** This is the Trajectory Quality Invariant from Invariant Theory, applied to compression routing.

---

### 2.8 Convergence Inhibition Load (NEW)

$$L_{\text{aci}}(s_t) = \mathbb{1}[\text{inhibit}(s_t)] \cdot \frac{\theta_{\text{entropy}} - \text{entropy}(s_t)}{\theta_{\text{entropy}}}$$

The cost of activating Automatic Convergence Inhibition.

**Components:**
- $\text{inhibit}(s_t) = \text{entropy}(s_t) < \theta_{\text{entropy}} \land \text{variance}(s_{t-k:t}) < \theta_{\text{variance}}$
- $\theta_{\text{entropy}}$: Entropy threshold for inhibition
- $\theta_{\text{variance}}$: Variance threshold for inhibition

**Interpretation:**
- $L_{\text{aci}} = 0$: No inhibition (system can converge)
- $L_{\text{aci}} > 0$: Inhibition active (prevents premature convergence)
- $L_{\text{aci}} \to 1$: Maximum inhibition (near threshold)

**Connection to GCL:** This is the ACI mechanism from Invariant Theory, preventing premature convergence to suboptimal compression states.

---

### 2.9 Total Load (Invariant-Enhanced)

$$L_{\text{total}} = \lambda_I \cdot \hat{l}_I + \lambda_E \cdot \hat{l}_E - \lambda_G \cdot \hat{l}_G + \lambda_R \cdot \hat{l}_R + \lambda_M \cdot \hat{l}_M + \lambda_{\text{inv}} \cdot \hat{l}_{\text{inv}} + \lambda_{\text{traj}} \cdot \hat{l}_{\text{traj}} + \lambda_{\text{aci}} \cdot \hat{l}_{\text{aci}}$$

**Weight interpretation:**
- $\lambda_I, \lambda_E, \lambda_R, \lambda_M$: Positive weights (cost)
- $-\lambda_G$: Negative weight (germane load is beneficial)
- $\lambda_{\text{inv}}$: Positive weight (invariant breaking is costly)
- $\lambda_{\text{traj}}$: Positive weight (suboptimal trajectory is costly)
- $\lambda_{\text{aci}}$: Positive weight (inhibition is costly but necessary)

**Normalization:** All $\hat{l}$ values are normalized to $[0,1]$ range.

---

## 3. Invariant Catalog for Compression

### 3.1 Structural Invariants

| Invariant | Description | Severity | Detection Method |
|-----------|-------------|----------|-----------------|
| Periodicity | Repeating patterns | Medium | Autocorrelation, FFT |
| Symmetry | Mirror/rotational symmetry | Low | Group theory analysis |
| Hierarchy | Nested structure | Medium | Tree decomposition |
| Sparsity | Zero/low-value regions | Low | Density analysis |

### 3.2 Semantic Invariants

| Invariant | Description | Severity | Detection Method |
|-----------|-------------|----------|-----------------|
| Meaning preservation | Semantic equivalence | Critical | NLP embeddings |
| Causal ordering | Temporal dependencies | High | Granger causality |
| Dependency structure | Variable relationships | High | Graph analysis |

### 3.3 Statistical Invariants

| Invariant | Description | Severity | Detection Method |
|-----------|-------------|----------|-----------------|
| Distribution moments | Mean, variance, skew, kurtosis | Medium | Moment analysis |
| Correlation structure | Variable correlations | Medium | Correlation matrix |
| Tail behavior | Extreme value distribution | Low | EVT analysis |

### 3.4 Topological Invariants

| Invariant | Description | Severity | Detection Method |
|-----------|-------------|----------|-----------------|
| Connectivity | Graph connectivity | High | BFS/DFS |
| Genus | Surface holes | Medium | Homology computation |
| Homology groups | Topological features | Low | Persistent homology |

---

## 4. Cognitive Process Adapter Integration

### 4.1 Adapter Output as Invariant Source

The Cognitive Process Adapter (from GCL) provides:

```text
ProcessAdapterPacket = {
  representation_shift,
  invariant_focus,
  threshold_pressure,
  obstruction_shape,
  proof_engine,
  search_strategy,
  underverse_shadow,
  surface_projection
}
```

**Integration:** The `invariant_focus` field from the adapter becomes a candidate invariant for $L_{\text{inv}}$.

### 4.2 Representation Shift as Trajectory

The `representation_shift` field maps to trajectory quality:

```text
representation_shift -> trajectory segment
invariant_focus -> invariant preservation check
obstruction_shape -> potential invariant breakage
```

### 4.3 Underverse Shadow as ACI Trigger

The `underverse_shadow` field (what the method excluded) maps to ACI:

```text
underverse_shadow -> potential convergence trap
ACI activation -> prevent convergence to shadow region
```

---

## 5. Updated Clock Integration

### 5.1 Load Profile to Clock Action

| Load Profile | Clock Action | Role | Meaning |
|---|---|---|---|
| Low $L_E$, high $\eta$, low $L_{\text{inv}}$ | ADD | Builder | Forward progress — system is confident |
| High $L_E$, high regret, broken invariant | PAUSE | Judge | Hold state — reassess, don't compound error |
| Load mismatch, $L_{\text{aci}}$ active | SUBTRACT | Warden | Reverse/verify — integrity check |
| High $L_{\text{traj}}$, inefficient path | SUBTRACT | Warden | Backtrack — find better trajectory |
| Critical invariant broken | PAUSE | Judge | Halt — invariant violation |

### 5.2 Invariant-Aware Decision Tree

```
START
  ↓
Check $L_{\text{inv}}$ for critical invariants
  ↓
If critical invariant broken → PAUSE (Judge)
  ↓
Check $L_{\text{aci}}$ (ACI status)
  ↓
If ACI active → SUBTRACT (Warden) or PAUSE (Judge)
  ↓
Check $L_{\text{traj}}$ (trajectory quality)
  ↓
If $L_{\text{traj}}$ high → SUBTRACT (Warden) to backtrack
  ↓
Check $L_E$ (extraneous load)
  ↓
If $L_E$ high with regret → PAUSE (Judge)
  ↓
Check $\eta$ (efficiency)
  ↓
If $\eta$ high → ADD (Builder)
```

---

## 6. 9D Feature Vector (Extended)

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
| 10 | invariantScore | Invariant preservation score (NEW) |
| 11 | trajectoryQuality | Trajectory quality metric (NEW) |
| 12 | aciStatus | ACI activation status (NEW) |

---

## 7. Mixture-of-Experts Predictor (Invariant-Aware)

$$P_w(x_i) = \sum_j w_j \cdot P_{m_j}(x_i | x_{<i}, \mathcal{I})$$

**Change:** Expert models now condition on invariant set $\mathcal{I}$.

**Expert types:**
- $m_1$: Compression expert (original)
- $m_2$: Invariant preservation expert (NEW)
- $m_3$: Trajectory optimization expert (NEW)
- $m_4$: ACI-aware expert (NEW)

---

## 8. Implementation

**Location:** `core/intrinsic/specs/COGNITIVE_LOAD_FUNCTIONS_SPEC_V3.md`

**Lean 4 Module:** `CognitiveLoadInvariantEnhanced.lean` (TODO: Create)

**New components:**
- Invariant detection module
- Trajectory quality computation module
- ACI status monitoring module
- Invariant-aware decision tree

---

## 9. Theorems

### 9.1 Invariant Preservation Theorem

$$\forall x, \forall i \in \mathcal{I}_{\text{critical}}, \text{broken}(i, x) \implies L_{\text{total}}(x) = \infty$$

Critical invariants cannot be broken without infinite cost.

### 9.2 Trajectory Quality Bound

$$L_{\text{traj}}(\gamma) \geq 0, \quad L_{\text{traj}}(\gamma) = 0 \iff \gamma \text{ is geodesic}$$

Trajectory quality is non-negative, zero only for optimal paths.

### 9.3 ACI Convergence Guarantee

$$\text{ACI}(s_0) \land \text{wellFormed}(s_0) \land L_{\text{aci}}(s_t) > 0 \implies \exists! s_\infty, \lim_{t \to \infty} s_t = s_\infty$$

ACI ensures convergence to unique optimal state.

### 9.4 Invariant-Aware Efficiency

$$\eta_{\text{inv}} = \frac{L_I}{L_{\text{total}} - L_{\text{inv}}}$$

Efficiency measured excluding invariant preservation cost (invariant cost is unavoidable).

---

## 10. Comparison: Original vs Invariant-Enhanced

| Dimension | Original CLT | Invariant-Enhanced CLT |
|-----------|--------------|----------------------|
| Load components | 5 | 8 |
| Invariant awareness | None | Explicit ($L_{\text{inv}}$) |
| Trajectory quality | Implicit | Explicit ($L_{\text{traj}}$) |
| Convergence control | None | Explicit ($L_{\text{aci}}$) |
| Clock actions | 3 | 5 (with invariant checks) |
| Feature vector | 9D | 12D |
| Expert models | Compression only | Compression + invariant + trajectory + ACI |

---

## 11. References

- Sweller, J. (1988). Cognitive load during problem solving.
- Shannon, C.E. (1948). A mathematical theory of communication.
- Noether, E. (1918). Invariante Variationsprobleme.
- Research Stack, OTOM Ontology v2.3 (Invariant-Enhanced).
- Research Stack, GCL CognitiveProcessAdapter.md.
- Research Stack, Invariant Theory (08_Invariant_Theory.md).

---

## 12. Future Work

1. **Invariant catalog expansion:** Systematic identification of invariants across data types
2. **Trajectory optimization:** Geodesic computation in compression manifold
3. **ACI threshold tuning:** Adaptive threshold learning
4. **Invariant-aware expert training:** Train expert models on invariant preservation
5. **Empirical validation:** Benchmark invariant-enhanced CLT against original CLT
