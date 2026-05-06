# Master References: OTOM Research Stack

**Authors:** Research Stack Team
**Date:** May 2026
**Domain:** TTM Layer A (Compression/Routing) + Linguistic Invariants
**Purpose:** Master reference document mapping all equations, concepts, and structures to their source files

---

## Core Formalism (Lean 4)

### Information Manifold
**Source:** `0-Core-Formalism/lean/Semantics/Core/InformationManifold.lean`

**Equations/Concepts:**
- Fisher-Rao metric: $g_{ij}(\theta) = E_p[\partial_i \log p \cdot \partial_j \log p]$
- Affine connection: $\nabla = \nabla^{LC} + T$ (with torsion $T$)
- S1 Fisher-Geometric: Torsion-free, genus-3 topology
- S2 Alcubierre Warp: $dI^2 = -d\tau^2 + (dH - \beta d\tau)^2$
- S3 Sovereign Informatic Manifold (SIM): Torsion active, anisotropy $M^{ij} \neq g^{ij}$
- S4 Behavioral/MOIM: Discrete lattice, Genome18 addressing
- Bind primitive: $\text{Bind}(A, B, g) : A \times B \times \text{Metric} \rightarrow \mathbb{R}$

**Used in:**
- 17_Meta_Manifold_Language_Merging.md (manifold structure, bind primitive)
- 13_Language_as_Inverted_Manifold.md (manifold topology)

### Manifold Flow
**Source:** `0-Core-Formalism/lean/external/OTOM/ManifoldFlow.lean`

**Equations/Concepts:**
- Gradient flow for $\phi$: $\partial_t \phi = \nabla_i(M^{ij} \nabla_j \delta F/\delta \phi) - \sigma \partial \phi/\partial I_{lock}$
- Gradient flow for $X^A$: $\partial_t X^A = -\Gamma^A_{BC} \partial_i X^B \partial_i X^C - \Lambda^{AB}(X^B - X_0^B) - \delta F/\delta X^A + \tau T^A$
- Torsion tensor: $T^k_{ij} = \Gamma^k_{ij} - \Gamma^k_{ji}$
- Anisotropy tensor: $M^{ij}$ (directional information flow)
- Fold-back-lock invariant: $I_{lock}$

**Used in:**
- 17_Meta_Manifold_Language_Merging.md (gradient flow, torsion, anisotropy)
- 06_Manifold_Flow.md (core equations)

### Mass Number
**Source:** `0-Core-Formalism/lean/Semantics/Core/MassNumber.lean`

**Equations/Concepts:**
- Mass Number structure: (AdmissiblePacket, ResidualReceipt, BoundaryMarker)
- Admissibility gate: $\text{MassLe}(m, \tau) := A \leq \tau \cdot (R + \varepsilon)$
- Depth policy: max depth = 3
- Promotion readiness: $\text{MassLeDefault} \land \text{depthPolicyOk} \land \text{boundCheck}$
- Underverse rule: quarantine for failed gates

**Used in:**
- 17_Meta_Manifold_Language_Merging.md (admissibility gates, numerical calculations)

### FiveD Torus Topology
**Source:** `0-Core-Formalism/lean/Semantics/Semantics/FiveDTorusTopology.lean`

**Equations/Concepts:**
- Torus distance: $d_{torus} = \sum_{i=0}^{4} \min(|x_i - y_i|, k_i - |x_i - y_i|)$
- Torus diameter: $D_{torus} = \sum_{i=0}^{4} \lfloor k_i/2 \rfloor$
- Bisection bandwidth: $B = k_0 \cdot k_1 \cdot k_2 \cdot k_3 \cdot k_4 / 2$
- Node degree: 10 (2 neighbors per dimension)
- Total connectivity: $C_{total} = k_0 \cdot k_1 \cdot k_2 \cdot k_3 \cdot k_4$

**Used in:**
- 17_Meta_Manifold_Language_Merging.md (5D torus topology, routing)

### Menger Sponge Fractal Addressing
**Source:** `0-Core-Formalism/lean/Semantics/Semantics/MengerSpongeFractalAddressing.lean`

