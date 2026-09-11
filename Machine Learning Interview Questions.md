# Machine Learning Interview Questions

> A structured collection of Machine Learning interview questions and answers.

---

## 📊 Progress

| # | Area | Questions | Status |
|---|---|---:|---|
| 1 | ML Fundamentals | 0 / 20 | ⏳ |
| 2 | Mathematics for ML | 0 / 20 | ⏳ |
| 3 | Statistics & Probability | 0 / 20 | ⏳ |
| 4 | Data Preprocessing & Feature Engineering | 0 / 20 | ⏳ |
| 5 | Exploratory Data Analysis | 0 / 20 | ⏳ |
| 6 | Supervised Learning | 0 / 20 | ⏳ |
| 7 | Unsupervised Learning | 0 / 20 | ⏳ |
| 8 | Regression | 0 / 20 | ⏳ |
| 9 | Classification | 0 / 20 | ⏳ |
| 10 | Decision Trees | 0 / 20 | ⏳ |
| 11 | Random Forest & Bagging | 0 / 20 | ⏳ |
| 12 | Boosting Algorithms | 0 / 20 | ⏳ |
| 13 | XGBoost / LightGBM / CatBoost | 0 / 20 | ⏳ |
| 14 | Support Vector Machines | 0 / 20 | ⏳ |
| 15 | K-Nearest Neighbors | 0 / 20 | ⏳ |
| 16 | Naive Bayes | 0 / 20 | ⏳ |
| 17 | Clustering | 0 / 20 | ⏳ |
| 18 | Dimensionality Reduction | 0 / 20 | ⏳ |
| 19 | Anomaly Detection | 0 / 20 | ⏳ |
| 20 | Ensemble Learning | 0 / 20 | ⏳ |
| 21 | Model Evaluation & Metrics | 0 / 20 | ⏳ |
| 22 | Cross-Validation & Model Selection | 0 / 20 | ⏳ |
| 23 | Hyperparameter Optimization | 0 / 20 | ⏳ |
| 24 | Regularization | 0 / 20 | ⏳ |
| 25 | Feature Selection | 0 / 20 | ⏳ |
| 26 | Imbalanced Learning | 0 / 20 | ⏳ |
| 27 | Time-Series Machine Learning | 0 / 20 | ⏳ |
| 28 | Recommendation Systems | 0 / 20 | ⏳ |
| 29 | NLP & Classical ML | 0 / 20 | ⏳ |
| 30 | ML Algorithms from Scratch | 0 / 20 | ⏳ |
| 31 | Deep Learning Fundamentals | 0 / 20 | ⏳ |
| 32 | Neural Networks | 0 / 20 | ⏳ |
| 33 | CNNs | 0 / 20 | ⏳ |
| 34 | RNN / LSTM / GRU | 0 / 20 | ⏳ |
| 35 | Attention & Transformers | 0 / 20 | ⏳ |
| 36 | Generative AI Fundamentals | 0 / 20 | ⏳ |
| 37 | Model Explainability | 0 / 20 | ⏳ |
| 38 | ML System Design | 0 / 20 | ⏳ |
| 39 | MLOps & Production ML | 0 / 20 | ⏳ |
| 40 | ML Coding & Python | 0 / 20 | ⏳ |

**Total: 0 / 800 questions**

---

# 1. ML Fundamentals

---

## Daily Question

### What is overfitting?

**Answer:** _To be added._

---

## Daily Question

### What is underfitting?

**Answer:** _To be added._

---

## Daily Question

### What is the bias-variance tradeoff?

**Answer:** _To be added._

---

## Interview Question

### Explain precision, recall and F1.

**Answer:** Precision, recall, and F1-score are classification evaluation metrics. Precision tells us, out of all the instances the model predicted as positive, how many were actually positive, so it focuses on minimizing false positives. Recall tells us, out of all the actual positive instances, how many the model correctly identified, so it focuses on minimizing false negatives. F1-score is the harmonic mean of precision and recall and provides a single metric that balances both. For example, in fraud detection, if missing a fraudulent transaction is more costly, we may prioritize recall, whereas if investigating false fraud alerts is expensive, we may prioritize precision. F1-score is useful when we want a balance between precision and recall, especially when the classes are imbalanced.

---

## Interview Question

### Why can 99% accuracy be a terrible metric?

**Answer:** 99% accuracy can be a terrible metric when the dataset is highly imbalanced. For example, suppose we have 10,000 transactions, out of which 9,900 are legitimate and only 100 are fraudulent. If a model simply predicts every transaction as legitimate, it will achieve 99% accuracy, even though it detects zero fraudulent transactions. Therefore, accuracy can give a misleading impression of model performance when one class dominates the dataset. In such cases, we should also consider metrics such as precision, recall, F1-score, PR-AUC, or cost-based metrics, depending on the business objective.

---

## Interview Question

### Precision vs recall — when would you prioritize each?

**Answer:** 99% accuracy can be a terrible metric when the dataset is highly imbalanced. For example, suppose we have 10,000 transactions, out of which 9,900 are legitimate and only 100 are fraudulent. If a model simply predicts every transaction as legitimate, it will achieve 99% accuracy, even though it detects zero fraudulent transactions. Therefore, accuracy can give a misleading impression of model performance when one class dominates the dataset. In such cases, we should also consider metrics such as precision, recall, F1-score, PR-AUC, or cost-based metrics, depending on the business objective.

---

## Interview Question

### What is cross-validation, and why is it used?

**Answer:** Cross-validation is a model evaluation technique used to estimate how well a machine learning model will generalize to unseen data. In k-fold cross-validation, the dataset is divided into k subsets or folds. The model is trained on k-1 folds and validated on the remaining fold, and this process is repeated k times. The average validation performance is then used as the evaluation score. Cross-validation helps reduce the dependence of evaluation on a single train-test split and is especially useful for model selection and hyperparameter tuning.
