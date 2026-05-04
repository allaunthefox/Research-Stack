
# DIMENSIONAL REDUCTION: EMERGENCE OF FOUR TENSOR STRUCTURES FROM AN n-DIMENSIONAL GEOMETRIC FIELD

---

## D1. Geometric Setup and Fibration Structure

Let $(N, \gamma)$ be a smooth Riemannian manifold of dimension $n$, equipped with metric $\gamma_{AB}$ where $A,B \in \{1, \dots, n\}$. Let $\Phi: N \to \mathbb{R}$ be a smooth function with everywhere non-vanishing differential. The level sets $M_c = \Phi^{-1}(c)$ define a foliation of $N$. We select a single connected 4-dimensional level submanifold $M = M_{c_0}$, and denote the compact fiber by $F = N/M$ with $\dim(F) = d = n - 4$.

The fibration $\pi: N \to M$ induces an exact sequence of tangent bundles:
$$0 \longrightarrow VF \longrightarrow TN \longrightarrow \pi^* TM \longrightarrow 0 \tag{E1}$$
where $VF = \ker(d\pi)$ is the vertical subbundle. We equip $N$ with a connection, i.e., a horizontal subbundle $HN \subset TN$ complementary to $VF$, defining an Ehresmann decomposition $TN = HN \oplus VF$.

We choose adapted local coordinates $(x^\mu, y^a)$ where $x^\mu$ ($\mu = 1, \dots, 4$) parametrize $M$ and $y^a$ ($a = 1, \dots, d$) parametrize the fiber $F$. The metric $\gamma$ decomposes as:
$$\gamma_{AB} = \begin{pmatrix} g_{\mu\nu}(x) + h_{ab}(x,y) A^a_\mu A^b_\nu & h_{bc} A^b_\mu \\ h_{ac} A^c_\nu & h_{ab}(x,y) \end{pmatrix} \tag{E2}$$
where $g_{\mu\nu}$ is the induced metric on $M$, $h_{ab}$ is the metric on $F$, and $A^a = A^a_\mu dx^\mu$ are connection 1-forms. Equivalently, in the coframe $\{dx^\mu, \theta^a\}$ with $\theta^a = dy^a + A^a_\mu dx^\mu$:
$$\gamma = g_{\mu\nu}\, dx^\mu \otimes dx^\nu + h_{ab}\, \theta^a \otimes \theta^b. \tag{E3}$$

The fundamental field $\Phi$ is a smooth section of a tensor bundle over $N$. We write $\Phi(x,y)$ with the understanding that $x \in M$ and $y \in F$.

---

## D2. Harmonic Analysis on the Compact Fiber

Let $\Delta_F = d_F d_F^* + d_F^* d_F$ denote the Laplace--de Rham operator on $F$, where $d_F$ is the exterior derivative along the fiber and $d_F^*$ its adjoint with respect to the fiber metric $h_{ab}$. The spectrum of $\Delta_F$ is discrete and non-negative. We denote by $\{\Upsilon_\alpha^{(p)}\}$ a complete orthonormal basis of eigen-$p$-forms:
$$\Delta_F \Upsilon_\alpha^{(p)} = \lambda_\alpha^{(p)} \Upsilon_\alpha^{(p)}, \qquad \lambda_\alpha^{(p)} \geq 0. \tag{E4}$$

The orthonormality condition is:
$$\int_F \Upsilon_\alpha^{(p)} \wedge \star_F \Upsilon_\beta^{(p)} = \delta_{\alpha\beta}. \tag{E5}$$

For $p=0$ (scalar functions), the lowest eigenvalue is $\lambda_0^{(0)} = 0$ with eigenfunction the constant mode $Y_0 = \mathrm{Vol}(F)^{-1/2}$.

For $p=1$ (1-forms), the lowest eigenvalue is $\lambda_0^{(1)} = 0$ with multiplicity equal to the first Betti number $b_1(F)$. The zero modes are the harmonic 1-forms.

For $p=2$ (2-forms), the lowest eigenvalue is $\lambda_0^{(2)} = 0$ with multiplicity $b_2(F)$.

