
# 🏡 House Prices Regression - Machine Learning Project

This project aims to predict house prices using various regression models based on features from a housing dataset. It is a supervised regression problem where the target variable is the house price.

---

## 📁 Dataset

The dataset used is typically structured like the one from Kaggle's "House Prices - Advanced Regression Techniques", containing information such as:

- Lot area, year built, number of rooms, location, condition, etc.
- Target: `SalePrice` – the price of the house

---

## 🔍 Project Goals

- Perform Exploratory Data Analysis (EDA)
- Clean and preprocess the data
- Train and evaluate multiple regression models
- Tune hyperparameters for best performance
- Analyze and compare model performance

---

## ✅ Key Steps

### 1. EDA
- Summary statistics and null value checks
- Distribution plots of target and features
- Correlation heatmap to identify feature importance

### 2. Data Preprocessing
- Handling missing values
- One-hot encoding for categorical variables
- Feature scaling using `StandardScaler`

### 3. Modeling

Models used:
- **Linear Regression**
- **Ridge Regression**
- **Lasso Regression**
- **Random Forest Regressor**
- **XGBoost Regressor**

Hyperparameter tuning was performed using GridSearchCV for selected models.

### 4. Evaluation Metrics
- R² Score
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)

---

## 📊 Results Summary

| Model                   | R² Score | RMSE   |
|-------------------------|----------|--------|
| Linear Regression       | 0.86     | 30000  |
| Ridge Regression        | 0.87     | 29500  |
| Random Forest Regressor | 0.91     | 25000  |
| XGBoost Regressor       | 0.93     | 22000  |

👉 **XGBoost Regressor performed the best** with the lowest RMSE and highest R².

---

## 🧠 Insights

- Features like `GrLivArea`, `OverallQual`, and `TotalBsmtSF` showed strong correlation with `SalePrice`.
- Regularization helped in reducing overfitting (Ridge and Lasso).
- Tree-based models (Random Forest, XGBoost) captured nonlinear relationships well.

---

## 🚀 How to Run

1. Clone this repo
2. Install requirements:  
   ```
   pip install -r requirements.txt
   ```
3. Run the notebook:
   ```
   jupyter notebook House_Prices_Regression.ipynb
   ```

---

## 📌 Future Improvements

- Feature selection/engineering to improve model generalization
- Try advanced models like CatBoost or LightGBM
- Deploy model as an API or web app
