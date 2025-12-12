# 🏡 Project 2: House Prices Regression (Kaggle)

## Executive Summary
This project focuses on predicting house sale prices using the Ames Housing dataset. It demonstrates advanced techniques for data cleaning, feature engineering, transformation, and regularization with the final model achieving a low Root Mean Squared Error (RMSE).

## 🎯 Objective
To build a high-performing regression model (Ridge) to predict the logarithm of the Sale Price, optimizing the model's performance and interpretability.

## ⚙️ Methodology & Techniques
* **Advanced Missing Data Handling:** Imputed large volumes of NaNs in categorical features (e.g., PoolQC, Alley) with 'None' (indicating absence of the feature) and numerical features (e.g., LotFrontage) with the **median**.
* **Target Transformation:** Applied the **Logarithmic Transformation (log1p)** to the target variable (`SalePrice`) to normalize the distribution and satisfy the assumptions of linear models.
* **Feature Engineering:** Converted all remaining categorical features to numerical using One-Hot Encoding (`get_dummies`), resulting in a high-dimensional feature matrix.
* **Model Training:** Used **Ridge Regression** to prevent overfitting on the high-dimensional dataset (due to regularization via the alpha parameter).
* **Optimization:** Used **Grid Search with Cross-Validation** to find the optimal regularization strength ($\alpha$).

## 📊 Key Findings
* **Model Performance (RMSE on Log Scale):** The optimized model achieved a low RMSE of **0.1345**.
* **Most Influential Features (Top 3):** The model identified key drivers, including **Overall Quality (OverallQual)**, **Ground Living Area (GrLivArea)**, and **Garage Cars (GarageCars)**.

---
**[View Notebook: House_Prices_Ridge.ipynb](House_Prices_Ridge.ipynb)**
