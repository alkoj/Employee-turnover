# 🧠 Employee Turnover Prediction

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/alkoj/ala-k-mod1-atsiskaitymas/blob/main/Employee_turnover.ipynb)

## 🎯 Project Goal

The main objective of this project is to predict employee turnover to help organizations retain valuable employees. By analyzing factors that influence employee satisfaction and retention, the model identifies key indicators that can guide management strategies, improve work conditions, and ultimately reduce employee attrition.

---

## 📊 Dataset Description

The dataset includes the following features for each employee:

| Feature                | Description                                                                 |
|------------------------|-----------------------------------------------------------------------------|
| `satisfaction_level`   | Employee satisfaction level (0 to 1)                                        |
| `last_evaluation`      | Last performance evaluation score                                           |
| `number_project`       | Number of projects the employee has worked on                               |
| `average_monthly_hours`| Average hours worked per month                                              |
| `time_spend_company`   | Number of years spent in the company                                        |
| `work_accident`        | Whether the employee had a work accident (0 = No, 1 = Yes)                  |
| `promotion_last_5years`| Whether the employee was promoted in the last 5 years (0 = No, 1 = Yes)     |
| `department`           | Department the employee belongs to                                          |
| `salary`               | Salary category (low, medium, high)                                         |
| `left`                 | Target variable: whether the employee left (1 = Yes, 0 = No)                |

---

## 🧹 Data Processing

-Before training the models, the following steps were performed:

- **Missing value removal**: Rows with missing values ​​were removed or filled with the median.
- **Categorical feature encoding**: `LabelEncoder` and `OneHotEncoder` were used.
- **Feature scaling**: `StandardScaler` was applied to normalize numeric columns.
- **Class balancing**: using `SMOTE` or `class_weight` (depending on the model).
- **Train/test split**: `train_test_split` with `test_size=0.2`.


---

## 🤖 Machine Learning

The following models were tested in the project:

- **Logistic Regression**
- **Random Forest Classifier**
- **Gradient Boosting (XGBoost)**
- **Support Vector Machine (SVM)**
- **Neural Network (MLPClassifier)**

---

## 📈 Results

Best Model: Random Forest

Accuracy: 0.990
F1-score (C1): 0.98
Precision (C1): 0.99
Recall (C1): 0.96
These figures demonstrate the high accuracy of forecasting employee layoffs.

---
## Dependencies

pandas, numpy
scikit-learn
matplotlib, seaborn
xgboost
imbalanced-learn
tensorflow / keras (for MLP)
---
## 📂 Project Structure

```
employee-turnover/
│
├── data/
│   └── employee_data.csv         # Initial data
│
├── images/
│   ├── feature_importance.png    # Importance of features
│   ├── correlation_matrix.png    # Correlation matrix
│   └── model_results.png         # Comparison table of models
│
├── notebooks/
│   └── employee_attrition.ipynb  # Basic Jupyter Notebook
│
├── src/
│   ├── preprocessing.py          # Data Processing
│   ├── models.py                 # Training models
│   └── utils.py                  # Auxiliary functions
│
├── README.md                     # Оproject description
└── requirements.txt              # Dependencies

```

---

## 🚀 How to Run

You can open the notebook in Google Colab using the badge above. Alternatively, clone this repo and run locally:

```bash
git clone https://github.com/alkoj/employee-turnover.git
cd employee-turnover
jupyter notebook Employee_turnover.ipynb
```

---

## 📌 Author

- [alkoj](https://github.com/alkoj)

---

## 📃 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
