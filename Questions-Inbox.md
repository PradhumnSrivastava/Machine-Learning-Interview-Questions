# Questions Inbox

19. Why is KNN sensitive to the choice of distance metric? Ans- KNN determines its neighbors using a distance metric, so changing the metric can change which observations are considered nearest. Euclidean, Manhattan, Minkowski, and other metrics can produce different neighborhoods, especially when features have different distributions or structures.

20. Can KNN produce probability estimates, and how? Ans- Yes. In classification, KNN can estimate class probabilities by calculating the proportion of neighbors belonging to each class. For example, if 7 out of 10 nearest neighbors belong to class 1, the basic KNN probability estimate for class 1 is 0.7. Distance-weighted KNN can produce weighted probability estimates.
