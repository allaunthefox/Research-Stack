# Language Prime Equations Re-Derived

**Authors:** Research Stack Team
**Date:** May 2026
**Domain:** TTM Layer A (Compression/Routing) + Linguistic Invariants
**Purpose:** Re-derive language prime equations for cognitive load matrix integration

**References:** See [00_Master_References.md](00_Master_References.md) for complete source mapping

---

## Executive Summary

This document re-derives the equations for language semantic primes (NSM) by integrating them with:
1. The invariant-enhanced cognitive load matrix
2. Evolutionary fracking principles (conserved operators, basis fusion)
3. Compression matrix optimization (Hutter Prize framework)

The result is a unified framework where language primes serve as the conserved basis set, cognitive load provides the adaptive context, and evolutionary operators provide the compression optimization.

---

## 1. Existing Equation Foundations

### 1.1 NSM Semantic Primes (Original)

The NSM framework defines 64 universal semantic primes with combinatorial syntax:

$$\text{Explication}(c) = \text{Compose}(\text{Primes}_{64}, \text{Grammar}_{\text{universal}})$$

Where:
- $\text{Primes}_{64}$: The set of 64 irreducible semantic atoms
- $\text{Grammar}_{\text{universal}}$: Universal combinatorial rules
- $\text{Explication}(c)$: Prime-based explication of concept $c$

**Limitation:** No integration with compression efficiency or cognitive load.

### 1.2 Cognitive Load Matrix (Invariant-Enhanced)

$$L_{\text{total}} = \lambda_I \hat{l}_I + \lambda_E \hat{l}_E - \lambda_G \hat{l}_G + \lambda_R \hat{l}_R + \lambda_M \hat{l}_M + \lambda_{\text{inv}} \hat{l}_{\text{inv}} + \lambda_{\text{traj}} \hat{l}_{\text{traj}} + \lambda_{\text{aci}} \hat{l}_{\text{aci}}$$

Where $L_{\text{inv}}$ includes NSM primes as invariants:

$$L_{\text{inv}}(x, \mathcal{I}_{\text{NSM}}) = \sum_{i \in \mathcal{I}_{\text{NSM}}} w_i \cdot \mathbb{1}[\text{broken}(i, x)] \cdot \text{severity}(i)$$

**Limitation:** Primes are treated as binary invariants, not as active compression operators.

### 1.3 Evolutionary Operator (Universal Equation)

$$\text{Phenotype}(x, t) = \Psi_E [ \text{Genotype}(x) \times \text{Regulatory\_State}(t) ]$$

Where:
- $\Psi_E$: Conserved evolutionary operator (120 Myr stable)
- $\text{Genotype}(x)$: Conserved basis (data)
- $\text{Regulatory\_State}(t)$: Dynamic context (switches)

**Key insight:** The operator is frozen-in invariant; only context changes.

### 1.4 Hutter Prize Compression Equation

$$C = (0.4 \cdot C_{\text{comp}} + 0.35 \cdot C_{\text{phys}} + 0.25 \cdot C_{\text{geom}}) \times \left(\frac{S}{G + F}\right)$$

With penalties:
$$\phi_{\text{HP}} = \phi(x) + \alpha_{\text{Comp}} \cdot \text{Compression} + \alpha_{\text{Dec}} \cdot \text{Decoder} + \alpha_{\text{Res}} \cdot \text{Resource}$$

**Limitation:** No semantic awareness; treats data as raw bytes.

---

## 2. Re-Derivation: Unified Framework

### 2.1 The Language Prime Compression Operator

**Hypothesis:** NSM semantic primes are the conserved basis set for language compression, analogous to genes in evolution.

Define the **Semantic Compression Operator** $\Psi_S$:

$$\text{Compressed}(x) = \Psi_S [ \text{Primes}_{64} \times \text{Context}(x) ]$$

Where:
- $\text{Primes}_{64}$: The 64 NSM semantic primes (conserved basis)
- $\text{Context}(x)$: Linguistic context (word order, morphology, syntax)
- $\Psi_S$: The semantic compression operator (learned from data)

