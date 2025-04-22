
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
- **Random Forest Regressor**
- **XGBoost Regressor**
-  **Ridge**

Hyperparameter tuning was performed using GridSearchCV for selected models.

### 4. Evaluation Metrics
- R² Score
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)

---



## 🧠 Insights

- Features like `GrLivArea`, `OverallQual`, and `TotalBsmtSF` showed strong correlation with `SalePrice`.
- Regularization helped in reducing overfitting (Ridge).
- Tree-based models (Random Forest, XGBoost) captured nonlinear relationships well.

---

## 🚀 How to Run

1. Clone this repo
2. Install requirements:  
3. Run the notebook:
   ```
   jupyter notebook House_Prices_Regression.ipynb
   ```

---

## 📌 Future Improvements

- Feature selection/engineering to improve model generalization
- Try advanced models like CatBoost or LightGBM
- Deploy model as an API or web app
