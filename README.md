# Shipment Delay Prediction & Explainability System

A complete end-to-end machine learning pipeline for predicting shipment delays in logistics operations, with a strong focus on explainability, data integrity, and production readiness.

---

## Overview

This project builds a predictive system that estimates whether a shipment will be delayed and by how much, using historical logistics data.

It combines:

* Classification (delay / no delay)
* Regression (delay duration)
* Explainable AI (SHAP)
* Production-ready pipeline

---

## Objectives

* Predict shipment delays before delivery
* Estimate delay duration in hours
* Identify key factors driving delays
* Provide interpretable insights for business decisions

---

## Key Features

* Advanced Feature Engineering

  * Speed requirements
  * Route-level statistics
  * Partner performance metrics

* ML Pipeline (Scikit-learn)

  * Preprocessing + Model in one pipeline
  * No data leakage in transformations

* Explainability (SHAP)

  * Global feature importance
  * Local prediction explanations

* Production-Oriented Design

  * Saved models with `joblib`
  * Inference function (`predict_shipment_delay`)
  * Risk categorization (Low / Medium / High)

---

## Models Used

* Logistic Regression
* Random Forest
* Gradient Boosting
* (Optional) XGBoost / LightGBM

---

## Evaluation

* Classification:

  * Accuracy
  * F1-score
  * ROC-AUC

* Regression:

  * RMSE (global)

> Note: The regression model predicts both early and delayed deliveries. Business focus is primarily on delayed shipments.

---

## Important Considerations

* Avoided target leakage by removing post-delivery features
* Target encoding computed on training data only
* Stratified train-test split used
* SHAP used for model interpretability

---

##  How to Run

```bash
git clone https://github.com/your-username/shipment-delay-prediction-system.git
cd shipment-delay-prediction-system
pip install -r requirements.txt
```

Run the notebook:

```bash
jupyter notebook
```

---

## Future Improvements

* Hyperparameter tuning (RandomizedSearchCV)
* Cross-validation
* Time-based data splitting
* Threshold optimization for classification
* Real-time deployment (API)

---

## Author

Abdullah Ashraf Emara
AI Engineer

---

## ⭐ If you found this useful

Feel free to ⭐ the repo and share feedback!
