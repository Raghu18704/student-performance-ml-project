# Student Performance Prediction using Machine Learning

## Overview
This project focuses on analyzing student performance data and predicting **math scores** using machine learning regression techniques.  
The workflow follows a complete data science pipeline, including Exploratory Data Analysis (EDA), data preprocessing, feature engineering, model building, evaluation, and comparison.

The objective is to understand how academic and socio-economic factors influence student performance and to build reliable predictive models.

---

## Dataset
- **Dataset Name:** Student Performance Dataset
- **Description:** Contains demographic information, educational background, and exam scores of students.
- **Key Features:**
  - Gender
  - Race/Ethnicity
  - Parental Level of Education
  - Lunch Type
  - Test Preparation Course
  - Math, Reading, and Writing Scores

---

## Exploratory Data Analysis (EDA)
EDA was performed to understand the structure and patterns in the dataset.

### Key EDA Steps:
- Verified dataset shape, data types, and structure
- Checked for missing values and duplicate records
- Performed univariate analysis on numerical and categorical features
- Conducted multivariate analysis to study relationships between features
- Visualized score distributions and categorical impacts using plots

### Insights:
- Students who completed the test preparation course generally scored higher.
- Students with standard lunch showed better performance on average.
- Strong positive correlation exists between math, reading, and writing scores.

---

## Feature Engineering
- Created new features:
  - **Total Score** = Math + Reading + Writing
  - **Average Score** = Total Score / 3
- Removed derived features during modeling to avoid data leakage.

---

## Data Preprocessing
- Separated target variable (**math score**) and input features
- Applied **one-hot encoding** to categorical variables
- Split data into training (80%) and testing (20%) sets
- Applied **feature scaling** for regularized models

---

## Machine Learning Models
The following regression models were implemented:

- **Linear Regression** (baseline model)
- **Ridge Regression** (L2 regularization)
- **Lasso Regression** (L1 regularization and feature selection)

---

## Model Evaluation
Models were evaluated using:
- **Mean Squared Error (MSE)**
- **R² Score**

### Model Comparison Summary:
- Linear and Ridge Regression showed similar and stable performance.
- Lasso Regression performed feature selection by shrinking less important coefficients.
- Regression models demonstrated strong predictive capability for this dataset.

---

## Model Diagnostics
- Residual analysis was performed to validate linear regression assumptions.
- Residual plots confirmed:
  - Linearity
  - Constant variance
  - Approximate normality of errors

---

## Technologies Used
- **Programming Language:** Python
- **Libraries:**
  - Pandas, NumPy
  - Matplotlib, Seaborn
  - Scikit-learn

---

---

## Conclusion
This project demonstrates a complete machine learning workflow for predicting student performance.  
Through EDA, feature engineering, and regression modeling, meaningful insights were derived and reliable predictive models were built.  
The results confirm that linear regression and its regularized variants are effective for this problem.

---

## Future Improvements
- Try non-linear models such as Random Forest or XGBoost
- Perform hyperparameter tuning using cross-validation
- Deploy the model using a web framework like Flask or Streamlit

---

## Author
**Raghu Ram**  
BTech Student | Aspiring AI Engineer

