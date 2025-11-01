# Supply Chain Demand & Operations Analysis

## Project summary

This repository contains exploratory analysis and modeling experiments for a supply-chain dataset (uploaded as supply_chain_data.csv) and the analysis notebook experiments.ipynb.

The goal of the analysis is to understand demand patterns, inventory levels, lead times and cost drivers and to develop forecasting and optimization models that can reduce stockouts, lower costs, and improve on-time delivery.

## Contents

- supply_chain_data.csv — raw dataset used for analysis

- experiments.ipynb — Jupyter notebook containing EDA, visualizations and modeling experiments

- README.md — this file (project overview, key findings, how to reproduce and next steps)

## Dataset overview

- Rows: 100

- Columns: 24

- Numeric columns: 15

- Missing values: none detected in the uploaded CSV (no columns with missing counts > 0)

## Example columns

Product type, SKU, Price, Availability, Number of products sold, Revenue generated, Stock levels, Lead times, Order quantities, Shipping times, Shipping costs, Supplier name, Location, Production volumes, Manufacturing costs, Defect rates, Costs, etc.

## Key EDA findings

The following concise statistics were extracted programmatically from the dataset:

- Average price: ~ ₹49.46

- Average number of units sold (per record): ~ 461

- Average revenue (per record): ~ ₹5,776.05

- Average stock level (per record): ~ 47.77 units

- Average lead time: ~ 15.96 days

- Average shipping cost (per shipment/record): ~ ₹5.55

- Average total costs (per record): ~ ₹529.25

Top correlated variable pairs (absolute Pearson correlations) — these are the strongest relationships found among numeric features (absolute correlation shown):

- Price ↔ Manufacturing lead time: 0.301

- Defect rates ↔ Lead time: 0.297

- Costs ↔ Lead times: 0.244

- Revenue generated ↔ Manufacturing costs: 0.214

- Production volumes ↔ Lead time: 0.213

Interpretation: Lead times and manufacturing-related variables (manufacturing lead time, defect rates, production volumes) show the strongest associations with other operational metrics. Costs and lead time are also moderately correlated, suggesting that reducing lead time could help lower costs.