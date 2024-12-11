# Argumentation-Identification-Task
# Argumentation Identification in Scientific Papers

## Overview
This project explores the task of argumentation identification in scientific papers by investigating whether adding argument-level textual features improves prediction performance. Specifically, experiments are conducted to predict argumentative components and relations using various models, with and without argument-level textual features. The dataset used is the Dr. Inventor Corpus, with additional argumentation tagging by Lauscher et al.

---

## Research Question
**Does adding argument-level textual features help the argumentation identification task in scientific papers?**

---

## Tasks and Methodology

### Task 1: Feature Set Reproduction

Reproduce the feature sets described in Section 4.1 of the project specification, focusing on Dr. Inventor’s Corpus.

#### Feature Details:
1. **n-grams:**
   - Extract unigram, bigram, and trigram features from Dr. Inventor’s Corpus.
   - Use Python libraries (e.g., `nltk`, `sklearn`) for implementation.

2. **Argument Lexicons:**
   - Obtain agreement and disagreement lexicons from Rosenthal et al.'s work.
   - Use these lexicons to extract features from the corpus.

3. **Hedge Features:**
   - Investigate Dr. Tan’s paper and its project page for hedge feature extraction methods.
   - Implement the feature extraction if necessary, using Dr. Inventor’s Corpus.

4. **Modal Verbs:**
   - Extract modal verbs using Python's `spacy` library.

6. **Negation:**
   - Detect negation using Python libraries like `spacy` or custom logic.

---

### Task 2: Experiment Design

#### Experiment Details:

**Goal:** Conduct experiments to predict argumentative components and relations, with and without argument-level textual features.

1. **Models:**
   - **Logistic Regression:** Implement a baseline similar to previous work.
   - **BERT:** Utilize pre-trained BERT for contextual embeddings.
   - **SciBERT:** Leverage SciBERT by Allen AI, designed for scientific text.
   - **LLM Prompting:** Use open-source LLMs such as LLaMA for zero-shot or fine-tuned tasks.

2. **Comparison:**
   - Perform experiments with and without argument-level textual features for each model.

---

## Dataset

### Source
- **Dr. Inventor Corpus:** Original corpus containing rhetorical labels.
  - Downloaded from the provided source.

- **Compiled Corpus by Lauscher et al.:** Augmented version with argumentation tagging.
  - Contains 40 articles with argumentation tagging.
  - Corpus and relevant paper are included in the project files.

---

## References

- Rosenthal et al. (2017). Agreement and disagreement lexicons.
- Tan et al. (2018). Hedge feature extraction in argumentation mining.
- Lauscher et al. (2018). Argumentation tagging on Dr. Inventor Corpus.