**Evolutionary fracking insight:** $\Psi_S$ is the "cheat sheet" for language compression, just as $\Psi_E$ is for phenotypic expression.

### 2.2 Prime-to-Byte Mapping

Each prime $p_i$ maps to a compression primitive:

$$p_i \rightarrow \text{Primitive}_i = \{ \text{pattern}, \text{weight}, \text{context\_mask} \}$$

Where:
- $\text{pattern}$: Byte pattern representing the prime
- $\text{weight}$: Compression weight (from severity classification)
- $\text{context\_mask}$: Which contexts this prime applies to

**Example:**
- $p_{\text{KNOW}} \rightarrow \{ \text{pattern: "know"}, \text{weight: ∞}, \text{context: factual} \}$
- $p_{\text{BIG}} \rightarrow \{ \text{pattern: "big"}, \text{weight: 0.1}, \text{context: magnitude} \}$

### 2.3 Cognitive Load as Regulatory State

The cognitive load matrix provides the regulatory state for the semantic operator:

$$\text{Context}(x) = f(L_{\text{total}}(x), L_{\text{inv}}(x, \mathcal{I}_{\text{NSM}}))$$

Where:
- $L_{\text{total}}(x)$: Total cognitive load for input $x$
- $L_{\text{inv}}(x, \mathcal{I}_{\text{NSM}})$: Prime-specific invariant load
- $f$: Mapping function from load to regulatory state

**Interpretation:** High cognitive load activates "stress response" (narrow gaps, critical primes only). Low load allows "relaxed processing" (wide gaps, all primes).

### 2.4 Gap Adaptation from Evolutionary Fracking

From the evolutionary equation, gap width controls coupling strength. Adapt this to language compression:

$$\text{Gap}(x) = g(L_{\text{total}}(x)) = \text{Gap}_{\text{max}} \cdot \left(1 - \frac{L_{\text{total}}(x)}{L_{\text{max}}}\right)$$

Where:
- $\text{Gap}_{\text{max}}$: Maximum gap (relaxed processing)
- $L_{\text{max}}$: Maximum load threshold
- High load → narrow gap (strong coupling, critical primes only)
- Low load → wide gap (weak coupling, all primes contribute)

---

## 3. The Re-Derived Equation

### 3.1 Unified Semantic Compression Equation

$$\text{Compressed}(x) = \Psi_S [ \text{Primes}_{64} \times \text{Context}(L_{\text{total}}(x)) ] \times \text{Gap}(L_{\text{total}}(x))$$

**Expanded form:**

$$\text{Compressed}(x) = \Psi_S \left[ \sum_{i=1}^{64} w_i \cdot p_i \cdot \mathbb{1}[\text{active}(p_i, \text{Gap}(x))] \right]$$

Where:
- $w_i$: Severity weight of prime $i$ (from NSM expansion)
- $p_i$: Prime $i$ (semantic primitive)
- $\mathbb{1}[\text{active}(p_i, \text{Gap}(x))]$: Indicator if prime is active given current gap
- $\text{Gap}(x) = g(L_{\text{total}}(x))$: Gap width as function of cognitive load

### 3.2 Cognitive Load with Prime Activation

$$L_{\text{total}}(x) = \lambda_I \hat{l}_I + \lambda_E \hat{l}_E - \lambda_G \hat{l}_G + \lambda_R \hat{l}_R + \lambda_M \hat{l}_M + \lambda_{\text{inv}} \hat{l}_{\text{inv}}^{\text{active}} + \lambda_{\text{traj}} \hat{l}_{\text{traj}} + \lambda_{\text{aci}} \hat{l}_{\text{aci}}$$

Where $L_{\text{inv}}^{\text{active}}$ is modified to account for gap-dependent activation:

