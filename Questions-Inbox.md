# Questions Inbox

13. What is Hyperparameter Tuning in an ML Pipeline? Ans- Hyperparameter tuning is the process of finding suitable values for parameters that are not learned directly from the training data, such as learning rate, tree depth, regularization strength, or number of neighbors. Techniques such as Grid Search, Random Search, and Bayesian optimization can be integrated into ML Pipelines.

14. What is Model Evaluation in an ML Pipeline? Ans- Model evaluation measures how well a trained model performs using appropriate metrics. For classification, metrics may include accuracy, precision, recall, F1-score, and ROC-AUC, while regression commonly uses MAE, MSE, RMSE, and R².

15. How can ML Pipelines be made reproducible? Ans- Reproducibility can be improved by versioning datasets, code, configurations, dependencies, preprocessing logic, and model artifacts. Fixed random seeds, experiment tracking tools, Git, DVC, containers, and workflow orchestration can also help reproduce experiments and models.

16. What is the role of CI/CD in an ML Pipeline? Ans- CI/CD automates software integration, testing, building, and deployment processes. In ML systems, CI can test data-processing and model code, while CD can automate the packaging and deployment of validated models and pipeline components.

17. What is an ML Orchestrator? Ans- An ML orchestrator manages and coordinates different steps of an ML workflow. It can handle task dependencies, scheduling, retries, parallel execution, monitoring, and pipeline execution. Examples include Airflow, Kubeflow, Prefect, and Dagster.

18. What is Model Versioning in an ML Pipeline? Ans- Model versioning involves maintaining different versions of trained models along with their associated code, data, parameters, metrics, and artifacts. It allows teams to reproduce experiments, compare models, roll back deployments, and track which model is running in production.

19. How does an ML Pipeline handle model retraining? Ans- A production pipeline can be triggered periodically or when conditions such as new data, data drift, performance degradation, or a business-defined event occur. The pipeline can ingest new data, validate it, retrain the model, evaluate the new model, and deploy it only if it satisfies predefined criteria.

20. What is the difference between an ML Pipeline and an ML Production Lifecycle? Ans- An ML Pipeline represents an automated sequence of connected ML tasks, such as data processing, training, and evaluation. The ML Production Lifecycle is broader and includes data collection, pipeline execution, deployment, monitoring, model versioning, feedback, retraining, and continuous improvement of the production system.
