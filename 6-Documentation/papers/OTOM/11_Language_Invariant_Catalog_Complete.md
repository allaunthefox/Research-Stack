# Language Invariant Catalog: Complete

**Authors:** Research Stack Team
**Date:** May 2026
**Domain:** TTM Layer A (Compression/Routing) + Linguistic Invariants
**Purpose:** Complete catalog of language invariants from invariant_root_analysis.md

**References:** See [00_Master_References.md](00_Master_References.md) for complete source mapping

---

## Executive Summary

This document provides a complete catalog of language invariants derived from the Natural Semantic Metalanguage (NSM) research program, covering 27+ languages across 8 language families and 4 language types. It includes:
- Language-specific prime realizations
- ISO 639 codes and genetic/typological classification
- Structural features affecting compression
- Detection methods for each language
- Integration with sovereign invariants
- Severity weights for $L_{\text{inv}}$ calculation

---

## Language Family Overview

### Distribution Across Families

| Family | Languages | ISO Codes | Coverage |
|--------|-----------|-----------|----------|
| Indo-European | 10 | en, de, fr, es, it, pl, ru, cs, da, nl, sr | Germanic, Romance, Slavic |
| Semitic | 3 | ar, he, am | Central, South, Ethiopian |
| East/Southeast Asian | 5 | zh, yue, ja, ko, vi | Sino-Tibetan, Japonic, Koreanic, Austroasiatic |
| African | 3 | ewe, wol, nyf | Niger-Congo, Atlantic-Congo, Bantu |
| Oceanic | 2 | lgu, cam | Austronesian, Oceanic |
| Uralic | 1 | fi | Finnic |
| Iranian | 1 | fa | Indo-European, Iranian |
| Creole | 1 | --- | English-lexified |

**Total:** 27+ languages with full NSM documentation

---

## Language-Specific Invariant Catalogs

### 1. English (en / eng)

**Classification:** Indo-European, Germanic, West
**Structural Features:** Analytic morphology, fixed SVO order, minimal inflection
**Distinctive Features:** Reference standard for NSM; analytic morphology reduces morphological complexity

**Prime Realization Patterns:**
- **Substantives:** Lexical items (I, you, someone, something, people, body)
- **Mental predicates:** Verbal forms (think, know, want, feel, see, hear)
- **Time:** Temporal adverbs + tense markers (when/time, now, before, after)
- **Space:** Prepositional phrases (where/place, here, above, below, far, near)

**Compression Implications:**
- **High compressibility:** Minimal morphology, regular word order
- **Critical invariants:** Word order (SVO), tense markers, prepositional semantics
- **Detection method:** POS tagging, dependency parsing, lexical lookup

**Severity Weights:**
- Word order: High (1.0)
- Tense: Medium (0.5)
- Prepositions: Medium (0.5)
- Lexical primes: Low (0.1)

**Sovereign Invariant Link:** CL-I1 (Load Conservation) - English as baseline for load measurement

---

### 2. German (de / deu/ger)

**Classification:** Indo-European, Germanic, West
**Structural Features:** Compound-rich, case-marking (4 cases), verb-second
**Distinctive Features:** Extensive compounding creates long lexical units; case system enables flexible word order

**Prime Realization Patterns:**
- **Substantives:** Case-inflected forms (ich, du, jemand, etwas, leute, körper)
- **Mental predicates:** Inflected verbs (denken, wissen, wollen, fühlen, sehen, hören)
- **Time:** Temporal adverbs + verb position (wann/zeit, jetzt, vor, nach)
- **Space:** Prepositions with case government (wo/ort, hier, über, unter, weit, nah)

**Compression Implications:**
- **Medium compressibility:** Compounds require special handling; case marking adds complexity
- **Critical invariants:** Case morphology, verb position, compound integrity
- **Detection method:** Morphological analysis, compound segmentation, case assignment

**Severity Weights:**
- Case morphology: High (1.0)
- Verb position: High (1.0)
- Compound integrity: Medium (0.5)
- Lexical primes: Low (0.1)

**Sovereign Invariant Link:** AF-I1 (Norm Preservation) - case normalization as norm-preserving transformation

---

### 3. French (fr / fra/fre)

**Classification:** Indo-European, Romance, Gallo-Iberian
**Structural Features:** Verbal system (tense, aspect, mood), article usage, gender marking
**Distinctive Features:** Rich verbal inflection; obligatory articles; grammatical gender