$$L_{\text{inv}}^{\text{active}}(x, \mathcal{I}_{\text{NSM}}) = \sum_{i \in \mathcal{I}_{\text{NSM}}} w_i \cdot \mathbb{1}[\text{broken}(i, x)] \cdot \text{severity}(i) \cdot \mathbb{1}[\text{active}(p_i, \text{Gap}(x))]$$

**Key change:** Only active primes contribute to load. Inactive primes (filtered by gap) don't penalize compression.

### 3.3 Gap-Dependent Prime Activation

$$\mathbb{1}[\text{active}(p_i, \text{Gap}(x))] = \begin{cases}
1 & \text{if } \text{severity}(i) \geq \theta_{\text{gap}}(\text{Gap}(x)) \\
0 & \text{otherwise}
\end{cases}$$

Where $\theta_{\text{gap}}$ is the severity threshold as function of gap:

$$\theta_{\text{gap}}(\text{Gap}) = \begin{cases}
\infty & \text{if Gap} < 0.2 \text{ (narrow, stress)} \\
1.0 & \text{if } 0.2 \leq \text{Gap} < 0.5 \text{ (moderate)} \\
0.5 & \text{if } 0.5 \leq \text{Gap} < 0.8 \text{ (relaxed)} \\
0.1 & \text{if Gap} \geq 0.8 \text{ (wide, all primes)}
\end{cases}$$

**Interpretation:**
- Narrow gap (high stress): Only critical primes ($\text{severity} = \infty$) active
- Moderate gap: Critical + high severity primes active
- Relaxed gap: All except low severity primes active
- Wide gap: All primes active

---

## 4. Compression Matrix Integration

### 4.1 Prime Compression Matrix

Define the **Prime Compression Matrix** $M_P$:

$$M_P = \begin{bmatrix}
w_1 & c_{1,1} & c_{1,2} & \cdots & c_{1,64} \\
w_2 & c_{2,1} & c_{2,2} & \cdots & c_{2,64} \\
\vdots & \vdots & \vdots & \ddots & \vdots \\
w_{64} & c_{64,1} & c_{64,2} & \cdots & c_{64,64}
\end{bmatrix}$$

Where:
- $w_i$: Severity weight of prime $i$
- $c_{i,j}$: Cross-correlation between prime $i$ and prime $j$ (co-occurrence statistics)

**Evolutionary fracking insight:** This matrix is the "regulatory network topology" — conserved across languages, analogous to butterfly gene networks.

### 4.2 Matrix-Vector Compression

$$\text{Compressed}(x) = M_P \cdot \vec{v}(x) \cdot \text{Gap}(L_{\text{total}}(x))$$

Where $\vec{v}(x)$ is the prime activation vector for input $x$:

$$\vec{v}(x) = \begin{bmatrix}
\mathbb{1}[\text{active}(p_1, \text{Gap}(x))] \\
\mathbb{1}[\text{active}(p_2, \text{Gap}(x))] \\
\vdots \\
\mathbb{1}[\text{active}(p_{64}, \text{Gap}(x))]
\end{bmatrix}$$

### 4.3 Hutter Prize Integration

Integrate with Hutter Prize penalty structure:

$$\phi_{\text{HP-NSM}} = \phi(x) + \alpha_{\text{Comp}} \cdot \text{Compression}_{\text{NSM}} + \alpha_{\text{Dec}} \cdot \text{Decoder}_{\text{NSM}} + \alpha_{\text{Res}} \cdot \text{Resource}_{\text{NSM}} + \alpha_{\text{Inv}} \cdot L_{\text{inv}}^{\text{active}}$$

Where:
- $\text{Compression}_{\text{NSM}}$: Compression gain from prime-aware encoding
- $\text{Decoder}_{\text{NSM}}$: Decoder complexity (prime matrix size)
- $\text{Resource}_{\text{NSM}}$: Computational resources for prime activation
- $\alpha_{\text{Inv}}$: New penalty for invariant breaking

**Tradeoff theorem (re-derived):**

