# Questions Inbox
5. Explain precision, recall and F1.
Ans- Precision, recall, and F1-score are classification evaluation metrics. Precision tells us, out of all the instances the model predicted as positive, how many were actually positive, so it focuses on minimizing false positives. Recall tells us, out of all the actual positive instances, how many the model correctly identified, so it focuses on minimizing false negatives. F1-score is the harmonic mean of precision and recall and provides a single metric that balances both. For example, in fraud detection, if missing a fraudulent transaction is more costly, we may prioritize recall, whereas if investigating false fraud alerts is expensive, we may prioritize precision. F1-score is useful when we want a balance between precision and recall, especially when the classes are imbalanced.

6. Why can 99% accuracy be a terrible metric?
Ans- 99% accuracy can be a terrible metric when the dataset is highly imbalanced. For example, suppose we have 10,000 transactions, out of which 9,900 are legitimate and only 100 are fraudulent. If a model simply predicts every transaction as legitimate, it will achieve 99% accuracy, even though it detects zero fraudulent transactions. Therefore, accuracy can give a misleading impression of model performance when one class dominates the dataset. In such cases, we should also consider metrics such as precision, recall, F1-score, PR-AUC, or cost-based metrics, depending on the business objective.

7. Precision vs recall — when would you prioritize each?
Ans- 99% accuracy can be a terrible metric when the dataset is highly imbalanced. For example, suppose we have 10,000 transactions, out of which 9,900 are legitimate and only 100 are fraudulent. If a model simply predicts every transaction as legitimate, it will achieve 99% accuracy, even though it detects zero fraudulent transactions. Therefore, accuracy can give a misleading impression of model performance when one class dominates the dataset. In such cases, we should also consider metrics such as precision, recall, F1-score, PR-AUC, or cost-based metrics, depending on the business objective.
































