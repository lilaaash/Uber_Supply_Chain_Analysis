# 🚕 Uber Supply Chain: Solving the 58% Fulfillment Gap

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]([PASTE_YOUR_COLAB_URL_HERE](https://colab.research.google.com/github/lilaaash/Uber_Supply_Chain_Analysis/blob/main/Uber_Supply_Chain_Analysis.ipynb))
![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Industry](https://img.shields.io/badge/Industry-Logistics%20%26%20Supply%20Chain-06C167)

## 📖 Project Overview
Analyzing Uber's service reliability between City and Airport hubs to identify supply-demand mismatches and revenue leakage.

## ⚠️ Problem Statement
Uber is facing a **58% service failure rate**. This analysis diagnoses whether these failures are caused by driver behavior (cancellations) or physical inventory shortages (no cars available).

## 📊 Datasets Summary
* **Volume:** 6,745 ride requests.
* **Nodes:** City and Airport pickup points.
* **Attributes:** Timestamps, Trip Status, and Driver IDs.

## 🛠️ Tools Used
* **Language:** Python 3.x
* **Libraries:** Pandas (Cleaning), Seaborn & Matplotlib (Visuals).
* **Environment:** Google Colab & GitHub.

## 🧪 Methodology & Analytical Approach

### 1. Data Cleaning & Preparation
* **Temporal Normalization:** Developed parsing logic to standardize inconsistent date delimiters (handling `/` and `-`), ensuring 100% chronological accuracy.
* **Structural Integrity:** Conducted a missing value audit, identifying `NaN` values in `Driver ID` as a business signal for **Inventory Stockouts** rather than data errors.
* **Feature Engineering:** Derived a `Request Hour` attribute to discretize the 24-hour cycle into **5 Strategic Time-Bins** for granular bottleneck identification.

🧪 Methodology & Analytical Approach
* **Data Normalization:** Standardized inconsistent date delimiters (`/` and `-`) to ensure chronological integrity.
* **Feature Engineering:** Engineered raw timestamps into **5 Strategic Time-Bins** to isolate peak-hour failure modes.
* **Logistics Logic:** Classified `NaN` values as **Inventory Stockouts** rather than missing data to measure true supply-demand gaps.
* **Multivariate EDA:** Correlated trip status with geographic nodes to identify mirrored bottlenecks.

## 📉 Summary of Analysis & Visualizations
> **Insight:** We found a mirrored bottleneck. City failures are driven by cancellations in the morning; Airport failures are driven by car shortages in the evening.

![Executive Dashboard](ExecutiveDashboard.png)

## 🚀 Strategic Recommendations
* **Morning (City):** Incentivize airport-bound trips to prevent cancellations.
* **Evening (Airport):** Pre-position "idle" city drivers to the airport 30 minutes before peak flight landings.

## 📦 Deliverables
1. **Interactive Notebook:** [View on Google Colab](PASTE_YOUR_COLAB_URL_HERE)
2. **Cleaned Data:** Available in the repository root.

## 📚 Data Source & Citation
* **Author:** Manish Kumar (UpGrad/IIIT-B).
* **Source:** [Kaggle - Uber Request Data](https://www.kaggle.com/datasets/hellbuoy/uber-supplydemand-gap).