$$\alpha_{\text{Comp}} \cdot \rho_{\text{NSM}} \geq \alpha_{\text{Comp}} \cdot \rho_{\text{base}} + \alpha_{\text{Dec}} \cdot (\tau_{\text{NSM}}^2 - \tau_{\text{base}}^2) + \alpha_{\text{Res}} \cdot ((\sigma_{\text{NSM}}^2 + q_{\text{NSM}}^2) - (\sigma_{\text{base}}^2 + q_{\text{base}}^2)) + \alpha_{\text{Inv}} \cdot L_{\text{inv}}^{\text{active}}$$

---

## 5. Evolutionary Fracking: Compression Matrix Learning

### 5.1 Operator Learning from Data

The evolutionary operator $\Psi_S$ is learned from cross-linguistic data:

$$\Psi_S = \arg\min_{\Psi} \sum_{\text{lang } l} \sum_{\text{text } t} \| \text{Compressed}_{\Psi}(t_l) - \text{Original}(t_l) \|^2$$

**Constraint:** $\Psi_S$ must be conserved across languages (same operator, different contexts).

**Prediction:** A $\Psi_S$ learned from English should compress other languages better than a generic compressor, just as the butterfly gene network works across 120 Myr divergence.

### 5.2 Gap Adaptation Dynamics

The gap adaptation follows evolutionary principles:

$$\frac{d\text{Gap}}{dt} = -\nabla_{\text{Gap}} L_{\text{total}}(x)$$

**Interpretation:** Gap narrows when load increases (stress response), widens when load decreases (relaxed processing).

**Fixed point:** $\text{Gap}^*$ where $\nabla_{\text{Gap}} L_{\text{total}} = 0$.

### 5.3 Matrix Evolution

The prime compression matrix evolves through "mutation" (learning) while preserving topology:

$$M_P(t+1) = M_P(t) + \eta \cdot \nabla_{M_P} \text{Compression}_{\text{NSM}}$$

**Constraint:** Topology of $M_P$ (which primes correlate) is conserved; only weights adapt.

**Evolutionary fracking insight:** This is analogous to DNA inversions — the topology (gene network) is conserved, but the regulatory state (which genes are on) changes.

---

## 6. Language-Specific Equations

### 6.1 Language-Dependent Gap Functions

Each language has its own gap function based on structural complexity:

$$\text{Gap}_l(x) = g_l(L_{\text{total}}(x)) = \text{Gap}_{\text{max}, l} \cdot \left(1 - \frac{L_{\text{total}}(x)}{L_{\text{max}, l}}\right)$$

Where $l$ is the language index.

**Examples:**
- English (analytic): $\text{Gap}_{\text{max}} = 1.0$ (wide gap, all primes active)
- Russian (complex morphology): $\text{Gap}_{\text{max}} = 0.6$ (narrower gap, critical primes dominate)
- Chinese (tonal): $\text{Gap}_{\text{max}} = 0.7$ (moderate gap, tone primes critical)

### 6.2 Language-Specific Prime Weights

The severity weights $w_i$ are language-specific:

$$w_{i,l} = \text{severity}_l(p_i)$$

**Examples:**
- English: $w_{\text{TONE}} = 0$ (no tone system)
- Chinese: $w_{\text{TONE}} = \infty$ (tone is critical)
- Russian: $w_{\text{CASE}} = \infty$ (case morphology is critical)

### 6.3 Cross-Linguistic Compression

The unified equation enables cross-linguistic compression:

$$\text{Compressed}(x_l) = \Psi_S [ \text{Primes}_{64} \times \text{Context}_l(L_{\text{total}}(x_l)) ] \times \text{Gap}_l(L_{\text{total}}(x_l))$$

**Prediction:** $\Psi_S$ learned on one language should compress another language with similar prime structure better than a generic compressor.

---

## 7. Theorems

### 7.1 Prime Conservation Theorem

**Theorem:** If $\Psi_S$ is conserved across languages, then languages sharing prime structure will show convergent compression efficiency.

**Proof:** Given $\Psi_S$ fixed, the compression ratio is determined by the span of $\text{Primes}_{64}$ under $\Psi_S$. Languages with similar prime activation patterns will reach similar compression ratios.