**Equations/Concepts:**
- Hausdorff dimension: $d_H \approx 2.7268$
- Fractal occupancy: $|P_{occ}| = \rho_{occ} \cdot N^{d_H}$
- State space reduction: $R_{reduction} = N^{d_H - 3}$
- Menger hash: $\text{menger\_hash}(x, y, z) = x \oplus (y \ll 1) \oplus (z \ll 2)$
- Fractal offset: $\text{fractal\_offset}(x, y, z) = (x + y + z) \cdot d_H / 65536$
- Menger address: $\text{address} = \text{menger\_hash} \oplus \text{fractal\_offset}$

**Used in:**
- 17_Meta_Manifold_Language_Merging.md (fractal addressing, state space reduction)

### Hybrid TSM-PIST-Torus
**Source:** `0-Core-Formalism/lean/Semantics/Semantics/HybridTSMPISTTorus.lean`

**Equations/Concepts:**
- PIST phase classification: Grounded/Drift/Seismic
- Normalized tension ratio: $\rho(n) = 4m(n)/(2k+1)^2$
- Genetic optimization score: $I = (H \times G) \times (1 - D/64)$
- Lyapunov functional: $\Lambda(S) = m(n) + \lambda f + \mu c(rej)$
- Mirror involution: $\sigma_k(k^2+t) = (k+1)^2-t$
- Resonance check: $m(\sigma_k(n)) = m(n)$

**Used in:**
- 17_Meta_Manifold_Language_Merging.md (PIST phase classification, genetic optimization)

---

## GCL Documentation

### Mass Number Surface Translation
**Source:** `0-Core-Formalism/otom/docs/gcl/MassNumberSurfaceTranslation.md`

**Equations/Concepts:**
- Surface translation: Mass Number → Surface
- Surface fields: height, slope, curvature, basins, ridges, holes, seams, scar field
- MassSurfacePacket structure
- Surface translation rule (8 questions)

**Used in:**
- 17_Meta_Manifold_Language_Merging.md (surface fields, MassSurfacePacket)

---

## CAD Models

### Gabriel's Horn
**Source:** `3-Mathematical-Models/cad_models/gabriels_horn.scad`

**Equations/Concepts:**
- Horn profile: $y = 1/x$
- Horn volume: $V = \int_1^\infty \pi (1/x)^2 dx = \pi$
- Horn surface area: $A = \int_1^\infty 2\pi (1/x) \sqrt{1 + 1/x^4} dx = \infty$
- Byte container surface interpretation

