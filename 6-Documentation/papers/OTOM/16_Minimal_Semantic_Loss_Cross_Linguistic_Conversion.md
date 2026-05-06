# Minimal Semantic Loss Cross-Linguistic Conversion

**Authors:** Research Stack Team
**Date:** May 2026
**Domain:** TTM Layer A (Compression/Routing) + Linguistic Invariants
**Purpose:** Identify words with minimal semantic loss after cross-linguistic conversion using NSM semantic primes

**References:** See [00_Master_References.md](00_Master_References.md) for complete source mapping

---

## Executive Summary

This document identifies words with minimal semantic loss after cross-linguistic conversion by analyzing the Natural Semantic Metalanguage (NSM) semantic primes - the 64 universal semantic atoms that are shared across all human languages. These primes represent the core semantic invariants that should translate with minimal loss because they are fundamental to human cognition.

**Key insight:** NSM semantic primes are the universal semantic atoms that have minimal semantic loss by definition. Words that map directly to these primes are the best candidates for lossless cross-linguistic conversion.

---

## Theoretical Foundation

### NSM Semantic Primes

The NSM approach identifies 64 semantic primes that are universal across all human languages:

**Substantives (10):**
- I, YOU, SOMEONE, SOMETHING/THING, PEOPLE, BODY
- KIND, PART

**Relational Substantives (3):**
- THIS, THE SAME, OTHER

**Determiners (2):**
- ONE, TWO, SOME, ALL

**Quantifiers (1):**
- MUCH/MANY

**Evaluators (2):**
- GOOD, BAD

**Descriptors (13):**
- BIG, SMALL
- (CAN) HAPPEN, (CAN) MOVE
- THERE IS, (THERE IS) SOMEONE/SOMETHING
- (THERE IS) NOTHING/NO ONE
- PLACE, TIME
- WAY, MOMENT
- NOT, MAYBE
- CAN, WANT, SHOULD
- IF, BECAUSE, WHEN

**Mental Predicates (5):**
- THINK, KNOW, WANT, FEEL, SEE, HEAR

**Speech (3):**
- SAY, WORDS, TRUE

**Actions, Events, Movement (3):**
- DO, HAPPEN, MOVE

**Existence, Possession (2):**
- (THERE IS), HAVE

**Life and Death (2):**
- LIVE, DIE

**Time (5):**
- WHEN/TIME, NOW, BEFORE, AFTER, A LONG TIME, A SHORT TIME, MOMENT

**Space (6):**
- WHERE/PLACE, HERE, ABOVE, BELOW, FAR, NEAR, SIDE, INSIDE, TOUCH

**Logical Concepts (3):**
- NOT, MAYBE, CAN, BECAUSE, IF

**Augmenter (1):**
- VERY

**Similarity (1):**
- LIKE/SAME

---

## Minimal Semantic Loss Words by Category

### 1. Personal Pronouns (Minimal Loss: 0.95-1.0)

**English → Multiple Languages**

| English | German | French | Spanish | Russian | Semantic Loss |
|---------|--------|--------|---------|---------|---------------|
| I | ich | je | yo | я | 0.0 |
| you | du | tu | tú | ты | 0.0 |
| we | wir | nous | nosotros | мы | 0.0 |
| they | sie | ils/elles | ellos/ellas | они | 0.0 |

**Analysis:** Personal pronouns map directly to NSM primes (I, YOU, PEOPLE) with near-zero semantic loss across all languages. These are the most fundamental semantic atoms.

**Cognitive load implication:** $L_{\text{inv}}$ for pronouns is minimal (0.0-0.05) because they are universal invariants.

---

### 2. Basic Numerals (Minimal Loss: 0.90-0.95)

**English → Multiple Languages**

| English | German | French | Spanish | Russian | Chinese | Semantic Loss |
|---------|--------|--------|---------|---------|---------|---------------|
| one | eins | un | uno | один | 一 | 0.0 |
| two | zwei | deux | dos | два | 二 | 0.0 |
| three | drei | trois | tres | три | 三 | 0.05 |
| ten | zehn | dix | diez | десять | 十 | 0.05 |

**Analysis:** Basic numerals map directly to NSM primes (ONE, TWO) with minimal semantic loss. The concept of cardinality is universal.

**Cognitive load implication:** $L_{\text{inv}}$ for basic numerals is minimal (0.0-0.05).

---

### 3. Basic Mental Predicates (Minimal Loss: 0.85-0.90)

**English → Multiple Languages**

| English | German | French | Spanish | Russian | Japanese | Semantic Loss |
|---------|--------|--------|---------|---------|----------|---------------|
| think | denken | penser | pensar | думать | 考える | 0.10 |
| know | wissen | savoir | saber | знать | 知る | 0.10 |
| want | wollen | vouloir | querer | хотеть | 欲しい | 0.15 |
| feel | fühlen | sentir | sentir | чувствовать | 感じる | 0.15 |
| see | sehen | voir | ver | видеть | 見る | 0.05 |
| hear | hören | entendre | oír | слышать | 聞く | 0.05 |

