# credit-risk-classification
Module 20 Challenge Repo

Analysis:

The logistic regression model trained on the original data performs quite well in predicting both healthy loans (label 0) and high-risk loans (label 1). It achieves a high accuracy score of around 99%, indicating that it correctly classifies a majority of the instances. The confusion matrix further reveals that the model's predictions are mostly accurate: it successfully identifies 18679 healthy loans and 558 high-risk loans, with only 80 false positives and 67 false negatives.

The precision and recall scores in the classification report are also informative. The precision for label 1 (high-risk loans) is 0.87, which means that out of all instances predicted as high-risk loans, around 87% are actually high-risk loans. The recall for label 1 is 0.89, indicating that the model identifies 89% of the actual high-risk loans. Overall, the F1-score for label 1 is 0.88, which is a harmonic mean of precision and recall and provides a balanced assessment of the model's performance.

After resampling the training data to address the class imbalance, the logistic regression model's performance significantly improves. The accuracy score reaches around 100%, indicating near-perfect classification on the testing data. The confusion matrix shows only a few misclassifications: 91 false positives and 2 false negatives.

The classification report demonstrates the high precision (0.87) and recall (1.00) for label 1, indicating that the model is almost flawless in identifying high-risk loans. The F1-score for label 1 increases to 0.93, suggesting a strong balance between precision and recall.

Overall Conclusion:

Resampling the training data using random oversampling greatly improved the model's performance, resulting in a highly accurate and reliable classifier for both healthy and high-risk loans. The resampling strategy effectively mitigated the impact of class imbalance, allowing the model to achieve excellent results in identifying high-risk loans while maintaining high accuracy overall.
