# 📊 E-Commerce Sales Forecasting using Machine Learning

## 📌 Project Overview

This project focuses on predicting future e-commerce sales using **Machine Learning (Linear Regression)**. It analyzes historical sales data, performs feature engineering, and builds a predictive model to forecast future trends.

The model also generates **90 days of future sales predictions** based on learned patterns.

---

## 📂 Dataset

* File used: `ecommerce_sales_forecast_dataset.csv`
* The dataset contains historical sales-related information.
* If the dataset does not contain a `Date` column, it is automatically generated.

---

## ⚙️ Technologies Used

* Python 🐍
* Pandas & NumPy
* Matplotlib & Seaborn
* Scikit-learn (Linear Regression)

---

## 🔄 Project Workflow

### 1. Data Loading

```python
df = pd.read_csv('ecommerce_sales_forecast_dataset.csv')
```

### 2. Data Preprocessing

* Handle missing values
* Remove duplicates
* Convert `Date` column to datetime
* Automatically detect target column (`Sales`, `Revenue`, etc.)

### 3. Feature Engineering

* Extract:

  * Day
  * Month
  * Year
  * Day of Week
* Create:

  * Weekend indicator
  * Seasonal features (Winter, Summer, Monsoon, Autumn)

### 4. Data Visualization

* Sales trend over time
* Correlation heatmap

### 5. Model Training

* Algorithm: **Linear Regression**
* Train-test split (80% training, 20% testing)

### 6. Model Evaluation

* Mean Squared Error (MSE)
* R² Score

### 7. Prediction

* Predict test data
* Forecast next 90 days of sales

---

## 📈 Output Visualizations

### ✔️ Sales Trend Graph

<img width="983" height="452" alt="image" src="https://github.com/user-attachments/assets/d8bdb54c-66b4-47e3-8ead-7bde192197df" />


### ✔️ Correlation Heatmap

Displays relationships between numerical features.
<img width="895" height="494" alt="image" src="https://github.com/user-attachments/assets/4e5a6076-d7d6-46a2-a2a6-0a7d1022ef04" />


### ✔️ Actual vs Predicted

Compares real values with model predictions.
<img width="641" height="489" alt="image" src="https://github.com/user-attachments/assets/d2612209-7831-4a27-8164-0492bacbb7af" />

---

## 🚀 Future Forecasting

The model predicts sales for the next **90 days** using generated future dates and engineered features.

---

## 🧠 Key Features of the Project

* Automatic target column detection
* Seasonal feature creation
* Time-based feature engineering
* Future forecasting capability
* Clean and simple ML pipeline

---

## 📊 Model Performance

* **MSE (Mean Squared Error):** Printed in output
* **R² Score:** Printed in output

---

## 📁 Project Structure

```
├── ai_&_ml_2.py
├── ecommerce_sales_forecast_dataset.csv
└── README.md
```

---

## ▶️ How to Run the Project

1. Install required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

2. Place dataset in the same folder.

3. Run the script:

```bash
python ai_&_ml_2.py
```

---

## 📌 Notes

* The model automatically handles missing `Date` columns.
* Categorical features are converted using one-hot encoding.
* Future predictions align with training features.

---

## 🔗 Reference

Original notebook source:

---

## 👩‍💻 Author
**
Lakshiya S S**

---

## ⭐ Conclusion

This project demonstrates how machine learning can be applied to real-world e-commerce data to predict future sales trends and support business decision-making.
