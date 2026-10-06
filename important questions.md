Question 1- What is Machine Learning?
ans- Machine Learning is a branch of Artificial Intelligence where machines learn patterns and relationships from data using algorithms, without being explicitly programmed for every rule, so that they can make predictions or decisions on new data.

Question 2- What is Features?
ans- A feature is an individual measurable property, characteristic, or input variable of a dataset that is used by a machine learning model to make predictions or decisions.

Question 3- What is Target?
ans- A target is the output variable or characteristic that a machine learning model is trained to predict.

Question 4- What is Observation or Sample in Machine learning?
ans- An observation or sample is a single individual data point or record in a dataset.

Question 5- What is Training Data?
ans- Training data is the portion of the dataset used to train the machine learning model and learn patterns between features and the target.

Question 6- What is Validation Data?
ans- Validation data is a portion of the dataset used to evaluate and tune a model during the model development process.

Questoin 7- What is Test Data?
ans- Test Data is the portion of the dataset used to test the model learning and meansure the performance of the model.

Question 8- What is Model?
ans- A model is a learned mathematical representation of patterns or relationships between input features and the target, obtained from training data.

Question 9- What is Algorithm?
ans- An algorithm is a systematic procedure or set of rules used to learn a model from data.

Question 10- What is Parameters?
ans- Parameters are values learned automatically by the model from the training data during the training process.

Question 11- What is Hyperparameters?
ans- Hyperparameters are settings specified before or outside the training process that control how a machine learning algorithm learns.

Question 12- What is Prediction?
ans- Prediction is the output produced by a trained machine learning model for a given input.

Question 13- What is Inference?
ans- Inference is the process of using a trained model to generate predictions on new, unseen input data.

Question 14- What is Generalization?
ans- Generalization is the ability of a trained machine learning model to perform well on new, unseen data.

Question 15- What is Training Error?
ans- Training error is the error made by a model when making predictions on the same data used to train it.

Question 16- What is Validation Error?
ans- Validation error is the error made by the model on the validation dataset during the model development and tuning process.

Question 17- What is Test Dataset?
ans- Test error is the error made by the final trained model on previously unseen test data.

Question 18- What is Train-Test Split?
ans- Train-Test Split is the process of dividing a dataset into two separate subsets: training data and test data. The training set is used to train the machine learning model, while the test set is kept unseen during training and used to evaluate the final performance of the model.

Question 19- What is Train-Validation-Test Split?
ans- Train-Validation-Test Split divides a dataset into three subsets: training, validation, and test data. Training data is used to learn model parameters, validation data is used during development for model selection and hyperparameter tuning, and test data is reserved for the final unbiased evaluation of the selected model.

Question 20- What is Random Split?
ans- Random Split is a data-splitting technique in which observations are randomly assigned to training and testing or validation subsets. Randomization reduces the possibility that the split is influenced by the original ordering of the data and generally works well when observations are independently and identically distributed (i.i.d.).

Question 21- What is Data Leakage?
ans- In artificial intelligence and statistics, data leakage happens when a model learns from information it should not have access to during training. This makes the model look very accurate during testing, but it fails badly when used in the real world.

Question 22. What is Target Leakage?
ans- Target leakage occurs when information about the target variable is directly or indirectly included in the input features during model training, causing the model to achieve unrealistically high performance.

Question 23. What is Train Test Contamination?
ans- Train-test contamination occurs when information from the test set accidentally influences the training process, causing the model's performance to appear better than it actually is.

Question 24. What is MCAR — Missing Completely At Random?
ans- MCAR occurs when the probability of a value being missing is completely unrelated to any observed or unobserved variable in the dataset. The missing values occur purely by random chance.

Question 25. What is MAR — Missing At Random>
ans- MAR occurs when the probability of a value being missing depends on other observed variables in the dataset, but not on the missing value itself after considering those observed variables.

Question 25. MNAR — Missing Not At Random
ans- MNAR occurs when the probability of a value being missing depends on the missing value itself or on some unobserved information related to that value.

Question 26. What is KNN Imputation?
ans- KNN Imputation is a technique for handling missing values by finding the K most similar observations (nearest neighbors) and using their values to estimate the missing value.

