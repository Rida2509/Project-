# Project-
# Capital Structure Determinants - Trade-off Theory vs Pecking Order Theory

An empirical capital structure model built in Python to test whether the financing behavior of US public companies follows Trade-off Theory or Pecking Order Theory, using firm-level financial data derived from SEC filings.

## Dataset

Source: [Financial Statement Data Sets (Company Facts) - Kaggle](https://www.kaggle.com/datasets/vadimvanak/company-facts-2)

The dataset contains US-GAAP financial statement data extracted from SEC EDGAR filings of listed United States companies from January 2009 onward, provided as raw XBRL facts across 9,641 unique tags, together with filing-level metadata.

## Project Steps

1. Environment Setup and Data Ingestion
2. Filtering to Required Financial Tags
3. Merging with Filing Metadata and Restriction to Annual (10-K) Filings
4. Deduplication and Correction of Financial Values
5. Reshaping to a Company-Year Panel
6. Recovery of Missing Liabilities Using the Accounting Identity
7. Construction of Capital Structure Variables
8. Outlier Treatment and Winsorization
9. Descriptive Statistics and Exploratory Data Analysis
10. Correlation Analysis
11. OLS Regression Modeling
12. Sector-Level Leverage Analysis

## Key Findings

- Final analytical panel consists of 9,733 firm-year observations across approximately 6,600 unique companies
- Profitability shows a negative and statistically significant relationship with Leverage in both regression models (coefficients of -0.2305 and -0.3425), supporting Pecking Order Theory over Trade-off Theory
- Tangibility shows a positive and statistically significant relationship with Leverage in the larger sample, consistent with tangible assets serving as collateral
- Size shows a small positive and statistically significant relationship with Leverage in the larger sample
- Revenue Growth shows no statistically significant relationship with Leverage
- Retail Trade, Agriculture, and Wholesale Trade show the highest average leverage by sector, while Manufacturing and Finance, Insurance, and Real Estate show the lowest

## Tools and Libraries

- Python 3
- Pandas, NumPy
- PyArrow
- Statsmodels (OLS Regression)
- Matplotlib, Seaborn
- Jupyter Notebook

## Setup

1. Clone this repository
2. Install the required packages: pandas, pyarrow, numpy, matplotlib, seaborn, statsmodels
3. Add your Kaggle API credentials (kaggle.json) to download the dataset
4. Run `Untitled1.ipynb` cells in sequence to reproduce the full analysis

## Author

Rida Mustafa
