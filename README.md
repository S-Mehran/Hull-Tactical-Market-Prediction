# Hull Tactical – Market Prediction

This repository contains my work on the **Hull Tactical Kaggle competition**, focused on predicting **daily excess returns under volatility constraints**. The competition emphasizes **risk-adjusted performance**, where the primary evaluation metric is the **Sharpe ratio**.

---

## Repository Structure

- `Hull_Tactical_Training_Pipeline.ipynb`  
  This notebook contains the **end-to-end training pipeline**, including:
  - Data loading and time-aware splitting
  - Exploratory data analysis (EDA)
  - Feature engineering (lagged features, PACF analysis, periodograms, missing-value flags, SVD)
  - Model training and evaluation (Linear Regression, Random Forest, XGBoost, LSTM variants)
  - Risk-adjusted evaluation using Sharpe ratio

- `Hull_Tactical_Submission_File.ipynb`  
  This notebook demonstrates how to generate the **final submission file** from the trained models.

---

## Key Highlights

- **Feature Engineering:** Lag features, Fourier terms, cycle identification, missing value flags, and dimensionality reduction.  
- **Modeling:** Baseline linear regression, tree-based models (Random Forest, XGBoost), and sequence models (LSTM).  
- **Validation:** Time-aware validation aligned with the test horizon to avoid leakage.  
- **Evaluation:** Sharpe ratio for risk-adjusted performance, with R², RMSE, and MSE as secondary metrics.  
- **Insights:** Feature design and data understanding are more important than model complexity in noisy financial datasets.

---

## How to Use

1. Clone the repository:
```bash
git clone https://github.com/<your-username>/<repo-name>.git
