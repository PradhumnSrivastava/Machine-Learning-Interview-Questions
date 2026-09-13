# Questions Inbox

48. Can Linear Regression be solved using Gradient Descent? Ans- Yes, Linear Regression can be optimized using Gradient Descent. Gradient Descent starts with initial parameter values and repeatedly updates the coefficients in the direction that reduces the loss function. For large datasets, variants such as Stochastic Gradient Descent or Mini-Batch Gradient Descent can be more computationally efficient than calculating the exact solution using the normal equation.

49. What is the Normal Equation in Linear Regression? Ans- The Normal Equation is a closed-form mathematical solution for finding the coefficients that minimize the squared error in Linear Regression. In matrix form, the solution is β = (XᵀX)⁻¹Xᵀy when the inverse exists. It does not require iterative optimization, but computing the matrix inverse can become expensive for datasets with a very large number of features.

50. Why should categorical variables be encoded before using Linear Regression? Ans- Linear Regression requires numerical input features, so categorical variables must be converted into numerical representations. One common approach is One-Hot Encoding, which creates binary indicator variables for categories. Care must be taken to avoid perfect multicollinearity, often by dropping one category when an intercept is included.