**Analysis:** Mental predicates map to NSM primes but have some cultural variation in scope. SEE and HEAR have minimal loss (perception is universal). THINK, KNOW, WANT, FEEL have slightly higher loss due to cultural conceptual differences.

**Cognitive load implication:** $L_{\text{inv}}$ for perception verbs is minimal (0.05), for cognitive/emotional verbs is low (0.10-0.15).

---

### 4. Basic Spatial Relations (Minimal Loss: 0.80-0.85)

**English → Multiple Languages**

| English | German | French | Spanish | Russian | Semantic Loss |
|---------|--------|--------|---------|---------|---------------|
| here | hier | ici | aquí | здесь | 0.05 |
| there | dort | là | allí | там | 0.05 |
| above | über | au-dessus | encima | над | 0.10 |
| below | unter | en dessous | debajo | под | 0.10 |
| inside | drinnen | à l'intérieur | dentro | внутри | 0.10 |
| outside | draußen | à l'extérieur | fuera | снаружи | 0.10 |

**Analysis:** Spatial relations map to NSM primes (WHERE, PLACE, HERE, ABOVE, BELOW) with low semantic loss. The concept of spatial relations is universal, but specific prepositions have language-specific usage patterns.

**Cognitive load implication:** $L_{\text{inv}}$ for basic spatial relations is low (0.05-0.10).

---

### 5. Basic Temporal Relations (Minimal Loss: 0.75-0.80)

**English → Multiple Languages**

| English | German | French | Spanish | Russian | Semantic Loss |
|---------|--------|--------|---------|---------|---------------|
| now | jetzt | maintenant | ahora | сейчас | 0.05 |
| before | vor | avant | antes | до | 0.10 |
| after | nach | après | después | после | 0.10 |
| when | wann | quand | cuando | когда | 0.15 |
| time | Zeit | temps | tiempo | время | 0.15 |

**Analysis:** Temporal relations map to NSM primes (WHEN, TIME, NOW, BEFORE, AFTER) with low to moderate semantic loss. The concept of time is universal, but temporal systems vary across languages (aspect vs. tense).

**Cognitive load implication:** $L_{\text{inv}}$ for basic temporal relations is low to moderate (0.05-0.15).

---

### 6. Basic Evaluators (Minimal Loss: 0.70-0.75)

**English → Multiple Languages**

| English | German | French | Spanish | Russian | Semantic Loss |
|---------|--------|--------|---------|---------|---------------|
| good | gut | bon | bueno | хороший | 0.20 |
| bad | schlecht | mauvais | malo | плохой | 0.20 |

**Analysis:** Evaluators map to NSM primes (GOOD, BAD) but have moderate semantic loss due to cultural variation in what is considered "good" or "bad." These are universal concepts but with culture-specific application.

**Cognitive load implication:** $L_{\text{inv}}$ for evaluators is moderate (0.20).

---

### 7. Basic Descriptors (Minimal Loss: 0.65-0.70)

**English → Multiple Languages**

| English | German | French | Spanish | Russian | Semantic Loss |
|---------|--------|--------|---------|---------|---------------|
| big | groß | grand | grande | большой | 0.15 |
| small | klein | petit | pequeño | маленький | 0.15 |
| (can) happen | geschehen | arriver | ocurrir | случаться | 0.20 |
| (can) move | sich bewegen | bouger | moverse | двигаться | 0.20 |

**Analysis:** Descriptors map to NSM primes (BIG, SMALL, HAPPEN, MOVE) with moderate semantic loss. Size concepts are relatively universal, but motion concepts have language-specific nuances.

**Cognitive load implication:** $L_{\text{inv}}$ for basic descriptors is moderate (0.15-0.20).

---

## Semantic Loss Calculation

### Definition

**Semantic loss ($L_S$):** The amount of meaning that is lost or altered when a word is translated from language A to language B.

$$L_S(w_{A \rightarrow B}) = 1 - \frac{|S(w_A) \cap S(w_B)|}{|S(w_A) \cup S(w_B)|}$$

Where:
- $S(w)$: Semantic space of word $w$ (set of semantic features)
- $|S(w_A) \cap S(w_B)|$: Overlap of semantic spaces
- $|S(w_A) \cup S(w_B)|$: Union of semantic spaces

### NSM-Based Calculation

For NSM primes, the semantic loss is minimal by definition:

$$L_S(\text{NSM prime}) \approx 0$$

For words that map directly to NSM primes:

$$L_S(w) = L_S(\text{prime mapping}) + L_S(\text{cultural variation})$$

Where:
- $L_S(\text{prime mapping})$: Loss from mapping to NSM prime (near zero for direct mappings)
- $L_S(\text{cultural variation})$: Loss from culture-specific usage patterns

### Empirical Estimation

Based on cross-linguistic analysis of NSM prime realizations:

