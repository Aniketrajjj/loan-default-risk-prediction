# Loan Default Risk Analysis & Prediction

A machine-learning project that explores borrower and loan characteristics and compares supervised classification models for predicting loan default.

## Project overview

The project uses the **Credit Risk Dataset** and follows a typical data-science workflow:

- Inspect the dataset, data types, summary statistics, and target distribution.
- Clean the data by handling duplicates, missing values, and implausible records.
- Perform exploratory data analysis (EDA) with plots and correlation analysis.
- Prepare features, encode categorical variables, and split the data into training and test sets.
- Train and evaluate classification models, including Logistic Regression, K-Nearest Neighbors, Gaussian Naive Bayes, Decision Tree, and Random Forest.
- Compare evaluation metrics such as accuracy, precision, recall, F1-score, and confusion matrix.

> **Important:** This project is for learning and analysis. Its predictions should not be used as the sole basis for real lending or credit decisions.

## Repository contents

Keep the files in the repository root with these names (or update the paths below if your uploaded filenames differ):

| File | Purpose |
| --- | --- |
| `Loan_Credit_Risk_Prediction.ipynb` | Main notebook covering preprocessing, EDA, and model comparison |
| `credit_risk_dataset.csv` | Dataset used by the notebook |
| `Project_Report.docx` | Project report/documentation |
| `requirements.txt` | Python package dependencies |

If you prefer to keep both notebooks, place the additional exploratory notebook (`ldrp.ipynb`) in the repository as well.

## Dataset

The notebook expects the CSV to be named `credit_risk_dataset.csv` in the same folder as the notebook. The target variable is `loan_status`:

- `0`: loan was not recorded as default
- `1`: loan was recorded as default

The dataset contains applicant and loan attributes such as age, income, home ownership, employment length, loan purpose, loan grade, loan amount, interest rate, loan-to-income ratio, previous default history, and credit history length.

## Getting started

### 1. Create an environment (recommended)

```bash
python -m venv .venv
```

Activate it:

- **Windows (PowerShell):** `.venv\\Scripts\\Activate.ps1`
- **macOS/Linux:** `source .venv/bin/activate`

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Launch Jupyter

```bash
jupyter notebook
```

Open `Loan_Credit_Risk_Prediction.ipynb` and run the cells from top to bottom. Make sure the CSV file is in the same directory.

## Main tools

- Python
- Jupyter Notebook
- pandas and NumPy
- Matplotlib and Seaborn
- scikit-learn

## Evaluation

The notebook evaluates multiple classification models using standard classification metrics. Review the notebook outputs for the actual scores; results can vary depending on preprocessing choices, data split, and random seed.

## Future improvements

- Add cross-validation and systematic hyperparameter tuning.
- Evaluate class imbalance with precision-recall curves and ROC-AUC alongside F1-score.
- Add a reproducible pipeline and save the final model.
- Build a small demo interface only after validating model performance and limitations.

## Author

**Aniket Raj**

---

This repository is an academic/data-science project. Please verify dataset licensing and attribution requirements before redistribution.
