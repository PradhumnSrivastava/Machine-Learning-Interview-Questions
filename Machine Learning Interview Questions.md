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

---

## Interview Question

### What is the bias-variance tradeoff?

**Answer:** The bias-variance tradeoff is the balance between underfitting and overfitting. High bias means the model is too simple and tends to underfit, while high variance means the model is too sensitive to training data and tends to overfit. A good model aims to find a balance between bias and variance.

---

## Interview Question

### What is cross-validation and why is it used?

**Answer:** Cross-validation is a model evaluation technique in which the dataset is divided into multiple folds. The model is trained on some folds and validated on the remaining fold, repeating the process so each fold is used for validation. It provides a more reliable estimate of model performance and helps in model selection and hyperparameter tuning.

---

## Interview Question

### What is regularization in machine learning?

**Answer:** Regularization is a technique used to reduce overfitting by adding a penalty for model complexity to the loss function. L1 regularization can drive some feature coefficients to zero, while L2 regularization shrinks coefficients toward zero without usually making them exactly zero.

---

## Interview Question

### What is the difference between L1 and L2 regularization?

**Answer:** L1 regularization adds the absolute values of model coefficients to the loss function and can produce sparse models by making some coefficients exactly zero. L2 regularization adds the squared values of coefficients and generally shrinks them toward zero. L1 is useful for feature selection, while L2 is useful for controlling model complexity.

---

## Interview Question

### What is hyperparameter tuning?

**Answer:** Hyperparameter tuning is the process of finding the best values for parameters that are set before model training, such as learning rate, tree depth, number of estimators, or regularization strength. Common techniques include grid search, random search, and Bayesian optimization.

---

## Interview Question

### What is the difference between a parameter and a hyperparameter?

**Answer:** A parameter is learned automatically from the training data during model training, such as weights and coefficients. A hyperparameter is specified before training and controls the learning process or model structure, such as learning rate, maximum tree depth, or the number of trees in a random forest.

---

## Interview Question

### What is an ensemble learning method?

**Answer:** Ensemble learning combines predictions from multiple models to produce a stronger and more robust prediction. Bagging, boosting, and stacking are common ensemble techniques. Examples include Random Forest, AdaBoost, Gradient Boosting, and XGBoost.

---

## Interview Question

### What is the difference between bagging and boosting?

**Answer:** Bagging trains multiple models independently, usually on different bootstrap samples, and combines their predictions to reduce variance. Boosting trains models sequentially, where each new model focuses more on errors made by previous models, primarily improving predictive performance and reducing bias.

---

## Interview Question

### What is Linear Regression and how does it work?

**Answer:** Linear Regression is a supervised machine learning algorithm used to predict a continuous target variable. It models the relationship between input features and the target using a linear equation. The model learns the coefficients that minimize the difference between actual and predicted values, typically using the Ordinary Least Squares method.

---

## Interview Question

### What is the equation of simple Linear Regression?

**Answer:** The equation of simple Linear Regression is ŷ = b₀ + b₁x, where ŷ is the predicted value, b₀ is the intercept, b₁ is the coefficient or slope, and x is the input feature. The slope represents the expected change in the target variable for a one-unit increase in the feature.

---

## Interview Question

### What is the difference between simple and multiple Linear Regression?

**Answer:** Simple Linear Regression uses only one independent variable to predict the target, while Multiple Linear Regression uses two or more independent variables. Simple Linear Regression can be represented as ŷ = b₀ + b₁x, whereas Multiple Linear Regression is represented as ŷ = b₀ + b₁x₁ + b₂x₂ + ... + bₙxₙ.

---

## Interview Question

### How does Ordinary Least Squares work in Linear Regression?

**Answer:** Ordinary Least Squares estimates the model coefficients by minimizing the sum of squared residuals between the actual and predicted target values. The objective is to find the line that produces the smallest total squared error across the training observations.

---

## Interview Question

### What is the cost function used in Linear Regression?

**Answer:** A common cost function for Linear Regression is Mean Squared Error, which calculates the average of the squared differences between actual and predicted values. The model tries to find coefficients that minimize this error. Squaring the errors also gives greater importance to larger prediction errors.

---

## Interview Question

### What assumptions does Linear Regression make?

**Answer:** Important assumptions include linearity between predictors and the target, independence of observations, constant variance of errors or homoscedasticity, normally distributed residuals for reliable statistical inference, and low or no perfect multicollinearity among independent variables.

