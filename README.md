# Predictive Maintenance Analysis

This project focuses on predicting machine failures in a mechanical industry using machine learning models.  
It analyzes operational data from a drilling tool used on a lathe machine to identify patterns leading to failure and helps prevent unexpected breakdowns.

---

## 📋 Project Overview

In mechanical industries, machines sometimes fail unexpectedly due to improper handling, power outages, faulty instruments, incorrect machine parameters, etc.  
By analyzing a dataset of a **drilling tool**, we built a machine learning model to predict if the machine will fail before starting production.

---

## 🚀 Future Scope

- Improves productivity by reducing downtime.
- Predicts failures beforehand by providing input parameters.
- Prevents machine failures and improves safety.
- Reduces accidents in the workplace.

---

## 📂 Data Information

- Dataset represents the drilling tool used in a lathe machine.
- Input Features:
  1. Air temperature [K]
  2. Process temperature [K]
  3. Rotational speed [RPM]
  4. Torque [Nm]
  5. Tool wear [min]
  6. Type (L, M, H — product quality)
  7. Failure Type
- Output:
  - Target: `0` = No Failure, `1` = Failure
  - Failure Types:
    - Heat Dissipation Failure
    - Power Failure
    - Overstrain Failure
    - Tool Wear Failure
    - Random Failures

---

## 🔎 Data Insights

- Data has no null values and contains categorical features.
- Data is normally distributed.
- Imbalance exists between failure and no-failure classes.
- Most failures occur due to:
  - Heat Dissipation
  - Power Failure
  - Overstrain
  - Tool Wear
- Low quality products make up ~60%, Medium ~30%, High ~10%.
- Rotational speed, torque, and tool wear strongly influence failures.

---

## 🧪 Models Used

- Logistic Regression
- K-Nearest Neighbors
- Decision Tree
- Random Forest

We built a function to test multiple models and selected the one with the highest accuracy.

---

## 📈 Model Evaluation

- Metrics:
  - Accuracy
  - Precision
  - Classification Report
  - Confusion Matrix
- Hyperparameter tuning performed.
- Final model tested on sample values.

---

## 🖥️ Languages & Libraries

- **Languages:** Python, Excel
- **Libraries:**
  - numpy
  - pandas
  - matplotlib
  - seaborn
  - scikit-learn
  - warnings filter

---

## 🧪 Example Test Cases

| Type | Air Temp [K] | Process Temp [K] | RPM  | Torque [Nm] | Tool wear [min] | Target |
|------|--------------|------------------|------|-------------|-----------------|--------|
| M    | 298.2        | 308.5            | 2678 | 10.7        | 86              | 1      |
| H    | 298.4        | 308.9            | 1782 | 23.9        | 24              | 0      |

---

## 📋 Prescriptive Analysis

Failures mainly occur due to:
1. Improper rotational speed.
2. Incorrect torque.
3. Excessive tool wear.

### Measures to Prevent Failures:
- Set rotational speed properly.
- Adjust torque to recommended values.
- Replace tools before excessive wear.
- Use medium or high-quality products.
- Provide coolant to avoid overheating.
- Install backup power supply.

---

This project is for educational and research purposes only and part of my portfolio, showcasing the machine learning skills essential for data science roles. If you have any questions, feedback, or would like to collaborate, feel free to get in touch!

- **LinkedIn**: [Connect with me professionally](https://www.linkedin.com/in/adii8/)

**Thank you, I look forward to connecting with you!**


---