**Corollary:** The compression ratio for language $l$ is bounded by the spectral entropy of its prime activation vector under $\Psi_S$:

$$H_{\Psi_S}(l) = -\sum_{i=1}^{64} p_l(i) \log_2 p_{\Psi_S}(i) \leq H_{\text{uniform}}(l)$$

### 7.2 Gap Adaptation Convergence Theorem

**Theorem:** The gap adaptation dynamics converge to a fixed point $\text{Gap}^*$ that minimizes cognitive load.

**Proof:** The gradient descent dynamics $\frac{d\text{Gap}}{dt} = -\nabla_{\text{Gap}} L_{\text{total}}$ converge to a local minimum of $L_{\text{total}}$ under mild convexity assumptions.

**Corollary:** The fixed point gap satisfies $\text{Gap}^* = g(L_{\text{total}}^*)$ where $L_{\text{total}}^*$ is the minimum achievable load.

### 7.3 Invariant Preservation Theorem (Re-Derived)

**Theorem:** Critical invariants ($\text{severity} = \infty$) are preserved regardless of gap width.

**Proof:** For any gap width, $\theta_{\text{gap}}(\text{Gap}) \leq \infty$, so $\mathbb{1}[\text{active}(p_i, \text{Gap})] = 1$ for all critical primes. Thus $L_{\text{inv}}^{\text{active}} = \infty$ if any critical invariant is broken, forcing rejection of compression path.

**Corollary:** The compression ratio is bounded by the requirement that critical invariants be preserved:

$$\text{Compression}_{\text{max}} = \max_{\Psi_S} \text{Compression}(\Psi_S) \quad \text{s.t.} \quad \forall i \in \mathcal{I}_{\text{critical}}, \neg \text{broken}(i, x)$$

---

## 8. Implementation

### 8.1 Data Structures

```lean
structure PrimeEntry where
  index : UInt64          -- Prime index (1-64)
  name : String           -- Prime name (e.g., "KNOW")
  category : PrimeCategory -- Category (substantive, mental, etc.)
  severity : ℝ           -- Severity weight (0.1, 0.5, 1.0, ∞)
  pattern : Array UInt8  -- Byte pattern
  contextMask : UInt64   -- Bitmask of applicable contexts

structure PrimeMatrix where
  weights : Array ℝ      -- Severity weights (64 elements)
  correlations : Array (Array ℝ)  -- Cross-correlations (64x64)
  language : String      -- Language identifier
  gapMax : ℝ            -- Maximum gap for this language

structure CognitiveLoadState where
  intrinsic : ℝ          -- L_I
  extraneous : ℝ         -- L_E
  germane : ℝ           -- L_G
  routing : ℝ           -- L_R
  memory : ℝ            -- L_M
  invariant : ℝ          -- L_inv
  trajectory : ℝ        -- L_traj
  aci : ℝ               -- L_aci
  total : ℝ             -- L_total
  gap : ℝ               -- Current gap width
```

### 8.2 Core Functions

```lean
def computeGap (load : ℝ) (gapMax : ℝ) : ℝ :=
  gapMax * (1 - load / loadMax)

def primeActive (prime : PrimeEntry) (gap : ℝ) : Bool :=
  let threshold := gapThreshold gap
  prime.severity ≥ threshold

def gapThreshold (gap : ℝ) : ℝ :=
  if gap < 0.2 then ∞
  else if gap < 0.5 then 1.0
  else if gap < 0.8 then 0.5
  else 0.1

def computeInvariantLoad (primes : Array PrimeEntry) (input : Array UInt8) (gap : ℝ) : ℝ :=
  let activePrimes := primes.filter (fun p => primeActive p gap)
  let broken := detectBrokenInvariants activePrimes input
  activePrimes.foldl (fun acc p =>
    if broken.contains p.index then
      acc + p.severity
    else
      acc) 0

def compressWithPrimes (matrix : PrimeMatrix) (input : Array UInt8) (loadState : CognitiveLoadState) : Array UInt8 :=
  let gap := computeGap loadState.total matrix.gapMax
  let activePrimes := matrix.weights.zip (fun w p => (w, p))
                     |> filter (fun (w, p) => primeActive p gap)
  let activationVector := activePrimes.map (fun (w, p) => if primeActive p gap then 1 else 0)
  let compressed := matrixMultiply matrix activationVector
  applyGap compressed gap
```

