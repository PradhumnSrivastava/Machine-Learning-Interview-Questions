# Machine Learning Interview Questions

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

---

## Interview Question

### What is the difference between confidence intervals and prediction intervals in Linear Regression?

**Answer:** A confidence interval estimates the uncertainty around the expected mean response at a particular predictor value, while a prediction interval estimates the range in which an individual future observation is expected to fall. Prediction intervals are wider because they include both uncertainty in estimating the mean response and the natural variability of individual observations.

---

## Interview Question

### What is data preprocessing, and why is it important in a machine learning pipeline?

**Answer:** Data preprocessing is the process of cleaning, transforming, and preparing raw data before it is given to a machine learning model. It includes tasks such as handling missing values, encoding categorical variables, scaling numerical features, and removing inconsistent data. It is important because real-world data is often incomplete, noisy, or unsuitable for direct use by machine learning algorithms.

---

## Interview Question

### What is the difference between numerical, categorical, ordinal, and nominal data?

**Answer:** Numerical data represents quantities and can be discrete or continuous, such as age, salary, or height. Categorical data represents groups or labels, such as city or department. Ordinal data is categorical data with a meaningful order, such as Low, Medium, and High. Nominal data consists of categories without any meaningful order, such as Red, Blue, and Green.

---

## Interview Question

### How do you handle missing values in a dataset?

**Answer:** Missing values can be handled using techniques such as mean, median, or mode imputation, depending on the type of feature and data distribution. More advanced approaches include KNN imputation, regression-based imputation, and iterative imputation. If a feature contains an excessive amount of missing data and provides limited useful information, it may also be removed. The choice depends on the amount, pattern, and nature of the missing values.

---

## Interview Question

### What is the difference between mean, median, and mode imputation?

**Answer:** Mean imputation replaces missing numerical values with the average of the observed values. Median imputation replaces them with the middle value after sorting the data. Mode imputation replaces missing values with the most frequently occurring value. Median is generally preferred when numerical data is highly skewed or contains outliers because it is less affected by extreme values than the mean.

---

## Interview Question

### What is feature scaling, and why is it required for some machine learning algorithms?

**Answer:** Feature scaling transforms numerical features so that they have comparable scales. It is particularly important for distance-based and gradient-based algorithms such as KNN, K-Means, SVM, Logistic Regression, and neural networks. Without scaling, features with larger numerical ranges can disproportionately influence the model. Tree-based algorithms such as Decision Trees and Random Forests generally do not require feature scaling.

---

## Interview Question

### What is the difference between normalization and standardization?

**Answer:** Normalization commonly refers to Min-Max Scaling, which transforms values into a fixed range, usually 0 to 1, using the formula X_scaled = (X - X_min) / (X_max - X_min). Standardization transforms a feature so that it has approximately zero mean and unit variance using Z = (X - μ) / σ. Min-Max scaling is sensitive to outliers, while standardization is generally more suitable when centered features are desirable.

---

## Interview Question

### What is One-Hot Encoding, and what problem can occur when a categorical feature has many unique categories?

**Answer:** One-Hot Encoding converts each category into a separate binary feature. For example, a City column containing Delhi, Mumbai, and Jaipur can become City_Delhi, City_Mumbai, and City_Jaipur. When a feature has many unique categories, One-Hot Encoding can create a very large number of features, increasing memory usage, computational cost, and potentially the risk of overfitting.

---

## Interview Question

### What is Label Encoding, and why can it be problematic for nominal categorical features?

**Answer:** Label Encoding assigns an integer to each category, such as Red = 0, Blue = 1, and Green = 2. For nominal variables, this can be problematic because the numerical values may create an artificial ordering that does not actually exist. A model could incorrectly interpret Green as being greater than Blue and Blue as greater than Red. Therefore, One-Hot Encoding or another suitable encoding method is often preferred for nominal features.

---

## Interview Question

### Suppose a categorical feature contains 100 different categories. How would you preprocess it?

**Answer:** I would first examine the feature's cardinality, frequency distribution, relationship with the target, and the type of model being used. One-Hot Encoding would create 100 features, which may be acceptable for some datasets but inefficient for others. Alternatives include frequency encoding, target encoding, hashing, or grouping rare categories into an "Other" category. The choice should also consider dataset size, overfitting risk, computational cost, and interpretability.

---

## Interview Question

### What is data leakage during preprocessing? Give a practical example and explain how you would prevent it.

**Answer:** Data leakage occurs when information from validation or test data is unintentionally used during model training. For example, calculating the mean and standard deviation using the entire dataset before splitting it into training and test sets allows information from the test set to influence the preprocessing. To prevent this, the dataset should first be split, preprocessing parameters should be learned only from the training data, and those parameters should then be applied to validation and test data. Scikit-learn Pipeline and ColumnTransformer can help enforce this workflow.

---

## Interview Question

### What is Logistic Regression?

