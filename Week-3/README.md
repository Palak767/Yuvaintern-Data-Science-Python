# YUVaintern Week 3 – Statistical Analysis and Hypothesis Testing

## 📌 Project Overview

This repository contains my Week 3 task for the YUVaintern Data Science with Python Virtual Internship.

The objective of this task is to perform statistical analysis and hypothesis testing using Python. The analysis investigates the relationship between social support and life evaluation using data from the World Happiness Report.

---

## 🎯 Research Question

Do countries with higher social support have significantly higher life evaluation scores than countries with lower social support?

---

## 🧪 Hypotheses

### Null Hypothesis (H₀)

There is no statistically significant difference in mean life evaluation between countries with high social support and countries with low social support.

### Alternative Hypothesis (H₁)

Countries with high social support have significantly higher mean life evaluation scores than countries with low social support.

### Significance Level

α = 0.05

---

## 📊 Dataset

The analysis uses the World Happiness Report Figure 2.1 dataset.

Important variables used:

- Life evaluation (3-year average)
- Social support
- Log GDP per capita
- Healthy life expectancy
- Freedom to make life choices
- Generosity
- Perceptions of corruption

The primary variables used for hypothesis testing are:

- Social Support
- Life Evaluation

---

## 🔬 Methodology

The following steps were performed:

1. Loaded the dataset using Pandas.
2. Inspected the dataset structure and data types.
3. Checked for missing values.
4. Selected Social Support and Life Evaluation variables.
5. Removed observations with missing values.
6. Divided observations into High Social Support and Low Social Support groups using the median Social Support value.
7. Calculated descriptive statistics for both groups.
8. Performed Welch's independent two-sample t-test.
9. Calculated the 95% confidence interval for the mean difference.
10. Calculated Cohen's d effect size.
11. Calculated Pearson correlation between Social Support and Life Evaluation.
12. Created visualizations to support the statistical findings.
13. Interpreted the results and formulated the conclusion.

---

## 📈 Statistical Results

| Measure | Result |
|---|---:|
| High Social Support observations | 510 |
| Low Social Support observations | 1606 |
| High Social Support Mean | 6.1921 |
| Low Social Support Mean | 5.2350 |
| Mean Difference | 0.9572 |
| t-statistic | 21.3493 |
| p-value | 5.8955689150e-86 |
| 95% Confidence Interval | [0.8692, 1.0451] |
| Cohen's d | 0.9143 |
| Pearson Correlation | 0.7014 |
| Correlation p-value | 9.8948725698e-152 |

---

## 📌 Interpretation

The Welch's independent two-sample t-test produced a p-value far below the significance level of 0.05.

Therefore, the null hypothesis is rejected.

The high-social-support group had an average life evaluation score of approximately 6.19, while the low-social-support group had an average of approximately 5.23.

The mean difference was approximately 0.96 points.

The 95% confidence interval ranged from 0.8692 to 1.0451 and did not include zero, providing further evidence that the difference between the two groups is statistically significant.

Cohen's d was approximately 0.9143, indicating a large effect size.

Pearson correlation was approximately 0.7014, indicating a strong positive association between social support and life evaluation.

---

## 📊 Visualizations

### 1. Mean Life Evaluation by Social Support Group

This visualization compares the average life evaluation scores of the high and low social support groups.

### 2. 95% Confidence Interval

This visualization shows the confidence interval for the difference in mean life evaluation between the two groups.

### 3. Social Support vs Life Evaluation

This visualization illustrates the positive relationship between social support and life evaluation.

---

## 💡 Key Findings

- Countries with higher social support had considerably higher average life evaluation.
- The difference between the two groups was statistically significant.
- The effect size was large.
- Social support and life evaluation showed a strong positive correlation.
- The findings support the alternative hypothesis.

---

## ⚠️ Limitations

The analysis has several limitations:

- The dataset contains country-level observations rather than individual-level observations.
- The analysis identifies association rather than causation.
- Other factors such as GDP, health, freedom and corruption may influence life evaluation.
- Dividing countries into high and low social support groups using the median is a methodological choice.
- Further multivariate analysis could provide deeper insights.

---

## 🚀 Future Improvements

Future analysis could include:

- Multiple linear regression
- ANOVA
- Multiple years of World Happiness data
- Machine learning models
- Controlling for potential confounding variables
- Comparing multiple statistical tests
- Performing cross-country and regional analysis

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- SciPy
- Matplotlib
- Seaborn
- Jupyter Notebook
- Microsoft Excel

---

## 👩‍💻 Internship

**YUVaintern – Data Science with Python Virtual Internship**

**Task:** Week 3 – Statistical Analysis and Hypothesis Testing