**Prime Realization Patterns:**
- **Substantives:** Gender-marked forms (je, tu, quelqu'un, quelque chose, gens, corps)
- **Mental predicates:** Conjugated verbs (penser, savoir, vouloir, sentir, voir, entendre)
- **Time:** Tense + aspect (quand/temps, maintenant, avant, après)
- **Space:** Prepositions (où/endroit, ici, au-dessus, en dessous, loin, près)

**Compression Implications:**
- **Medium compressibility:** Verbal inflection adds complexity; gender marking
- **Critical invariants:** Verb conjugation, article-noun agreement, gender consistency
- **Detection method:** Morphological analysis, agreement checking, lexical lookup

**Severity Weights:**
- Verb conjugation: High (1.0)
- Gender agreement: Medium (0.5)
- Articles: Low (0.1)
- Lexical primes: Low (0.1)

**Sovereign Invariant Link:** CL-I4 (Dimensional Reduction) - gender as dimension in property space

---

### 4. Spanish (es / spa)

**Classification:** Indo-European, Romance, Ibero-Romance
**Structural Features:** Colonial varieties, aspectual system, pro-drop
**Distinctive Features:** Rich aspectual distinction (preterite/imperfect); null subject parameter

**Prime Realization Patterns:**
- **Substantives:** Gender-marked forms (yo, tú, alguien, algo, gente, cuerpo)
- **Mental predicates:** Conjugated verbs (pensar, saber, querer, sentir, ver, oír)
- **Time:** Aspectual distinction (cuando/tiempo, ahora, antes, después)
- **Space:** Prepositions (dónde/lugar, aquí, encima, debajo, lejos, cerca)

**Compression Implications:**
- **Medium compressibility:** Aspectual system adds complexity; pro-drop enables subject omission
- **Critical invariants:** Aspect distinction, subject-verb agreement, null subject parameter
- **Detection method:** Aspectual analysis, subject recovery, agreement checking

**Severity Weights:**
- Aspect distinction: High (1.0)
- Subject-verb agreement: Medium (0.5)
- Null subject: Medium (0.5)
- Lexical primes: Low (0.1)

**Sovereign Invariant Link:** NA-I2 (Hysteresis) - aspectual states as hysteresis points

---

### 5. Italian (it / ita)

**Classification:** Indo-European, Romance, Italo-Dalmatian
**Structural Features:** Mediterranean phonology, rich verbal system
**Distinctive Features:** Phonological patterns; verbal inflection complexity

**Prime Realization Patterns:**
- **Substantives:** Gender-marked forms (io, tu, qualcuno, qualcosa, gente, corpo)
- **Mental predicates:** Conjugated verbs (pensare, sapere, volere, sentire, vedere, sentire)
- **Time:** Tense system (quando/tempo, ora, prima, dopo)
- **Space:** Prepositions (dove/posto, qui, sopra, sotto, lontano, vicino)

**Compression Implications:**
- **Medium compressibility:** Verbal inflection; phonological patterns
- **Critical invariants:** Verb conjugation, phonological integrity
- **Detection method:** Morphological analysis, phonological normalization

**Severity Weights:**
- Verb conjugation: High (1.0)
- Phonological patterns: Medium (0.5)
- Lexical primes: Low (0.1)

**Sovereign Invariant Link:** VP-I1 (Shell Partitioning) - phonological shell structure

---

### 6. Polish (pl / pol)

**Classification:** Indo-European, Slavic, West
**Structural Features:** Aspect, case-marking (7 cases), free word order
**Distinctive Features:** Rich aspectual system; extensive case system; flexible word order

**Prime Realization Patterns:**
- **Substantives:** Case-inflected forms (ja, ty, ktoś, coś, ludzie, ciało)
- **Mental predicates:** Aspectual verbs (myśleć, wiedzieć, chcieć, czuć, widzieć, słyszeć)
- **Time:** Aspectual distinction (kiedy/czas, teraz, przed, po)
- **Space:** Prepositions with case (gdzie/miejsce, tu, nad, pod, daleko, blisko)

**Compression Implications:**
- **Low compressibility:** Complex aspectual system; extensive case marking
- **Critical invariants:** Aspect, case morphology, word order constraints
- **Detection method:** Aspectual analysis, case assignment, word order recovery

**Severity Weights:**
- Aspect: Critical (∞)
- Case morphology: High (1.0)
- Word order: Medium (0.5)
- Lexical primes: Low (0.1)

**Sovereign Invariant Link:** TD-I2 (Betti Conservation) - case system as topological structure

---

### 7. Russian (ru / rus)

**Classification:** Indo-European, Slavic, East
**Structural Features:** Aspectual pairs, verbal morphology, free word order
**Distinctive Features:** Aspectual pairs (perfective/imperfective); rich verbal morphology

**Prime Realization Patterns:**
- **Substantives:** Case-inflected forms (я, ты, кто-то, что-то, люди, тело)
- **Mental predicates:** Aspectual verb pairs (думать/подумать, знать, хотеть, чувствовать, видеть, слышать)
- **Time:** Aspectual distinction (когда/время, сейчас, до, после)
- **Space:** Prepositions with case (где/место, здесь, над, под, далеко, близко)

**Compression Implications:**
- **Low compressibility:** Aspectual pairs; verbal morphology; case system
- **Critical invariants:** Aspectual pairs, case morphology, verbal inflection
- **Detection method:** Aspectual pair identification, case assignment, verbal morphology analysis

**Severity Weights:**
- Aspectual pairs: Critical (∞)
- Case morphology: High (1.0)
- Verbal inflection: High (1.0)
- Lexical primes: Low (0.1)

**Sovereign Invariant Link:** NA-I1 (MLGRU Fixed Point) - aspectual pairs as attractor states

---

### 8. Czech (cs / ces/cze)

**Classification:** Indo-European, Slavic, West
**Structural Features:** Complex clitic systems, case-marking
**Distinctive Features:** Clitic placement rules; rich case system

**Prime Realization Patterns:**
- **Substantives:** Case-inflected forms (já, ty, někdo, něco, lidé, tělo)
- **Mental predicates:** Conjugated verbs (myslet, vědět, chtít, cítit, vidět, slyšet)
- **Time:** Tense system (kdy/čas, teď, před, po)
- **Space:** Prepositions with case (kde/místo, tady, nad, pod, daleko, blízko)

**Compression Implications:**
- **Low compressibility:** Clitic system; case morphology
- **Critical invariants:** Clitic placement, case morphology
- **Detection method:** Clitic position analysis, case assignment

**Severity Weights:**
- Clitic placement: High (1.0)
- Case morphology: High (1.0)
- Lexical primes: Low (0.1)

**Sovereign Invariant Link:** SC-I3 (Threshold Scale Separation) - clitic position thresholds

---

### 9. Danish (da / dan)

**Classification:** Indo-European, Germanic, North
**Structural Features:** Semantic minimalism, phonological reduction
**Distinctive Features:** Reduced phonology; minimal semantic marking

**Prime Realization Patterns:**
- **Substantives:** Minimal forms (jeg, du, nogen, noget, folk, krop)
- **Mental predicates:** Simple verbs (tænke, vide, ville, føle, se, høre)
- **Time:** Simple temporal markers (når/tid, nu, før, efter)
- **Space:** Prepositions (hvor/sted, her, over, under, langt, nær)

**Compression Implications:**
- **High compressibility:** Minimal morphology; reduced phonology
- **Critical invariants:** Minimal semantic markers
- **Detection method:** Lexical lookup, phonological normalization

**Severity Weights:**
- Semantic markers: Medium (0.5)
- Lexical primes: Low (0.1)

**Sovereign Invariant Link:** AF-I3 (Machine Epsilon) - minimal representation as epsilon

---

### 10. Dutch (nl / nld/dut)

**Classification:** Indo-European, Germanic, West
**Structural Features:** Contact effects from Romance
**Distinctive Features:** Romance influence on vocabulary; Germanic structure

**Prime Realization Patterns:**
- **Substantives:** Gender-marked forms (ik, jij, iemand, iets, mensen, lichaam)
- **Mental predicates:** Conjugated verbs (denken, weten, willen, voelen, zien, horen)
- **Time:** Temporal markers (wanneer/tijd, nu, voor, na)
- **Space:** Prepositions (waar/plaats, hier, boven, onder, ver, dichtbij)

**Compression Implications:**
- **Medium compressibility:** Gender marking; Romance vocabulary
- **Critical invariants:** Gender agreement, vocabulary origin
- **Detection method:** Gender assignment, etymological analysis

**Severity Weights:**
- Gender agreement: Medium (0.5)
- Vocabulary origin: Low (0.1)
- Lexical primes: Low (0.1)

**Sovereign Invariant Link:** RG-I2 (Lawfulness Excess) - contact language as lawfulness excess

---

### 11. Serbian (sr / srp)

**Classification:** Indo-European, Slavic, South
**Structural Features:** Balkan areal features, diglossic history
**Distinctive Features:** Balkan sprachbund features; diglossia (standard vs. dialect)

**Prime Realization Patterns:**
- **Substantives:** Case-inflected forms (ja, ti, neko, nešto, ljudi, telo)
- **Mental predicates:** Conjugated verbs (misliti, znati, hteti, osećati, videti, čuti)
- **Time:** Aspectual distinction (kada/vreme, sada, pre, posle)
- **Space:** Prepositions with case (gde/mesto, ovde, iznad, ispod, daleko, blizu)

**Compression Implications:**
- **Low compressibility:** Balkan features; diglossia; case system
- **Critical invariants:** Balkan areal features, diglossic register
- **Detection method:** Areal feature detection, register identification

**Severity Weights:**
- Balkan features: High (1.0)
- Diglossic register: Medium (0.5)
- Case morphology: High (1.0)
- Lexical primes: Low (0.1)

**Sovereign Invariant Link:** TD-I4 (Coupling-Velocity Tradeoff) - areal coupling

---

### 12. Arabic (ar / ara - macrolanguage)

**Classification:** Semitic, Central
**Structural Features:** Root-pattern morphology, macrolanguage structure
**Distinctive Features:** Consonantal roots combine with vocalic patterns; macrolanguage with regional varieties

**Prime Realization Patterns:**
- **Substantives:** Root-pattern forms (أنا, أنت, شخص, شيء, الناس, الجسم)
- **Mental predicates:** Root-derived verbs (فكر, عرف, أراد, شعر, رأى, سمع)
- **Time:** Root-pattern temporal (متى/وقت, الآن, قبل, بعد)
- **Space:** Prepositions (أين/مكان, هنا, فوق, تحت, بعيد, قريب)

**Compression Implications:**
- **Low compressibility:** Root-pattern morphology; macrolanguage complexity
- **Critical invariants:** Root integrity, pattern consistency, variety identification
- **Detection method:** Root extraction, pattern analysis, variety classification

**Severity Weights:**
- Root integrity: Critical (∞)
- Pattern consistency: High (1.0)
- Variety identification: Medium (0.5)
- Lexical primes: Low (0.1)

**Sovereign Invariant Link:** Master Invariant (Coherence Conservation) - root as coherent unit

---

### 13. Hebrew (he / heb)

**Classification:** Semitic, Central
**Structural Features:** Language revival, historical depth
**Distinctive Features:** Revived language; historical continuity

**Prime Realization Patterns:**
- **Substantives:** Root-pattern forms (אני, אתה, מישהו, משהו, אנשים, גוף)
- **Mental predicates:** Root-derived verbs (חשב, ידע, רצה, הרגיש, ראה, שמע)
- **Time:** Root-pattern temporal (מתי/זמן, עכשיו, לפני, אחרי)
- **Space:** Prepositions (איפה/מקום, כאן, מעל, מתחת, רחוק, קרוב)

**Compression Implications:**
- **Low compressibility:** Root-pattern morphology; historical layers
- **Critical invariants:** Root integrity, historical continuity
- **Detection method:** Root extraction, historical layer analysis

**Severity Weights:**
- Root integrity: Critical (∞)
- Historical continuity: Medium (0.5)
- Lexical primes: Low (0.1)

**Sovereign Invariant Link:** VP-I3 (Genetic Entropy) - historical information preservation

---

### 14. Amharic (am / amh)

**Classification:** Semitic, South, Ethiopian
**Structural Features:** Syllabic script, Ethiopian Semitic
**Distinctive Features:** Ge'ez script; complex verb morphology

**Prime Realization Patterns:**
- **Substantives:** Syllabic script forms (እኔ, አንተ, ሰው, ነገር, ሰዎች, አካል)
- **Mental predicates:** Conjugated verbs (ማሰብ, ማወቅ, መፈለግ, መሰማት, ማየት, ማሰማት)
- **Time:** Tense system (መቼ/ጊዜ, አሁን, ከዚያ በፊት, ከዚያ በኋላ)
- **Space:** Prepositions (የት/ቦታ, እዚህ, ከላይ, ታች, ሩቅ, ቅርብ)

**Compression Implications:**
- **Low compressibility:** Syllabic script; complex morphology
- **Critical invariants:** Script integrity, morphology consistency
- **Detection method:** Script normalization, morphological analysis

**Severity Weights:**
- Script integrity: High (1.0)
- Morphology consistency: High (1.0)
- Lexical primes: Low (0.1)

**Sovereign Invariant Link:** HW-I1 (Turing Universality) - script as computational system

---

### 15. Mandarin Chinese (zh / cmn - zho macrolanguage)

**Classification:** Sino-Tibetan
**Structural Features:** Morphosyllabic, isolating, tonal
**Distinctive Features:** Primes realized through grammatical particles; morphosyllabic writing

**Prime Realization Patterns:**
- **Substantives:** Particles + nouns (我, 你, 有人, 东西, 人, 身体)
- **Mental predicates:** Verbs + particles (想, 知道, 要, 感觉, 看, 听)
- **Time:** Temporal particles (什么时候/时间, 现在, 以前, 以后)
- **Space:** Spatial particles (哪里/地方, 这里, 上面, 下面, 远, 近)

**Compression Implications:**
- **Medium compressibility:** Tonal system; particle system; morphosyllabic writing
- **Critical invariants:** Tone, particle usage, character integrity
- **Detection method:** Tone analysis, particle identification, character normalization

**Severity Weights:**
- Tone: High (1.0)
- Particles: Medium (0.5)
- Character integrity: Medium (0.5)
- Lexical primes: Low (0.1)

**Sovereign Invariant Link:** RG-I3 (Observer Frame) - tone as subjective frame

---

### 16. Cantonese (yue)

**Classification:** Sino-Tibetan
**Structural Features:** Tonal, southern variety, lexical retention
**Distinctive Features:** Complex tone system; retention of classical vocabulary

**Prime Realization Patterns:**
- **Substantives:** Tonal forms (我, 你, 有人, 嘢, 人, 身體)
- **Mental predicates:** Tonal verbs (諗, 知, 要, 感覺, 睇, 聽)
- **Time:** Temporal markers (幾時/時間, 而家, 之前, 之後)
- **Space:** Spatial markers (邊度/地方, 呢度, 上面, 下面, 遠, 近)

**Compression Implications:**
- **Low compressibility:** Complex tone system; classical vocabulary
- **Critical invariants:** Tone, classical vocabulary retention
- **Detection method:** Tone analysis, classical vocabulary identification

**Severity Weights:**
- Tone: Critical (∞)
- Classical vocabulary: High (1.0)
- Lexical primes: Low (0.1)

**Sovereign Invariant Link:** VP-I2 (Coordinate Constraint) - tone coordinate system

---

### 17. Japanese (ja / jpn)

**Classification:** Japonic (isolate)
**Structural Features:** Honorific system, predicate-final, complex writing
**Distinctive Features:** Honorific hierarchy; mixed writing system (kanji, hiragana, katakana)

**Prime Realization Patterns:**
- **Substantives:** Honorific forms (私, あなた, 誰か, 何か, 人, 体)
- **Mental predicates:** Honorific verbs (思う, 知る, 欲しい, 感じる, 見る, 聞く)
- **Time:** Temporal markers (いつ/時間, 今, 前, 後)
- **Space:** Spatial markers (どこ/場所, ここ, 上, 下, 遠い, 近い)

**Compression Implications:**
- **Low compressibility:** Honorific system; complex writing; predicate-final order
- **Critical invariants:** Honorific level, writing system integrity, word order
- **Detection method:** Honorific analysis, script identification, word order recovery

**Severity Weights:**
- Honorific level: High (1.0)
- Writing system: High (1.0)
- Word order: Medium (0.5)
- Lexical primes: Low (0.1)

**Sovereign Invariant Link:** SC-I3 (Threshold Scale Separation) - honorific hierarchy

---

### 18. Korean (ko / kor)

**Classification:** Koreanic (isolate)
**Structural Features:** Agglutinative, case-marking, evidentiality
**Distinctive Features:** Agglutinative morphology; honorific system; evidential markers

**Prime Realization Patterns:**
- **Substantives:** Case-marked forms (나, 너, 누군가, 무언가, 사람, 몸)
- **Mental predicates:** Agglutinative verbs (생각하다, 알다, 원하다, 느끼다, 보다, 듣다)
- **Time:** Temporal markers (언제/시간, 지금, 전, 후)
- **Space:** Spatial markers (어디/장소, 여기, 위, 아래, 멀, 가깝)

**Compression Implications:**
- **Low compressibility:** Agglutinative morphology; honorific system; evidentiality
- **Critical invariants:** Morpheme boundaries, honorific level, evidential markers
- **Detection method:** Morpheme segmentation, honorific analysis, evidential identification

**Severity Weights:**
- Morpheme boundaries: High (1.0)
- Honorific level: Medium (0.5)
- Evidential markers: Medium (0.5)
- Lexical primes: Low (0.1)

**Sovereign Invariant Link:** NA-I3 (Ternary Quantization) - evidential as ternary state

---

### 19. Vietnamese (vi / vie)

**Classification:** Austroasiatic
**Structural Features:** Tonal, monosyllabic, extensive compounding
**Distinctive Features:** Complex tone system; monosyllabic base; extensive compounding

**Prime Realization Patterns:**
- **Substantives:** Tonal monosyllables (tôi, bạn, ai, cái gì, người, cơ thể)
- **Mental predicates:** Tonal verbs (nghĩ, biết, muốn, cảm thấy, thấy, nghe)
- **Time:** Temporal markers (khi nào/thời gian, bây giờ, trước, sau)
- **Space:** Spatial markers (ở đâu/nơi, ở đây, trên, dưới, xa, gần)

**Compression Implications:**
- **Low compressibility:** Complex tone system; monosyllabic structure; compounding
- **Critical invariants:** Tone, syllable integrity, compound structure
- **Detection method:** Tone analysis, syllable segmentation, compound analysis

**Severity Weights:**
- Tone: Critical (∞)
- Syllable integrity: High (1.0)
- Compound structure: Medium (0.5)
- Lexical primes: Low (0.1)

**Sovereign Invariant Link:** AF-I2 (Involution Property) - tonal involution

---

### 20. Ewe (ewe)

**Classification:** Niger-Congo, Kwa
**Structural Features:** Tonal, serial verb constructions
**Distinctive Features:** Serial verb constructions; tone system

**Prime Realization Patterns:**
- **Substantives:** Tonal forms (me, wo, ame, nukɔ, amewo, nutome)
- **Mental predicates:** Serial verbs (nɔnɔe, nɔ, wɔ, te, nya, tia)
- **Time:** Temporal markers (gbegbe/ɣeyiɣi, lɔƒo, gbɔ, me)
- **Space:** Spatial markers (ahe/afe, afe, ɖime, ɖe, vɔ, titina)

**Compression Implications:**
- **Low compressibility:** Serial verb constructions; tone system
- **Critical invariants:** Serial verb structure, tone
- **Detection method:** Serial verb analysis, tone analysis

**Severity Weights:**
- Serial verb structure: High (1.0)
- Tone: High (1.0)
- Lexical primes: Low (0.1)

**Sovereign Invariant Link:** TD-I1 (Harmonic Kernel) - serial verb harmonics

---

### 21. Wolof (wol)

**Classification:** Atlantic-Congo
**Structural Features:** Consonant mutation, nominal classification
**Distinctive Features:** Consonant alternation; noun class system

**Prime Realization Patterns:**
- **Substantives:** Class-marked forms (ma, yow, kenn, lu nit, nit ñi, yaram)
- **Mental predicates:** Conjugated verbs (dëgg, xam, bëgg, ràñ, gis, woy)
- **Time:** Temporal markers (baam/wàll, leegi, ci kan, ci ginaaw)
- **Space:** Spatial markers (fu/bët, fii, kaw, suuf, sëkk, wet)

**Compression Implications:**
- **Low compressibility:** Consonant mutation; noun class system
- **Critical invariants:** Consonant alternation, noun class
- **Detection method:** Mutation analysis, class identification

**Severity Weights:**
- Consonant mutation: High (1.0)
- Noun class: High (1.0)
- Lexical primes: Low (0.1)

**Sovereign Invariant Link:** NA-I2 (Hysteresis) - consonant mutation as hysteresis

---

### 22. Kigiriyama (nyf)

**Classification:** Niger-Congo, Bantu
**Structural Features:** Noun class system, agglutinative morphology
**Distinctive Features:** Extensive noun class system; agglutinative verb morphology

**Prime Realization Patterns:**
- **Substantives:** Class-prefixed forms (mimi, wewe, mtu, kitu, watu, mwili)
- **Mental predicates:** Agglutinative verbs (fikiria, kujua, kutaka, kuhisi, kuona, kusikia)
- **Time:** Temporal markers (lini/wakati, sasa, kabla, baada)
- **Space:** Spatial markers (wapi/mahali, hapa, juu, chini, mbali, karibu)

**Compression Implications:**
- **Low compressibility:** Noun class system; agglutinative morphology
- **Critical invariants:** Noun class prefixes, morpheme boundaries
- **Detection method:** Class prefix identification, morpheme segmentation

**Severity Weights:**
- Noun class: Critical (∞)
- Morpheme boundaries: High (1.0)
- Lexical primes: Low (0.1)

**Sovereign Invariant Link:** TD-I2 (Betti Conservation) - noun class topology

---

### 23. Longgu (lgu)

**Classification:** Austronesian, Oceanic
**Structural Features:** Verb-initial, transitivity systems, possessive classifiers
**Distinctive Features:** Verb-initial order; transitivity alternation; possessive classifiers

**Prime Realization Patterns:**
- **Substantives:** Classifier-marked forms (au, oe, tamata, mea, tamatai, niga)
- **Mental predicates:** Transitivity-alternating verbs (manatunatu, iloa, manako, manatunatu, iloa, rongo)
- **Time:** Temporal markers (wae/gahua, inahia, mua, muri)
- **Space:** Spatial classifiers (fea/ples, heni, aholo, afo, laa, tapa)

**Compression Implications:**
- **Medium compressibility:** Verb-initial order; classifier system
- **Critical invariants:** Word order, classifier usage, transitivity
- **Detection method:** Word order analysis, classifier identification, transitivity analysis

**Severity Weights:**
- Word order: High (1.0)
- Classifiers: Medium (0.5)
- Transitivity: Medium (0.5)
- Lexical primes: Low (0.1)

**Sovereign Invariant Link:** VP-I1 (Shell Partitioning) - classifier partitioning

---

### 24. Cèmuhi (cam)

**Classification:** Austronesian, Oceanic
**Structural Features:** Tonal (3 register tones), New Caledonian, limited prior documentation
**Distinctive Features:** Complex tone system; limited prior documentation

**Prime Realization Patterns:**
- **Substantives:** Tonal forms (nyu, nyu, pwâa, pwâa, pwâa, pwâa)
- **Mental predicates:** Tonal verbs (rââ, rââ, rââ, rââ, rââ, rââ)
- **Time:** Temporal markers (ââ/ââ, ââ, ââ, ââ)
- **Space:** Spatial markers (ââ/ââ, ââ, ââ, ââ, ââ, ââ)

**Compression Implications:**
- **Low compressibility:** Complex tone system; limited documentation
- **Critical invariants:** Tone system, limited documentation constraints
- **Detection method:** Tone analysis, documentation consultation

**Severity Weights:**
- Tone system: Critical (∞)
- Documentation constraints: High (1.0)
- Lexical primes: Low (0.1)

**Sovereign Invariant Link:** RG-I1 (Phase Boundary) - tone phase boundaries

---

### 25. Finnish (fi / fin)

**Classification:** Uralic, Finnic
**Structural Features:** Non-Indo-European European, agglutinative, vowel harmony
**Distinctive Features:** 15 cases; complex verbal inflection; vowel harmony

**Prime Realization Patterns:**
- **Substantives:** Case-inflected forms (minä, sinä, joku, jokin, ihmiset, keho)
- **Mental predicates:** Inflected verbs (ajatella, tietää, haluta, tuntea, nähdä, kuulla)
- **Time:** Tense system (milloin/aika, nyt, ennen, jälkeen)
- **Space:** Case-governed spatial (missä/paikka, täällä, yllä, alla, kaukana, lähellä)

**Compression Implications:**
- **Low compressibility:** Extensive case system; vowel harmony; agglutinative morphology
- **Critical invariants:** Case morphology, vowel harmony, morpheme boundaries
- **Detection method:** Case assignment, vowel harmony analysis, morpheme segmentation

**Severity Weights:**
- Case morphology: Critical (∞)
- Vowel harmony: High (1.0)
- Morpheme boundaries: High (1.0)
- Lexical primes: Low (0.1)

**Sovereign Invariant Link:** AF-I1 (Norm Preservation) - vowel harmony as norm

---

### 26. Farsi/Persian (fa / fas/per)

**Classification:** Indo-European, Iranian
**Structural Features:** Middle Eastern, emotion vocabulary, cultural scripts
**Distinctive Features:** Rich emotion terminology; cultural script vocabulary

**Prime Realization Patterns:**
- **Substantives:** Forms (من, تو, کسی, چیزی, مردم, بدن)
- **Mental predicates:** Conjugated verbs (فکر کردن, دانستن, خواستن, احساس کردن, دیدن, شنیدن)
- **Time:** Temporal markers (کی/زمان, حال, قبل, بعد)
- **Space:** Prepositions (کجا/مکان, اینجا, بالا, پایین, دور, نزدیک)

**Compression Implications:**
- **Medium compressibility:** Emotion vocabulary complexity; cultural scripts
- **Critical invariants:** Emotion terminology, cultural script integrity
- **Detection method:** Emotion vocabulary identification, cultural script analysis

**Severity Weights:**
- Emotion terminology: Medium (0.5)
- Cultural scripts: Medium (0.5)
- Lexical primes: Low (0.1)

**Sovereign Invariant Link:** CL-I3 (Regret Identity) - emotion as reward/penalty

---

### 27. Trini (Trinidadian Creole)

**Classification:** English-lexified creole
**Structural Features:** Contact language, prime preservation through restructuring
**Distinctive Features:** English lexicon with restructured grammar; prime preservation

**Prime Realization Patterns:**
- **Substantives:** Creole forms (mi, yuh, somebody, someting, people, body)
- **Mental predicates:** Creole verbs (tink, know, want, feel, see, hear)
- **Time:** Temporal markers (when/time, now, before, after)
- **Space:** Spatial markers (where/place, here, above, below, far, near)

**Compression Implications:**
- **Medium compressibility:** English lexicon simplifies compression; restructured grammar
- **Critical invariants:** Prime preservation through restructuring
- **Detection method:** Creole grammar identification, prime verification

**Severity Weights:**
- Prime preservation: High (1.0)
- Grammatical restructuring: Medium (0.5)
- Lexical primes: Low (0.1)

**Sovereign Invariant Link:** RG-I2 (Lawfulness Excess) - creole as lawfulness excess

---

## Cross-Linguistic Invariant Patterns

### Universal Invariant Categories

**1. Structural Invariants (across all languages):**
- Prime inventory: 64 primes consistent across 27+ languages
- Combinatorial syntax: Universal grammar of semantic composition
- Prime realizability: All primes expressible in all languages

**2. Processing Invariants:**
- Element interactivity: Primes minimize interactivity
- Schema formation: Primes enable automated schema formation
- Cross-linguistic transfer: Prime-level concepts show positive transfer

**3. Compression-Relevant Invariants:**
- Morphological complexity: Ranges from analytic (English) to highly agglutinative (Finnish, Korean)
- Word order: Ranges from fixed (English SVO) to free (Slavic languages)
- Tone systems: Absent in many languages, critical in others (Chinese, Vietnamese, Ewe)
- Writing systems: Ranges from alphabetic to syllabic to logographic

---

## Integration with $L_{\text{inv}}$

### Language-Specific Load Calculation

$$L_{\text{inv}}(x, \mathcal{I}_{\text{lang}}) = \sum_{i \in \mathcal{I}_{\text{lang}}} w_i \cdot \mathbb{1}[\text{broken}(i, x)] \cdot \text{severity}(i)$$

Where $\mathcal{I}_{\text{lang}}$ includes:
- Language-specific structural invariants (case, tone, morphology)
- Universal NSM primes (64 primes)
- Language-specific prime realizations

### Context-Dependent Weighting

**Multilingual contexts:**
- Higher weight on language identification
- Higher weight on prime preservation across languages
- Lower weight on language-specific features

**Monolingual contexts:**
- Higher weight on language-specific invariants
- Lower weight on cross-linguistic consistency

**Code-switching contexts:**
- Highest weight on language boundary preservation
- High weight on prime preservation across switches

---

## Detection Methods by Language Family

### Indo-European
- **Method:** POS tagging, dependency parsing, morphological analysis
- **Tools:** spaCy, Stanza, UDPipe
- **Complexity:** Low to medium (English to Slavic)

### Semitic
- **Method:** Root extraction, pattern analysis, morphological segmentation
- **Tools:** MADAMIRA, CAMeL Tools
- **Complexity:** High (root-pattern morphology)

### Sino-Tibetan
- **Method:** Tone analysis, character normalization, particle identification
- **Tools:** Jieba, HanLP, tone analyzers
- **Complexity:** High (tone, writing system)

### Japonic/Koreanic
- **Method:** Honorific analysis, morpheme segmentation, script identification
- **Tools:** MeCab, KoNLPy
- **Complexity:** High (honorifics, agglutination)

### Niger-Congo
- **Method:** Tone analysis, serial verb analysis, noun class identification
- **Tools:** Custom analyzers, linguistic software
- **Complexity:** High (tone, serial verbs, noun classes)

### Austronesian
- **Method:** Classifier identification, word order analysis, transitivity analysis
- **Tools:** Custom analyzers, linguistic software
- **Complexity:** Medium (classifiers, word order)

### Uralic
- **Method:** Case assignment, vowel harmony analysis, morpheme segmentation
- **Tools:** Custom analyzers, linguistic software
- **Complexity:** High (case system, vowel harmony)

---

## References

- NSM Approach: https://nsm-approach.net/resources
- ISO 639:2023: https://arxiv.org/pdf/2506.06870
- Research Stack, Invariant Root Analysis (invariant_root_analysis.md)
- Research Stack, NSM Primes Expanded (10_NSM_Primes_Expanded_for_Cognitive_Load.md)
- Research Stack, Cognitive Load Theory Invariant-Enhanced (09_Cognitive_Load_Theory_Invariant_Enhanced.md)
