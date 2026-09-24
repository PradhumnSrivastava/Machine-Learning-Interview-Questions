# Questions Inbox

5. How do you choose the value of K in KNN? Ans- The value of K is usually selected using validation techniques such as cross-validation. A small K can make the model sensitive to noise and lead to overfitting, while a very large K can make the model too smooth and lead to underfitting.

6. Why is feature scaling important in KNN? Ans- Feature scaling is important because KNN relies on distance calculations. If one feature has a much larger numerical scale than another, it can dominate the distance calculation. Standardization or normalization can help ensure that features contribute more appropriately to the distance.

7. Is KNN a parametric or non-parametric algorithm? Ans- KNN is a non-parametric algorithm because it does not assume a specific probability distribution or fixed functional form for the underlying data. Instead, it makes predictions based directly on the training examples.

8. What is the difference between KNN Classification and KNN Regression? Ans- KNN Classification predicts a categorical class by using the labels of the nearest neighbors, usually through majority voting. KNN Regression predicts a continuous value, commonly by taking the average of the target values of the nearest neighbors.

9. What are the advantages and disadvantages of KNN? Ans- KNN is simple to understand, requires little training computation, and can model complex decision boundaries. However, prediction can be computationally expensive for large datasets, it requires appropriate feature scaling, and its performance can decrease when there are many irrelevant or high-dimensional features.

10. What is the Curse of Dimensionality in KNN? Ans- The Curse of Dimensionality refers to the problems that occur when the number of features becomes very large. In high-dimensional spaces, data points tend to become relatively similar in terms of distance, making it difficult for KNN to identify meaningful nearest neighbors. Feature selection or dimensionality reduction can help address this problem.
