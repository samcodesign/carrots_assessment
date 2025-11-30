# Carrots Product Analyst Assessment

Small, self-contained dataset and notebook for the Carrots analyst assessment. The repo keeps the source CSV exports, a PDF prompt, and the exploratory notebook used to compute KPI summaries.

## What's inside
- `carrots_analysis.ipynb` — pandas/numpy notebook used for KPI calculations.
- `kpi_conversion.csv`, `kpi_revenue_summary.csv`, `kpi_retention.csv`, `kpi_purchases_by_paywall.csv`, `kpi_packages.csv` — derived KPI tables by test variant/paywall.
- `revenuecat.csv`, `user_behaviour.csv` — raw user and RevenueCat event exports.
- `Product Analyst Intern Test.pdf` — original exercise description.

## Quickstart
1) Install Python 3.10+ and create a virtual env: `python -m venv .venv` then activate it.
2) Install dependencies: `pip install -r requirements.txt`.
3) Open the notebook to reproduce or extend the analysis: `jupyter lab carrots_analysis.ipynb` (or `jupyter notebook`).
4) Export any additional tables with `pandas.DataFrame.to_csv` to keep outputs versioned alongside the source data.

## Publishing as a public repo
This folder is already git-ready; to publish it:
1) `git init && git add . && git commit -m "Initial public repo"`
2) Create an empty public repo on GitHub (or your provider of choice).
3) Point the remote and push: `git remote add origin <git-url>` then `git push -u origin main` (or `master`, depending on your default branch).
