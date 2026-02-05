# AI-ML-Assessment-2025-01 group assessment 
[View my Canva design](https://www.canva.com/design/DAGY5CPXjes/xAVObv02qTYRY3h3UZaAaw/view?utm_content=DAGY5CPXjes&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=had8489d4f4)


# Car Price Prediction (Machine Learning Regression)

> Predict used-car prices from vehicle attributes using a clean, reproducible ML pipeline (EDA → preprocessing → modeling → evaluation).
>
> **Why this matters:** Pricing is a classic real-world regression problem with messy data (categoricals, outliers, skew, leakage risk) — this project demonstrates practical ML workflow and decision-making, not just a single model run.

---

## Quick links
- 📓 Notebook: `TECH3200_Ass2_Share.ipynb`
- 🎥 Slides (Canva): **View my Canva design** (link in this repo)

---

## Highlights (recruiter-friendly)
- End-to-end workflow: **data understanding → feature prep → baseline → model comparison → evaluation**
- Practical ML skills: **categorical encoding, train/test split discipline, metric selection, error analysis**
- Reproducibility mindset: clear steps to rerun locally + suggestions for production hardening

---

## Problem statement
Given a dataset of used-car listings, train a regression model to predict **car selling price** from available features (e.g., year/age, kms driven, fuel type, transmission, owner count, seller type — exact fields shown in the notebook).

---

## Approach (what I did)
1. **Exploratory Data Analysis (EDA)**
   - Checked schema, missing values, distributions, correlations, and outliers
2. **Preprocessing**
   - Cleaned/standardised data types
   - Encoded categorical features (e.g., one-hot)
   - Split data into train/test to avoid leakage
3. **Modeling**
   - Built a **baseline regression model**
   - Trained and compared stronger models (e.g., tree-based ensembles where appropriate)
   - (If used) Tuned hyperparameters via cross-validation
4. **Evaluation**
   - Reported regression metrics (typical: **MAE / RMSE / R²**)
   - Compared predicted vs actual and reviewed largest errors

---

## Results (replace with your real outputs)
> **TODO:** Fill in these numbers from your notebook so recruiters can judge quality in 10 seconds.

| Model | MAE | RMSE | R² |
|------|-----:|-----:|---:|
| Baseline (e.g., Linear Regression) | TODO | TODO | TODO |
| Best model (name) | TODO | TODO | TODO |

**Key takeaway:** TODO (1–2 lines: what improved performance + what features mattered most, based on your analysis)

---

## Project structure
```

.
├── TECH3200_Ass2_Share.ipynb     # Main notebook (EDA → preprocessing → models → evaluation)
├── README.md
└── .gitignore

````

---

## How to run locally

### Option A — venv (recommended)
```bash
# 1) Create & activate environment
python -m venv .venv
# Windows:
.venv\Scripts\activate
# macOS/Linux:
source .venv/bin/activate

# 2) Install dependencies
pip install -U pip
pip install numpy pandas scikit-learn matplotlib seaborn jupyter
````

### Run the notebook

```bash
jupyter notebook
# open TECH3200_Ass2_Share.ipynb
```

> **Tip:** If your notebook already imports extra libraries, add them to the install line above or create a `requirements.txt`.

---

## Notes on data & ethics

* This project uses a supplied educational dataset. Treat predictions as **estimates**, not guarantees.
* A real deployment should include:

  * data drift checks (market changes)
  * bias checks (e.g., geography/brand segments)
  * privacy controls (remove personal identifiers)

---

## What I’d do next (to make it production-grade)

* Add `requirements.txt` + `Makefile` (1-command setup)
* Save the best model (`joblib`) and build a small **API** (FastAPI) or **demo app** (Streamlit)
* Add experiment tracking (MLflow) and CI (GitHub Actions) to rerun tests/notebook checks
* Stronger evaluation: cross-validation, leakage audit, and robust handling of rare categories

---

## About this project

Built as part of **Kaplan Business School — TECH3200 (Artificial Intelligence and Machine Learning in IT)** assessment work, then cleaned up to be recruiter-readable and reproducible.

---

## Author

**Candy Cheng**
GitHub: [https://github.com/CandyCheng-git](https://github.com/CandyCheng-git)
Email: [candycheng.it@gmail.com](mailto:candycheng.it@gmail.com)

```

