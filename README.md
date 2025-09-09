# Interpretable-Machine-Learning

Overview

This project performs heart disease prediction using machine learning. It applies three different feature selection methods to choose the most important features and trains a Random Forest classifier to evaluate performance.

1. Data Loading and Preprocessing

    Loads a dataset related to heart disease.

    Converts the target variable into a binary outcome (disease or no disease).

    Splits the data into training and test sets.

    Applies SMOTE to balance the classes in the training data.

    Scales features for standardization.

2. Feature Selection and Modeling
  a. RFE (Recursive Feature Elimination)

      Selects the most important features by recursively removing less important ones.

      Trains a Random Forest classifier using the selected features.

      Evaluates the model on the test set (accuracy, ROC AUC, classification report).

  b. LASSO-based Feature Selection

     Uses LASSO (L1-regularized logistic regression) to select important features based on coefficients.

      Trains a Random Forest classifier using the selected features.

      Evaluates the model on the test set.

  c. ANOVA F-test Feature Selection

      Uses ANOVA F-test to select the top features most correlated with the target.

      Trains a Random Forest classifier using the selected features.

      Evaluates the model on the test set.

3. Output

    For each feature selection method, the code prints:

    The top selected features.

    Final model accuracy.

    ROC AUC score.

    Classification report (precision, recall, f1-score).
