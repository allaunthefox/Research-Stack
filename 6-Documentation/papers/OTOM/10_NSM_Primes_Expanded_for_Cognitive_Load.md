# NSM Semantic Primes Expanded for Cognitive Load

**Authors:** Research Stack Team
**Date:** May 2026
**Domain:** TTM Layer A (Compression/Routing) + Linguistic Invariants
**Purpose:** Expand NSM semantic primes for cognitive load invariants

**References:** See [00_Master_References.md](00_Master_References.md) for complete source mapping

---

## Executive Summary

The 64 Natural Semantic Metalanguage (NSM) primes provide a catalog of universal semantic atoms that can serve as invariant constraints for compression. While not mathematically "solid" invariants, they offer a flexible framework for meaning-preserving compression decisions. This document expands each prime with:
- Compression-relevant interpretation
- Detection method
- Severity weight for $L_{\text{inv}}$
- Integration with sovereign invariants

---

## Prime Categories and Compression Mapping

### Category 1: Substantives (6 primes)

**I** (self-reference)
- **Compression role:** First-person perspective preservation
- **Detection:** Pronoun resolution, entity tracking
- **Severity:** Medium (meaning change if lost)
- **Sovereign invariant link:** CL-I1 (Load Conservation) - self-reference as state anchor

**YOU** (other-reference)
- **Compression role:** Second-person perspective preservation
- **Detection:** Dialogue parsing, address terms
- **Severity:** Medium (conversational coherence)
- **Sovereign invariant link:** TD-I1 (Harmonic Kernel) - relational symmetry

**SOMEONE** (generic person)
- **Compression role:** Generic entity reference
- **Detection:** Indefinite pronoun patterns
- **Severity:** Low (can often be compressed)
- **Sovereign invariant link:** NA-I1 (MLGRU Fixed Point) - attractor state

**SOMETHING** (generic entity)
- **Compression role:** Generic object reference
- **Detection:** Indefinite noun phrases
- **Severity:** Low (highly compressible)
- **Sovereign invariant link:** AF-I1 (Norm Preservation) - entity normalization

**PEOPLE** (collective persons)
- **Compression role:** Collective reference preservation
- **Detection:** Plural entity tracking
- **Severity:** Medium (group identity)
- **Sovereign invariant link:** TD-I2 (Betti Conservation) - topological group structure

**BODY** (physical body)
- **Compression role:** Embodiment reference
- **Detection:** Body part vocabulary, embodied language
- **Severity:** Medium (embodied cognition)
- **Sovereign invariant link:** VP-I1 (Shell Partitioning) - physical containment

---

### Category 2: Relational (2 primes)

**KIND** (type/category)
- **Compression role:** Taxonomic relationship preservation
- **Detection:** Class membership, inheritance
- **Severity:** High (structural integrity)
- **Sovereign invariant link:** CL-I4 (Dimensional Reduction) - hierarchy preservation

**PART** (mereological part)
- **Compression role:** Part-whole relationship preservation
- **Detection:** Part-of relations, containment
- **Severity:** High (structural integrity)
- **Sovereign invariant link:** TD-I2 (Betti Conservation) - topological decomposition

---

### Category 3: Determiners (3 primes)

**THIS** (deictic proximal)
- **Compression role:** Proximal deixis preservation
- **Detection:** Proximal demonstratives, indexicals
- **Severity:** Medium (reference resolution)
- **Sovereign invariant link:** RG-I3 (Observer Frame) - subjective reference point

**THE SAME** (identity)
- **Compression role:** Identity equivalence preservation
- **Detection:** Coreference chains, anaphora
- **Severity:** Critical (identity is fundamental)
- **Sovereign invariant link:** SC-I2 (Deterrence Consistency) - logical equivalence

**OTHER** (contrast)
- **Compression role:** Contrastive distinction preservation
- **Detection:** Contrastive markers, alternation
- **Severity:** Medium (distinction preservation)
- **Sovereign invariant link:** NA-I2 (Hysteresis) - state discrimination

