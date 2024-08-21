# Predictive Analysis of Alcohol Consumption of Portuguese Students

## Overview

This project aims to develop a predictive model that classifies the weekend alcohol consumption levels of secondary school students in Portugal. The model predicts whether a student will have low (1-2) or high (3-5) weekend alcohol consumption, which can be used by educational institutions to identify students at higher risk of engaging in excessive drinking.

## Objectives

- **Primary Objective:** Develop a binary classification model to predict the weekend alcohol consumption level of students.
- **Secondary Objective:** Ensure the model is interpretable and reliable for practical use by school counselors and administrators.

## Methodology

### 1. Data Collection & Preparation
- **Dataset:** The dataset contains demographic, academic, and behavioral information of students collected from two Portuguese schools in 2008.
- **Data Cleaning:** Handling of missing values, standardization of variable names, and encoding of categorical variables.
- **Exploratory Data Analysis (EDA):** Initial exploration of data through summary statistics, visualizations (histograms, boxplots, scatterplots), and correlation analysis to understand variable relationships.

### 2. Feature Selection
- Consideration of multiple variables, including:
  - **Demographics:** Age, gender
  - **Family Factors:** Quality of family relationships ("famrel")
  - **Academic Engagement:** Number of absences, study time
  - **Existing Drinking Behavior:** Weekday alcohol consumption levels ("Dalc")
- **Correlation Analysis:** Conducted to check for multicollinearity and assess relationships among variables.

### 3. Model Development
- **Logistic Regression:** Chosen for its simplicity and interpretability.
- **Backward Elimination:** Used to refine the model by removing non-significant variables.
- **Cross-Validation:** K-fold cross-validation employed to validate the model and prevent overfitting.

### 4. Model Evaluation
- **Metrics:** Model performance evaluated using Area Under the Curve (AUC), precision, recall, and F1-score.
- **ROC Analysis:** Used to analyze the trade-off between true positive rate (TPR) and false positive rate (FPR).

### 5. Results & Interpretation
- The model effectively classifies students based on their weekend alcohol consumption levels, with a focus on minimizing false negatives to identify high-risk students accurately.
- **Limitations:** The dataset's age and geographical focus may limit the generalizability of the model. Incorporating more recent data or additional socioeconomic factors could improve the model's robustness.

## Dependencies

The project requires the following Python libraries:

- `pandas`
- `numpy`
- `seaborn`
- `matplotlib`
- `statsmodels`
- `scikit-learn`