Question 27. What is Mean Imputation?
ans- Mean imputation replaces missing numerical values with the mean (average) of the available values in that feature.

Question 28. What is Mode Imputation?
ans- Mode imputation replaces missing values with the most frequently occurring value in that feature.

Question 29. What is Median Imputation?
ans- Median imputation replaces missing numerical values with the median (middle value) of the available values in that feature.

Question 30. What is Categorical Variables?
ans- Categorical variables are variables that contain values representing groups or categories rather than numerical quantities.

Question 31. What is Nominal Variables?
ans- Nominal variables are categorical variables whose categories have no natural order or ranking.

Question 32. What is Ordinal Variables?
ans- Ordinal variables are categorical variables whose categories have a meaningful order or ranking, but the difference between categories is not necessarily equal.

Question 33. What is Encoding?
ans- Encoding means converting categorical data into numerical form so that a machine learning algorithm can process it.

Question 34. What is One-Hot Encoding?
ans- One-Hot Encoding converts each category into a separate binary column, where 1 indicates the presence of a category and 0 indicates its absence.

Question 35. What is Label Encoding
ans- Label Encoding assigns a unique integer to each category.

Question 36. What is Ordinal Encoding?
ans- Ordinal Encoding converts categories into numerical values according to their natural order or ranking.

Question 37. What is Target Encoding
ans- Target Encoding replaces each category with a statistic calculated from the target variable, usually the mean target value for that category.

Question 38. What is Frequency Encoding?
ans- Frequency Encoding replaces each category with the number of times or proportion of times that category appears in the dataset.

Question 39. What is Scaling?
ans- Feature scaling is the process of transforming numerical features to a similar scale so that features with larger numerical values do not dominate the model.

Question 40. Why Feature Scaling?
ans- Feature scaling is needed because some machine learning algorithms are sensitive to the magnitude and scale of features.

Question 41. What is Standardization?
ans- Standardization transforms a feature so that it has a mean of 0 and a standard deviation of 1.

Question 42. Essential code for Standardization.
ans- from sklearn.preprocessing import StandardScaler

scaler = StandardScaler()

X_train_scaled = scaler.fit_transform(X_train)
X_test_scaled = scaler.transform(X_test)

Question 43. What is Normalization?
ans- Normalization is a broader term for transforming data to a specific or comparable scale. In many ML contexts, people use "normalization" to refer specifically to scaling values to a fixed range such as 0 to 1. This is commonly done using Min-Max Scaling.

Question 44. What is Min-Max Scaling?
ans- Min-Max Scaling transforms values to a fixed range, usually between 0 and 1.

Question 45. What is Robust Scaling?
ans- Robust Scaling scales features using the median and interquartile range (IQR), making it less sensitive to outliers.

Questoin 46. When is Scaling Required?
ans- Scaling is particularly important for algorithms that depend on distance, magnitude, or gradient optimization.
Common examples like Distance-based Models.

Question 47. When Scaling is NOT Required?
ans- Tree-based algorithms generally don't require feature scaling because they make decisions using thresholds, rather than distances or feature magnitudes. like Decision Tree,
Random Forest, XGBoost, LightGBM, and CatBoost.

Question 48. What is an Outlier?
ans- An outlier is an observation that is significantly different from the majority of the observations in a dataset.

Question 49. What is Univariate Outlier?
ans- A univariate outlier is an unusual observation detected by considering only one variable or feature.

Question 50. What is Multivariate Outlier?
ans- A multivariate outlier is an observation that may not be unusual in any single feature but is unusual because of the combination of multiple features.

Question 51. What is Z-Score?
ans- Z-score measures how many standard deviations an observation is away from the mean.

Question 52. What is IQR Method?z
ans- The IQR method identifies potential outliers using the interquartile range, which is the difference between the third quartile (Q3) and first quartile (Q1).

Question 53. What is Box Plot?
ans- A box plot is a graphical method for visualizing the distribution of numerical data and identifying potential outliers.

Question 54. What is Winsorization?
ans- Winsorization is a technique that limits extreme values by replacing them with specified percentile values instead of removing them.
