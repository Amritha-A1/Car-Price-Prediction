# 🚗 Car Price Prediction Using Machine Learning

## 📌 Project Overview

The objective of this project is to predict car prices in the American automobile market using Machine Learning regression algorithms.

A Chinese automobile company plans to enter the US market and wants to understand the factors that influence car prices. This project analyzes different car features and develops a machine learning model to predict car prices accurately.

## 🎯 Problem Statement

The company wants to identify the important variables affecting car prices and understand how these factors influence pricing in the American market.

This project uses machine learning techniques to analyze car specifications and predict their prices.

## 📂 Dataset Information

- **Dataset:** Car Price Assignment Dataset
- **Rows:** 205
- **Columns:** 26
- **Target Variable:** `price`
- **Problem Type:** Supervised Machine Learning – Regression

The dataset contains car-related information such as:

- Engine Size
- Horsepower
- Curb Weight
- Car Width
- Car Length
- Highway MPG
- City MPG
- Wheelbase
- Fuel Type
- Body Style

## 🛠️ Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook / Google Colab

## ⚙️ Project Workflow

### 1. Data Loading and Exploration
- Loaded the dataset using Pandas.
- Checked dataset shape, data types, and statistical information.
- Explored numerical and categorical features.

### 2. Data Preprocessing
- Separated independent variables (X) and the target variable (y).
- Identified categorical features.
- Applied One-Hot Encoding.
- Split the dataset into training and testing sets using an 80:20 ratio.

### 3. Exploratory Data Analysis (EDA)
- Analyzed relationships between different car features and prices.
- Used visualizations to understand data patterns and distributions.

### 4. Model Building

Implemented and compared five regression algorithms:

1. Linear Regression
2. Decision Tree Regressor
3. Random Forest Regressor
4. Gradient Boosting Regressor
5. Support Vector Regressor (SVR)

### 5. Model Evaluation

Evaluated model performance using:

- R² Score
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)

### 6. Feature Importance

Used Random Forest to identify the most important features influencing car price predictions.

**Top important features:**
- Engine Size
- Curb Weight
- Highway MPG
- Horsepower
- Car Width

### 7. Feature Selection

Selected the top 10 features based on Random Forest feature importance to focus on the most relevant input variables.

### 8. Hyperparameter Tuning

Applied GridSearchCV with 5-fold cross-validation to optimize the Random Forest model.

**Best Parameters:**

```python
{
    'n_estimators': 300,
    'max_depth': 20,
    'min_samples_split': 2,
    'min_samples_leaf': 2
}
```

### 9. Final Model Evaluation

The tuned Random Forest model achieved the following results:

| Metric | Score |
|---|---:|
| Training R² Score | 0.9762 |
| Testing R² Score | 0.9545 |
| MAE | 1338.71 |
| MSE | 3588950.11 |
| RMSE | 1894.45 |

## 📊 Key Insights

- Engine size and curb weight were the most important features in the Random Forest model.
- Feature selection helped focus on the top 10 important features.
- Random Forest performed better than the other evaluated regression models.
- Hyperparameter tuning improved model performance.
- The small difference between training and testing R² scores indicates good generalization performance.

## 📈 Actual vs Predicted Prices

An Actual vs Predicted scatter plot was created to compare the actual car prices with the model's predicted prices.

Points closer to the diagonal reference line indicate more accurate predictions.

## 🏆 Conclusion

The Car Price Prediction project successfully developed a machine learning regression model to estimate car prices based on different automobile features.

After comparing five regression algorithms and applying hyperparameter tuning, the Random Forest Regressor achieved the best performance, with a testing R² score of approximately **95.45%**.

This project demonstrates how machine learning can help identify important car pricing factors and support data-driven pricing decisions in the automobile industry.

## 👩‍💻 Author

**Amritha Nandakumar A**



