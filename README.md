# Predicting S&P 500 Returns with Macro-Financial Indicators

This repository contains the source files, saved data, model outputs, final report, and website for my **JSC370 Final Project**.

## Website

The project website is available here:

https://lijack032.github.io/JSC370-Project/

The website includes a project overview, the final report, interactive visualizations, a downloadable PDF report, and an About page.

## Project Summary

This project examines whether macro-financial indicators can meaningfully predict future **S&P 500 returns**. The analysis combines daily financial market data with macroeconomic indicators and compares regression and classification models across **1-day**, **5-day**, and **20-day** forecast horizons.

The modeling workflow includes feature engineering, chronological train/validation/test splitting, hyperparameter tuning, model comparison, and feature-importance analysis.

For a fuller narrative of the project, see the website homepage and final report.

## Data Sources

The project uses data from:

- **Yahoo Finance chart API** for daily market indicators, including the S&P 500, Dow Jones Industrial Average, Treasury yields, U.S. Dollar Index, VIX, and crude oil prices.
- **Federal Reserve Economic Data (FRED) API** for macroeconomic indicators, including the Federal Funds Rate, CPI, unemployment rate, industrial production, consumer sentiment, and corporate bond yields.

Saved data files used for rendering are stored in the `data/` folder.

## Methods

The project compares several predictive models, including:

- Historical mean benchmark
- Majority-class benchmark
- Ordinary Least Squares
- Ridge Regression
- Lasso Regression
- Logistic Regression
- Random Forest
- XGBoost

Regression performance is evaluated using **RMSE**, **MAE**, and out-of-sample **R²**. Classification performance is evaluated using **accuracy** and **ROC-AUC**.

## Repository Structure

- `index.qmd`: website homepage
- `report.qmd`: final written report
- `interactive-viz.qmd`: interactive Plotly visualizations
- `about.qmd`: author and project context page
- `_quarto.yml`: Quarto website configuration
- `styles.css`: custom website styling
- `report.pdf`: downloadable PDF version of the final report
- `data/`: saved datasets and model outputs
- `README.md`: repository overview and reproducibility notes

## Reproducibility

The project uses saved data files and saved model outputs to avoid repeated API calls and long model-fitting times during website rendering. The repository includes the source code used for data acquisition, cleaning, feature engineering, modeling, evaluation, and visualization.

To render the website locally, run:

```bash
quarto render