---

### Category 4: Quantifiers (7 primes)

**ONE** (unit)
- **Compression role:** Singularity preservation
- **Detection:** Singular markers, unit quantifiers
- **Severity:** Low (often compressible)
- **Sovereign invariant link:** AF-I2 (Involution Property) - 2-periodicity

**TWO** (pair)
- **Compression role:** Duality preservation
- **Detection:** Pair markers, binary quantifiers
- **Severity:** Low (often compressible)
- **Sovereign invariant link:** VP-I2 (Coordinate Constraint) - binary partition

**SOME** (existential)
- **Compression role:** Existential quantification
- **Detection:** Existential quantifiers, indefinites
- **Severity:** Low (highly compressible)
- **Sovereign invariant link:** AF-I3 (Machine Epsilon) - approximation tolerance

**ALL** (universal)
- **Compression role:** Universal quantification
- **Detection:** Universal quantifiers, totality markers
- **Severity:** High (universal claims are sensitive)
- **Sovereign invariant link:** CL-I2 (Efficiency Boundedness) - completeness

**MUCH/MANY** (large quantity)
- **Compression role:** Plurality preservation
- **Detection:** Plural markers, quantifiers
- **Severity:** Low (often compressible)
- **Sovereign invariant link:** RG-I1 (Phase Boundary) - critical mass

**LITTLE/FEW** (small quantity)
- **Compression role:** Scarcity preservation
- **Detection:** Negation, scarcity markers
- **Severity:** Low (often compressible)
- **Sovereign invariant link:** TD-I3 (Anti-Collision Bound) - minimal separation

---

### Category 5: Evaluators (2 primes)

**GOOD** (positive evaluation)
- **Compression role:** Positive valuation preservation
- **Detection:** Positive sentiment, approval markers
- **Severity:** Medium (affective content)
- **Sovereign invariant link:** CL-I3 (Regret Identity) - reward signal

**BAD** (negative evaluation)
- **Compression role:** Negative valuation preservation
- **Detection:** Negative sentiment, disapproval markers
- **Severity:** Medium (affective content)
- **Sovereign invariant link:** SC-I1 (Escalation Fixed Point) - penalty signal

---

### Category 6: Descriptors (2 primes)

**BIG** (large magnitude)
- **Compression role:** Magnitude preservation (large)
- **Detection:** Size adjectives, magnitude quantifiers
- **Severity:** Low (often compressible to scale factor)
- **Sovereign invariant link:** HW-I2 (Logarithmic Scaling) - magnitude encoding

**SMALL** (small magnitude)
- **Compression role:** Magnitude preservation (small)
- **Detection:** Size adjectives, magnitude quantifiers
- **Severity:** Low (often compressible to scale factor)
- **Sovereign invariant link:** AF-I3 (Machine Epsilon) - minimal representation

---

### Category 7: Mental Predicates (6 primes)

**THINK** (cognition)
- **Compression role:** Cognitive process preservation
- **Detection:** Mental state verbs, epistemic markers
- **Severity:** High (epistemic status)
- **Sovereign invariant link:** NA-I1 (MLGRU Fixed Point) - cognitive attractor

**KNOW** (knowledge)
- **Compression role:** Knowledge state preservation
- **Detection:** Factive verbs, certainty markers
- **Severity:** Critical (knowledge claims are fundamental)
- **Sovereign invariant link:** SC-I2 (Deterrence Consistency) - factual consistency

**WANT** (volition)
- **Compression role:** Volitional state preservation
- **Detection:** Desire verbs, intention markers
- **Severity:** Medium (agentive intent)
- **Sovereign invariant link:** CL-I3 (Regret Identity) - preference ordering

**FEEL** (affect)
- **Compression role:** Affective state preservation
- **Detection:** Emotion verbs, affect markers
- **Severity:** Medium (emotional content)
- **Sovereign invariant link:** VP-I3 (Genetic Entropy) - affective information

