# 📊 Customer Retention Analytics Dashboard (CATE)

A production-style **causal inference dashboard** for analyzing heterogeneous treatment effects (CATE) in customer retention data using meta-learners and causal forests.

Built with **Streamlit, EconML, and Plotly**, this project demonstrates end-to-end causal ML: from model training outputs to business decision simulation.

---

## 🚀 Live Demo
https://your-app-url.streamlit.app

---

## 📌 Overview

This dashboard analyzes **treatment effect heterogeneity** across 100,000 synthetic customers to answer:

- Who benefits most from the intervention?
- Which customers should be targeted?
- What is the expected ROI of targeting policies?
- How reliable are causal estimates under confounding?

---

## 🧠 Key Features

### 📈 Causal Modeling
- T-Learner (XGBoost-based)
- X-Learner (propensity-weighted)
- Causal Forest (DML via EconML)
- Ensemble model

### 📊 Evaluation & Validation
- Qini curves (targeting performance)
- AUUC (Area Under Uplift Curve)
- Placebo permutation tests (statistical significance)
- Oracle benchmark comparison

### 👥 Customer Segmentation
- KMeans clustering (k=4)
- Segment-wise CATE analysis
- Cross-model agreement heatmaps

### 💰 Business Simulator
- ROI estimation for targeting campaigns
- Cost vs revenue modeling
- Optimal targeting threshold selection
- Interactive sensitivity analysis

---

## 🏗️ Project Structure

```text
dashboard-repo/
│
├── app.py
├── requirements.txt
├── README.md
│
├── data/
│   └── processed/
│       └── features_engineered.csv
│
├── results/
│   └── validation_results.json
│
├── models/
│   ├── causal_summary.csv
│   └── cate_predictions.csv
│
└── assets/
    └── favicon.png
