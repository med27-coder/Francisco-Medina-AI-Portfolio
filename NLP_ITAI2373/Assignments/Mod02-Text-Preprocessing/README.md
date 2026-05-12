# Mod02 — Text Preprocessing: Cleaning, TF-IDF & Word Embeddings

## Problem Statement

Build a complete text preprocessing pipeline from scratch — the foundational layer that every NLP model depends on — covering text cleaning, keyword extraction with TF-IDF, and semantic similarity with word embeddings.

## Approach

Three-task assignment building the pipeline step by step:

1. **Task 1 — The Cleaner:** Built a `clean_text()` function using regex to lowercase text, strip special characters, and normalize whitespace. Validated against test cases including `"[ALERT]!!! Go to the... KITCHEN"` → `"alert go to the kitchen"`.

2. **Task 2 — TF-IDF Keyword Extraction:** Used `TfidfVectorizer` from Scikit-learn on a small document corpus. Extracted which terms were most distinctive per document — demonstrating how TF-IDF down-weights common words and up-weights rare ones.

3. **Task 3 — Word Embeddings (Semantic Algebra):** Loaded GloVe pre-trained vectors (50-dimensional, trained on Wikipedia) via Gensim. Computed semantic similarity scores (e.g., `robot` vs `machine`) and performed vector arithmetic to explore how word relationships are encoded geometrically.

## Results

All three tasks passed assertion tests. Word similarity scores confirmed that GloVe captures semantic relationships — `robot` and `machine` scored high similarity while unrelated words scored near zero. Vector arithmetic demonstrated that word meanings can be combined and compared mathematically.

## Key Findings

Text preprocessing is not optional cleanup — it is the first model decision. Every downstream component (TF-IDF scores, embedding lookups) depends entirely on what the cleaning step preserved or discarded. GloVe's geometric encoding of meaning showed that "understanding" language can be approximated as position in a very large vector space.

## Technologies Used

Python · Scikit-learn (`TfidfVectorizer`) · Gensim (GloVe vectors) · NumPy · Pandas · Regex

## How to Run

Open `Mod02_FranciscoMedina_ITAI2373.ipynb` in [Google Colab](https://colab.research.google.com/) and run all cells in order.

## Files

| File | Description |
|---|---|
| `Mod02_FranciscoMedina_ITAI2373.ipynb` | Full text preprocessing assignment notebook |
