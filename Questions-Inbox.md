# Questions Inbox

49. What is the Normal Equation in Linear Regression? Ans- The Normal Equation is a closed-form mathematical solution for finding the coefficients that minimize the squared error in Linear Regression. In matrix form, the solution is β = (XᵀX)⁻¹Xᵀy when the inverse exists. It does not require iterative optimization, but computing the matrix inverse can become expensive for datasets with a very large number of features.

50. Why should categorical variables be encoded before using Linear Regression? Ans- Linear Regression requires numerical input features, so categorical variables must be converted into numerical representations. One common approach is One-Hot Encoding, which creates binary indicator variables for categories. Care must be taken to avoid perfect multicollinearity, often by dropping one category when an intercept is included.
