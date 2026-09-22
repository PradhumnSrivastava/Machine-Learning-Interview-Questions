# Questions Inbox

7. How are the weights learned in Logistic Regression? Ans- The weights and bias are learned by minimizing the loss function using an optimization algorithm such as Gradient Descent. The gradients of the loss with respect to the model parameters are calculated, and the parameters are updated iteratively to reduce the loss.

8. What is the decision boundary in Logistic Regression? Ans- The decision boundary is the boundary where the predicted probability reaches the classification threshold, commonly 0.5. For a standard Logistic Regression model, this corresponds to WᵀX + b = 0, which forms a linear decision boundary.

9. What are the assumptions and limitations of Logistic Regression? Ans- Logistic Regression assumes a linear relationship between the input features and the log-odds of the target. It can be affected by multicollinearity, extreme outliers, and highly non-linear relationships. Standard Logistic Regression also produces a linear decision boundary unless features are transformed or additional non-linear features are introduced.

10. What is the difference between Logistic Regression and Linear Regression? Ans- Linear Regression predicts continuous numerical values, while Logistic Regression predicts the probability of a class. Linear Regression commonly uses Mean Squared Error for optimization, whereas Logistic Regression commonly uses Binary Cross-Entropy or Log Loss. Logistic Regression uses the Sigmoid function for binary classification.