**SEE** (visual perception)
- **Compression role:** Visual perception preservation
- **Detection:** Perception verbs, evidentiality markers
- **Severity:** Low (often compressible)
- **Sovereign invariant link:** RG-I3 (Observer Frame) - visual perspective

**HEAR** (auditory perception)
- **Compression role:** Auditory perception preservation
- **Detection:** Perception verbs, evidentiality markers
- **Severity:** Low (often compressible)
- **Sovereign invariant link:** TD-I4 (Coupling-Velocity Tradeoff) - signal transmission

---

### Category 8: Speech (3 primes)

**SAY** (speech act)
- **Compression role:** Speech act preservation
- **Detection:** Reporting verbs, quotation markers
- **Severity:** Medium (attribution)
- **Sovereign invariant link:** SC-I2 (Deterrence Consistency) - communicative consistency

**WORDS** (linguistic form)
- **Compression role:** Linguistic form preservation
- **Detection:** Metalinguistic reference
- **Severity:** Low (often compressible)
- **Sovereign invariant link:** AF-I1 (Norm Preservation) - form normalization

**TRUE** (veridicality)
- **Compression role:** Truth value preservation
- **Detection:** Truth predicates, veridicality markers
- **Severity:** Critical (truth is fundamental)
- **Sovereign invariant link:** Master Invariant (Coherence Conservation) - truth preservation

---

### Category 9: Actions, Events, Movement (3 primes)

**DO** (agentive action)
- **Compression role:** Agentive action preservation
- **Detection:** Action verbs, agency markers
- **Severity:** Medium (agency)
- **Sovereign invariant link:** NA-I3 (Ternary Quantization) - discrete action states

**HAPPEN** (event occurrence)
- **Compression role:** Event occurrence preservation
- **Detection:** Event verbs, aspect markers
- **Severity:** Medium (event structure)
- **Sovereign invariant link:** TD-I1 (Harmonic Kernel) - event harmonics

**MOVE** (movement)
- **Compression role:** Movement preservation
- **Detection:** Motion verbs, path descriptions
- **Severity:** Low (often compressible)
- **Sovereign invariant link:** VP-I1 (Shell Partitioning) - spatial partitioning

---

### Category 10: Existence and Possession (4 primes)

**BE (SOMEWHERE)** (existence at location)
- **Compression role:** Existential location preservation
- **Detection:** Existential locatives
- **Severity:** Medium (spatial anchoring)
- **Sovereign invariant link:** RG-I3 (Observer Frame) - spatial reference

**THERE IS** (existence)
- **Compression role:** Existence preservation
- **Detection:** Existential constructions
- **Severity:** Medium (ontological commitment)
- **Sovereign invariant link:** Master Invariant (Coherence Conservation) - existence

**BE (SOMEONE/SOMETHING)** (predication)
- **Compression role:** Predication preservation
- **Detection:** Copular constructions
- **Severity:** Low (often compressible)
- **Sovereign invariant link:** CL-I4 (Dimensional Reduction) - property space

**HAVE** (possession)
- **Compression role:** Possession preservation
- **Detection:** Possessive constructions
- **Severity:** Medium (ownership/relationship)
- **Sovereign invariant link:** TD-I2 (Betti Conservation) - mereological structure

---

### Category 11: Life and Death (2 primes)

**LIVE** (living state)
- **Compression role:** Vitality preservation
- **Detection:** Life predicates, vitality markers
- **Severity:** Medium (biological status)
- **Sovereign invariant link:** VP-I3 (Genetic Entropy) - biological information

**DIE** (death state)
- **Compression role:** Mortality preservation
- **Detection:** Death predicates, mortality markers
- **Severity:** Critical (irreversible state change)
- **Sovereign invariant link:** Master Invariant (Coherence Conservation) - state transition

---

### Category 12: Time (8 primes)

**WHEN/TIME** (temporal reference)
- **Compression role:** Temporal reference preservation
- **Detection:** Temporal adverbs, tense markers
- **Severity:** Medium (temporal anchoring)
- **Sovereign invariant link:** RG-I1 (Phase Boundary) - temporal phase

