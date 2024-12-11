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

## File Structure

```
|-- data/
    |-- DRI_Corpus.zip
    |-- compiled_corpus_DrInventor.zip
|-- src/
    |-- feature_extraction.py
    |-- model_training.py
    |-- evaluation.py
|-- README.md
|-- requirements.txt
|-- results/
    |-- experiment_logs/
    |-- model_checkpoints/
```

### Key Files:
- **`data/`:** Contains the datasets and preprocessed files.
- **`src/`:** Scripts for feature extraction, model training, and evaluation.
- **`results/`:** Stores experiment logs and model checkpoints.

---

## Requirements

Install the necessary Python packages using the provided `requirements.txt`:

```bash
pip install -r requirements.txt
```

Key Libraries:
- `nltk`
- `scikit-learn`
- `spacy`
- `transformers`
- `pandas`
- `numpy`

---

## How to Run

1. **Prepare Data:**
   - Extract the datasets from `data/DRI_Corpus.zip` and `data/compiled_corpus_DrInventor.zip`.
   - Ensure proper directory structure.

2. **Feature Extraction:**
   - Run `src/feature_extraction.py` to generate feature sets.

3. **Model Training:**
   - Run `src/model_training.py` to train models with the extracted features.

4. **Evaluation:**
   - Run `src/evaluation.py` to evaluate performance and compare results.

---

## Results
Results will be stored in the `results/` directory, including logs and model checkpoints. Detailed analysis of results will highlight the impact of argument-level textual features on model performance.

---

## References

- Rosenthal et al. (2017). Agreement and disagreement lexicons.
- Tan et al. (2018). Hedge feature extraction in argumentation mining.
- Lauscher et al. (2018). Argumentation tagging on Dr. Inventor Corpus.