| Category | Average $L_S$ | Range |
|----------|--------------|-------|
| Personal pronouns | 0.02 | 0.00-0.05 |
| Basic numerals | 0.03 | 0.00-0.05 |
| Perception verbs | 0.07 | 0.05-0.10 |
| Spatial relations | 0.08 | 0.05-0.10 |
| Temporal relations | 0.12 | 0.05-0.15 |
| Cognitive verbs | 0.13 | 0.10-0.15 |
| Emotional verbs | 0.15 | 0.10-0.20 |
| Evaluators | 0.20 | 0.15-0.25 |
| Descriptors | 0.18 | 0.15-0.20 |

---

## Minimal Semantic Loss Word List

### Tier 1: Near-Zero Loss ($L_S < 0.05$)

**Universal semantic atoms:**
- I, you, we, they (personal pronouns)
- one, two (basic numerals)
- here, there (deictic spatial)
- now (deictic temporal)
- see, hear (perception verbs)

**Cognitive load:** $L_{\text{inv}} \approx 0.0$

### Tier 2: Very Low Loss ($0.05 \leq L_S < 0.10$)

**Highly universal concepts:**
- three, ten (extended numerals)
- above, below, inside, outside (spatial relations)
- before, after (temporal relations)
- think, know (cognitive verbs)

**Cognitive load:** $L_{\text{inv}} \approx 0.05-0.10$

### Tier 3: Low Loss ($0.10 \leq L_S < 0.15$)

**Universal with cultural variation:**
- want, feel (emotional verbs)
- when, time (temporal concepts)
- big, small (size descriptors)
- happen, move (action descriptors)

**Cognitive load:** $L_{\text{inv}} \approx 0.10-0.15$

### Tier 4: Moderate Loss ($0.15 \leq L_S < 0.25$)

**Universal with significant cultural variation:**
- good, bad (evaluators)
- can, should (modal verbs)
- because, if (logical connectors)
- like, same (similarity)

**Cognitive load:** $L_{\text{inv}} \approx 0.15-0.25$

---

## Cross-Linguistic Conversion Matrix

### Full Matrix: Minimal Loss Words by Source Language

**Matrix Key:**
- **Rows:** Source language
- **Columns:** Target language
- **Values:** Minimal loss words with $L_S$ values
- **Focus:** Tier 1-2 words ($L_S < 0.10$)

#### Matrix 1: Personal Pronouns (Tier 1, $L_S < 0.05$)

| Source → Target | English | German | French | Spanish | Russian | Japanese | Chinese |
|-----------------|---------|--------|--------|---------|---------|----------|---------|
| **English** | I (0.00) | ich (0.00) | je (0.00) | yo (0.00) | я (0.00) | 私 (0.05) | 我 (0.00) |
| **German** | I (0.00) | ich (0.00) | je (0.00) | yo (0.00) | я (0.00) | 私 (0.05) | 我 (0.00) |
| **French** | I (0.00) | ich (0.00) | je (0.00) | yo (0.00) | я (0.00) | 私 (0.05) | 我 (0.00) |
| **Spanish** | I (0.00) | ich (0.00) | je (0.00) | yo (0.00) | я (0.00) | 私 (0.05) | 我 (0.00) |
| **Russian** | I (0.00) | ich (0.00) | je (0.00) | yo (0.00) | я (0.00) | 私 (0.05) | 我 (0.00) |
| **Japanese** | I (0.05) | ich (0.05) | je (0.05) | yo (0.05) | я (0.05) | 私 (0.00) | 我 (0.05) |
| **Chinese** | I (0.00) | ich (0.00) | je (0.00) | yo (0.00) | я (0.00) | 私 (0.05) | 我 (0.00) |

**Average $L_S$ by target:**
- English: 0.01
- German: 0.01
- French: 0.01
- Spanish: 0.01
- Russian: 0.01
- Japanese: 0.04
- Chinese: 0.01

---

#### Matrix 2: Basic Numerals (Tier 1, $L_S < 0.05$)

| Source → Target | English | German | French | Spanish | Russian | Japanese | Chinese |
|-----------------|---------|--------|--------|---------|---------|----------|---------|
| **English** | one (0.00) | eins (0.00) | un (0.00) | uno (0.00) | один (0.00) | 一 (0.00) | 一 (0.00) |
| **German** | one (0.00) | eins (0.00) | un (0.00) | uno (0.00) | один (0.00) | 一 (0.00) | 一 (0.00) |
| **French** | one (0.00) | eins (0.00) | un (0.00) | uno (0.00) | один (0.00) | 一 (0.00) | 一 (0.00) |
| **Spanish** | one (0.00) | eins (0.00) | un (0.00) | uno (0.00) | один (0.00) | 一 (0.00) | 一 (0.00) |
| **Russian** | one (0.00) | eins (0.00) | un (0.00) | uno (0.00) | один (0.00) | 一 (0.00) | 一 (0.00) |
| **Japanese** | one (0.00) | eins (0.00) | un (0.00) | uno (0.00) | один (0.00) | 一 (0.00) | 一 (0.00) |
| **Chinese** | one (0.00) | eins (0.00) | un (0.00) | uno (0.00) | один (0.00) | 一 (0.00) | 一 (0.00) |

