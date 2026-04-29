# Predicting S&P 500 Returns with Macro-Financial Indicators

This repository contains my JSC370 final project website, final report, data files, and source code.

## Website

The project website is available here:

https://lijack032.github.io/JSC370-Project/

## Project Description

This project examines whether macro-financial indicators can meaningfully predict future S&P 500 returns. The analysis combines market data from Yahoo Finance with macroeconomic indicators from Federal Reserve Economic Data. The project compares benchmark models, regularized linear models, Random Forest, and XGBoost across 1-day, 5-day, and 20-day forecast horizons.

## Data Sources

- Yahoo Finance chart API
- Federal Reserve Economic Data API

The data used for the final website are stored in the `data/` folder.

## Files

- `index.qmd`: website homepage
- `report.qmd`: final written report
- `interactive-viz.qmd`: interactive visualizations
- `about.qmd`: project/about page
- `_quarto.yml`: website configuration
- `styles.css`: custom website styling
- `JSC370_Final_Report.pdf`: downloadable PDF report
- `data/`: saved data and model outputs

## Reproducibility

The project uses saved data files and saved model outputs to avoid repeated API calls and long model-fitting times during rendering. Source code for data processing, feature engineering, modeling, evaluation, and visualization is included in the repository.