# Questions Inbox
## Set 2 — Data Preprocessing

### 1. What is data preprocessing, and why is it important in a machine learning pipeline?

Answer:
Data preprocessing is the process of cleaning, transforming, and preparing raw data before giving it to a machine learning model. It may include handling missing values, encoding categorical variables, scaling numerical features, removing duplicates, and handling inconsistent data. It is important because real-world data is often incomplete, noisy, or in an unsuitable format for machine learning algorithms.

---

### 2. What is the difference between numerical, categorical, ordinal, and nominal data?

Answer:
Numerical data represents quantities and can be continuous or discrete, such as age or salary. Categorical data represents groups or labels, such as gender or city. Ordinal data is categorical data that has a meaningful order, such as Low, Medium, and High. Nominal data consists of categories with no meaningful order, such as Red, Blue, and Green.

---

### 3. How do you handle missing values in a dataset?

Answer:
Missing values can be handled using several techniques. Numerical missing values can be replaced using mean or median, while categorical values can be replaced using mode. More advanced methods include KNN imputation, regression-based imputation, or iterative imputation. If a feature has too many missing values and provides little useful information, it may be removed. The choice depends on the amount and pattern of missing data and the nature of the feature.

---

### 4. What is the difference between mean, median, and mode imputation?

Answer:
Mean imputation replaces missing values with the average of the available values. Median imputation replaces them with the middle value after sorting the data. Mode imputation replaces missing values with the most frequently occurring value. Median is generally preferable to mean when the numerical feature contains significant outliers or is highly skewed because the median is less affected by extreme values.

---

### 5. What is feature scaling, and why is it required for some machine learning algorithms?

Answer:
Feature scaling is the process of bringing numerical features to a comparable scale. It is important for algorithms that depend on distances or gradient-based optimization, such as KNN, K-Means, SVM, Logistic Regression, and many neural networks. Without scaling, a feature with a larger numerical range can dominate other features. Tree-based algorithms such as Decision Trees and Random Forests generally do not require feature scaling.

---

### 6. What is the difference between Normalization and Standardization?

Answer:
Normalization usually refers to Min-Max Scaling, which transforms values into a fixed range, commonly 0 to 1.

Formula:
X_scaled = (X - X_min) / (X_max - X_min)

Standardization transforms data so that it has approximately mean 0 and standard deviation 1.

Formula:
Z = (X - μ) / σ

Min-Max scaling is sensitive to outliers, while standardization is generally more suitable when the data follows an approximately Gaussian distribution or when the algorithm benefits from centered features.

---

### 7. What is One-Hot Encoding, and what problem can occur with high-cardinality categorical features?

Answer:
One-Hot Encoding converts each category into a separate binary column. For example, if a City column contains Delhi, Mumbai, and Jaipur, it can be converted into separate columns such as City_Delhi, City_Mumbai, and City_Jaipur.

The main problem with high-cardinality features is that they can create a very large number of columns, increasing memory usage, computational cost, and potentially the risk of overfitting.

---

### 8. What is Label Encoding, and why can it be problematic for nominal categorical features?

Answer:
Label Encoding assigns an integer to each category. For example:

Red → 0
Blue → 1
Green → 2

The problem is that these numbers can create an artificial order between categories. For example, assigning Red = 0, Blue = 1, and Green = 2 may make a model interpret Green as greater than Blue and Blue as greater than Red, even though no such relationship exists. Therefore, One-Hot Encoding is often more appropriate for nominal categorical variables.

---

### 9. Suppose a categorical column has 100 different categories. How would you preprocess it?

Answer:
I would first examine the feature and understand whether the categories have meaningful relationships with the target. One-Hot Encoding is possible but would create 100 additional features. Depending on the problem, I could consider frequency encoding, target encoding, hashing, or grouping rare categories into an "Other" category. The choice depends on the dataset size, model type, cardinality, risk of overfitting, and whether interpretability is important.

---

### 10. What is data leakage during preprocessing? Give an example and explain how to prevent it.

Answer:
Data leakage occurs when information from the validation or test data is accidentally used during the training process.

For example, suppose we calculate the mean and standard deviation using the entire dataset before splitting it into training and test sets. The test data has now influenced the preprocessing parameters used for training.

The correct approach is to first split the data into training and test sets. Then fit the preprocessing technique only on the training data and use the learned parameters to transform both training and test data.

In practice, Scikit-learn Pipelines and ColumnTransformer can help prevent this type of leakage.