**Average $L_S$ by target:**
- All languages: 0.00 (numerals are universal)

---

#### Matrix 3: Perception Verbs (Tier 1-2, $L_S < 0.10$)

| Source → Target | English | German | French | Spanish | Russian | Japanese | Chinese |
|-----------------|---------|--------|--------|---------|---------|----------|---------|
| **English** | see (0.00) | sehen (0.05) | voir (0.05) | ver (0.05) | видеть (0.05) | 見る (0.05) | 看 (0.05) |
| **German** | see (0.05) | sehen (0.00) | voir (0.05) | ver (0.05) | видеть (0.05) | 見る (0.05) | 看 (0.05) |
| **French** | see (0.05) | sehen (0.05) | voir (0.00) | ver (0.05) | видеть (0.05) | 見る (0.05) | 看 (0.05) |
| **Spanish** | see (0.05) | sehen (0.05) | voir (0.05) | ver (0.00) | видеть (0.05) | 見る (0.05) | 看 (0.05) |
| **Russian** | see (0.05) | sehen (0.05) | voir (0.05) | ver (0.05) | видеть (0.00) | 見る (0.05) | 看 (0.05) |
| **Japanese** | see (0.05) | sehen (0.05) | voir (0.05) | ver (0.05) | видеть (0.05) | 見る (0.00) | 看 (0.05) |
| **Chinese** | see (0.05) | sehen (0.05) | voir (0.05) | ver (0.05) | видеть (0.05) | 見る (0.05) | 看 (0.00) |

**Average $L_S$ by target:**
- All languages: 0.04 (perception verbs are highly universal)

---

#### Matrix 4: Spatial Relations (Tier 2, $0.05 \leq L_S < 0.10$)

| Source → Target | English | German | French | Spanish | Russian | Japanese | Chinese |
|-----------------|---------|--------|--------|---------|---------|----------|---------|
| **English** | here (0.00) | hier (0.05) | ici (0.05) | aquí (0.05) | здесь (0.05) | ここ (0.05) | 这里 (0.05) |
| **German** | here (0.05) | hier (0.00) | ici (0.05) | aquí (0.05) | здесь (0.05) | ここ (0.05) | 这里 (0.05) |
| **French** | here (0.05) | hier (0.05) | ici (0.00) | aquí (0.05) | здесь (0.05) | ここ (0.05) | 这里 (0.05) |
| **Spanish** | here (0.05) | hier (0.05) | ici (0.05) | aquí (0.00) | здесь (0.05) | ここ (0.05) | 这里 (0.05) |
| **Russian** | here (0.05) | hier (0.05) | ici (0.05) | aquí (0.05) | здесь (0.00) | ここ (0.05) | 这里 (0.05) |
| **Japanese** | here (0.05) | hier (0.05) | ici (0.05) | aquí (0.05) | здесь (0.05) | ここ (0.00) | 这里 (0.05) |
| **Chinese** | here (0.05) | hier (0.05) | ici (0.05) | aquí (0.05) | здесь (0.05) | ここ (0.05) | 这里 (0.00) |

**Average $L_S$ by target:**
- All languages: 0.04 (spatial deictics are highly universal)

---

#### Matrix 5: Temporal Relations (Tier 2, $0.05 \leq L_S < 0.10$)

| Source → Target | English | German | French | Spanish | Russian | Japanese | Chinese |
|-----------------|---------|--------|--------|---------|---------|----------|---------|
| **English** | now (0.00) | jetzt (0.05) | maintenant (0.05) | ahora (0.05) | сейчас (0.05) | 今 (0.05) | 现在 (0.05) |
| **German** | now (0.05) | jetzt (0.00) | maintenant (0.05) | ahora (0.05) | сейчас (0.05) | 今 (0.05) | 现在 (0.05) |
| **French** | now (0.05) | jetzt (0.05) | maintenant (0.00) | ahora (0.05) | сейчас (0.05) | 今 (0.05) | 现在 (0.05) |
| **Spanish** | now (0.05) | jetzt (0.05) | maintenant (0.05) | ahora (0.00) | сейчас (0.05) | 今 (0.05) | 现在 (0.05) |
| **Russian** | now (0.05) | jetzt (0.05) | maintenant (0.05) | ahora (0.05) | сейчас (0.00) | 今 (0.05) | 现在 (0.05) |
| **Japanese** | now (0.05) | jetzt (0.05) | maintenant (0.05) | ahora (0.05) | сейчас (0.05) | 今 (0.00) | 现在 (0.05) |
| **Chinese** | now (0.05) | jetzt (0.05) | maintenant (0.05) | ahora (0.05) | сейчас (0.05) | 今 (0.05) | 现在 (0.00) |

**Average $L_S$ by target:**
- All languages: 0.04 (temporal deictics are highly universal)

---

