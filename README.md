# 🏠 California Housing Price Prediction

This project focuses on predicting housing prices using the **California Housing Dataset** from Scikit-Learn. Various regression models are tested and compared based on their **Root Mean Squared Error (RMSE)** using **10-fold cross-validation**.

---

## 📂 Dataset

The dataset provides information such as:

- Median income
- House age
- Total rooms
- Population
- Proximity to the ocean  
...and more, with the target variable being **median house value**.

---

## ⚙️ Models Implemented

### 1. 🔹 Linear Regression
- Simple baseline model.
- No regularization applied.
- **Mean RMSE:** 69104  
- **Standard Deviation:** 2880

### 2. 🌳 Decision Tree Regressor
- Captures non-linear patterns but prone to overfitting.
- **Mean RMSE:** 71522  
- **Standard Deviation:** 2534

### 3. 🌲 Random Forest Regressor
- Ensemble method for higher accuracy and stability.
- **Mean RMSE:** 50379  
- **Standard Deviation:** 2190

---

## 📉 RMSE Comparison (10-Fold Cross-Validation)

| Model                   | Mean RMSE | Std Deviation |
|------------------------|-----------|----------------|
| Linear Regression       | 69104     | 2880           |
| Decision Tree Regressor| 71522     | 2534           |
| Random Forest Regressor| **50379** | **2190**       |

✅ **Random Forest Regressor** performed the best with the lowest average RMSE and smallest variation.

---

## 🧪 Evaluation Method

Each model is evaluated using:

- `mean_squared_error` (converted to RMSE)
- `cross_val_score` from `sklearn.model_selection`
- Scoring metric: `"neg_mean_squared_error"` (converted back to positive RMSE)

---

## 🛠️ Libraries Used

- `scikit-learn`
- `numpy`

---



## 🚀 Future Scope

- Hyperparameter tuning (e.g., GridSearchCV)
- Adding more advanced models like XGBoost
- Feature scaling and selection
- Visualizing model performance

---

## 📄 License

This project is licensed under the MIT License. Feel free to use or modify it.

---
