# Churn Prediction (Olist)

End-to-end churn prediction case study using the Olist Brazilian ecommerce dataset.

## Goal
Identify “at-risk” customers and rank them for a retention intervention (e.g., coupons).

## Churn definition & dataset design
- **Churn horizon:** 60 days (no purchase in the next 60 days)
- **Snapshotting:** weekly customer snapshots
- **At-risk cohort:** customers with **7–60 days since last order** (actionable window)
- **Leakage prevention:** chronological train/val/test split and label cutoff near dataset end

## Evaluation
- **Top-K precision/recall/lift** (coupon budget style targeting)
- Confusion matrix / classification report for reference

## Data
CSV files are not included in this repo. Download the dataset from Kaggle and place the extracted CSVs under `data/`:
https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce

## How to run
1. Install dependencies: `pandas`, `numpy`, `scikit-learn`, `matplotlib` (and optionally `lightgbm`, `torch`)
2. Open `Churn Prediction.ipynb` and run cells top-to-bottom