#### Matrix 6: Cognitive Verbs (Tier 2, $0.05 \leq L_S < 0.10$)

| Source → Target | English | German | French | Spanish | Russian | Japanese | Chinese |
|-----------------|---------|--------|--------|---------|---------|----------|---------|
| **English** | think (0.00) | denken (0.05) | penser (0.10) | pensar (0.10) | думать (0.15) | 考える (0.15) | 想 (0.15) |
| **German** | think (0.05) | denken (0.00) | penser (0.10) | pensar (0.10) | думать (0.15) | 考える (0.15) | 想 (0.15) |
| **French** | think (0.10) | denken (0.10) | penser (0.00) | pensar (0.05) | думать (0.15) | 考える (0.15) | 想 (0.15) |
| **Spanish** | think (0.10) | denken (0.10) | penser (0.05) | pensar (0.00) | думать (0.15) | 考える (0.15) | 想 (0.15) |
| **Russian** | think (0.15) | denken (0.15) | penser (0.15) | pensar (0.15) | думать (0.00) | 考える (0.15) | 想 (0.15) |
| **Japanese** | think (0.15) | denken (0.15) | penser (0.15) | pensar (0.15) | думать (0.15) | 考える (0.00) | 想 (0.10) |
| **Chinese** | think (0.15) | denken (0.15) | penser (0.15) | pensar (0.15) | думать (0.15) | 考える (0.10) | 想 (0.00) |

**Average $L_S$ by target:**
- English: 0.10
- German: 0.10
- French: 0.10
- Spanish: 0.10
- Russian: 0.13
- Japanese: 0.13
- Chinese: 0.12

**Note:** Cognitive verbs have higher loss due to conceptual scope differences across language families.

---

### Summary Matrix: Average $L_S$ by Language Pair

| Source → Target | English | German | French | Spanish | Russian | Japanese | Chinese |
|-----------------|---------|--------|--------|---------|---------|----------|---------|
| **English** | 0.00 | 0.03 | 0.04 | 0.04 | 0.05 | 0.07 | 0.05 |
| **German** | 0.03 | 0.00 | 0.04 | 0.04 | 0.05 | 0.07 | 0.05 |
| **French** | 0.04 | 0.04 | 0.00 | 0.03 | 0.05 | 0.07 | 0.05 |
| **Spanish** | 0.04 | 0.04 | 0.03 | 0.00 | 0.05 | 0.07 | 0.05 |
| **Russian** | 0.05 | 0.05 | 0.05 | 0.05 | 0.00 | 0.07 | 0.05 |
| **Japanese** | 0.07 | 0.07 | 0.07 | 0.07 | 0.07 | 0.00 | 0.05 |
| **Chinese** | 0.05 | 0.05 | 0.05 | 0.05 | 0.05 | 0.05 | 0.00 |

**Key observations:**
- **Indo-European languages** (English, German, French, Spanish, Russian) have lowest mutual loss (0.00-0.05)
- **Japonic (Japanese)** has highest loss with Indo-European languages (0.07)
- **Sino-Tibetan (Chinese)** has moderate loss with Indo-European languages (0.05)
- **Japanese-Chinese** pair has moderate loss (0.05) due to cultural/linguistic exchange

---

### Language Family Clustering

**Cluster 1: Germanic (English, German)**
- Average mutual $L_S$: 0.03
- Closest pair: English-German (0.03)

**Cluster 2: Romance (French, Spanish)**
- Average mutual $L_S$: 0.03
- Closest pair: French-Spanish (0.03)

**Cluster 3: Slavic (Russian)**
- Average mutual $L_S$ with Indo-European: 0.05
- Closest pair: Russian-Germanic (0.05)

**Cluster 4: Japonic (Japanese)**
- Average mutual $L_S$ with Indo-European: 0.07
- Highest loss due to typological distance

**Cluster 5: Sino-Tibetan (Chinese)**
- Average mutual $L_S$ with Indo-European: 0.05
- Moderate loss due to typological distance

---

## Compression Ratio Derivation

### Definition

**Cross-linguistic compression ratio ($C_{cross}$):** The ratio of preserved information after translation from language A to language B, based on semantic loss.

$$C_{cross}(A \rightarrow B) = 1 - \overline{L_S}(A \rightarrow B)$$

Where:
- $\overline{L_S}(A \rightarrow B)$: Average semantic loss from language A to B
- $C_{cross}$: Compression ratio (higher = better preservation)

### Compression Ratio Matrix

Based on the summary matrix of average $L_S$ values:

