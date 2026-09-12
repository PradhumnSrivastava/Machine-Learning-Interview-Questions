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

---

## Interview Question

### What is overfitting, and how can you prevent it?

**Answer:** Overfitting occurs when a machine learning model learns the training data too closely, including noise and random patterns, resulting in excellent training performance but poor performance on unseen data. Common ways to reduce overfitting include using a simpler model, applying regularization, collecting more training data, performing feature selection, using cross-validation, applying early stopping in neural networks, and using ensemble methods such as random forests.

---

## Interview Question

### What is underfitting, and how can you fix it?

**Answer:** Underfitting occurs when a model is too simple to capture the underlying patterns in the data, resulting in poor performance on both the training and test datasets. It can be addressed by using a more complex model, adding informative features, reducing excessive regularization, training the model for longer when appropriate, or improving the feature engineering process.

---

## Interview Question

### What is the bias-variance tradeoff?

**Answer:** The bias-variance tradeoff describes the balance between two sources of prediction error. High bias means the model makes overly simplistic assumptions and may underfit the data, while high variance means the model is highly sensitive to the training data and may overfit. The goal is to choose a model complexity that achieves a good balance between bias and variance and therefore generalizes well to unseen data.

---

## Interview Question

### What is the difference between training error and test error?

**Answer:** Training error is the error calculated on the same data used to train the model, while test error measures the model's performance on previously unseen data. A large difference between low training error and high test error is often an indication of overfitting. Test error provides a better estimate of how the model is likely to perform on new real-world data.

---

## Interview Question

### What is the difference between parameters and hyperparameters?

**Answer:** Parameters are values learned automatically by a machine learning model during training, such as the weights in linear regression or neural networks. Hyperparameters are configuration values specified before or during training that control the learning process or model structure, such as the learning rate, maximum tree depth, number of trees, or regularization strength. Hyperparameters are typically selected using techniques such as grid search, random search, or Bayesian optimization.

---

## Interview Question

### What is regularization in machine learning?

**Answer:** Regularization is a technique used to reduce overfitting by adding a penalty for model complexity to the objective function. L1 regularization adds a penalty based on the absolute values of the model coefficients and can drive some coefficients to zero, enabling feature selection. L2 regularization adds a penalty based on the squared coefficients and tends to shrink coefficients toward zero. Regularization encourages the model to learn simpler patterns that generalize better.

---

## Interview Question

### What is the difference between L1 and L2 regularization?

**Answer:** L1 regularization adds a penalty proportional to the absolute value of model coefficients, while L2 regularization adds a penalty proportional to the squared value of the coefficients. L1 can produce sparse models because some coefficients can become exactly zero, making it useful for feature selection. L2 generally keeps all features but reduces the magnitude of their coefficients and is often more stable when features are correlated.

---

## Interview Question

### What is data leakage in machine learning?

**Answer:** Data leakage occurs when information that would not be available at prediction time is unintentionally used during model training. This can lead to unrealistically high validation or test performance while causing poor performance in production. Examples include scaling the entire dataset before splitting it into training and test sets, using future information in time-series prediction, or including features that are directly derived from the target variable. Data preprocessing and feature engineering should therefore be performed using only information available from the appropriate training data.

---

## Interview Question

### What is the difference between a validation set and a test set?

**Answer:** A validation set is used during model development to compare models, tune hyperparameters, and make design decisions. A test set is kept separate and is used only for the final evaluation of the selected model. The test set should not influence model selection because repeatedly using it during development can lead to the overfitting to the test data and produce an overly optimistic estimate of generalization performance.

---

## Interview Question

### What is overfitting and how can you prevent it?

**Answer:** Overfitting occurs when a machine learning model learns the training data too closely, including noise and random patterns, resulting in poor performance on unseen data. It can be prevented using cross-validation, regularization, pruning, feature selection, dropout for neural networks, and by collecting more training data.

---

## Interview Question

### What is underfitting in machine learning?

**Answer:** Underfitting occurs when a model is too simple to capture the underlying patterns in the data. It performs poorly on both training and unseen data. It can be reduced by using a more complex model, adding useful features, reducing excessive regularization, or training the model for longer.