**NOW** (present moment)
- **Compression role:** Present moment preservation
- **Detection:** Present tense, deictic now
- **Severity:** Medium (temporal deixis)
- **Sovereign invariant link:** NA-I2 (Hysteresis) - present state dependence

**BEFORE** (prior time)
- **Compression role:** Temporal ordering (prior)
- **Detection:** Past tense, anterior markers
- **Severity:** Medium (temporal sequence)
- **Sovereign invariant link:** TD-I4 (Coupling-Velocity Tradeoff) - temporal coupling

**AFTER** (subsequent time)
- **Compression role:** Temporal ordering (subsequent)
- **Detection:** Future tense, posterior markers
- **Severity:** Medium (temporal sequence)
- **Sovereign invariant link:** SC-I3 (Threshold Scale Separation) - temporal scaling

**A LONG TIME** (extended duration)
- **Compression role:** Extended duration preservation
- **Detection:** Duration quantifiers
- **Severity:** Low (often compressible)
- **Sovereign invariant link:** HW-I2 (Logarithmic Scaling) - duration encoding

**A SHORT TIME** (brief duration)
- **Compression role:** Brief duration preservation
- **Detection:** Duration quantifiers
- **Severity:** Low (often compressible)
- **Sovereign invariant link:** AF-I3 (Machine Epsilon) - minimal duration

**FOR SOME TIME** (duration)
- **Compression role:** Duration preservation
- **Detection:** Duration constructions
- **Severity:** Low (often compressible)
- **Sovereign invariant link:** RG-I2 (Lawfulness Excess) - duration accounting

**MOMENT** (instant)
- **Compression role:** Instant preservation
- **Detection:** Instant markers, punctual aspect
- **Severity:** Low (often compressible)
- **Sovereign invariant link:** VP-I2 (Coordinate Constraint) - point event

---

### Category 13: Space (9 primes)

**WHERE/PLACE** (spatial reference)
- **Compression role:** Spatial reference preservation
- **Detection:** Spatial adverbs, locative markers
- **Severity:** Medium (spatial anchoring)
- **Sovereign invariant link:** VP-I1 (Shell Partitioning) - spatial partitioning

**HERE** (proximal location)
- **Compression role:** Proximal location preservation
- **Detection:** Proximal demonstratives, deictic here
- **Severity:** Medium (spatial deixis)
- **Sovereign invariant link:** RG-I3 (Observer Frame) - spatial reference point

**ABOVE** (superior position)
- **Compression role:** Vertical relation (above)
- **Detection:** Spatial prepositions, vertical markers
- **Severity:** Low (often compressible)
- **Sovereign invariant link:** TD-I1 (Harmonic Kernel) - vertical symmetry

**BELOW** (inferior position)
- **Compression role:** Vertical relation (below)
- **Detection:** Spatial prepositions, vertical markers
- **Severity:** Low (often compressible)
- **Sovereign invariant link:** TD-I1 (Harmonic Kernel) - vertical symmetry

**FAR** (distant)
- **Compression role:** Distance preservation (far)
- **Detection:** Distance adjectives, remote markers
- **Severity:** Low (often compressible)
- **Sovereign invariant link:** HW-I2 (Logarithmic Scaling) - distance encoding

**NEAR** (proximate)
- **Compression role:** Distance preservation (near)
- **Detection:** Distance adjectives, proximal markers
- **Severity:** Low (often compressible)
- **Sovereign invariant link:** TD-I3 (Anti-Collision Bound) - proximity constraint

**SIDE** (lateral)
- **Compression role:** Lateral relation preservation
- **Detection:** Lateral prepositions, side markers
- **Severity:** Low (often compressible)
- **Sovereign invariant link:** VP-I2 (Coordinate Constraint) - lateral coordinate

**INSIDE** (containment)
- **Compression role:** Containment preservation
- **Detection:** Containment prepositions, inclusion markers
- **Severity:** Medium (mereological structure)
- **Sovereign invariant link:** TD-I2 (Betti Conservation) - topological containment