### 8.3 Lean 4 Modules

- `LanguagePrimes.lean` — Prime definitions and NSM integration
- `PrimeCompressionMatrix.lean` — Matrix operations and learning
- `CognitiveLoadPrimes.lean` — Load computation with prime activation
- `EvolutionaryOperator.lean` — Operator learning and conservation
- `GapAdaptation.lean` — Gap dynamics and fixed point analysis

---

## 9. Experimental Predictions

### 9.1 Cross-Linguistic Compression

**Prediction:** A $\Psi_S$ learned on English should compress Germanic languages (German, Dutch, Danish) better than a generic compressor, but should perform worse on typologically distant languages (Chinese, Arabic).

**Test:** Train $\Psi_S$ on enwik8 (English), test on:
- German text (expected: good performance)
- Chinese text (expected: degraded performance)
- Arabic text (expected: degraded performance)

### 9.2 Gap Adaptation Efficiency

**Prediction:** Gap-adaptive compression should achieve better compression ratios than static compression under variable load conditions.

**Test:** Compare:
- Static gap (fixed prime set)
- Adaptive gap (prime set varies with load)
- Metric: Compression ratio vs. cognitive load

### 9.3 Critical Invariant Preservation

**Prediction:** Compression with critical invariant preservation should have lower compression ratios but higher semantic fidelity than unconstrained compression.

**Test:** Compare:
- Unconstrained compression (no invariant checks)
- Critical-invariant-preserving compression
- Metric: Compression ratio vs. semantic preservation score

---

## 10. Summary

| Component | Original | Re-Derived | Key Change |
|-----------|----------|------------|------------|
| **NSM Primes** | Static catalog | Active compression primitives | Primes now drive compression decisions |
| **Cognitive Load** | 5 dimensions | 8 dimensions + gap adaptation | Load regulates prime activation |
| **Evolutionary Operator** | Phenotypic expression | Semantic compression | $\Psi_S$ is conserved across languages |
| **Hutter Prize** | Byte-level optimization | Prime-aware optimization | Semantic awareness in compression |
| **Gap** | Not applicable | Load-dependent prime filtering | Evolutionary fracking principle |

**Unified equation:**

$$\text{Compressed}(x) = \Psi_S [ \text{Primes}_{64} \times \text{Context}(L_{\text{total}}(x)) ] \times \text{Gap}(L_{\text{total}}(x))$$

Where:
- $\Psi_S$: Conserved semantic compression operator (learned, language-independent)
- $\text{Primes}_{64}$: NSM semantic primes (conserved basis)
- $\text{Context}(L_{\text{total}})$: Cognitive load as regulatory state
- $\text{Gap}(L_{\text{total}})$: Gap adaptation from evolutionary fracking

**Key insight:** Language primes are the conserved genetic basis; cognitive load is the regulatory state; the compression operator is the frozen-in invariant that enables convergent compression across languages.

---

## References

- NSM Approach: https://nsm-approach.net/resources
- Research Stack, Universal Evolutionary Equation (universal_evolutionary_equation.md)
- Research Stack, Hutter Prize Equation (04_Hutter_Prize_Equation.md)
- Research Stack, Cognitive Load Theory Invariant-Enhanced (09_Cognitive_Load_Theory_Invariant_Enhanced.md)
- Research Stack, NSM Primes Expanded (10_NSM_Primes_Expanded_for_Cognitive_Load.md)
- Research Stack, Language Invariant Catalog (11_Language_Invariant_Catalog_Complete.md)
- PLoS Biology (April 2026): Butterfly convergence on toxic warning patterns