**Used in:**
- 17_Meta_Manifold_Language_Merging.md (Gabriel's horn geometry, finite volume/infinite surface)

---

## OTOM Papers

### 04_Hutter_Prize_Equation.md
**Source:** `6-Documentation/papers/OTOM/04_Hutter_Prize_Equation.md`

**Equations/Concepts:**
- Winning equation: $C = (0.4 \cdot C_{comp} + 0.35 \cdot C_{phys} + 0.25 \cdot C_{geom}) \times (S/(G + F))$
- Compression gain: $-\rho$ (linear penalty)
- Decoder penalty: $\tau^2$ (quadratic penalty)
- Resource penalty: $\sigma^2 + q^2$ (quadratic penalty)
- Tradeoff theorem: sufficient compression gain can offset penalties

**Used in:**
- 17_Meta_Manifold_Language_Merging.md (Hutter Prize integration, penalty terms)

### 09_Cognitive_Load_Theory_Invariant_Enhanced.md
**Source:** `6-Documentation/papers/OTOM/09_Cognitive_Load_Theory_Invariant_Enhanced.md`

**Equations/Concepts:**
- Invariant load: $L_{inv} = \sum_{i=1}^{N_w} w_i \cdot L_S(w_i)$
- NSM primes as invariants
- Cognitive load with invariants

**Used in:**
- 16_Minimal_Semantic_Loss_Cross_Linguistic_Conversion.md (cognitive load integration)
- 17_Meta_Manifold_Language_Merging.md (cognitive load calculations)

### 10_NSM_Primes_Expanded_for_Cognitive_Load.md
**Source:** `6-Documentation/papers/OTOM/10_NSM_Primes_Expanded_for_Cognitive_Load.md`

**Equations/Concepts:**
- 64 NSM semantic primes (expanded list)
- Cognitive load mapping for each prime
- Invariant weights

**Used in:**
- 16_Minimal_Semantic_Loss_Cross_Linguistic_Conversion.md (NSM primes reference)
- 17_Meta_Manifold_Language_Merging.md (anchor points)

### 11_Language_Invariant_Catalog_Complete.md
**Source:** `6-Documentation/papers/OTOM/11_Language_Invariant_Catalog_Complete.md`

**Equations/Concepts:**
- Language invariant catalog (27+ languages)
- Language family classification
- Prime realization patterns
- Compression implications
- Severity weights

**Used in:**
- 15_Public_Domain_Language_Exemplars.md (language list)
- 16_Minimal_Semantic_Loss_Cross_Linguistic_Conversion.md (language families)
- 17_Meta_Manifold_Language_Merging.md (language parameters)

### 12_Language_Prime_Equations_ReDerived.md
**Source:** `6-Documentation/papers/OTOM/12_Language_Prime_Equations_ReDerived.md`

**Equations/Concepts:**
- Language prime equations
- Cognitive load matrix integration
- Prime-based compression

**Used in:**
- 17_Meta_Manifold_Language_Merging.md (language prime equations)

### 13_Language_as_Inverted_Manifold.md
**Source:** `6-Documentation/papers/OTOM/13_Language_as_Inverted_Manifold.md`

**Equations/Concepts:**
- Inverted manifold hypothesis
- Language manifold: $\mathcal{L}(t) = (M, g_{ij}(t), \tau(t))$
- Stress-induced reconfiguration
- Manifold curvature changes

**Used in:**
- 17_Meta_Manifold_Language_Merging.md (manifold reconfiguration)

### 14_Phonon_Mediated_Languages_Mined.md
**Source:** `6-Documentation/papers/OTOM/14_Phonon_Mediated_Languages_Mined.md`

**Equations/Concepts:**
- Cartesian phonon prime integration
- Manhattan distance metric
- Phonon force law
- Forgotten punctuation symbols
- Cognitive load tradeoff conjecture

**Used in:**
- 17_Meta_Manifold_Language_Merging.md (phonon-mediated language patterns)

### 15_Public_Domain_Language_Exemplars.md
**Source:** `6-Documentation/papers/OTOM/15_Public_Domain_Language_Exemplars.md`

**Equations/Concepts:**
- Archive.org public domain exemplars
- 27+ languages with canonical works
- URLs and significance notes
- Resource constraint note

**Used in:**
- 17_Meta_Manifold_Language_Merging.md (language exemplars reference)

### 16_Minimal_Semantic_Loss_Cross_Linguistic_Conversion.md
**Source:** `6-Documentation/papers/OTOM/16_Minimal_Semantic_Loss_Cross_Linguistic_Conversion.md`

**Equations/Concepts:**
- Semantic loss: $L_S(w_{A \rightarrow B}) = 1 - |S(w_A) \cap S(w_B)| / |S(w_A) \cup S(w_B)|$
- Cross-linguistic compression ratio: $C_{cross} = 1 - \overline{L_S}$
- Language distance: $D_{ling} = 1 - E_{cross}$
- Semantic loss tiers (T1-T4)
- Severity weights

**Used in:**
- 17_Meta_Manifold_Language_Merging.md (semantic loss matrix, compression ratios)

### 17_Meta_Manifold_Language_Merging.md
**Source:** `6-Documentation/papers/OTOM/17_Meta_Manifold_Language_Merging.md`

**Equations/Concepts:**
- Language manifold: $\mathcal{M}_L \subset \mathbb{R}^d$
- Meta-manifold: $\mathcal{M}_{meta} = \bigcup_{L \in \mathcal{L}} \mathcal{M}_L$
- Geometric structure folding (Torus-Menger-Horn)
- Mass Number integration
- Numerical calculations

**Used in:**
- (This document is the synthesis of all above)

---

## CAD Models

### MetaManifoldLanguageMerging.lean
**Source:** `0-Core-Formalism/lean/Semantics/Semantics/MetaManifoldLanguageMerging.lean`

**Equations/Concepts:**
- Language manifold: $\mathcal{M}_L \subset \mathbb{R}^d$
- Meta-manifold: $\mathcal{M}_{meta} = \bigcup_{L \in \mathcal{L}} \mathcal{M}_L$
- Torus distance: $d_{torus} = \sum_{i=0}^{4} \min(|x_i - y_i|, k_i - |x_i - y_i|)$
- Menger hash: $\text{menger\_hash}(x, y, z) = x \oplus (y \ll 1) \oplus (z \ll 2)$
- Horn radius: $r(x) = 1/x$
- Fold energy: $E_{fold} = \alpha E_{torus} + \beta E_{menger} + \gamma E_{horn}$
- Mass Number gates for manifold merging
- Surface translation

**Used in:**
- 17_Meta_Manifold_Language_Merging.md (foundational formalization)
- 01_Cognitive_Load_Theory.md (geometric structure folding)
- 05_Bind_Primitive.md (manifold merging gates)
- 06_Manifold_Flow.md (fold dynamics)
- 04_Hutter_Prize_Equation.md (unified compression)
- 08_Invariant_Theory.md (anchor points)

---

## Citation Format

**Inline citation format:**
- For Lean files: `[Source.lean]`
- For documentation: `[Source.md]`
- For papers: `[XX_Paper_Name.md]`

**Example:**
- Fisher-Rao metric [InformationManifold.lean]
- Mass admissibility gate [MassNumber.lean]
- Hutter Prize equation [04_Hutter_Prize_Equation.md]

---

## Cross-Reference Matrix

| Concept | Source | Used In |
|---------|--------|---------|
| Fisher-Rao metric | InformationManifold.lean | 17_Meta_Manifold_Language_Merging.md, MetaManifoldLanguageMerging.lean |
| Gradient flow | ManifoldFlow.lean | 17_Meta_Manifold_Language_Merging.md, 06_Manifold_Flow.md, MetaManifoldLanguageMerging.lean |
| Mass Number gate | MassNumber.lean | 17_Meta_Manifold_Language_Merging.md, MetaManifoldLanguageMerging.lean |
| 5D torus topology | FiveDTorusTopology.lean | 17_Meta_Manifold_Language_Merging.md, MetaManifoldLanguageMerging.lean |
| Menger sponge | MengerSpongeFractalAddressing.lean | 17_Meta_Manifold_Language_Merging.md, MetaManifoldLanguageMerging.lean |
| Gabriel's horn | gabriels_horn.scad | 17_Meta_Manifold_Language_Merging.md, MetaManifoldLanguageMerging.lean |
| Hutter Prize equation | 04_Hutter_Prize_Equation.md | 17_Meta_Manifold_Language_Merging.md, MetaManifoldLanguageMerging.lean |
| NSM primes | 10_NSM_Primes_Expanded_for_Cognitive_Load.md | 16_Minimal_Semantic_Loss_Cross_Linguistic_Conversion.md, 17_Meta_Manifold_Language_Merging.md, MetaManifoldLanguageMerging.lean |
| Language invariants | 11_Language_Invariant_Catalog_Complete.md | 15_Public_Domain_Language_Exemplars.md, 16_Minimal_Semantic_Loss_Cross_Linguistic_Conversion.md, MetaManifoldLanguageMerging.lean |
| Semantic loss | 16_Minimal_Semantic_Loss_Cross_Linguistic_Conversion.md | 17_Meta_Manifold_Language_Merging.md, MetaManifoldLanguageMerging.lean |
| Compression ratios | 16_Minimal_Semantic_Loss_Cross_Linguistic_Conversion.md | 17_Meta_Manifold_Language_Merging.md, MetaManifoldLanguageMerging.lean |
| Inverted manifold | 13_Language_as_Inverted_Manifold.md | 17_Meta_Manifold_Language_Merging.md, MetaManifoldLanguageMerging.lean |
| Phonon-mediated languages | 14_Phonon_Mediated_Languages_Mined.md | 17_Meta_Manifold_Language_Merging.md, MetaManifoldLanguageMerging.lean |
| Meta-manifold | MetaManifoldLanguageMerging.lean | 01_Cognitive_Load_Theory.md, 02_KDA_Physics.md, 03_SSMS_Master_Recurrence.md, 04_Hutter_Prize_Equation.md, 05_Bind_Primitive.md, 06_Manifold_Flow.md, 07_Braid_Structure.md, 08_Invariant_Theory.md |
| Fold dynamics | MetaManifoldLanguageMerging.lean | 02_KDA_Physics.md, 03_SSMS_Master_Recurrence.md, 06_Manifold_Flow.md, 07_Braid_Structure.md, 17_Meta_Manifold_Language_Merging.md |
| Surface translation | MassNumberSurfaceTranslation.md | MetaManifoldLanguageMerging.lean, 17_Meta_Manifold_Language_Merging.md |
