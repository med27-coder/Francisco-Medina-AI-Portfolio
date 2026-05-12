# L08 — Video Game Sales Prediction: Machine Learning Lab

## What I Did

Built a binary classifier to predict whether a video game would be a commercial "hit" (>1M units sold) using historical sales data. The lab included the full ML pipeline: data loading, EDA, feature engineering, model training, evaluation — and discovering and fixing a critical data leakage bug.

## What I Learned

**The data leakage lesson:** My first model produced suspiciously perfect metrics — 99.94% accuracy, 100% recall, 99.97% ROC AUC. The moment I wrote out the math — `Total_Regional_Sales = NA + EU + JP + Other = Global_Sales` — I understood what happened. I had created a feature that directly encoded the target variable. The model wasn't learning patterns; it was reading the answer off the test sheet. Fixing it by engineering derived features and dropping the leaking columns produced honest results: 91.14% accuracy, 62.97% F1, 78.85% ROC AUC.

**The class imbalance lesson:** Only 12.37% of games are "hits." A naive model predicting "not a hit" for everything would achieve 87% accuracy without learning anything. This is why F1, precision, recall, and ROC AUC matter far more than accuracy for imbalanced datasets.

**The bigger lesson:** Perfect metrics are a warning sign. Lower, honest metrics from a model that learned real patterns are more valuable than impressive numbers from a broken one.

## Results

| Metric | Flawed Model | Corrected Model |
|---|---|---|
| Accuracy | 99.94% | 91.14% |
| Precision | 99.50% | 63.29% |
| Recall | 100% | 62.66% |
| F1-Score | 99.75% | 62.97% |
| ROC AUC | 99.97% | 78.85% |

## Technologies Used

Python · Pandas · NumPy · Scikit-learn (Decision Tree, train/test split) · Matplotlib · Seaborn · Google Colab

## Dataset

Video game sales dataset loaded from course GitHub repository. Not included in this repo — loaded automatically via `git clone` in the notebook.

## How to Run

Open `L08_Notebook_FranciscoMedina_ITAI2377.ipynb` in [Google Colab](https://colab.research.google.com/) and run all cells in order.

## Files

| File | Description |
|---|---|
| `L08_Notebook_FranciscoMedina_ITAI2377.ipynb` | Full ML prediction notebook |
| `L08_Journal_FranciscoMedina_ITAI2377.pdf` | Reflective journal — includes data leakage discovery |
