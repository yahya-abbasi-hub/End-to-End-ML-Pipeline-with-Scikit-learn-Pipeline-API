# End-to-End-ML-Pipeline-with-Scikit-learn-Pipeline-API
## Project Overview

This project builds an end-to-end machine learning pipeline to predict customer churn using the Telco Customer Churn dataset.

The project demonstrates:
- Data preprocessing
- Feature engineering
- Scikit-learn Pipeline API
- Hyperparameter tuning with GridSearchCV
- Model evaluation
- Production-ready model export using joblib

---

## Dataset

Dataset Used:
Telco Customer Churn Dataset

The dataset contains customer information such as:
- Gender
- Monthly Charges
- Contract Type
- Internet Service
- Payment Method
- Churn Status

Target Variable:
- Churn (Yes / No)

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Joblib

---

## Machine Learning Workflow

### 1. Data Cleaning
- Removed customerID column
- Converted TotalCharges to numeric
- Handled missing values
- Encoded target variable

### 2. Data Preprocessing
Implemented using Scikit-learn Pipeline API:
- StandardScaler for numerical features
- OneHotEncoder for categorical features
- SimpleImputer for missing values

### 3. Models Trained
- Logistic Regression
- Random Forest Classifier

### 4. Hyperparameter Tuning
Used GridSearchCV to find the best parameters for:
- Logistic Regression
- Random Forest

### 5. Model Evaluation
Evaluated using:
- Accuracy Score
- ROC-AUC Score
- Classification Report

### 6. Model Export
Exported the complete trained pipeline using Joblib.

---

## Project Structure

```bash
├── Telco-Customer-Churn.csv
├── churn_pipeline.pkl
├── churn_prediction.ipynb
├── README.md
└── requirements.txt
```

---

## Results

Best performing model selected automatically based on ROC-AUC score.

Example metrics:
- Accuracy: ~80%
- ROC-AUC: ~84%

---

## Model Saving

```python
joblib.dump(best_pipeline, 'churn_pipeline.pkl')
```

Load model again:

```python
loaded = joblib.load('churn_pipeline.pkl')
```

---

## Skills Demonstrated

- Machine Learning Pipelines
- Feature Preprocessing
- Hyperparameter Tuning
- Production-ready ML Workflow
- Model Serialization
- Binary Classification

---

## Future Improvements

- Deploy using Streamlit or Flask
- Add real-time predictions
- Build interactive dashboard
- Use advanced boosting models

---

## Author
Yahya Abbasi

Machine Learning Project using Scikit-learn Pipeline API