---

## Interview Question

### What is the difference between R-squared and Adjusted R-squared?

**Answer:** R-squared measures the proportion of variance in the target variable explained by the model. However, R-squared generally does not decrease when unnecessary features are added. Adjusted R-squared accounts for the number of predictors and can decrease when irrelevant features are added, making it more useful for comparing models with different numbers of features.

---

## Interview Question

### What is multicollinearity in Linear Regression and why is it a problem?

**Answer:** Multicollinearity occurs when two or more independent variables are highly correlated with each other. It makes coefficient estimates unstable, increases their variance, and makes it difficult to determine the individual effect of each feature. Variance Inflation Factor, or VIF, is commonly used to detect multicollinearity.

---

## Interview Question

### What is the difference between Linear Regression and Logistic Regression?

**Answer:** Linear Regression is primarily used to predict continuous numerical values, such as house prices or sales. Logistic Regression is used for classification problems and predicts probabilities that can be converted into class labels. Linear Regression produces an unbounded continuous output, while Logistic Regression uses a sigmoid function to produce values between 0 and 1.

---

## Interview Question

### What is the difference between Linear Regression and Ridge Regression?

**Answer:** Linear Regression minimizes the prediction error without a regularization penalty, while Ridge Regression adds an L2 regularization penalty to the loss function. Ridge Regression shrinks model coefficients toward zero and can help reduce overfitting and handle multicollinearity more effectively.

---

## Interview Question

### Why is Mean Squared Error commonly used as the loss function in Linear Regression?

**Answer:** Mean Squared Error measures the average squared difference between actual and predicted values. Squaring makes all errors positive and penalizes larger errors more heavily. It is also differentiable, which makes it convenient for optimization methods such as gradient descent.

---

## Interview Question

### What is the role of the intercept in Linear Regression?

**Answer:** The intercept is the predicted value of the target when all input features are zero. It represents the point where the regression line or hyperplane crosses the target axis. In multiple Linear Regression, it provides the baseline prediction before considering the effects of the features.

---

## Interview Question

### What is a residual in Linear Regression?

**Answer:** A residual is the difference between an observed target value and the value predicted by the regression model. It is calculated as residual = actual value - predicted value. Residuals are useful for evaluating model fit and checking whether important assumptions of Linear Regression are satisfied.

---

## Interview Question

### What is homoscedasticity and why is it important in Linear Regression?

**Answer:** Homoscedasticity means that the variance of the residuals remains approximately constant across different levels of the predicted values or independent variables. It is important because heteroscedasticity can make standard errors and statistical inference unreliable, even though the coefficient estimates may still be unbiased under certain conditions.

---

## Interview Question

### What is heteroscedasticity in Linear Regression and how can you detect it?

**Answer:** Heteroscedasticity occurs when the variance of residuals changes across different levels of the predictors or fitted values. It can be detected using residual plots, where a funnel-shaped pattern may indicate unequal variance, or statistical tests such as the Breusch-Pagan test. Transformations such as log transformation or using robust standard errors can help address it.

---

## Interview Question

### Why can outliers be a problem in Linear Regression?

**Answer:** Linear Regression is sensitive to outliers because the squared-error loss gives large errors disproportionately high influence. A few extreme observations can significantly change the fitted coefficients and regression line. Outliers should be investigated carefully and handled using valid methods such as data correction, transformation, robust regression, or appropriate removal when justified.

---

## Interview Question

### What is the difference between correlation and the coefficient in Linear Regression?

**Answer:** Correlation measures the strength and direction of the linear relationship between two variables and is symmetric, meaning the correlation between X and Y is the same as between Y and X. A regression coefficient describes the expected change in the target for a one-unit change in a predictor while holding other predictors constant in a multiple regression model.

---

## Interview Question

### Can Linear Regression be solved using Gradient Descent?

**Answer:** Yes, Linear Regression can be optimized using Gradient Descent. Gradient Descent starts with initial parameter values and repeatedly updates the coefficients in the direction that reduces the loss function. For large datasets, variants such as Stochastic Gradient Descent or Mini-Batch Gradient Descent can be more computationally efficient than calculating the exact solution using the normal equation.

---

## Interview Question

### What is the Normal Equation in Linear Regression?

