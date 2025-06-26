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

- Missing value checks
- Encoding of categorical variables
- Feature scaling
- Data splitting (train/test)

---

## 🤖 Machine Learning

Various classification algorithms were tested and compared to predict employee attrition. Metrics like accuracy, precision, recall, and F1-score were used for evaluation.

---

## 📈 Results

(Добавьте сюда информацию о лучших результатах модели — точность, F1-метрика и т.д.)

---

## 📂 Project Structure

```
├── Employee_turnover.ipynb   # Main notebook with full analysis and modeling
├── data/                     # (Если есть) данные
├── images/                   # (Если есть) графики и визуализации
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
