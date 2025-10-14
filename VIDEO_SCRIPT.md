# VIDEO_SCRIPT.md — 10-minute Talk Track

**Opening (0:00–0:30)**  
Hi, I’m <Your Name>. This is a short walkthrough of my supervised learning project: predicting malignant vs benign breast tumors.

**Problem & Goal (0:30–1:30)**  
- Objective: Given diagnostic features, classify tumors as malignant (1) or benign (0).  
- Value: Faster triage to support clinical workflows.  
- Primary metric: ROC‑AUC, with F1 and Recall as supporting metrics.

**Data (1:30–2:15)**  
- Source: scikit‑learn Breast Cancer Wisconsin (Diagnostic).  
- 569 samples, 30 numeric features.  
- I simulate ~3% missingness to demonstrate cleaning and imputation.

**EDA (2:15–3:30)**  
- Class balance is slightly imbalanced; benign is more common.  
- Correlation heatmap reveals correlated radius/area/concavity families.  
- Outliers handled via winsorization (1st/99th percentile).

**Modeling (3:30–6:00)**  
- 3 models: Logistic Regression (scaled), SVC RBF (scaled), Random Forest (class_weight balanced).  
- 5‑fold stratified CV and grid search (C, gamma, depth, estimators).  
- Overfitting mitigation: regularization, cross‑validation, and balanced class weights.

**Results (6:00–8:00)**  
- Compare models on test set: show AUC, F1, Precision, Recall, Accuracy.  
- Display ROC overlays and confusion matrix.  
- Best model: <filled by run> with AUC ≈ <value>. Key features include <feature names>.

**Conclusion & Next Steps (8:00–9:00)**  
- What worked: Robust preprocessing + tuned models yielded strong AUC.  
- Improvements: Probability calibration, threshold tuning, SHAP, more models (GBM/XGBoost).

**Demo (9:00–10:00)**  
- Run the evaluation cell in the notebook, show metrics/plots.  
- Point viewers to GitHub and the notebook for details.

**Closing**  
Thanks for watching! Links are in the README.
