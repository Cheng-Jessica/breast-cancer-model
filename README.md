# breast-cancer-model

Classification Technique on the Breast Cancer dataset

[Introduction]
Specifically, build a decision tree, logistic regression and k-nearest neighbors that predicts the diagnose result based on ten real-valued features (mean, standard error, and "worst" or largest of these features).
Explore how well different model perform for several different parameter values. When is overfitting and when is underfitting? Show how you set the model that provides the best predictive performance.
Present a brief overview of your predictive modeling process, explorations, and discuss your results. Make sure you present information about the model “goodness” (possible things to think about: confusion matrix, predictive accuracy, classification error, precision, recall, f-measure).

[Conclusion]
Based on performance matrix below, I would choose logistic regression since all the matrix are working better in the brease cancer data set.

Model | Mean | Accuracy	| Mean | Precision	|Mean |Recall	|Mean |Roc_acu	|Hyper |Parameter
Decision Tree	0.92	0.94	0.93	0.92	max_dept=5
KMM	0.93	0.93	0.95	0.97	k=9
Logistic Regression	0.94	0.95	0.96	0.99	C = 0.0183
