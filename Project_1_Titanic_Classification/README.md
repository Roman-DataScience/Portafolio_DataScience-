# 🚢 Project 1: Titanic Survival Classification

## Executive Summary
This project tackles the classic Kaggle challenge of predicting passenger survival on the Titanic, demonstrating core Machine Learning classification techniques. The final model achieves a high predictive accuracy, highlighting the critical impact of socio-economic factors on survival.

## 🎯 Objective
To build a robust classification model capable of predicting whether a passenger survived (1) or not (0) based on features like passenger class, age, and sex.

## ⚙️ Methodology & Techniques
* **Data Cleaning:** Handled missing values (NaN) in the 'Age' column using the **median** and 'Embarked' using the **mode**.
* **Feature Engineering:** Created the binary feature 'Is_Child' to capture the "women and children first" effect.
* **Encoding:** Applied One-Hot Encoding (`get_dummies`) to convert categorical features ('Sex', 'Embarked') into numerical formats suitable for modeling.
* **Modeling:** Two powerful models were used:
    * **Logistic Regression:** Used for its **interpretability** and ability to showcase feature impact (coefficients).
    * **Random Forest Classifier:** Used for higher **predictive accuracy**.

## 📊 Key Findings
* **Most Important Predictors:** **'Sex' (Female)** and **'Pclass' (Passenger Class)** were the two most significant predictors of survival across both models.
* **Model Performance (Accuracy):**
    * **Logistic Regression:** Achieved an accuracy of approximately **71.88**%.
    * **Random Forest:** Achieved an accuracy of approximately **81.25**%.

---
**[View Notebook: Titanic_Clasificacion.ipynb](Titanic_Clasificacion.ipynb)**
