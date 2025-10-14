# Supervised Learning Project — Breast Cancer Classification

This repository contains the complete project for a **supervised learning** task (classification): predicting whether a tumor is malignant or benign using diagnostic features.

Contents
- `notebooks/Final_Project_Supervised_Learning_Breast_Cancer.ipynb` — main report-style notebook with EDA, cleaning, modeling, and conclusions.
- `SLIDES.md` — talk-track slides outline for your 5–15 minute video.
- `VIDEO_SCRIPT.md` — a concise script you can narrate while screen‑recording.
- `requirements.txt` — Python dependencies.
- `figures/` — (optional) save generated plots here if exporting.
- `data/` — empty dir (no large/binary files committed).

Problem
- **Type:** Supervised learning — **binary classification**.  
- **Goal:** Predict `malignant` (1) vs `benign` (0) given 30 diagnostic features.  
- **Why it matters:** Better triage and prioritization can assist clinical workflows.

Data
- **Source:** `sklearn.datasets.load_breast_cancer()` — *Breast Cancer Wisconsin (Diagnostic)*, originally by W. H. Wolberg, W. N. Street, and O. L. Mangasarian (UCI ML Repository).  
- **Size:** 569 samples, 30 numeric features.
- **License/Use:** Educational/research use via scikit‑learn.

> Note: The notebook **simulates small missingness** to demonstrate data cleaning and imputation for grading purposes.

Methods
- **EDA:** Descriptives, class balance, correlation heatmap, outlier handling (winsorization).  
- **Models:** Logistic Regression, SVC (RBF), Random Forest.  
- **Validation:** 5‑fold Stratified CV; grid search on key hyperparameters.  
- **Metrics:** Accuracy, Precision, Recall, F1, ROC‑AUC (primary).  
- **Fairness/Imbalance:** Used `class_weight='balanced'` where appropriate.

## 📜 Citation
- Wolberg, W. H., Street, W. N., &amp; Mangasarian, O. L. (1995). Breast Cancer Wisconsin (Diagnostic) Data Set. UCI Machine Learning Repository.
- scikit-learn: Pedregosa et al. (2011). *Journal of Machine Learning Research*.

## 📁 GitHub Tips
- Keep large files (data/videos) **out** of git; link them instead.
- Consider enabling notebook diffs with tools like ReviewNB.

---
*Prepared for the Supervised Learning Final Project.*
