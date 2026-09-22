# Questions Inbox
1. What is Logistic Regression? Ans- Logistic Regression is a supervised machine learning algorithm mainly used for classification problems. It predicts the probability of a class by applying the Sigmoid function to a linear combination of input features.

2. Why is Logistic Regression called Regression if it is used for Classification? Ans- Logistic Regression is called regression because it models the relationship between input features and the log-odds of the target probability. Although its output is a probability, that probability is commonly converted into a class label for classification.

3. What is the mathematical equation of Logistic Regression? Ans- The linear part of Logistic Regression is z = w1x1 + w2x2 + ... + wnxn + b, or z = WᵀX + b. The value z is then passed through the Sigmoid function to obtain the predicted probability.

4. What is the role of the Sigmoid function in Logistic Regression? Ans- The Sigmoid function converts the linear output z into a value between 0 and 1. This value represents the predicted probability of the positive class. Its formula is σ(z) = 1 / (1 + e^(-z)).

5. How does Logistic Regression make a classification decision? Ans- Logistic Regression first calculates the predicted probability using the Sigmoid function. A threshold is then applied to convert the probability into a class label. With the commonly used threshold of 0.5, a probability greater than or equal to 0.5 is classified as class 1, while a probability below 0.5 is classified as class 0.

6. What is the Loss Function used in Logistic Regression? Ans- Logistic Regression commonly uses Binary Cross-Entropy Loss, also called Log Loss, for binary classification. It penalizes incorrect predictions, especially predictions made with high confidence, and provides a differentiable objective for optimization.

7. How are the weights learned in Logistic Regression? Ans- The weights and bias are learned by minimizing the loss function using an optimization algorithm such as Gradient Descent. The gradients of the loss with respect to the model parameters are calculated, and the parameters are updated iteratively to reduce the loss.

8. What is the decision boundary in Logistic Regression? Ans- The decision boundary is the boundary where the predicted probability reaches the classification threshold, commonly 0.5. For a standard Logistic Regression model, this corresponds to WᵀX + b = 0, which forms a linear decision boundary.

9. What are the assumptions and limitations of Logistic Regression? Ans- Logistic Regression assumes a linear relationship between the input features and the log-odds of the target. It can be affected by multicollinearity, extreme outliers, and highly non-linear relationships. Standard Logistic Regression also produces a linear decision boundary unless features are transformed or additional non-linear features are introduced.

10. What is the difference between Logistic Regression and Linear Regression? Ans- Linear Regression predicts continuous numerical values, while Logistic Regression predicts the probability of a class. Linear Regression commonly uses Mean Squared Error for optimization, whereas Logistic Regression commonly uses Binary Cross-Entropy or Log Loss. Logistic Regression uses the Sigmoid function for binary classification.