We henceforth assume the compact fiber $F$ is geometrically distinguished such that the zero eigenspaces of $\Delta_F$ in degrees $p=0,1,2$ satisfy:
$$\dim \ker \Delta_F^{(0)} = 1, \quad \dim \ker \Delta_F^{(1)} = 1, \quad \dim \ker \Delta_F^{(2)} = 2. \tag{E6}$$

This yields exactly four lowest modes:
- One constant scalar mode $Y_0$ (degree 0);
- One harmonic 1-form $\omega$ (degree 1);
- Two harmonic 2-forms $\eta_1, \eta_2$ (degree 2).

These four modes constitute the complete lowest band of the Laplace--de Rham spectrum on $F$. Higher modes correspond to strictly positive eigenvalues and decouple at the level of the massless sector.

---

## D3. Harmonic Decomposition of the Fundamental Field

We expand the fundamental field $\Phi$ in the harmonic basis of the fiber. Taking $\Phi$ to be a 2-form on $N$ (the curvature form of the fibration connection, or equivalently the field strength of the geometric data), we decompose:
$$\Phi(x,y) = \sum_{k=1}^{4} \Phi^{(k)}(x) \wedge \Psi^{(k)}(y) + \text{(higher modes)} \tag{E7}$$
where the four lowest modes $\{\Psi^{(k)}\}_{k=1}^{4}$ are:
$$\Psi^{(1)}(y) = Y_0(y) \quad \text{(constant scalar)}, \tag{E8}$$
$$\Psi^{(2)}(y) = \omega(y) \quad \text{(harmonic 1-form)}, \tag{E9}$$
$$\Psi^{(3)}(y) = \eta_1(y) \quad \text{(harmonic 2-form, first)}, \tag{E10}$$
$$\Psi^{(4)}(y) = \eta_2(y) \quad \text{(harmonic 2-form, second)}. \tag{E11}$$

The expansion coefficients $\Phi^{(k)}(x)$ are differential forms on $M$ of degree determined by the total degree of $\Phi$ and the degree of $\Psi^{(k)}$. Specifically, if $\Phi$ is a 2-form on $N$, then:
- $\Phi^{(1)}$ is a 2-form on $M$;
- $\Phi^{(2)}$ is a 1-form on $M$;
- $\Phi^{(3)}, \Phi^{(4)}$ are 0-forms (scalars) on $M$.

However, via exterior differentiation and Hodge duality on $M$, all four structures induce 2-tensors on $M$ as we now demonstrate.

---

## D4. Emergence of the Four Independent Tensor Structures

### Structure $k=1$: Scalar-Type Symmetric 2-Tensor

The constant mode $Y_0$ yields a purely horizontal 2-form on $M$:
$$\Phi^{(1)}(x) = F^{(1)}_{\mu\nu}(x)\, dx^\mu \wedge dx^\nu. \tag{E12}$$

By the decomposition theorem for 2-forms in four dimensions, any 2-form decomposes into self-dual and anti-self-dual parts. The symmetric tensor structure is obtained from the Hodge-dualized trace-reversed combination:
$$S_{\mu\nu} = F^{(1)}_{\mu\rho} F^{(1)}_{\nu\sigma} g^{\rho\sigma} - \frac{1}{4} g_{\mu\nu} F^{(1)}_{\alpha\beta} F^{(1)\alpha\beta}. \tag{E13}$$

However, the fundamental scalar-type structure is the symmetric 2-tensor defined directly from the metric perturbation:
$$\boxed{F^{(1)}_{\mu\nu} := D_\mu \phi_\nu + D_\nu \phi_\mu} \tag{E14}$$
where $\phi_\mu$ is the 1-form coefficient of the decomposition and $D_\mu$ denotes the Levi-Civita covariant derivative on $(M, g)$. This is a symmetric 2-tensor of scalar type, emerging from the constant mode on the fiber.

### Structure $k=2$: Vector-Type Antisymmetric 2-Tensor

