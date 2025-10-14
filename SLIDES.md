# Presentation Outline (SLIDES.md)

## Slide 1 — Title
**Predicting Malignant vs Benign Breast Tumors**  
Supervised Learning Final Project — Classification  
Your Name | 2025-10-14

## Slide 2 — Problem & Goal
- What problem do we solve?
- Why it matters (clinical triage)
- Goal: reliable classifier (ROC‑AUC as primary metric)

## Slide 3 — Data
- Source: sklearn Breast Cancer Wisconsin (Diagnostic)
- 569 samples, 30 numeric features
- Target mapping: 0=benign, 1=malignant

## Slide 4 — EDA Highlights
- Class balance bar plot
- Correlation heatmap
- Outliers & winsorization
- Simulated missingness → median imputation

## Slide 5 — Modeling Plan
- Logistic Regression (scaled)
- SVC (RBF, scaled)
- Random Forest (class_weight)
- 5‑fold stratified CV + GridSearch

## Slide 6 — Metrics
- Accuracy, Precision, Recall, F1
- Primary: ROC‑AUC (slight imbalance)

## Slide 7 — Results
- Table: AUC/F1/Recall/Precision per model
- ROC curves overlay

## Slide 8 — Best Model & Interpretation
- Best by ROC‑AUC
- Feature importances / coefficients

## Slide 9 — Demo
- Run the notebook cell live: evaluate best model on test set
- Show confusion matrix & ROC curve

## Slide 10 — Conclusions
- What worked & why
- Limitations
- Next steps

## Slide 11 — Links
- GitHub repo URL
- Video URL (after upload)
