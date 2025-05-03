# Home Credit Default Risk

> **b2metric Case Study**\
> **Author:** Bora Boyacıoğlu\
> **E-Mail:** boraboyacioglu@icloud.com

This repository contains my solution for the Home Credit Default Risk prediction task. I applied a full machine learning workflow, from data cleaning to model explanation.

## Project Steps

1. **Data Cleaning**
   - Removed outliers from numeric features.
   - Handled missing values with imputations or simple replacements.

2. **Feature Engineering**
   - Created new features such as income-to-credit ratios and flags.
   - Selected important features using **LOFO Importance**.

3. **Model Training**
   - Trained two models: **CatBoostClassifier** and **RidgeClassifier**.
   - Used **StratifiedKFold Cross-Validation** for evaluation.

4. **Hyperparameter Tuning**
   - Tuned hyperparameters using **Optuna** for both models.

5. **Model Explanation**
   - Used **SHAP** to explain CatBoost predictions.

## Results

| Model        | ROC-AUC |
|--------------|---------|
| CatBoost      | ~0.76   |
| Ridge Classifier | ~0.75   |

There was only a small improvement after tuning and adding new features.

## 💡 Insights

- The dataset was challenging, with many weak features.
- CatBoost already captures feature interactions well.
- Better domain-specific features could help further.

## 📝 Final Comments

This project included the full ML process:
- Outlier detection
- Feature engineering
- Model training & validation
- Parameter tuning
- Model explanation

Although the model scores didn’t increase much, this experiment helped me practice a complete pipeline from scratch.