The harmonic 1-form $\omega$ on $F$ yields a 1-form $A = A_\mu dx^\mu$ on $M$. Its exterior derivative defines the emergent antisymmetric field strength:
$$\boxed{F^{(2)}_{\mu\nu} := \partial_\mu A_\nu - \partial_\nu A_\mu} \tag{E15}$$
which satisfies $dF^{(2)} = 0$ by the Poincar\'e lemma. This is a closed 2-form on $M$, hence an antisymmetric 2-tensor of vector type.

### Structures $k=3,4$: Higher-Form Types from Fiber Holonomy

The two harmonic 2-forms $\eta_1, \eta_2$ on $F$ exist by virtue of the reduced holonomy of the fiber metric. Let $\mathrm{Hol}(F) \subset SO(d)$ denote the holonomy group of $F$. The invariant subspaces of $\Lambda^2 T^*F$ under $\mathrm{Hol}(F)$ determine the parallel 2-forms. We assume $\dim \Lambda^2_{\mathrm{inv}} = 2$, giving exactly two harmonic 2-forms.

These induce scalar fields $B_1, B_2$ on $M$ through the expansion coefficients. Their gradients define 1-forms, and by Hodge duality on $M$ (where $\star_M^2 = (-1)^{p(4-p)} = +\mathrm{id}$ for $p=2$ in 4D with Euclidean signature), we construct antisymmetric 2-tensors:
$$\boxed{F^{(k)}_{\mu\nu} := \star_M (dB_k)_{\mu\nu\rho}\, dx^\rho = \varepsilon_{\mu\nu\rho\sigma} g^{\sigma\lambda} D_\lambda B_k, \quad k = 3, 4} \tag{E16}$$
where $\varepsilon_{\mu\nu\rho\sigma}$ is the volume form on $M$. Alternatively, if $\Phi$ contains a 3-form component on $N$, the mixed terms $\Phi_{\mu ab}$ expanded along $\eta_k$ yield 2-forms directly:
$$F^{(k)}_{\mu\nu} = \partial_\mu C^{(k)}_\nu - \partial_\nu C^{(k)}_\mu, \quad k = 3,4 \tag{E17}$$
where $C^{(k)}$ are 1-forms on $M$ emerging from the 2-form harmonics on $F$ via the holonomy reduction.

---

## D5. Emergent Currents $J^{(k)}$

The field equations on $N$ for the fundamental field $\Phi$ are:
$$d\Phi = 0, \qquad d\star \Phi = 0. \tag{E18}$$

Projecting onto the $k$-th harmonic mode by fiber integration against $\Psi^{(k)}$ yields the emergent currents:
$$\boxed{J^{(k)}_\mu := \int_F \Psi^{(k)} \wedge \star_F \left( d\Phi \right)_\mu} \tag{E19}$$
where the subscript $\mu$ denotes the horizontal component. Equivalently, for each structure:

**For $k=1$:**
$$J^{(1)}_\mu = D^\nu F^{(1)}_{\mu\nu} - \frac{1}{2} D_\mu F^{(1)}. \tag{E20}$$

**For $k=2$:**
$$J^{(2)}_\mu = D^\nu F^{(2)}_{\mu\nu}. \tag{E21}$$

**For $k=3,4$:**
$$J^{(k)}_\mu = D^\nu F^{(k)}_{\mu\nu} + \mathcal{O}_k(A, B), \tag{E22}$$
where $\mathcal{O}_k$ denotes covariant coupling terms arising from the holonomy structure of $F$.

---

## D6. Field Equations for Each Structure

Integrating the master equations $(E18)$ over the fiber and using the orthonormality $(E5)$ yields decoupled field equations on $M$:

**$k=1$ (Scalar-type symmetric 2-tensor):**
$$\boxed{D^\nu F^{(1)}_{\mu\nu} - \frac{1}{2} D_\mu F^{(1)} = J^{(1)}_\mu} \tag{E23}$$
where $F^{(1)} = g^{\mu\nu} F^{(1)}_{\mu\nu}$ is the trace. This is the divergence equation for a symmetric 2-tensor.

