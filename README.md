# Drug Prescription Classification

## Project Overview

This project applies supervised Machine Learning techniques to predict the prescribed drug using demographic and clinical information from a synthetic healthcare dataset.

The objective is to compare different classification algorithms, evaluate their predictive performance and analyze their strengths and limitations.

---

## Dataset

The dataset contains **1,000 synthetic patient records** and includes demographic, clinical and treatment-related information.

### Features

| Feature | Description |
|---------|-------------|
| Age | Patient age |
| Gender | Patient gender |
| Condition | Medical condition |
| Drug_Name | Prescribed drug (target variable) |
| Dosage_mg | Drug dosage |
| Treatment_Duration_days | Treatment duration |
| Side_Effects | Reported side effect |
| Improvement_Score | Treatment effectiveness score |

> **Note:** This is a synthetic dataset created for educational purposes and does not contain real patient information.

---

## Workflow

The project follows a complete Machine Learning workflow:

- Data loading
- Exploratory Data Analysis (EDA)
- Data preprocessing
- Train/Test split
- Feature encoding
- Model training
- Hyperparameter tuning with GridSearchCV
- Cross-validation
- Model evaluation
- Error analysis

---

## Models Used

- Logistic Regression
- Decision Tree
- Random Forest

---

## Results

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- ROC Curve
- Precision-Recall Curve

Random Forest achieved the best overall performance after hyperparameter tuning.

---

## Key Insights

Most prediction errors occur between drugs belonging to the same therapeutic category.

This suggests that the available features contain enough information to identify the general medical condition, but are often insufficient to distinguish between alternative drugs prescribed for the same disease.

To further investigate this limitation, the notebook also includes a binary classification task focused on **Ibuprofen** prescriptions.

---

## Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