**TOUCHING** (contact)
- **Compression role:** Contact relation preservation
- **Detection:** Contact prepositions, adjacency markers
- **Severity:** Low (often compressible)
- **Sovereign invariant link:** TD-I3 (Anti-Collision Bound) - contact constraint

---

### Category 14: Logical Concepts (4 primes)

**NOT** (negation)
- **Compression role:** Negation preservation
- **Detection:** Negation markers, logical operators
- **Severity:** Critical (logical structure)
- **Sovereign invariant link:** SC-I2 (Deterrence Consistency) - logical consistency

**MAYBE** (possibility)
- **Compression role:** Possibility preservation
- **Detection:** Modal markers, possibility operators
- **Severity:** Medium (epistemic modality)
- **Sovereign invariant link:** RG-I2 (Lawfulness Excess) - modal accounting

**CAN** (ability/possibility)
- **Compression role:** Ability preservation
- **Detection:** Ability modals, capability markers
- **Severity:** Medium (agentive capability)
- **Sovereign invariant link:** NA-I4 (Activation Bound) - capability constraint

**BECAUSE** (causation)
- **Compression role:** Causal relation preservation
- **Detection:** Causal connectives, explanation markers
- **Severity:** High (causal structure)
- **Sovereign invariant link:** Master Invariant (Coherence Conservation) - causal coherence

**IF** (conditionality)
- **Compression role:** Conditional relation preservation
- **Detection:** Conditional markers, hypothetical constructions
- **Severity:** High (logical structure)
- **Sovereign invariant link:** SC-I2 (Deterrence Consistency) - conditional logic

---

### Category 15: Augmentor and Similarity (2 primes)

**VERY** (intensification)
- **Compression role:** Intensification preservation
- **Detection:** Intensifiers, degree adverbs
- **Severity:** Low (often compressible)
- **Sovereign invariant link:** HW-I2 (Logarithmic Scaling) - intensity encoding

**LIKE** (similarity)
- **Compression role:** Similarity preservation
- **Detection:** Simile markers, comparison constructions
- **Severity:** Low (often compressible)
- **Sovereign invariant link:** RG-I3 (Observer Frame) - similarity reference

---

## Severity Weight Assignment

### Critical Invariants (severity = ∞)
- **THE SAME** (identity)
- **KNOW** (knowledge)
- **TRUE** (veridicality)
- **DIE** (mortality)
- **NOT** (negation)
- **BECAUSE** (causation)
- **IF** (conditionality)

**Rationale:** These represent fundamental logical, epistemic, or irreversible state changes. Breaking them would fundamentally alter meaning.

### High Severity (severity = 1.0)
- **KIND** (taxonomy)
- **PART** (mereology)
- **ALL** (universal quantification)
- **THINK** (cognition)
- **BE (SOMEWHERE)** (existential location)
- **THERE IS** (existence)
- **HAVE** (possession)
- **LIVE** (vitality)
- **WHEN/TIME** (temporal reference)
- **NOW** (present moment)
- **BEFORE** (prior time)
- **AFTER** (subsequent time)
- **WHERE/PLACE** (spatial reference)
- **HERE** (proximal location)
- **INSIDE** (containment)

**Rationale:** These represent important structural, ontological, or anchoring relationships that should be preserved with high priority.

### Medium Severity (severity = 0.5)
- **I** (self-reference)
- **YOU** (other-reference)
- **PEOPLE** (collective persons)
- **BODY** (physical body)
- **THIS** (deictic proximal)
- **OTHER** (contrast)
- **GOOD** (positive evaluation)
- **BAD** (negative evaluation)
- **THINK** (cognition)
- **WANT** (volition)
- **FEEL** (affect)
- **SAY** (speech act)
- **DO** (agentive action)
- **HAPPEN** (event occurrence)
- **BE (SOMEONE/SOMETHING)** (predication)
- **MAYBE** (possibility)
- **CAN** (ability)

