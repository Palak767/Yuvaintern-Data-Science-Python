# YUVaintern Week 5 – Comprehensive Data Science Project

## Global Happiness Analysis: From Data Exploration to Strategic Recommendations

### Project Overview

This repository contains my final project for the YUVaintern Data Science with Python Virtual Internship.

The project integrates the analytical techniques developed throughout Weeks 1–4 into a single end-to-end data science workflow.

The analysis focuses on understanding the factors associated with life evaluation using the World Happiness Report dataset.

The project progresses from data acquisition and cleaning to exploratory analysis, advanced visualization, statistical hypothesis testing, machine learning, and strategic recommendations.

---

## Project Objective

The primary objective is to identify important patterns and relationships associated with global life evaluation and translate the analytical findings into meaningful strategic recommendations.

---

## Key Questions

The project addresses the following questions:

1. How is life evaluation distributed across observations?
2. Which factors are strongly associated with life evaluation?
3. Does social support significantly differ in relation to life evaluation?
4. Can socioeconomic and well-being indicators predict high and low life-evaluation categories?
5. What strategic insights can stakeholders derive from the analysis?

---

## Dataset

The project uses the World Happiness Report Figure 2.1 dataset.

Important variables include:

- Life evaluation
- Social support
- Log GDP per capita
- Healthy life expectancy
- Freedom to make life choices
- Generosity
- Perceptions of corruption

---

# Methodology

The project follows an end-to-end data science workflow.

## Phase 1 – Data Acquisition and Cleaning

The dataset was loaded using Pandas and examined for:

- Missing values
- Duplicate records
- Data types
- Numerical consistency
- Relevant analytical variables

Appropriate preprocessing was performed before analysis.

---

## Phase 2 – Exploratory Data Analysis

Descriptive statistics and exploratory visualizations were used to understand:

- Distribution of life evaluation
- Relationships between major variables
- Potential outliers
- Correlations
- Important trends and patterns

---

## Phase 3 – Data Storytelling

Advanced visualizations were developed using Python visualization libraries.

The visualizations were designed to communicate important findings to both technical and non-technical audiences.

---

## Phase 4 – Statistical Analysis

A hypothesis was formulated to investigate the relationship between social support and life evaluation.

### Null Hypothesis

There is no statistically significant difference in mean life evaluation between high and low social-support groups.

### Alternative Hypothesis

Countries with high social support have significantly higher mean life evaluation.

A significance level of 0.05 was used.

Welch's independent two-sample t-test, confidence intervals, effect size, and Pearson correlation were used.

---

## Phase 5 – Machine Learning

A Logistic Regression classifier was developed to classify observations into high and low life-evaluation categories.

The model was evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix
- ROC Curve

---

# Key Findings

The statistical analysis showed a strong relationship between social support and life evaluation.

The high-social-support group had a higher average life evaluation than the low-social-support group.

The statistical test produced a very small p-value, providing strong evidence against the null hypothesis.

The correlation analysis also indicated a strong positive association between social support and life evaluation.

The machine-learning model achieved approximately:

- 81.28% testing accuracy
- 81.37% precision
- 81.37% recall
- 81.37% F1-score
- 0.9241 ROC-AUC

---

# Strategic Insights

Based on the analysis, several strategic areas can be identified:

### 1. Strengthen Social Support

Policies and programs that encourage community engagement, social networks, and support systems may contribute to improved well-being.

### 2. Improve Health Outcomes

Healthy life expectancy was an important predictive feature. Investment in healthcare, preventive care, and healthy lifestyles can therefore be considered important areas for policymakers.

### 3. Support Economic Well-being

GDP per capita showed a meaningful relationship with life evaluation. Economic stability and opportunities can contribute to better living conditions.

### 4. Promote Individual Freedom

Freedom to make life choices was also associated with life evaluation, highlighting the importance of autonomy and personal decision-making.

### 5. Use Data-Driven Policy

Governments and organizations can use happiness and well-being indicators alongside traditional economic metrics when evaluating societal progress.

---

# Business and Research Impact

The analysis demonstrates how data science can support evidence-based decision-making.

Organizations can use similar approaches to:

- Identify important factors affecting well-being.
- Prioritize interventions.
- Monitor changes over time.
- Compare regions.
- Build predictive models.
- Support policy planning.

---

# Limitations

The project has several limitations:

- The data is primarily country-level.
- Association does not imply causation.
- Important variables may not be included.
- The classification target depends on the selected threshold.
- Logistic Regression assumes a linear relationship between predictors and log-odds.
- Results may change with different datasets or years.

---

# Future Work

Future improvements could include:

- Multi-year analysis.
- Regional comparisons.
- Multiple linear regression.
- Random Forest and Gradient Boosting models.
- Hyperparameter tuning.
- Cross-validation.
- Feature engineering.
- More detailed causal analysis.
- Time-series analysis.

---

# Technologies

- Python
- Pandas
- NumPy
- SciPy
- Scikit-learn
- Matplotlib
- Seaborn
- Plotly
- Jupyter Notebook
- Microsoft Word

---

## Internship

YUVaintern – Data Science with Python Virtual Internship

Final Task: Week 5 – Comprehensive Data Science Project Reporting and Strategic Recommendations
