# SensIT Vehicle Classification (DS4400 Midterm)

Multi-class supervised ML project on [OpenML SensIT-Vehicle-Combined (id 1593)](https://www.openml.org/d/1593): classify sensor readings as **AAV**, **DW**, or **noise**.

## Submission artifact

- **Notebook (only file to submit for the midterm):** [`DS4400_SensIT_Vehicle_Classification.ipynb`](DS4400_SensIT_Vehicle_Classification.ipynb)
- Open in **Google Colab** → Runtime → Run all
- Record a **&lt;15 minute** walkthrough video for Canvas

## Pipeline overview

1. Load OpenML 1593 (~98.5k × 100 numeric features)
2. EDA: class balance (~1:1:2), distributions, correlations, outliers
3. Preprocess: stratified 80/20 split, `StandardScaler`, `class_weight`
4. Feature selection: **SelectKBest (ANOVA F)** only
5. Models: Logistic Regression + Random Forest
6. Tuning: RandomizedSearchCV → refit on full train
7. Evaluation: accuracy, macro-F1, confusion matrices, stratified 5-fold CV

## Local setup

```bash
pip install -r requirements.txt
jupyter notebook DS4400_SensIT_Vehicle_Classification.ipynb
```

## Resume draft

See [`RESUME_DRAFT.md`](RESUME_DRAFT.md) for English/Chinese bullets to replace the GTA project entry.