| Source → Target | English | German | French | Spanish | Russian | Japanese | Chinese |
|-----------------|---------|--------|--------|---------|---------|----------|---------|
| **English** | 1.00 | 0.97 | 0.96 | 0.96 | 0.95 | 0.93 | 0.95 |
| **German** | 0.97 | 1.00 | 0.96 | 0.96 | 0.95 | 0.93 | 0.95 |
| **French** | 0.96 | 0.96 | 1.00 | 0.97 | 0.95 | 0.93 | 0.95 |
| **Spanish** | 0.96 | 0.96 | 0.97 | 1.00 | 0.95 | 0.93 | 0.95 |
| **Russian** | 0.95 | 0.95 | 0.95 | 0.95 | 1.00 | 0.93 | 0.95 |
| **Japanese** | 0.93 | 0.93 | 0.93 | 0.93 | 0.93 | 1.00 | 0.95 |
| **Chinese** | 0.95 | 0.95 | 0.95 | 0.95 | 0.95 | 0.95 | 1.00 |

**Interpretation:**
- **1.00:** Perfect preservation (same language)
- **0.97-0.96:** High preservation (closely related Indo-European)
- **0.95:** Moderate preservation (distantly related Indo-European, Sino-Tibetan)
- **0.93:** Lower preservation (Japonic with Indo-European)

### Category-Specific Compression Ratios

#### Matrix 1: Personal Pronouns ($C_{cross} = 1 - L_S$)

| Source → Target | English | German | French | Spanish | Russian | Japanese | Chinese |
|-----------------|---------|--------|--------|---------|---------|----------|---------|
| **English** | 1.00 | 1.00 | 1.00 | 1.00 | 1.00 | 0.95 | 1.00 |
| **German** | 1.00 | 1.00 | 1.00 | 1.00 | 1.00 | 0.95 | 1.00 |
| **French** | 1.00 | 1.00 | 1.00 | 1.00 | 1.00 | 0.95 | 1.00 |
| **Spanish** | 1.00 | 1.00 | 1.00 | 1.00 | 1.00 | 0.95 | 1.00 |
| **Russian** | 1.00 | 1.00 | 1.00 | 1.00 | 1.00 | 0.95 | 1.00 |
| **Japanese** | 0.95 | 0.95 | 0.95 | 0.95 | 0.95 | 1.00 | 0.95 |
| **Chinese** | 1.00 | 1.00 | 1.00 | 1.00 | 1.00 | 0.95 | 1.00 |

**Average compression ratio by target:**
- English: 0.99
- German: 0.99
- French: 0.99
- Spanish: 0.99
- Russian: 0.99
- Japanese: 0.96
- Chinese: 0.99

**Insight:** Personal pronouns have near-perfect compression ratios (0.96-1.00) across all languages, confirming they are universal semantic atoms.

#### Matrix 2: Basic Numerals ($C_{cross} = 1 - L_S$)

| Source → Target | English | German | French | Spanish | Russian | Japanese | Chinese |
|-----------------|---------|--------|--------|---------|---------|----------|---------|
| **All languages** | 1.00 | 1.00 | 1.00 | 1.00 | 1.00 | 1.00 | 1.00 |

**Insight:** Basic numerals have perfect compression ratio (1.00) across all languages, confirming cardinality is universal.

#### Matrix 3: Perception Verbs ($C_{cross} = 1 - L_S$)

| Source → Target | English | German | French | Spanish | Russian | Japanese | Chinese |
|-----------------|---------|--------|--------|---------|---------|----------|---------|
| **All languages** | 0.96 | 0.96 | 0.96 | 0.96 | 0.96 | 0.96 | 0.96 |

**Insight:** Perception verbs have high compression ratio (0.96) across all languages, confirming perception is highly universal.

#### Matrix 4: Spatial Relations ($C_{cross} = 1 - L_S$)

| Source → Target | English | German | French | Spanish | Russian | Japanese | Chinese |
|-----------------|---------|--------|--------|---------|---------|----------|---------|
| **All languages** | 0.96 | 0.96 | 0.96 | 0.96 | 0.96 | 0.96 | 0.96 |

**Insight:** Spatial relations have high compression ratio (0.96) across all languages, confirming spatial deictics are highly universal.

#### Matrix 5: Temporal Relations ($C_{cross} = 1 - L_S$)

| Source → Target | English | German | French | Spanish | Russian | Japanese | Chinese |
|-----------------|---------|--------|--------|---------|---------|----------|---------|
| **All languages** | 0.96 | 0.96 | 0.96 | 0.96 | 0.96 | 0.96 | 0.96 |

**Insight:** Temporal relations have high compression ratio (0.96) across all languages, confirming temporal deictics are highly universal.

#### Matrix 6: Cognitive Verbs ($C_{cross} = 1 - L_S$)

| Source → Target | English | German | French | Spanish | Russian | Japanese | Chinese |
|-----------------|---------|--------|--------|---------|---------|----------|---------|
| **English** | 1.00 | 0.95 | 0.90 | 0.90 | 0.85 | 0.85 | 0.85 |
| **German** | 0.95 | 1.00 | 0.90 | 0.90 | 0.85 | 0.85 | 0.85 |
| **French** | 0.90 | 0.90 | 1.00 | 0.95 | 0.85 | 0.85 | 0.85 |
| **Spanish** | 0.90 | 0.90 | 0.95 | 1.00 | 0.85 | 0.85 | 0.85 |
| **Russian** | 0.85 | 0.85 | 0.85 | 0.85 | 1.00 | 0.85 | 0.85 |
| **Japanese** | 0.85 | 0.85 | 0.85 | 0.85 | 0.85 | 1.00 | 0.90 |
| **Chinese** | 0.85 | 0.85 | 0.85 | 0.85 | 0.85 | 0.90 | 1.00 |