**Answer:** Logistic Regression is a supervised machine learning algorithm mainly used for classification problems. It predicts the probability of a class by applying the Sigmoid function to a linear combination of input features.

---

## Interview Question

### Why is Logistic Regression called Regression if it is used for Classification?

**Answer:** Logistic Regression is called regression because it models the relationship between input features and the log-odds of the target probability. Although its output is a probability, that probability is commonly converted into a class label for classification.

---

## Interview Question

### What is the mathematical equation of Logistic Regression?

**Answer:** The linear part of Logistic Regression is z = w1x1 + w2x2 + ... + wnxn + b, or z = WᵀX + b. The value z is then passed through the Sigmoid function to obtain the predicted probability.

---

## Interview Question

### What is the role of the Sigmoid function in Logistic Regression?

**Answer:** The Sigmoid function converts the linear output z into a value between 0 and 1. This value represents the predicted probability of the positive class. Its formula is σ(z) = 1 / (1 + e^(-z)).

---

## Interview Question

### How does Logistic Regression make a classification decision?

**Answer:** Logistic Regression first calculates the predicted probability using the Sigmoid function. A threshold is then applied to convert the probability into a class label. With the commonly used threshold of 0.5, a probability greater than or equal to 0.5 is classified as class 1, while a probability below 0.5 is classified as class 0.

---

## Interview Question

### What is the Loss Function used in Logistic Regression?

**Answer:** Logistic Regression commonly uses Binary Cross-Entropy Loss, also called Log Loss, for binary classification. It penalizes incorrect predictions, especially predictions made with high confidence, and provides a differentiable objective for optimization.

---

## Interview Question

### How are the weights learned in Logistic Regression?

**Answer:** The weights and bias are learned by minimizing the loss function using an optimization algorithm such as Gradient Descent. The gradients of the loss with respect to the model parameters are calculated, and the parameters are updated iteratively to reduce the loss.

---

## Interview Question

### What is the decision boundary in Logistic Regression?

**Answer:** The decision boundary is the boundary where the predicted probability reaches the classification threshold, commonly 0.5. For a standard Logistic Regression model, this corresponds to WᵀX + b = 0, which forms a linear decision boundary.

---

## Interview Question

### What are the assumptions and limitations of Logistic Regression?

**Answer:** Logistic Regression assumes a linear relationship between the input features and the log-odds of the target. It can be affected by multicollinearity, extreme outliers, and highly non-linear relationships. Standard Logistic Regression also produces a linear decision boundary unless features are transformed or additional non-linear features are introduced.

---

## Interview Question

### What is the difference between Logistic Regression and Linear Regression?

**Answer:** Linear Regression predicts continuous numerical values, while Logistic Regression predicts the probability of a class. Linear Regression commonly uses Mean Squared Error for optimization, whereas Logistic Regression commonly uses Binary Cross-Entropy or Log Loss. Logistic Regression uses the Sigmoid function for binary classification.

---

## Interview Question

### What is K-Nearest Neighbors (KNN)?

**Answer:** K-Nearest Neighbors (KNN) is a supervised machine learning algorithm used for classification and regression. It makes predictions based on the closest training data points to a new data point.

---

## Interview Question

### How does the KNN algorithm work?

**Answer:** KNN calculates the distance between a new data point and the training data points. It selects the K nearest data points and uses their labels or values to make a prediction. For classification, it usually uses majority voting, while for regression, it commonly uses the average of the neighbors' values.

---

## Interview Question

### What does K represent in KNN?

**Answer:** K represents the number of nearest neighbors considered when making a prediction. For example, if K = 5, the algorithm considers the five closest training data points to determine the prediction.

---

## Interview Question

### What distance metrics are commonly used in KNN?

**Answer:** Common distance metrics include Euclidean distance, Manhattan distance, and Minkowski distance. Euclidean distance is commonly used for continuous numerical features, while the appropriate metric depends on the nature and scale of the data.

---

## Interview Question

### How do you choose the value of K in KNN?

**Answer:** The value of K is usually selected using validation techniques such as cross-validation. A small K can make the model sensitive to noise and lead to overfitting, while a very large K can make the model too smooth and lead to underfitting.

---

## Interview Question

### Why is feature scaling important in KNN?

**Answer:** Feature scaling is important because KNN relies on distance calculations. If one feature has a much larger numerical scale than another, it can dominate the distance calculation. Standardization or normalization can help ensure that features contribute more appropriately to the distance.

---

## Interview Question

### Is KNN a parametric or non-parametric algorithm?

**Answer:** KNN is a non-parametric algorithm because it does not assume a specific probability distribution or fixed functional form for the underlying data. Instead, it makes predictions based directly on the training examples.

---

## Interview Question

### What is the difference between KNN Classification and KNN Regression?

**Answer:** KNN Classification predicts a categorical class by using the labels of the nearest neighbors, usually through majority voting. KNN Regression predicts a continuous value, commonly by taking the average of the target values of the nearest neighbors.

