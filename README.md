# 📊 HAMS Data Science Challenge – Bayesian Media Mix Modeling

## 🧠 Overview

This repository contains my solution to the **HAMS Data Science Challenge**, focused on applying a **Bayesian Media Mix Model (MMM)** using **PyMC** to evaluate the effectiveness of marketing spend across seven paid channels.

The goal was to model delayed effects of marketing, estimate uncertainty, and derive channel-specific return on investment (ROI).


---

## 📁 Folder Structure

| Path | Description |
|------|-------------|
| `DataScience_202209/MMM_test_data.csv` | Provided dataset with weekly revenue and spend for 7 channels |
| `Notebook_Shayekh_Mohiuddin_Ahmed_Navid_DataScience_202209.ipynb` | Full analysis notebook: EDA, modeling, inference, validation, insights |
| `Report.pdf` | A 4-page summary report with modeling overview, insights, and answers to challenge questions |
| `README.md` | This file |

---

## 🔍 Approach Summary

- Performed exploratory data analysis to understand revenue trends, channel behavior, and correlations
- Modeled **carryover effects** using exponential adstock transformations
- Built a Bayesian regression model using **PyMC v5**
- Included trend and seasonality as control features
- Validated model with **posterior predictive checks** and visual fit
- Estimated **ROI per channel** from posterior samples
- Tested model robustness by comparing results with and without Channel 7

---

## ✅ Key Insights

- **Channel 5** emerged as the strongest performer in both ROI and impact
- **Channel 3** showed low ROI and limited contribution
- **Channel 7**, despite high spend, had a weaker marginal effect
- The model captured delayed effects and time dynamics effectively

---

## 📦 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/shayekh00/DataScience_202209_Solution.git
   cd DataScience_202209_Solution