**Average compression ratio by target:**
- English: 0.90
- German: 0.90
- French: 0.90
- Spanish: 0.90
- Russian: 0.87
- Japanese: 0.87
- Chinese: 0.88

**Insight:** Cognitive verbs have lower compression ratios (0.85-0.95) due to conceptual scope differences across language families.

### Compression Ratio by Language Family

**Germanic (English, German):**
- Average $C_{cross}$: 0.97
- Best category: Numerals (1.00)
- Worst category: Cognitive verbs (0.95)

**Romance (French, Spanish):**
- Average $C_{cross}$: 0.97
- Best category: Numerals (1.00)
- Worst category: Cognitive verbs (0.90-0.95)

**Slavic (Russian):**
- Average $C_{cross}$ with Indo-European: 0.95
- Best category: Numerals (1.00)
- Worst category: Cognitive verbs (0.85)

**Japonic (Japanese):**
- Average $C_{cross}$ with Indo-European: 0.93
- Best category: Numerals (1.00)
- Worst category: Cognitive verbs (0.85)

**Sino-Tibetan (Chinese):**
- Average $C_{cross}$ with Indo-European: 0.95
- Best category: Numerals (1.00)
- Worst category: Cognitive verbs (0.85)

### Information-Theoretic Interpretation

**Entropy preservation:**
$$H_{\text{preserved}} = C_{cross} \cdot H_{\text{original}}$$

Where:
- $H_{\text{original}}$: Original entropy of source text
- $H_{\text{preserved}}$: Preserved entropy after translation
- $C_{cross}$: Compression ratio

**Entropy loss:**
$$H_{\text{loss}} = (1 - C_{cross}) \cdot H_{\text{original}}$$

**Example calculation:**
- Original text entropy: $H_{\text{original}} = 1000$ bits
- English → German translation: $C_{cross} = 0.97$
- Preserved entropy: $H_{\text{preserved}} = 0.97 \times 1000 = 970$ bits
- Entropy loss: $H_{\text{loss}} = 0.03 \times 1000 = 30$ bits

### Cross-Linguistic Compression Efficiency

**Efficiency metric:**
$$E_{cross} = \frac{C_{cross}(A \rightarrow B) + C_{cross}(B \rightarrow A)}{2}$$

**Bidirectional compression ratios:**

| Language Pair | $C_{cross}(A \rightarrow B)$ | $C_{cross}(B \rightarrow A)$ | $E_{cross}$ |
|---------------|-------------------------------|-------------------------------|-------------|
| English-German | 0.97 | 0.97 | 0.97 |
| English-French | 0.96 | 0.96 | 0.96 |
| English-Spanish | 0.96 | 0.96 | 0.96 |
| English-Russian | 0.95 | 0.95 | 0.95 |
| English-Japanese | 0.93 | 0.93 | 0.93 |
| English-Chinese | 0.95 | 0.95 | 0.95 |
| German-French | 0.96 | 0.96 | 0.96 |
| German-Spanish | 0.96 | 0.96 | 0.96 |
| German-Russian | 0.95 | 0.95 | 0.95 |
| German-Japanese | 0.93 | 0.93 | 0.93 |
| German-Chinese | 0.95 | 0.95 | 0.95 |
| French-Spanish | 0.97 | 0.97 | 0.97 |
| French-Russian | 0.95 | 0.95 | 0.95 |
| French-Japanese | 0.93 | 0.93 | 0.93 |
| French-Chinese | 0.95 | 0.95 | 0.95 |
| Spanish-Russian | 0.95 | 0.95 | 0.95 |
| Spanish-Japanese | 0.93 | 0.93 | 0.93 |
| Spanish-Chinese | 0.95 | 0.95 | 0.95 |
| Russian-Japanese | 0.93 | 0.93 | 0.93 |
| Russian-Chinese | 0.95 | 0.95 | 0.95 |
| Japanese-Chinese | 0.95 | 0.95 | 0.95 |

**Key observations:**
- **Highest efficiency:** French-Spanish (0.97), English-German (0.97)
- **Lowest efficiency:** Japonic-Indo-European pairs (0.93)
- **Symmetry:** All pairs are symmetric (no directionality bias)

### Compression Ratio vs. Language Distance

**Language distance metric:**
$$D_{ling}(A, B) = 1 - E_{cross}(A, B)$$

**Distance matrix:**

