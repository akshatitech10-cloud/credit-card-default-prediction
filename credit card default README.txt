# Credit Card Default Prediction

A machine learning classification project to predict next-month credit card payment defaults using customer credit and payment data.

## 📌 Project Overview

This project uses the **Default of Credit Card Clients** dataset containing information on 30,000 credit card customers. The objective is to predict whether a customer will default on their payment in the following month.

## 📊 Dataset

- **Dataset Size:** 30,000 customers
- **Target Variable:** `default payment next month`
- **0:** No Default
- **1:** Default

The dataset contains information related to credit limit, age, bill amounts, payment amounts, demographic characteristics, and previous payment history.

## 🔍 Exploratory Data Analysis

- Analyzed the distribution of the target variable to identify class imbalance.
- Studied customer demographics, credit limits, bill amounts, payment amounts, and repayment history.
- Compared credit and repayment patterns between default and non-default customers.

## ⚙️ Data Preprocessing

- Removed the `ID` column as it does not contribute to prediction.
- Applied One-Hot Encoding to categorical variables.
- Standardized numerical variables using `StandardScaler`.
- Used an **80:20 stratified train-test split**.
- Applied **class-weighted training** to give greater importance to the minority default class.

## 🤖 Models Used

- Logistic Regression
- Decision Tree
- Random Forest

Both baseline and class-weighted models were trained and evaluated.

## 📈 Model Evaluation

Models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC
- Confusion Matrix

### Balanced Logistic Regression Results

- **Accuracy:** 77.35%
- **Precision:** 0.49
- **Recall:** 0.55
- **F1-Score:** 0.52
- **ROC-AUC:** 0.76

The class-weighted approach was used to improve the model's focus on the minority default class without generating synthetic observations.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## 📁 Files

- `credit card default.ipynb` — Complete data analysis, preprocessing, model training, and evaluation
- `README.md` — Project documentation
- `requirements.txt` — Required Python libraries

## ▶️ How to Run

1. Download or clone this repository.
2. Install the required libraries:

```bash
pip install -r requirements.txt


## 📚 Dataset Source

Default of Credit Card Clients Dataset — UCI Machine Learning Repository.