---

## Interview Question

### What are the advantages and disadvantages of KNN?

**Answer:** KNN is simple to understand, requires little training computation, and can model complex decision boundaries. However, prediction can be computationally expensive for large datasets, it requires appropriate feature scaling, and its performance can decrease when there are many irrelevant or high-dimensional features.

---

## Interview Question

### What is the Curse of Dimensionality in KNN?

**Answer:** The Curse of Dimensionality refers to the problems that occur when the number of features becomes very large. In high-dimensional spaces, data points tend to become relatively similar in terms of distance, making it difficult for KNN to identify meaningful nearest neighbors. Feature selection or dimensionality reduction can help address this problem.

---

## Interview Question

### Why does KNN suffer from the Curse of Dimensionality?

**Answer:** As the number of features increases, the volume of the feature space grows rapidly, making data points relatively farther apart and distances less informative. As a result, identifying meaningful nearest neighbors becomes difficult. Feature selection or dimensionality reduction can help reduce this problem.

---

## Interview Question

### How does K affect the Bias-Variance Tradeoff in KNN?

**Answer:** A small value of K makes KNN highly sensitive to individual training points, resulting in low bias but high variance and possible overfitting. A large value of K produces smoother predictions, increasing bias but reducing variance and potentially causing underfitting.

---

## Interview Question

### Why can KNN be computationally expensive during prediction?

**Answer:** KNN is a lazy learning algorithm, so it performs very little computation during training. During prediction, it may need to calculate the distance between the new data point and many or all training samples, making prediction expensive for large datasets.

---

## Interview Question

### How can KNN prediction be optimized for large datasets?

**Answer:** KNN prediction can be optimized using efficient data structures and approximate nearest-neighbor methods such as KD-Trees, Ball Trees, or specialized vector search libraries. These methods can reduce the number of distance calculations required during prediction, although their effectiveness depends on the dataset and dimensionality.

---

## Interview Question

### What is Distance-Weighted KNN?

**Answer:** Distance-Weighted KNN gives greater importance to closer neighbors and less importance to farther neighbors. Instead of giving every neighbor equal voting weight, the contribution of a neighbor is typically based on a function of its distance from the query point.

---

## Interview Question

### What happens when KNN has tied votes between classes?

**Answer:** A tie can occur when multiple classes receive the same number of votes among the selected neighbors. The tie can be handled using an odd value of K for binary classification, distance-weighted voting, or a predefined tie-breaking rule depending on the implementation.

---

## Interview Question

### How do irrelevant features affect KNN?

**Answer:** Irrelevant features can distort distance calculations because KNN relies directly on feature distances. They may make unrelated data points appear closer or meaningful points appear farther apart. Feature selection or dimensionality reduction can therefore improve KNN performance.

---

## Interview Question

### How does KNN handle missing values?

**Answer:** Standard KNN distance calculations generally cannot directly handle missing feature values. Missing values should usually be handled through appropriate preprocessing, such as imputation, before applying KNN. The imputation method should be chosen carefully to avoid introducing bias or data leakage.

---

## Interview Question

### Why is KNN sensitive to the choice of distance metric?

**Answer:** KNN determines its neighbors using a distance metric, so changing the metric can change which observations are considered nearest. Euclidean, Manhattan, Minkowski, and other metrics can produce different neighborhoods, especially when features have different distributions or structures.

---

## Interview Question

### Can KNN produce probability estimates, and how?

**Answer:** Yes. In classification, KNN can estimate class probabilities by calculating the proportion of neighbors belonging to each class. For example, if 7 out of 10 nearest neighbors belong to class 1, the basic KNN probability estimate for class 1 is 0.7. Distance-weighted KNN can produce weighted probability estimates.

---

## Interview Question

### What is K-Means Clustering?

**Answer:** K-Means is an unsupervised machine learning algorithm used to partition data into K clusters. It assigns each data point to the nearest cluster centroid and iteratively updates the centroids until the cluster assignments stabilize.

---

## Interview Question

### What does K represent in K-Means?

**Answer:** K represents the number of clusters that the algorithm is expected to create. It must be specified before training the standard K-Means algorithm.

---

## Interview Question

### How does the K-Means algorithm work?

**Answer:** K-Means starts by initializing K centroids, assigns each data point to the nearest centroid, recalculates each centroid as the mean of the points assigned to it, and repeats the assignment and update steps until convergence or a stopping condition is reached.

---

## Interview Question

### What is a centroid in K-Means?

**Answer:** A centroid is the mean position of all data points assigned to a particular cluster. It acts as the representative center of that cluster and is updated during each iteration of the algorithm.

---

## Interview Question

### What objective function does K-Means minimize?

**Answer:** K-Means minimizes the Within-Cluster Sum of Squares (WCSS), also called inertia. It is the sum of the squared distances between each data point and the centroid of its assigned cluster.