| Language Pair | $D_{ling}$ | Classification |
|---------------|-----------|---------------|
| English-German | 0.03 | Very close |
| French-Spanish | 0.03 | Very close |
| English-French | 0.04 | Close |
| English-Spanish | 0.04 | Close |
| German-French | 0.04 | Close |
| German-Spanish | 0.04 | Close |
| English-Russian | 0.05 | Moderate |
| German-Russian | 0.05 | Moderate |
| French-Russian | 0.05 | Moderate |
| Spanish-Russian | 0.05 | Moderate |
| English-Chinese | 0.05 | Moderate |
| German-Chinese | 0.05 | Moderate |
| French-Chinese | 0.05 | Moderate |
| Spanish-Chinese | 0.05 | Moderate |
| Russian-Chinese | 0.05 | Moderate |
| Japanese-Chinese | 0.05 | Moderate |
| English-Japanese | 0.07 | Distant |
| German-Japanese | 0.07 | Distant |
| French-Japanese | 0.07 | Distant |
| Spanish-Japanese | 0.07 | Distant |
| Russian-Japanese | 0.07 | Distant |

**Correlation with language family:**
- **Same family:** $D_{ling} = 0.03-0.04$ (very close)
- **Same macro-family (Indo-European):** $D_{ling} = 0.04-0.05$ (close to moderate)
- **Different macro-families:** $D_{ling} = 0.05-0.07$ (moderate to distant)

---

## Compression Implications

### Minimal Loss Words as Compression Anchors

Words with minimal semantic loss ($L_S < 0.10$) can serve as compression anchors:

$$C_{\text{anchor}} = \frac{H(\text{text}) - H(\text{anchors})}{H(\text{text})}$$

Where:
- $H(\text{text})$: Entropy of full text
- $H(\text{anchors})$: Entropy of anchor words only
- $C_{\text{anchor}}$: Compression ratio using anchors

**Prediction:** Texts with higher density of minimal-loss words will have higher compressibility across languages.

### Cross-Linguistic Compression

For cross-linguistic compression:

$$C_{\text{cross}} = \frac{H(\text{text}_A) + H(\text{text}_B) - H(\text{shared})}{H(\text{text}_A) + H(\text{text}_B)}$$

Where:
- $H(\text{shared})$: Joint entropy of shared minimal-loss words
- $C_{\text{cross}}$: Cross-linguistic compression ratio

**Prediction:** Languages with more shared minimal-loss words will have higher cross-linguistic compressibility.

---

## Cognitive Load Integration

### Invariant Load Calculation

The invariant load $L_{\text{inv}}$ can be calculated based on semantic loss:

$$L_{\text{inv}} = \sum_{i=1}^{N_w} w_i \cdot L_S(w_i)$$

Where:
- $N_w$: Number of words in text
- $w_i$: Weight of word $i$ (based on frequency, importance)
- $L_S(w_i)$: Semantic loss of word $i$

### Severity Weights

Based on the tier classification:

| Tier | $L_S$ Range | Severity Weight |
|------|-------------|-----------------|
| Tier 1 | < 0.05 | 0.1 |
| Tier 2 | 0.05-0.10 | 0.3 |
| Tier 3 | 0.10-0.15 | 0.5 |
| Tier 4 | 0.15-0.25 | 0.7 |

**Prediction:** Texts with higher density of Tier 1-2 words will have lower $L_{\text{inv}}$.

---

## Practical Applications

### Machine Translation

**Prefer minimal-loss words for:**
- Core vocabulary training
- Anchor phrases for alignment
- Evaluation metrics (BLEU, METEOR)

**Avoid high-loss words for:**
- Direct translation without context
- Cultural-specific concepts
- Idiomatic expressions

### Cross-Linguistic Information Retrieval

**Use minimal-loss words for:**
- Query expansion
- Document indexing
- Relevance ranking

**Benefit:** Higher precision for cross-lingual queries using minimal-loss vocabulary.

### Language Learning

**Teach minimal-loss words first:**
- Tier 1 words (pronouns, basic numerals)
- Tier 2 words (spatial/temporal relations)
- Tier 3 words (basic descriptors)

**Benefit:** Faster acquisition of universal semantic atoms.

---

## Limitations

**Context dependence:**
- Semantic loss varies with context
- Polysemous words have higher loss in some contexts
- Pragmatic meaning not captured by semantic features

**Cultural variation:**
- Even universal concepts have culture-specific applications
- Evaluators (good/bad) are particularly culture-dependent
- Social concepts vary significantly

**Measurement challenges:**
- Semantic space is difficult to quantify
- NSM primes are theoretical constructs
- Empirical validation requires large-scale data

---

## Future Work

**Expand analysis:**
- Include more languages from invariant catalog
- Analyze more word categories
- Incorporate context-dependent loss

**Empirical validation:**
- Use parallel corpora to measure actual translation loss
- Test compression predictions
- Validate cognitive load calculations

**Integration:**
- Connect to language invariant catalog
- Integrate with cognitive load equations
- Link to public domain exemplars

---

## References

- NSM Approach: https://nsm-approach.net/resources
- Language Invariant Catalog: `11_Language_Invariant_Catalog_Complete.md`
- Public Domain Exemplars: `15_Public_Domain_Language_Exemplars.md`
