## breast-cancer-model

Classification Technique on the Breast Cancer dataset

## Overview
This GitHub repository contains a predictive modeling analysis for breast cancer outcomes using machine learning algorithms such as Decision Tree, K-Nearest Neighbors (KNN), Logistic Regression, and Support Vector Machine (SVM). The analysis is based on the Wisconsin Breast Cancer dataset, which includes real-valued features representing mean, standard error, and "worst" values.

## Dataset
The dataset used in this project is sourced from the UCI Machine Learning Repository and can be accessed here. It consists of feature vectors and binary labels, with the goal of predicting the diagnosis result (malignant or benign) based on ten real-valued features.

## Project Structure
1. Data Preparation: The breast cancer dataset is loaded and split into input features (X) and target labels (y).
  
2. Model Selection: Decision Tree, KNN, Logistic Regression, and SVM are chosen as the classification algorithms for breast cancer prediction.
  
3. Nested Cross-Validation: A nested cross-validation loop with 10 trials is implemented. Grid search is performed for hyperparameters, specifically 'max_depth' for Decision Tree, 'n_neighbors' and 'weights' for KNN, 'C' and 'penalty' for Logistic Regression, and 'C' and 'kernel' for SVM.

4. Performance Evaluation
Various performance metrics are computed and stored for each trial, including confusion matrices, precision, recall, and F1-score. ROC curves are generated to assess model performance.

5. Overfitting Detection: To detect overfitting, the accuracy of each trial is compared to the mean accuracy across trials. If a trial's accuracy is significantly higher than the mean, it suggests possible overfitting.

6. Mean Performance Metrics: The mean values of confusion matrices, precision, recall, and F1-score across all trials are calculated.

7. Grid Search: A final grid search is performed using the best hyperparameters found during the nested cross-validation process.

8. ROC and Lift Curves: ROC curves visualize the binary classifier's ability to discriminate between positive and negative cases at different threshold levels. Lift curves show how well the model performs relative to a random classifier at different threshold levels.

## Results

|Model Types| Average Accuracy | F1-Scores |
|-----------|------------------|-----------|
|Decision Tree | 0.927 | 0.987 |
|K-NN | 0.927 | 0.977|
|Logistic Regression | 0.977 | 0.985 |
|SVM Classification | 0.970 | 0.987 |

## How to Use
- Clone the repository: git clone [repository-url]
- Install required dependencies: pip install required packages.
- Run the Jupyter notebook or Python scripts to reproduce the analysis.
- Explore the results and fine-tune the models based on the specific requirements.

Feel free to contribute, report issues, or suggest improvements to enhance the project.