**Answer:** The Normal Equation is a closed-form mathematical solution for finding the coefficients that minimize the squared error in Linear Regression. In matrix form, the solution is β = (XᵀX)⁻¹Xᵀy when the inverse exists. It does not require iterative optimization, but computing the matrix inverse can become expensive for datasets with a very large number of features.

---

## Interview Question

### Why should categorical variables be encoded before using Linear Regression?

**Answer:** Linear Regression requires numerical input features, so categorical variables must be converted into numerical representations. One common approach is One-Hot Encoding, which creates binary indicator variables for categories. Care must be taken to avoid perfect multicollinearity, often by dropping one category when an intercept is included.

---

## Interview Question

### Why does the Ordinary Least Squares estimator have a closed-form solution, and when can this solution become problematic?

**Answer:** Ordinary Least Squares minimizes a quadratic loss function, whose derivative with respect to the coefficients produces a system of linear equations. Solving these equations gives the closed-form solution β = (XᵀX)⁻¹Xᵀy. It can become problematic when XᵀX is singular or nearly singular due to perfect or strong multicollinearity, and matrix inversion can also be computationally expensive when the number of features is very large.

---

## Interview Question

### What is the Gauss-Markov theorem and why is it important for Linear Regression?

**Answer:** The Gauss-Markov theorem states that under assumptions such as linearity, zero conditional mean of errors, no perfect multicollinearity, and constant error variance, the Ordinary Least Squares estimator is the Best Linear Unbiased Estimator, or BLUE. Best means it has the lowest variance among all linear unbiased estimators. The theorem does not require normally distributed errors.

---

## Interview Question

### Why is the OLS estimator unbiased, and what assumption is mainly responsible for this property?

**Answer:** The OLS estimator is unbiased when the conditional expectation of the error given the predictors is zero, written as E[ε|X] = 0. This means that the predictors do not systematically contain information about the error term. Under this assumption, the expected value of the estimated coefficients equals the true population coefficients.

---

## Interview Question

### What happens to Linear Regression coefficients when there is perfect multicollinearity?

**Answer:** With perfect multicollinearity, one or more predictors can be represented exactly as a linear combination of other predictors. As a result, XᵀX becomes singular and the unique OLS coefficient estimates cannot be computed using the standard normal equation. The issue can be addressed by removing redundant features or using regularization techniques such as Ridge Regression.

---

## Interview Question

### Why does Ridge Regression help with multicollinearity, and why does Lasso behave differently?

**Answer:** Ridge Regression adds an L2 penalty that shrinks correlated feature coefficients toward zero, which reduces coefficient variance and improves numerical stability. Lasso adds an L1 penalty, which can force some coefficients exactly to zero and therefore perform implicit feature selection. With highly correlated features, Lasso may arbitrarily select one or distribute the effect unevenly, while Ridge tends to distribute weights more smoothly among correlated predictors.

---

## Interview Question

### What is the difference between statistical significance of a regression coefficient and its practical significance?

**Answer:** Statistical significance indicates whether the observed coefficient is unlikely to have occurred by chance under a specified null hypothesis, often evaluated using a p-value and confidence interval. Practical significance concerns whether the magnitude of the effect is large enough to matter in the real-world application. A coefficient can be statistically significant but practically negligible, especially with a very large dataset.

---

## Interview Question

### What is endogeneity in Linear Regression, and why does it cause biased estimates?

**Answer:** Endogeneity occurs when a predictor is correlated with the error term, meaning E[ε|X] is not zero. It can arise from omitted variables, measurement error, or simultaneous causality. When endogeneity exists, OLS coefficients can become biased and inconsistent, meaning increasing the sample size does not necessarily make the estimates converge to the true parameters.

---

## Interview Question

### How does omitted variable bias affect a Linear Regression model?

**Answer:** Omitted variable bias occurs when an important variable that affects the target is excluded from the model and is correlated with an included predictor. The included predictor can then partially capture the effect of the omitted variable, causing its estimated coefficient to be biased. Adding the relevant variable or using appropriate causal or instrumental-variable methods can help address the problem.

---

## Interview Question

### Why does scaling affect Gradient Descent in Linear Regression but not the OLS prediction theoretically?

**Answer:** Feature scaling can greatly affect the optimization path and convergence speed of Gradient Descent because features with very different scales create an elongated loss surface, making optimization slower. In ordinary Linear Regression, rescaling a feature changes its coefficient correspondingly, but the model's fitted predictions remain theoretically equivalent when the transformation is handled consistently.
