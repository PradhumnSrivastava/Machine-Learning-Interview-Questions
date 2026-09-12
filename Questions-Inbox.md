# Questions Inbox

22. What is underfitting in machine learning? Ans- Underfitting occurs when a model is too simple to capture the underlying patterns in the data. It performs poorly on both training and unseen data. It can be reduced by using a more complex model, adding useful features, reducing excessive regularization, or training the model for longer.

23. What is the bias-variance tradeoff? Ans- The bias-variance tradeoff is the balance between underfitting and overfitting. High bias means the model is too simple and tends to underfit, while high variance means the model is too sensitive to training data and tends to overfit. A good model aims to find a balance between bias and variance.

24. What is cross-validation and why is it used? Ans- Cross-validation is a model evaluation technique in which the dataset is divided into multiple folds. The model is trained on some folds and validated on the remaining fold, repeating the process so each fold is used for validation. It provides a more reliable estimate of model performance and helps in model selection and hyperparameter tuning.

25. What is regularization in machine learning? Ans- Regularization is a technique used to reduce overfitting by adding a penalty for model complexity to the loss function. L1 regularization can drive some feature coefficients to zero, while L2 regularization shrinks coefficients toward zero without usually making them exactly zero.

26. What is the difference between L1 and L2 regularization? Ans- L1 regularization adds the absolute values of model coefficients to the loss function and can produce sparse models by making some coefficients exactly zero. L2 regularization adds the squared values of coefficients and generally shrinks them toward zero. L1 is useful for feature selection, while L2 is useful for controlling model complexity.

27. What is hyperparameter tuning? Ans- Hyperparameter tuning is the process of finding the best values for parameters that are set before model training, such as learning rate, tree depth, number of estimators, or regularization strength. Common techniques include grid search, random search, and Bayesian optimization.

28. What is the difference between a parameter and a hyperparameter? Ans- A parameter is learned automatically from the training data during model training, such as weights and coefficients. A hyperparameter is specified before training and controls the learning process or model structure, such as learning rate, maximum tree depth, or the number of trees in a random forest.

29. What is an ensemble learning method? Ans- Ensemble learning combines predictions from multiple models to produce a stronger and more robust prediction. Bagging, boosting, and stacking are common ensemble techniques. Examples include Random Forest, AdaBoost, Gradient Boosting, and XGBoost.

30. What is the difference between bagging and boosting? Ans- Bagging trains multiple models independently, usually on different bootstrap samples, and combines their predictions to reduce variance. Boosting trains models sequentially, where each new model focuses more on errors made by previous models, primarily improving predictive performance and reducing bias.
