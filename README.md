# Statistical Analysis of Investment Strategies

Two notebooks investigating how market indicators relate to future SPY price changes using **ordinary least squares (OLS)** and **logistic regression**. The analysis includes technical indicator engineering, model summaries, regression diagnostics, predicted probabilities, ROC/AUC, and a confusion matrix.

**Technologies:** Python, pandas, NumPy, yfinance, statsmodels, scikit-learn, Matplotlib, seaborn.

## Notebooks
- [`Reg_Anything.ipynb`](Reg_Anything.ipynb) — OLS analysis of future returns with engineered indicators and diagnostic plots.
- [`log_regression_template.ipynb`](log_regression_template.ipynb) — logistic regression for a next-period up/down target, with ROC/AUC and confusion matrix plots.

## Reproduce
Install `requirements.txt`, open either notebook and run the cells in order with an internet connection. Price history is downloaded at runtime via yfinance. Parameter settings and data windows can be adjusted in the opening cells.

## Recorded observations & limitations
The OLS notebook's saved output reports an **R² of approximately 0.001**, suggesting little explained variance for that particular specification. The notebooks are exploratory and do not establish predictive profitability. Several evaluations use predictions on data involved in model fitting; **holdout / walk-forward validation and transaction-cost analysis are still needed** to assess generalization and trading utility.
