# The Bind Primitive: Core Abstraction of OTOM

**Authors:** Research Stack Team  
**Date:** April 2026  
**Domain:** TTM Layer M (Lean Semantics - Core)  
**OTOM Version:** 2.2

---

## Abstract

The `bind` primitive is the fundamental operation underlying all computation in the OTOM framework. It provides a unified interface for state transitions across all domains, with explicit cost functions and invariant preservation guarantees.

---

## 1. The bind Signature

$$\text{bind} : (A \times B \times \text{Metric}) \rightarrow \text{Bind}\ A\ B$$

---

## 2. Five bind Classes

| Class | Domain | Signature |
|-------|--------|-----------|
| **informational_bind** | Information theory | $(\text{State} \times \text{Message} \times \text{Entropy}) \rightarrow \text{Bind}$ |
| **geometric_bind** | Geometry | $(\text{Manifold} \times \text{Point} \times \text{Distance}) \rightarrow \text{Bind}$ |
| **thermodynamic_bind** | Thermodynamics | $(\text{System} \times \text{Process} \times \text{Energy}) \rightarrow \text{Bind}$ |
| **physical_bind** | Physics | $(\text{Field} \times \text{Particle} \times \text{Action}) \rightarrow \text{Bind}$ |
| **control_bind** | Control theory | $(\text{Controller} \times \text{Plant} \times \text{Error}) \rightarrow \text{Bind}$ |

---

## 3. Required Components

Every bind instance must provide:

### 3.1 Lawful Check
$$\text{lawful} : \text{Bind}\ A\ B \rightarrow \text{Bool}$$

Predicate verifying state transition validity.

### 3.2 Cost Function
$$\text{cost} : \text{Bind}\ A\ B \rightarrow \text{UInt32}$$

Q16.16 fixed-point cost metric.

### 3.3 Invariant Extractor
$$\text{invariant} : A \rightarrow \text{String}$$

Human-readable invariant description.

---

## 4. The Collapse Principle

All domain logic reduces to bind instances. There are no:
- Utility files
- Helper functions
- Ad-hoc state machines

Every function belongs to a specific bind instance.

---

## 5. Implementation

**Lean 4 Module:** `Bind.lean`

```lean
structure Bind (A B : Type) where
  source : A
  target : B
  metric : Metric
  lawful : Bool
  cost : UInt32
  invariant : String
```

---

## 6. Theorems

### 6.1 bind Preserves Invariant

$$\forall b : \text{Bind}\ A\ B, \text{lawful}(b) \implies \text{invariant}(\text{source}(b)) = \text{invariant}(\text{target}(b))$$

---

## 7. References

- Research Stack, AGENTS.md §4
- Research Stack, OTOM Ontology v2.2.
