# Credit Risk Modeling: Probability of Default Prediction

A machine learning project for estimating **Probability of Default (PD)** in a consumer credit risk setting.

This repository uses `extra_credit_project_data.csv` to run an end-to-end workflow (EDA, preprocessing, model training, and evaluation) to predict whether a borrower will experience serious delinquency within two years (`SeriousDlqin2yrs`).

---

## Project Goals

- Build a binary classification model for default vs non-default risk.
- Provide a practical notebook-based baseline from exploration to evaluation.
- Keep the repository organized for GitHub collaboration and reproducibility.

---

## Repository Structure

```text
.
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   ├── bug_report.md
│   │   └── feature_request.md
│   └── pull_request_template.md
├── Project_1_credit_defult.ipynb
├── extra_credit_project_data.csv
├── extra_credit_project_data_dictionary.xls
├── .gitignore
├── CONTRIBUTING.md
├── LICENSE
├── requirements.txt
└── README.md
```

---

## Data

- `extra_credit_project_data.csv`: modeling dataset.
- `extra_credit_project_data_dictionary.xls`: variable definitions.
- Target column: `SeriousDlqin2yrs`.

> Do not commit personally identifiable information (PII) or confidential raw data to public repositories.

---

## Method Overview

The notebook (`Project_1_credit_defult.ipynb`) follows this flow:

1. Load data and perform initial inspection (`info`, null checks, distributions).
2. Separate/inspect numerical and categorical features.
3. Apply preprocessing (missing-value treatment, winsorization, etc.).
4. Train baseline classifiers (e.g., Logistic Regression, KNN, Random Forest).
5. Evaluate with confusion matrix, classification report, ROC-related metrics.

---

## Quick Start

### 1) Clone

```bash
git clone <your-repo-url>
cd Credit_Risk_Modeling-Probability_of_Default_Prediction
```

### 2) Create environment and install dependencies

```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

### 3) Launch notebook

```bash
jupyter notebook
```

Then open `Project_1_credit_defult.ipynb`.

---

## Suggested Next Improvements

- Add consistent cross-validation and stronger hyperparameter search.
- Improve handling for class imbalance (e.g., class weights, threshold tuning, resampling).
- Add model interpretability (feature importance, SHAP).
- Refactor notebook logic into reusable `src/` modules.

---

## Contributing

Issues and pull requests are welcome. Please read [CONTRIBUTING.md](CONTRIBUTING.md) first.

---

## License

This project is licensed under the [MIT License](LICENSE).