**$k=2$ (Vector-type antisymmetric 2-tensor):**
$$\boxed{D^\nu F^{(2)}_{\mu\nu} = J^{(2)}_\mu} \tag{E24}$$
which is the Bianchi identity for a closed 2-form coupled to a conserved current.

**$k=3,4$ (Higher-form types):**
$$\boxed{D^\nu F^{(k)}_{\mu\nu} = J^{(k)}_\mu, \quad k = 3, 4} \tag{E25}$$
with the additional constraint from fiber holonomy:
$$\varepsilon^{\mu\nu\rho\sigma} D_\nu F^{(k)}_{\rho\sigma} = \mathcal{H}^{(k)}\big(F^{(2)}, F^{(3)}, F^{(4)}\big) \tag{E26}$$
where $\mathcal{H}^{(k)}$ encodes the topological coupling induced by the structure constants of the fiber holonomy algebra.

---

## D7. Derivation of Coupling Constants $g_k$

The kinetic term on $N$ for the 2-form field $\Phi$ is:
$$S = \int_N \Phi \wedge \star \Phi = \int_M dx \int_F dy\, \sqrt{-g}\, \sqrt{h}\, \Phi_{AB} \Phi^{AB}. \tag{E27}$$

Substituting the harmonic expansion $(E7)$ and using orthonormality $(E5)$:
$$S = \sum_{k=1}^{4} \int_M \Phi^{(k)} \wedge \star_M \Phi^{(k)} \cdot \int_F \Psi^{(k)} \wedge \star_F \Psi^{(k)} + \text{(cross terms)}. \tag{E28}$$

The cross terms vanish due to orthogonality of distinct eigenforms of the Laplacian. The fiber integrals give normalization factors $N_k$:
$$N_k := \int_F \Psi^{(k)} \wedge \star_F \Psi^{(k)}. \tag{E29}$$

For the constant mode ($k=1$):
$$N_1 = \int_F Y_0 \wedge \star_F Y_0 = \int_F Y_0^2 \, d\mathrm{vol}_F = \mathrm{Vol}(F). \tag{E30}$$

For the harmonic 1-form ($k=2$), normalized such that $|\omega|^2 = \lambda_2^{(d-2)/2}$ in geometric units where the fiber size is set by $\lambda_2^{-1/2}$:
$$N_2 = \int_F \omega \wedge \star_F \omega = \mathrm{Vol}(F) \cdot \lambda_2^{(d-2)/2}. \tag{E31}$$

For the harmonic 2-forms ($k=3,4$), similarly:
$$N_k = \int_F \eta_{k-2} \wedge \star_F \eta_{k-2} = \mathrm{Vol}(F) \cdot \lambda_k^{(d-2)/2}, \quad k = 3, 4. \tag{E32}$$

To bring the kinetic term on $M$ to canonical normalization, we rescale:
$$F^{(k)}_{\text{can}} = \sqrt{N_k}\, F^{(k)}. \tag{E33}$$

The physical coupling constant $g_k$ is defined by the inverse square root of this normalization:
$$\frac{1}{g_k^2} := N_k = \int_F \Psi^{(k)} \wedge \star_F \Psi^{(k)}. \tag{E34}$$

Therefore:
$$\boxed{g_k^{-2} = \mathrm{Vol}(F) \cdot \lambda_k^{(d-2)/2}, \quad d = \dim(F) = n - 4} \tag{E35}$$
where for $k=1$ we set $\lambda_1 = 1$ in the exponent (as the constant mode has eigenvalue 0 and the formula is understood with the convention $0^0 = 1$ for $d=2$, or more generally the scalar mode normalization is purely volumetric). For the non-constant modes, $\lambda_k$ is the corresponding eigenvalue of the fiber Laplacian.

---

## D8. Fiber Integration Formula

The master quadratic form on $N$ decomposes under harmonic expansion as:
$$\int_F \Phi \wedge \star \Phi = \sum_{k=1}^{4} \left( \int_F \Psi^{(k)} \wedge \star_F \Psi^{(k)} \right) \Phi^{(k)} \wedge \star_M \Phi^{(k)}. \tag{E36}$$

