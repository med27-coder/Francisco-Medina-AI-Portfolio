# L05 — Data Preprocessing for Generative AI

## What I Did

Built a complete text preprocessing pipeline specifically designed for generative AI workflows — covering tokenization, cleaning, normalization, and embedding generation using both GloVe (static) and DistilBERT (contextual) embeddings. Applied to a BBC news article corpus.

## What I Learned

The most important lesson: code running without errors does not mean results are correct. The category column in the BBC dataset contained long mixed strings instead of clean labels — the pipeline produced results confidently using the wrong column until I checked intermediate outputs and caught the mismatch. This made "always validate mid-pipeline, not just at the end" a practice rather than advice.

The GloVe vs. DistilBERT comparison was the clearest demonstration of why contextual embeddings matter. GloVe assigns fixed vectors regardless of context; DistilBERT produces different representations for the same word in different sentences. Seeing DistilBERT group same-category articles more tightly in similarity matrices made the theoretical advantage concrete.

## Challenges

The BBC dataset's `category` column contained compound keyword strings requiring a custom parsing function to extract the correct topic label. NLTK required manual download commands (`punkt`, `stopwords`, `wordnet`) not included in the starter code. DistilBERT was used in place of full BERT due to Colab free-tier memory limits — same 768-dim output, fraction of the RAM.

## Technologies Used

Python · NLTK · Gensim (GloVe) · HuggingFace Transformers (DistilBERT) · Pandas · NumPy · Scikit-learn · Matplotlib · Google Colab

## How to Run

Open `L05_Notebook_FranciscoMedina_ITAI2377.ipynb` in [Google Colab](https://colab.research.google.com/) and run all cells in order.

## Files

| File | Description |
|---|---|
| `L05_Notebook_FranciscoMedina_ITAI2377.ipynb` | Full GenAI preprocessing notebook |
| `L05_Journal_FranciscoMedina_ITAI2377.pdf` | Reflective journal |
