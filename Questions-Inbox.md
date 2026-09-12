# Questions Inbox

26. What is the difference between L1 and L2 regularization? Ans- L1 regularization adds the absolute values of model coefficients to the loss function and can produce sparse models by making some coefficients exactly zero. L2 regularization adds the squared values of coefficients and generally shrinks them toward zero. L1 is useful for feature selection, while L2 is useful for controlling model complexity.

27. What is hyperparameter tuning? Ans- Hyperparameter tuning is the process of finding the best values for parameters that are set before model training, such as learning rate, tree depth, number of estimators, or regularization strength. Common techniques include grid search, random search, and Bayesian optimization.

28. What is the difference between a parameter and a hyperparameter? Ans- A parameter is learned automatically from the training data during model training, such as weights and coefficients. A hyperparameter is specified before training and controls the learning process or model structure, such as learning rate, maximum tree depth, or the number of trees in a random forest.

29. What is an ensemble learning method? Ans- Ensemble learning combines predictions from multiple models to produce a stronger and more robust prediction. Bagging, boosting, and stacking are common ensemble techniques. Examples include Random Forest, AdaBoost, Gradient Boosting, and XGBoost.

30. What is the difference between bagging and boosting? Ans- Bagging trains multiple models independently, usually on different bootstrap samples, and combines their predictions to reduce variance. Boosting trains models sequentially, where each new model focuses more on errors made by previous models, primarily improving predictive performance and reducing bias.