Using the identification of the emergent field strengths $F^{(k)}_{\mu\nu}$ with the components of $\Phi^{(k)}$, and the coupling definition $(E34)$, we obtain:
$$\int_F F \wedge \star F = \sum_{k=1}^{4} g_k^{-2} \cdot F^{(k)}_{\mu\nu} F^{(k)\mu\nu} \tag{E37}$$
where indices are raised with $g^{\mu\nu}$ on $M$.

Explicitly:
$$\boxed{\int_{N/M} F \wedge \star F = \sum_{k=1}^{4} g_k^{-2}\, F^{(k)}_{\mu\nu} F^{(k)\mu\nu}} \tag{E38}$$

---

## D9. Summary Table

| $k$ | Mode on Fiber | Eigenvalue | Tensor Type on $M$ | Structure | Coupling |
|:---:|:---|:---|:---|:---|:---|
| 1 | Constant scalar $Y_0$ | $\lambda_1 = 0$ | Symmetric 2-tensor | Scalar-type | $g_1^{-2} = \mathrm{Vol}(F)$ |
| 2 | Harmonic 1-form $\omega$ | $\lambda_2 > 0$ | Antisymmetric 2-tensor | Vector-type | $g_2^{-2} = \mathrm{Vol}(F)\, \lambda_2^{(d-2)/2}$ |
| 3 | Harmonic 2-form $\eta_1$ | $\lambda_3 > 0$ | Antisymmetric 2-tensor (Hodge-dual) | Higher-form type | $g_3^{-2} = \mathrm{Vol}(F)\, \lambda_3^{(d-2)/2}$ |
| 4 | Harmonic 2-form $\eta_2$ | $\lambda_4 > 0$ | Antisymmetric 2-tensor (Hodge-dual) | Higher-form type | $g_4^{-2} = \mathrm{Vol}(F)\, \lambda_4^{(d-2)/2}$ |

---

## D10. Geometric Origin of the Correspondences

The correspondence between $k$ and tensor type follows naturally from the degree of the harmonic mode on $F$:

**(i) $k=1$ (Scalar-type, symmetric 2-tensor):** The constant mode $Y_0$ is invariant under the full isometry group of $F$. Its coefficient is a scalar function on $M$ that enters the metric conformally. The symmetric tensor $F^{(1)}_{\mu\nu} = D_\mu \phi_\nu + D_\nu \phi_\mu$ is the unique rank-2 symmetric tensor constructible from a scalar field on a 4-manifold, modulo trace terms.

**(ii) $k=2$ (Vector-type, antisymmetric 2-tensor):** The harmonic 1-form $\omega$ on $F$ reduces the structure group by one dimension. Its coefficient is a 1-form $A$ on $M$, and the natural rank-2 tensor is its exterior derivative $F^{(2)} = dA$, which is antisymmetric by construction. This is the characteristic 2-form of a $U(1)$-type connection over $M$.

**(iii) $k=3,4$ (Higher-form types from fiber holonomy):** The harmonic 2-forms $\eta_1, \eta_2$ exist precisely when $\mathrm{Hol}(F)$ is a proper subgroup of $SO(d)$ leaving invariant subspaces of $\Lambda^2 T^*F$. Each such invariant 2-form on $F$ induces, via dimensional reduction, an effective 2-form structure on $M$. Because these originate from degree-2 forms on the fiber (rather than degree-0 or degree-1), they are classified as higher-form types. Their field strengths $F^{(3)}, F^{(4)}$ satisfy first-order equations $(E26)$ inherited from the integrability conditions of the holonomy reduction.

The entire construction is intrinsic to the geometry of the fibration $N \to M$ with compact fiber $F$. The number four $(4)$ is the sum of the dimensions of the lowest eigenspaces of the Laplace--de Rham operator on $F$ across form degrees $p = 0, 1, 2$ under the assumption $(E6)$.

---

*End of Derivation.*
