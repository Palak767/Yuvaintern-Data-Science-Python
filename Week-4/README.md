# YUVaintern Week 4 – Machine Learning Model Development and Evaluation

## Project Overview

This repository contains my Week 4 task for the YUVaintern Data Science with Python Virtual Internship.

The objective of this task is to develop, train, and evaluate a basic machine learning model using Python and Scikit-learn.

The project demonstrates a complete machine learning workflow, including data preprocessing, feature selection, target creation, train-test splitting, model training, prediction, evaluation, visualization, and interpretation.

---

## Problem Statement

The objective is to predict whether an observation belongs to a high or low life-evaluation category using socioeconomic and well-being indicators from the World Happiness Report dataset.

---

## Dataset

The analysis uses the World Happiness Report Figure 2.1 dataset.

The major features used in the model are:

- Social Support
- Healthy Life Expectancy
- GDP per Capita
- Freedom to Make Life Choices
- Generosity
- Perceptions of Corruption

The target variable is created from Life Evaluation.

### Target Variable

The continuous Life Evaluation score is converted into a binary classification target using the median value.

- 1 → High Life Evaluation
- 0 → Low Life Evaluation

---

## Machine Learning Algorithm

### Logistic Regression

Logistic Regression was selected because it is:

- Simple and computationally efficient.
- Suitable for binary classification.
- Easy to interpret.
- Capable of producing probability estimates.
- Useful as a strong baseline classification model.

---

## Machine Learning Workflow

The following steps were performed:

1. Loaded the dataset using Pandas.
2. Inspected the dataset structure.
3. Selected relevant features.
4. Checked and handled missing values.
5. Created a binary target variable.
6. Divided the dataset into training and testing sets.
7. Standardized numerical features.
8. Trained a Logistic Regression model.
9. Generated predictions.
10. Evaluated the model using multiple classification metrics.
11. Created a confusion matrix.
12. Created an ROC curve.
13. Examined model feature coefficients.
14. Discussed errors, limitations, and possible improvements.

---

## Model Evaluation

The model was evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC
- Confusion Matrix
- ROC Curve

---

## Results

| Metric | Result |
|---|---:|
| Dataset size after cleaning | 1013 |
| Training samples | 810 |
| Testing samples | 203 |
| Training Accuracy | 86.05% |
| Testing Accuracy | 81.28% |
| Precision | 81.37% |
| Recall | 81.37% |
| F1 Score | 81.37% |
| ROC-AUC | 0.9241 |

---

## Feature Coefficients

| Feature | Coefficient |
|---|---:|
| Social Support | 1.211062 |
| Healthy Life Expectancy | 1.161062 |
| GDP per Capita | 1.021024 |
| Freedom | 0.656020 |
| Generosity | 0.120200 |
| Corruption | 0.029399 |

The positive coefficients indicate that higher values of these variables increase the model's predicted probability of belonging to the high life-evaluation class, assuming other variables remain constant.

---

## Visualization

### 1. Confusion Matrix

The confusion matrix compares actual and predicted classes.

It helps identify:

- True Positives
- True Negatives
- False Positives
- False Negatives

This visualization provides a direct view of the classification errors made by the model.

### 2. ROC Curve

The ROC curve evaluates the model's ability to distinguish between the two classes at different classification thresholds.

The ROC-AUC score of approximately 0.9241 indicates strong classification performance.

### 3. Feature Coefficients

The coefficient plot shows the relative contribution of each feature to the Logistic Regression decision.

Social Support, Healthy Life Expectancy, and GDP per Capita have comparatively larger coefficients in the model.

---

## Interpretation

The Logistic Regression model achieved approximately 81.28% accuracy on unseen test data.

The training accuracy was approximately 86.05%, while the testing accuracy was approximately 81.28%. The difference between these values suggests some generalization loss, but it does not indicate severe overfitting.

The ROC-AUC score of 0.9241 indicates that the model has strong ability to distinguish between high and low life-evaluation categories.

Social Support, Healthy Life Expectancy, and GDP per Capita had the largest positive coefficients among the selected features.

---

## Error Analysis

Potential sources of error include:

- Observations close to the median classification threshold.
- Missing or noisy data.
- Important variables not included in the model.
- Country-level aggregation.
- Linear assumptions of Logistic Regression.
- Differences between countries that cannot be captured by the selected features.

---

## Model Limitations

The model has several limitations.

First, the dataset contains country-level observations, so the results should not be interpreted as individual-level predictions.

Second, the binary target depends on the selected median threshold. A different threshold could produce different results.

Third, Logistic Regression assumes a linear relationship between the predictors and the log-odds of the target.

Finally, the model demonstrates predictive association rather than causation.

---

## Future Improvements

The model could be improved by:

- Performing cross-validation.
- Hyperparameter tuning.
- Comparing Logistic Regression with Decision Trees.
- Testing Random Forest and Gradient Boosting.
- Testing Support Vector Machines.
- Performing feature selection.
- Using additional years of data.
- Performing more detailed error analysis.
- Investigating regional patterns.
- Using ensemble machine learning models.

---

## Conclusion

The Week 4 machine learning analysis successfully demonstrated the complete machine learning development pipeline.

A Logistic Regression classifier was trained to distinguish between high and low life-evaluation categories using socioeconomic and well-being indicators.

The model achieved approximately 81.28% testing accuracy and a ROC-AUC of 0.9241, indicating strong classification performance.

The analysis also demonstrated how model evaluation metrics and visualizations can be used to understand predictive performance and identify areas for improvement.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook
- OpenPyXL

---

## Internship

**YUVaintern – Data Science with Python Virtual Internship**

**Task:** Week 4 – Machine Learning Model Development and Evaluation
