# Cost-Aware Credit Card Fraud Detection

Judging fraud detection models by **the money they save**, not by accuracy.

## The problem
Fraud is very rare: only about 0.17% of card transactions in this dataset are fraud.
A model that never flags anything is already 99.8% "accurate" but catches no fraud.
This project compares models by cost instead:
- a **missed fraud** costs the stolen amount
- a **false alarm** costs an analyst's time to review it

## Dataset
**Credit Card Fraud Detection** – Machine Learning Group, Université Libre de Bruxelles (ULB)
- Link: [Kaggle – Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- 284,807 transactions from two days in September 2013 (European cardholders)
- 492 frauds (about 0.17%)

The data file is not stored in this repository. Download `creditcard.csv` from the Kaggle link above.

## Research questions
1. Do models rank differently when judged by cost instead of usual scores (F1, precision-recall)?
2. Do SMOTE, undersampling, or class weights actually lower the cost?
3. When few fraud labels are available, can anomaly detection compete with supervised models?
4. If analysts can only review a fixed number of alerts per day, which model catches the most fraud money?

## Tools
Python · pandas · scikit-learn · matplotlib · Jupyter Notebook

## Status
- [x] Milestone 1: project proposal
- [ ] Data audit
- [ ] Models and cost-based evaluation
- [ ] Final report