**Rationale:** These represent important but not fundamental aspects of meaning. Some compression may be acceptable.

### Low Severity (severity = 0.1)
- **SOMEONE** (generic person)
- **SOMETHING** (generic entity)
- **ONE** (unit)
- **TWO** (pair)
- **SOME** (existential)
- **MUCH/MANY** (large quantity)
- **LITTLE/FEW** (small quantity)
- **BIG** (large magnitude)
- **SMALL** (small magnitude)
- **SEE** (visual perception)
- **HEAR** (auditory perception)
- **WORDS** (linguistic form)
- **MOVE** (movement)
- **A LONG TIME** (extended duration)
- **A SHORT TIME** (brief duration)
- **FOR SOME TIME** (duration)
- **MOMENT** (instant)
- **ABOVE** (superior position)
- **BELOW** (inferior position)
- **FAR** (distant)
- **NEAR** (proximate)
- **SIDE** (lateral)
- **TOUCHING** (contact)
- **VERY** (intensification)
- **LIKE** (similarity)

**Rationale:** These represent highly compressible aspects of meaning. Significant compression is acceptable.

---

## Integration with $L_{\text{inv}}$

### Expanded Invariant Load Equation

$$L_{\text{inv}}(x, \mathcal{I}_{\text{NSM}}) = \sum_{i \in \mathcal{I}_{\text{NSM}}} w_i \cdot \mathbb{1}[\text{broken}(i, x)] \cdot \text{severity}(i)$$

Where:
- $\mathcal{I}_{\text{NSM}}$: Set of 64 NSM semantic primes
- $w_i$: Context-dependent weight (e.g., higher for dialogue, lower for technical text)
- $\text{severity}(i)$: Severity weight from table above

### Context-Dependent Weighting

**Dialogue contexts:**
- Higher weight on I, YOU, SAY, THINK, WANT, FEEL
- Lower weight on spatial primes

**Technical contexts:**
- Higher weight on KNOW, TRUE, BECAUSE, IF, NOT
- Lower weight on affective primes

**Narrative contexts:**
- Higher weight on temporal and spatial primes
- Lower weight on logical operators

---

## Detection Methods

### Linguistic Detection
- **NLP parsing:** Dependency parsing for prime identification
- **Lexicon matching:** Prime exponent lexicons per language
- **Pattern matching:** Syntactic patterns for prime realization

### Statistical Detection
- **Distribution analysis:** Prime frequency distributions
- **Entropy analysis:** Prime information content
- **Correlation analysis:** Prime co-occurrence patterns

### Semantic Detection
- **Embedding analysis:** Prime semantic similarity
- **Coreference resolution:** Prime reference tracking
- **Sentiment analysis:** Affective prime detection

---

## Compression Strategies by Severity

### Critical Invariants (No Compression)
- **Strategy:** Preserve exactly
- **Technique:** Dictionary encoding, explicit preservation
- **Fallback:** Reject compression if critical invariant broken

### High Severity Invariants (Minimal Compression)
- **Strategy:** Preserve with minimal loss
- **Technique:** Lossless encoding, symbolic compression
- **Fallback:** Backtrack if high severity invariant broken

### Medium Severity Invariants (Controlled Compression)
- **Strategy:** Preserve with acceptable loss
- **Technique:** Lossy encoding with quality threshold
- **Fallback:** Adjust compression ratio to preserve invariants

### Low Severity Invariants (Aggressive Compression)
- **Strategy:** Compress aggressively
- **Technique:** Statistical compression, entropy coding
- **Fallback:** No special handling

---

## References

- Wierzbicka, A. & Goddard, C. (1994). Semantic and lexical universals.
- NSM Approach: https://nsm-approach.net/resources
- Research Stack, Invariant Root Analysis (invariant_root_analysis.md)
- Research Stack, Sovereign Invariant Analysis (sovereign_invariant_analysis.json)
- Research Stack, Cognitive Load Theory Invariant-Enhanced (09_Cognitive_Load_Theory_Invariant_Enhanced.md)
